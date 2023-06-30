# Comparing `tmp/dspawpy-1.0.0-py3-none-any.whl.zip` & `tmp/dspawpy-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 74056 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-21 09:48 dspawpy/__init__.py
--rw-rw-rw-  2.0 fat    32073 b- defN 23-Jun-21 09:35 dspawpy/plot.py
+Zip file size: 74397 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat       48 b- defN 23-Jun-25 01:55 dspawpy/__init__.py
+-rw-rw-rw-  2.0 fat    32128 b- defN 23-Jun-30 09:35 dspawpy/plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
--rw-rw-rw-  2.0 fat    24376 b- defN 23-Jun-21 09:35 dspawpy/analysis/aimdtools.py
+-rw-rw-rw-  2.0 fat    24229 b- defN 23-Jun-29 01:16 dspawpy/analysis/aimdtools.py
 -rw-rw-rw-  2.0 fat    20177 b- defN 23-Jun-21 08:08 dspawpy/analysis/vacf.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 06:07 dspawpy/diffusion/__init__.py
 -rw-rw-rw-  2.0 fat     3986 b- defN 23-Jun-21 08:08 dspawpy/diffusion/neb.py
--rw-rw-rw-  2.0 fat    56985 b- defN 23-Jun-21 09:35 dspawpy/diffusion/nebtools.py
+-rw-rw-rw-  2.0 fat    56887 b- defN 23-Jun-29 01:16 dspawpy/diffusion/nebtools.py
 -rw-rw-rw-  2.0 fat    11045 b- defN 23-Jun-21 08:08 dspawpy/diffusion/pathfinder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
 -rw-rw-rw-  2.0 fat    62556 b- defN 23-Jun-21 08:08 dspawpy/io/read.py
 -rw-rw-rw-  2.0 fat    10548 b- defN 23-Jun-21 09:35 dspawpy/io/structure.py
--rw-rw-rw-  2.0 fat    27765 b- defN 23-Jun-21 09:35 dspawpy/io/utils.py
--rw-rw-rw-  2.0 fat    29270 b- defN 23-Jun-21 09:35 dspawpy/io/write.py
--rw-rw-rw-  2.0 fat     5169 b- defN 23-Jun-21 09:49 dspawpy-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-21 09:49 dspawpy-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-21 09:49 dspawpy-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1422 b- defN 23-Jun-21 09:49 dspawpy-1.0.0.dist-info/RECORD
-18 files, 285521 bytes uncompressed, 71752 bytes compressed:  74.9%
+-rw-rw-rw-  2.0 fat    27765 b- defN 23-Jun-29 01:15 dspawpy/io/utils.py
+-rw-rw-rw-  2.0 fat    30401 b- defN 23-Jun-30 09:35 dspawpy/io/write.py
+-rw-rw-rw-  2.0 fat     5579 b- defN 23-Jun-30 09:35 dspawpy-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 09:35 dspawpy-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-30 09:35 dspawpy-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1422 b- defN 23-Jun-30 09:35 dspawpy-1.0.1.dist-info/RECORD
+18 files, 286871 bytes uncompressed, 72093 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: dspawpy/io/utils.py
 Comment: 
 
 Filename: dspawpy/io/write.py
 Comment: 
 
-Filename: dspawpy-1.0.0.dist-info/METADATA
+Filename: dspawpy-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-1.0.0.dist-info/WHEEL
+Filename: dspawpy-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-1.0.0.dist-info/top_level.txt
+Filename: dspawpy-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-1.0.0.dist-info/RECORD
+Filename: dspawpy-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/__init__.py

```diff
@@ -1,2 +1,2 @@
 # -*- coding: utf-8 -*-
-__version__ = "0.9.10"
+__version__ = "1.0.1"
```

## dspawpy/plot.py

```diff
@@ -15,15 +15,15 @@
 def average_along_axis(
     datafile="potential.h5",
     task: str = "potential",
     axis=2,
     smooth=False,
     smooth_frac=0.8,
     raw=False,
-    key: str = None,
+    subtype: str = None,
     **kwargs,
 ):
     r"""绘制沿着某个轴向的物理量平均值曲线
 
     Parameters
     ----------
     datafile : str or list or np.ndarray
@@ -33,15 +33,17 @@
     axis : int
         沿着哪个轴向绘制势能曲线, 默认2
     smooth : bool
         是否平滑, 默认False
     smooth_frac : float
         平滑系数, 默认0.8
     raw : bool
-        是否返回原始数据到csv文件
+        是否返回绘图数据到csv文件
+    subtype : str
+        用于指定task数据子类，暂时只支持 TotalLocalPotential，默认None，代表绘制 TotalElectrostaticPotential
     **kwargs : dict
         其他参数, 传递给 matplotlib.pyplot.plot
 
     Returns
     -------
     axes: matplotlib.axes._subplots.AxesSubplot
         可传递给其他函数进行进一步处理
@@ -51,22 +53,26 @@
     >>> from dspawpy.plot import average_along_axis
 
     读取 potential.h5 文件中的数据，绘图并保存原始绘图数据到csv文件
 
     >>> average_along_axis(datafile='/data/home/hzw1002/dspawpy_repo/test/2.7/potential.h5', task='potential', axis=2, smooth=True, smooth_frac=0.8, raw=True)
     <module 'matplotlib.pyplot' from '/data/home/hzw1002/anaconda3/lib/python3.9/site-packages/matplotlib/pyplot.py'>
     """
-    assert task.lower() in [
+    assert task in [
         "rho",
         "potential",
         "elf",
         "pcharge",
         "rhoBound",
     ], "仅支持 rho, potential, elf, pcharge, rhoBound 任务类型"
-    assert key is None or isinstance(key, str), "key 必须是字符串"
+    if subtype is not None:
+        assert (
+            task == "potential" and subtype == "TotalLocalPotential"
+        ), '目前仅支持"potential"的"TotalLocalPotential"子类'
+
     # only for compatibility
     if isinstance(datafile, list) or isinstance(datafile, np.ndarray):
         ys = datafile  # expect np.ndarray or list
 
     # search datafile in the given directory
     elif os.path.isdir(datafile):
         directory = datafile  # specified datafile is actually a directory
@@ -81,85 +87,86 @@
             raise FileNotFoundError(f"未找到{task}.h5/{task}.json文件！")
 
     # parse the real datafile
     elif datafile.endswith(".h5"):
         hfile = datafile
         hdict = load_h5(hfile)
         grid = hdict["/AtomInfo/Grid"]
-        # pot = np.asarray(potential["/Potential/TotalElectrostaticPotential"]).reshape(grid, order="F")
-        # DS-PAW 数据写入h5 列优先
-        # h5py 从h5读取数据 默认行优先
-        # np.array(data_list) 默认行优先
-        # 所以这里先以 行优先 把 “h5 行优先 读进来的数据” 转成一维， 再以 列优先 转成 grid 对应的维度
-        if task.lower() == "rho":
-            if key is None:
+
+        if task == "rho":
+            if subtype is None:
                 _key = "/Rho/TotalCharge"
             else:
-                _key = f"/Rho/{key}"
-        elif task.lower() == "potential":
-            if key is None:
+                _key = f"/Rho/{subtype}"
+        elif task == "potential":
+            if subtype is None:
                 _key = "/Potential/TotalElectrostaticPotential"
-            else:
-                _key = f"/Potential/{key}"
-        elif task.lower() == "elf":
-            if key is None:
+            elif subtype == "TotalLocalPotential":
+                _key = f"/Potential/{subtype}"
+        elif task == "elf":
+            if subtype is None:
                 _key = "/ELF/TotalELF"
             else:
-                _key = f"/ELF/{key}"
-        elif task.lower() == "pcharge":
-            if key is None:
+                _key = f"/ELF/{subtype}"
+        elif task == "pcharge":
+            if subtype is None:
                 _key = "/Pcharge/1/TotalCharge"
             else:
-                _key = f"/Pcharge/1/{key}"
-        elif task.lower() == "rhoBound":
-            if key is None:
+                _key = f"/Pcharge/1/{subtype}"
+        elif task == "rhoBound":
+            if subtype is None:
                 _key = "/Rho"
             else:
-                _key = key
+                _key = subtype
 
         if _key not in hdict:
             raise KeyError(f"未找到{_key}键！")
+
+        # DS-PAW 数据写入h5 列优先
+        # h5py 从h5读取数据 默认行优先
+        # np.array(data_list) 默认行优先
+        # 所以这里先以 行优先 把 “h5 行优先 读进来的数据” 转成一维， 再以 列优先 转成 grid 对应的维度
         tmp_pot = np.asarray(hdict[_key]).reshape([-1, 1], order="C")
         ys = tmp_pot.reshape(grid, order="F")
 
     elif datafile.endswith(".json"):
         jfile = datafile
         with open(jfile, "r") as f:
             jdict = json.load(f)
         grid = jdict["AtomInfo"]["Grid"]
 
-        if task.lower() == "rho":
-            if key is None:
+        if task == "rho":
+            if subtype is None:
                 ys = np.asarray(jdict["Rho"]["TotalCharge"]).reshape(grid, order="F")
             else:
-                ys = np.asarray(jdict["Rho"][key]).reshape(grid, order="F")
-        elif task.lower() == "potential":
-            if key is None:
+                ys = np.asarray(jdict["Rho"][subtype]).reshape(grid, order="F")
+        elif task == "potential":
+            if subtype is None:
                 ys = np.asarray(
                     jdict["Potential"]["TotalElectrostaticPotential"]
                 ).reshape(grid, order="F")
             else:
-                ys = np.asarray(jdict["Potential"][key]).reshape(grid, order="F")
-        elif task.lower() == "elf":
-            if key is None:
+                ys = np.asarray(jdict["Potential"][subtype]).reshape(grid, order="F")
+        elif task == "elf":
+            if subtype is None:
                 ys = np.asarray(jdict["ELF"]["TotalELF"]).reshape(grid, order="F")
             else:
-                ys = np.asarray(jdict["ELF"][key]).reshape(grid, order="F")
-        elif task.lower() == "pcharge":
-            if key is None:
+                ys = np.asarray(jdict["ELF"][subtype]).reshape(grid, order="F")
+        elif task == "pcharge":
+            if subtype is None:
                 ys = np.asarray(jdict["Pcharge"][0]["TotalCharge"]).reshape(
                     grid, order="F"
                 )
             else:
-                ys = np.asarray(jdict["Pcharge"][0][key]).reshape(grid, order="F")
+                ys = np.asarray(jdict["Pcharge"][0][subtype]).reshape(grid, order="F")
         else:
-            if key is None:
+            if subtype is None:
                 ys = np.asarray(jdict["Rho"]).reshape(grid, order="F")
             else:
-                ys = np.asarray(jdict[key]).reshape(grid, order="F")
+                ys = np.asarray(jdict[subtype]).reshape(grid, order="F")
 
     else:
         raise TypeError("仅支持读取h5或json文件或直接传入数组！")
 
     all_axis = [0, 1, 2]
     all_axis.remove(axis)
     y = np.mean(ys, tuple(all_axis))
@@ -204,15 +211,15 @@
         子图编号.
         1. 动能
         2. 总能
         3. 压力
         4. 温度
         5. 体积
     raw : bool
-        是否输出原始数据到csv文件
+        是否输出绘图数据到csv文件
 
     Returns
     ----------
     figname : str
         图片路径，默认 'aimd.png'
 
     Examples
@@ -265,16 +272,15 @@
             axes[i].set_ylabel("Temperature (K)")
         else:
             axes[i].set_ylabel("Volume (Angstrom^3)")
 
     plt.tight_layout()
     # save and show
     if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.abspath(figname)), exist_ok=True)
         plt.savefig(figname, dpi=300)
         print(f"--> 图片已保存为 {os.path.abspath(figname)}")
     if show:
         plt.show()
 
 
 def plot_bandunfolding(
@@ -291,25 +297,25 @@
     ef : float
         费米能级，默认置于 y = 0 处
     de : float
         能带宽度，默认0.05
     dele : float
         能带间隔，默认0.06
     raw : bool
-        是否输出原始数据到rawbandunfolding.csv
+        是否输出绘图数据到rawbandunfolding.csv
 
     Returns
     -------
     axes: matplotlib.axes._subplots.AxesSubplot
         可传递给其他函数进行进一步处理
 
     Examples
     --------
 
-    绘图并保存原始数据到rawbandunfolding.csv
+    绘图并保存绘图数据到rawbandunfolding.csv
 
     >>> from dspawpy.plot import plot_bandunfolding
     >>> plot_bandunfolding("/data/home/hzw1002/dspawpy_repo/test/2.22/band.h5", raw=True)
     Reading /data/home/hzw1002/dspawpy_repo/test/2.22/band.h5...
     <module 'matplotlib.pyplot' from '/data/home/hzw1002/anaconda3/lib/python3.9/site-packages/matplotlib/pyplot.py'>
     """
     # search datafile in the given directory
@@ -396,15 +402,15 @@
     -------
     axes: matplotlib.axes._subplots.AxesSubplot
         可传递给其他函数进行进一步处理
 
     Examples
     --------
 
-    绘图并保存原始数据到rawoptical.csv
+    绘图并保存绘图数据到rawoptical.csv
 
     >>> from dspawpy.plot import plot_optical
     >>> plot_optical("/data/home/hzw1002/dspawpy_repo/test/2.12/scf.h5", "AbsorptionCoefficient", 0, raw=True)
     >>> plot_optical("/data/home/hzw1002/dspawpy_repo/test/2.12/optical.json", "AbsorptionCoefficient", 0, raw=True)
     """
     # search datafile in the given directory
     if os.path.isdir(datafile):
@@ -541,16 +547,15 @@
     plt.grid(alpha=0.2)
     plt.legend()
     plt.title("Thermal")
 
     plt.tight_layout()
     # save and show
     if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.abspath(figname)), exist_ok=True)
         plt.savefig(figname, dpi=300)
         print(f"--> 图片已保存为 {os.path.abspath(figname)}")
     if show:
         plt.show()
 
 
 def plot_polarization_figure(
@@ -664,16 +669,15 @@
 
         if raw:
             pd.DataFrame(ys, index=subfolders).to_csv(f"pol_{xyz[j]}.csv")
 
     plt.tight_layout()
     # save and show
     if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.abspath(figname)), exist_ok=True)
         plt.savefig(figname, dpi=300)
         print(f"--> 图片已保存为 {os.path.abspath(figname)}")
     if show:
         plt.show()
 
     return axes
```

## dspawpy/analysis/aimdtools.py

```diff
@@ -528,16 +528,15 @@
     if xlim:
         ax.set_xlim(xlim)
     if ylim:
         ax.set_ylim(ylim)
 
     plt.tight_layout()
     if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.abspath(figname)), exist_ok=True)
         plt.savefig(figname, dpi=300)
         print("MSD图片保存在", os.path.abspath(figname))
     if show and ishow:  # 画子图的话，不应每个子图都show
         plt.show()  # show会自动清空图片
 
     return ax
 
@@ -627,16 +626,15 @@
     if xlim:
         ax.set_xlim(xlim)
     if ylim:
         ax.set_ylim(ylim)
 
     plt.tight_layout()
     if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.abspath(figname)), exist_ok=True)
         plt.savefig(figname, dpi=300)
         print(f"图片已保存到 {os.path.abspath(figname)}")
     if show and ishow:  # 画子图的话，不应每个子图都show
         plt.show()  # show会自动清空图片
 
 
 def plot_rmsd(
@@ -707,15 +705,14 @@
     if xlim:
         ax.set_xlim(xlim)
     if ylim:
         ax.set_ylim(ylim)
 
     plt.tight_layout()
     if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.abspath(figname)), exist_ok=True)
         plt.savefig(figname, dpi=300)
         print(f"图片已保存到 {os.path.abspath(figname)}")
     if show and ishow:  # 画子图的话，不应每个子图都show
         plt.show()  # show会自动清空图片
 
     return ax
```

## dspawpy/diffusion/nebtools.py

```diff
@@ -145,15 +145,15 @@
     method : str, optional
         插值算法, 默认'PchipInterpolator'
     figname : str, optional
         能垒图名称, 默认'neb_barrier.png'
     show : bool, optional
         是否展示交互界面, 默认True
     raw : bool, optional
-        是否返回原始数据到csv
+        是否返回绘图数据到csv
 
     Raises
     ------
     ImportError
         指定了scipy.interpolate中不存在的插值算法
     ValueError
         传递给插值算法的参数不符合该算法要求
@@ -254,16 +254,15 @@
     plt.xlabel("Reaction Coordinate (Å)")
     plt.ylabel("Energy (eV)")
     plt.legend()
 
     plt.tight_layout()
     # save and show
     if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.abspath(figname)), exist_ok=True)
         plt.savefig(figname, dpi=300)
         print(f"--> 图片已保存为 {os.path.abspath(figname)}")
     if show:
         plt.show()
 
 
 def plot_neb_converge(
@@ -282,15 +281,15 @@
     image_key : str
         第几个构型，默认 "01"
     show : bool
         是否交互绘图
     image_name : str
         NEB收敛图名称，默认 "neb_conv.png"
     raw : bool
-        是否输出原始数据到csv文件
+        是否输出绘图数据到csv文件
 
     Returns
     -------
     ax1, ax2 : matplotlib.axes.Axes
         两个子图的Axes对象
 
     Examples
@@ -361,16 +360,15 @@
     ax2.set_ylabel("Energy (eV)")
     ax2.ticklabel_format(useOffset=False)  # y轴坐标显示绝对值而不是相对值
     fig.legend(loc=1, bbox_to_anchor=(1, 1), bbox_transform=ax1.transAxes)
 
     plt.tight_layout()
     # save and show
     if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.abspath(figname)), exist_ok=True)
         plt.savefig(figname, dpi=300)
         print(f"--> 图片已保存为 {os.path.abspath(figname)}")
     if show:
         plt.show()
 
     return ax1, ax2
```

## dspawpy/io/write.py

```diff
@@ -113,48 +113,64 @@
                         poses[i, 2],
                         i + 1,
                     )
                 )
     print(f"{dumpfile} 文件已保存！")
 
 
-def write_VESTA(in_filename: str, data_type, out_filename="DS-PAW.vesta"):
+def write_VESTA(in_filename: str, data_type, out_filename="DS-PAW.vesta", subtype=None):
     """从包含电子体系信息的json或h5文件中读取数据并写入VESTA格式的文件中
 
     Parameters
     ----------
     in_filename : str
         包含电子体系信息的json或h5文件路径
     data_type: str
         数据类型，支持 "rho", "potential", "elf", "pcharge", "rhoBound"
     out_filename : str
         输出文件路径, 默认 "DS-PAW.vesta"
+    subtype : str
+        用于指定data_type的数据子类型，目前仅支持 TotalLocalPotential（对应potential.type = total），默认为None，将读取 potential 的 TotalElectrostaticPotential 数据
 
     Returns
     --------
     out_filename : file
         VESTA格式的文件
 
     Examples
     --------
     >>> from dspawpy.io.write import write_VESTA
     >>> write_VESTA("/data/home/hzw1002/dspawpy_repo/test/2.2/rho.json", "rho", out_filename='/data/home/hzw1002/dspawpy_repo/test/out/rho.json')
     """
+    if subtype is not None:
+        assert (
+            data_type == "potential" and subtype == "TotalLocalPotential"
+        ), '目前仅支持"potential"的"TotalLocalPotential"子类'
+
     if in_filename.endswith(".h5"):
         data = load_h5(in_filename)
         if data_type == "rho" or data_type == "rhoBound":
             _write_VESTA_format(data, ["/Rho/TotalCharge"], out_filename)
         elif data_type == "potential":
-            _write_VESTA_format(
-                data,
-                [
-                    "/Potential/TotalElectrostaticPotential",
-                ],
-                out_filename,
-            )
+            if subtype == "TotalLocalPotential":
+                _write_VESTA_format(
+                    data,
+                    [
+                        "/Potential/TotalLocalPotential",
+                    ],
+                    out_filename,
+                )
+            else:
+                _write_VESTA_format(
+                    data,
+                    [
+                        "/Potential/TotalElectrostaticPotential",
+                    ],
+                    out_filename,
+                )
         elif data_type == "elf":
             _write_VESTA_format(data, ["/ELF/TotalELF"], out_filename)
         elif data_type == "pcharge":
             _write_VESTA_format(data, ["/Pcharge/1/TotalCharge"], out_filename)
         else:
             raise NotImplementedError("仅支持rho/potential/elf/pcharge/rhoBound")
 
@@ -162,21 +178,30 @@
         with open(in_filename, "r") as fin:
             data = json.load(fin)
         if data_type == "rho" or data_type == "rhoBound":
             _write_VESTA_format_json(
                 data["AtomInfo"], [data["Rho"]["TotalCharge"]], out_filename
             )
         elif data_type == "potential":
-            _write_VESTA_format_json(
-                data["AtomInfo"],
-                [
-                    data["Potential"]["TotalElectrostaticPotential"],
-                ],
-                out_filename,
-            )
+            if subtype == "TotalLocalPotential":
+                _write_VESTA_format_json(
+                    data["AtomInfo"],
+                    [
+                        data["Potential"]["TotalLocalPotential"],
+                    ],
+                    out_filename,
+                )
+            else:
+                _write_VESTA_format_json(
+                    data["AtomInfo"],
+                    [
+                        data["Potential"]["TotalElectrostaticPotential"],
+                    ],
+                    out_filename,
+                )
         elif data_type == "elf":
             _write_VESTA_format_json(
                 data["AtomInfo"], [data["ELF"]["TotalELF"]], out_filename
             )
         elif data_type == "pcharge":
             _write_VESTA_format_json(
                 data["AtomInfo"], [data["Pcharge"][0]["TotalCharge"]], out_filename
@@ -437,24 +462,24 @@
         "mcsqs",
         "yaml",
         "fleur-inpgen",
         "prismatic",
         "res",
     ]:
         if si:
-            structure[si].to(filename, fmt=fmt)
+            structure[si].to(filename=filename, fmt=fmt)
         else:
-            structure[-1].to(filename, fmt=fmt)
+            structure[-1].to(filename=filename, fmt=fmt)
 
     else:
         try:
             if si:
-                structure[si].to(filename)
+                structure[si].to(filename=filename)
             else:
-                structure[-1].to(filename)
+                structure[-1].to(filename=filename)
         except Exception as e:
             raise NotImplementedError(
                 f"除了 pdb, xyz, dump, json, as, hzw 六种格式外，其他格式一律移交 pymatgen 处理，然而\n--> pymatgen返回错误：{e}"
             )
 
     print(f"--> 成功写入文件 {os.path.abspath(filename)}")
```

## Comparing `dspawpy-1.0.0.dist-info/METADATA` & `dspawpy-1.0.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -32,14 +32,21 @@
 
 再重新用pip安装。
 
 详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
 
 ## 版本更新简述
 
+### 1.0.1
+
+- BUG修复： to_file绑定filename参数，避免老版本pymatgen的兼容性问题
+- BUG修复： average_along_axis的task参数改成大小写敏感，避免rhoBound任务类型解析错误
+- 功能强化： 将文件存入不存在的目录前，先创建（支持相对路径）
+- 功能强化： write_VESTA和average_along_axis增加subtype参数，指定TotalLocalPotential数据
+
 ### 1.0.0
 
 - BUG修复： 文件开头增加utf8编码声明
 - 功能强化： 电荷密度差分支持更多组分（不限二元）
 - 重要变更： io.utils的getZPE、getTSads、getTSgas函数，增加参数用于将计算结果存入文件
 - 重要变更： io.write.write_VESTA() data_type参数可选值从boundcharge改成rhoBound，且大小写敏感，从而保持与DS-PAW输出文件名相同
```

## Comparing `dspawpy-1.0.0.dist-info/RECORD` & `dspawpy-1.0.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-dspawpy/__init__.py,sha256=1febli7-GTHAsO2bjPYfYZvuBm0unC9UpL_XBptIG6I,49
-dspawpy/plot.py,sha256=cFlQdYN_OF9aMsYsfsUOkvbMdbfsFrWpR5MI3jlGmrs,32073
+dspawpy/__init__.py,sha256=VXg2fqcyJ7ncsvz1_mWntEY6sohgvbXekZ4ECgpQqWE,48
+dspawpy/plot.py,sha256=REZKrBxCEf8V6kaSUpSI2p0yINhTHH-UJ6XL4ZGFyoA,32128
 dspawpy/analysis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/analysis/aimdtools.py,sha256=GCoUrY4mTpIBs9Qm3dARpfqImqe4oLrxNliklaEgRTA,24376
+dspawpy/analysis/aimdtools.py,sha256=FtyLlo_hvhF8CSLBEYmCDe0ysfRqQI7bCX1Ms_GeeJA,24229
 dspawpy/analysis/vacf.py,sha256=Jj6t7D3FoxBKrjqkV4MVATcucKVW0mRG8aBAKdR6MQk,20177
 dspawpy/diffusion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/diffusion/neb.py,sha256=axFwZTg5HV_RIbZ1welrZAH_ayAH-4tswzjgkJZXugU,3986
-dspawpy/diffusion/nebtools.py,sha256=PpatcxYIcuCxg4M-Rc_VGXYyn3IQ8MIMVU-dCj9dm84,56985
+dspawpy/diffusion/nebtools.py,sha256=GGW43HDpHuUGnZXC3sZLvLUSHw-Mv712AKpR3feVPvw,56887
 dspawpy/diffusion/pathfinder.py,sha256=HhCVoh42Q2qIksBAruZ1atULfR5D55uzZvbaCtUxSig,11045
 dspawpy/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/io/read.py,sha256=tgcUjawulYsaR0x9aAsdvtNKlovUq7jLARYYQQ6v1DE,62556
 dspawpy/io/structure.py,sha256=DZfyoNBcWCeeJL2plJkwpQfPUiUUxmq3DdziFp2nS2w,10548
 dspawpy/io/utils.py,sha256=eWocKo11ApElBSFNrJ4QUuiVadQA2deyXpVQ9BrH7bE,27765
-dspawpy/io/write.py,sha256=GW6EkQJmUU_gps3aCVji9rCIFyNBI_VPZWCZlcsJffw,29270
-dspawpy-1.0.0.dist-info/METADATA,sha256=Zgex1wa9cRBrU6QQ9cLVpYsgN5M_x2oXlAR7XKz78eo,5169
-dspawpy-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dspawpy-1.0.0.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
-dspawpy-1.0.0.dist-info/RECORD,,
+dspawpy/io/write.py,sha256=D3b2dSKWskXwgzVXHqopQ4fz1jm9naBoRbl9Dlzc7LM,30401
+dspawpy-1.0.1.dist-info/METADATA,sha256=77MyK4yJ8GTZVQQV3dTmyZBdFqeqoTf60i-b9EwEs60,5579
+dspawpy-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dspawpy-1.0.1.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
+dspawpy-1.0.1.dist-info/RECORD,,
```

