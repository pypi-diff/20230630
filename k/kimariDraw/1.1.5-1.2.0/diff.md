# Comparing `tmp/kimariDraw-1.1.5.tar.gz` & `tmp/kimariDraw-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariDraw-1.1.5.tar", last modified: Thu Jun 29 16:04:47 2023, max compression
+gzip compressed data, was "kimariDraw-1.2.0.tar", last modified: Fri Jun 30 03:59:19 2023, max compression
```

## Comparing `kimariDraw-1.1.5.tar` & `kimariDraw-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.781459 kimariDraw-1.1.5/
--rw-rw-rw-   0        0        0     1086 2023-06-26 16:23:56.000000 kimariDraw-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      371 2023-06-29 16:04:47.781459 kimariDraw-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2550 2023-06-29 14:24:48.000000 kimariDraw-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.758398 kimariDraw-1.1.5/kimariDraw/
-drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.773439 kimariDraw-1.1.5/kimariDraw/Data/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/Data/__init__.py
--rw-rw-rw-   0        0        0     1145 2023-06-29 14:20:48.000000 kimariDraw-1.1.5/kimariDraw/Data/kd_data.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.777449 kimariDraw-1.1.5/kimariDraw/Parser/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/Parser/__init__.py
--rw-rw-rw-   0        0        0      913 2023-06-29 14:24:18.000000 kimariDraw-1.1.5/kimariDraw/Parser/kd_file.py
--rw-rw-rw-   0        0        0     2708 2023-06-29 15:59:51.000000 kimariDraw-1.1.5/kimariDraw/Parser/kd_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.779455 kimariDraw-1.1.5/kimariDraw/Plot/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/Plot/__init__.py
--rw-rw-rw-   0        0        0     2117 2023-06-29 15:59:14.000000 kimariDraw-1.1.5/kimariDraw/Plot/kd_plot.py
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/__init__.py
--rw-rw-rw-   0        0        0      777 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.770430 kimariDraw-1.1.5/kimariDraw.egg-info/
--rw-rw-rw-   0        0        0      371 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 16:04:47.782462 kimariDraw-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-06-29 16:02:14.000000 kimariDraw-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:59:19.011143 kimariDraw-1.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-26 16:23:56.000000 kimariDraw-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      371 2023-06-30 03:59:19.011143 kimariDraw-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2897 2023-06-30 03:59:09.000000 kimariDraw-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 03:59:18.989084 kimariDraw-1.2.0/kimariDraw/
+drwxrwxrwx   0        0        0        0 2023-06-30 03:59:19.000113 kimariDraw-1.2.0/kimariDraw/Data/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.2.0/kimariDraw/Data/__init__.py
+-rw-rw-rw-   0        0        0     1145 2023-06-30 03:05:08.000000 kimariDraw-1.2.0/kimariDraw/Data/kd_data.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:59:19.005127 kimariDraw-1.2.0/kimariDraw/Parser/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.2.0/kimariDraw/Parser/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-06-30 03:05:08.000000 kimariDraw-1.2.0/kimariDraw/Parser/kd_file.py
+-rw-rw-rw-   0        0        0     2710 2023-06-30 03:56:59.000000 kimariDraw-1.2.0/kimariDraw/Parser/kd_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:59:19.009138 kimariDraw-1.2.0/kimariDraw/Plot/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.2.0/kimariDraw/Plot/__init__.py
+-rw-rw-rw-   0        0        0     2890 2023-06-30 03:48:27.000000 kimariDraw-1.2.0/kimariDraw/Plot/kd_plot.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.2.0/kimariDraw/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-06-30 03:05:08.000000 kimariDraw-1.2.0/kimariDraw/main.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:59:18.997105 kimariDraw-1.2.0/kimariDraw.egg-info/
+-rw-rw-rw-   0        0        0      371 2023-06-30 03:59:18.000000 kimariDraw-1.2.0/kimariDraw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-06-30 03:59:18.000000 kimariDraw-1.2.0/kimariDraw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 03:59:18.000000 kimariDraw-1.2.0/kimariDraw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-30 03:59:18.000000 kimariDraw-1.2.0/kimariDraw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 03:59:18.000000 kimariDraw-1.2.0/kimariDraw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 03:59:18.000000 kimariDraw-1.2.0/kimariDraw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 03:59:19.011143 kimariDraw-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-06-30 03:59:09.000000 kimariDraw-1.2.0/setup.py
```

### Comparing `kimariDraw-1.1.5/LICENSE` & `kimariDraw-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.5/README.md` & `kimariDraw-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 使用 kimariDraw 绘制折线图需要一个 .kd 格式的文件。该文件应包含绘制折线图所需的数据和参数。以下是一个 .kd 文件的示例：
 
 ```basic
 # UNIT = Hartree
 # FIGURE_SIZE = 8, 4
 # COLOR_THEME = science
 # FONT_FAMILY = Arial
-# SAVE_IMAGE = png
+# PLOT_STYLE = line
 
 BEGIN
 1, 375.5
 2, 405.5
 3, 323.7
 4, 457.8
 5, 300.6
@@ -43,17 +43,17 @@
 END
 ```
 
 在示例中，以 `#` 开头的是文件的文件头，其包含了单位、画布的大小、颜色以及字体等参数，以 `=` 分隔。`BEGIN` 和 `END` 之间表示的数据行，数据行每行包含两个数，用逗号分隔，分别表示反应进度和能量。反应进度必须从 1 开始。注意，文件头和数据行的中间必须存在一个空格。
 
 - `UNIT:` 能量单位，例如 kJ/mol
 - `FIGURE_SIZE:` 画布大小，例如 8,6
-- `COLOR_THEME:` 颜色主题，例如 nature
-- `FONT_FAMILY:` 坐标字体，例如 Times New Roman
-- `SIVE_IMAGE:` 保存的图片格式，例如 PNG
+- `COLOR_THEME:` 颜色主题，例如 nature，不支持自定义颜色。可选择内置颜色主题，分别为 nature、science 和 normal
+- `FONT_FAMILY:` 坐标字体，例如 Times New Roman，只能使用系统已经安装过的字体
+- `PLOT_STYLE:` 绘制样式，例如 想要绘制折线图，则写上 line，暂不支持其他样式
 
 使用 kimariDraw 绘制折线图的命令如下：
 
 ```bash
 kimariDraw <filename>
 ```
 
@@ -65,14 +65,22 @@
 kimariDraw ./example/test2.kd -s test
 ```
 
 则可以在当前目录下得到 test.png:
 
 <img src="figure/test.png">
 
+目前仅支持三种内置的颜色主题。
+
+<img src="figure/figure1.png">
+
+<img src="figure/figure2.png">
+
+<img src="figure/figure3.png">
+
 ## 支持的参数
 
 kimariDraw 支持以下命令行参数：
 
 - `-s`, `--save_name`：指定输出文件名，默认为 figure.png
 
 ## 作者
```

### Comparing `kimariDraw-1.1.5/kimariDraw/Data/kd_data.py` & `kimariDraw-1.2.0/kimariDraw/Data/kd_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 
 
 class KDData:
 
-    def __init__(self, unit, figure_size, color_theme, font_family, save_image, num_data):
+    def __init__(self, unit, figure_size, color_theme, font_family, plot_style, num_data):
         self.unit = unit
         self.figure_size = figure_size
         self.color_theme = color_theme
         self.font_family = font_family
-        self.save_image = save_image
+        self.plot_style = plot_style
         self.num_Data = num_data
 
     def __str__(self):
-        return f"KDData(unit={self.unit}, figure_size={self.figure_size}, color_theme={self.color_theme}, font_family={self.font_family}, save_image={self.save_image}, num_data={self.num_Data})"
+        return f"KDData(unit={self.unit}, figure_size={self.figure_size}, color_theme={self.color_theme}, font_family={self.font_family}, plot_style={self.plot_style}, num_data={self.num_Data})"
 
     def get_num_x(self):
         """
         Returns the number of x-axis values
         """
         x = []
         for item in self.num_Data:
```

### Comparing `kimariDraw-1.1.5/kimariDraw/Parser/kd_file.py` & `kimariDraw-1.2.0/kimariDraw/Parser/kd_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,12 +19,12 @@
         """
         返回 KDDate 对象的数据列表
         """
         unit = self.header["unit"]
         figure_size = self.header["figure_size"]
         color_theme = self.header["color_theme"]
         font_family = self.header["font_family"]
-        save_image = self.header["save_image"]
+        plot_style = self.header["plot_style"]
         num_data = self.data
 
-        kd_data = KDData(unit, figure_size, color_theme, font_family, save_image, num_data)
+        kd_data = KDData(unit, figure_size, color_theme, font_family, plot_style, num_data)
         return kd_data
```

### Comparing `kimariDraw-1.1.5/kimariDraw/Parser/kd_parser.py` & `kimariDraw-1.2.0/kimariDraw/Parser/kd_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         if not self._validate():
             raise ValueError('Invalid KD file format')
 
         header = {'unit': None,
                   'figure_size': None,
                   'color_theme': None,
                   'font_family': None,
-                  'save_image': None}
+                  'plot_style': None}
 
         data = []
 
         with open(self.filepath, 'r', encoding="utf-8") as f:
             lines = f.readlines()
 
         # 解析文件头
@@ -80,7 +80,8 @@
                 x_str, y_str = line.strip().split(',')
                 x, y = float(x_str), float(y_str)
                 data.append((x, y))
             elif line.strip() == 'BEGIN':
                 data_started = True
 
         return header, data
+
```

### Comparing `kimariDraw-1.1.5/kimariDraw/Plot/kd_plot.py` & `kimariDraw-1.2.0/kimariDraw/Plot/kd_plot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
+from scipy.optimize import curve_fit
 from kimariDraw.Data.kd_data import KDData
 
 
-def kd_draw(data: KDData, save_name='figure'):
+def kd_draw(data: KDData, save_name='figure.png'):
     """
     使用 matplotlib 绘制能量折线图
     """
     # 设置全局字体
     plt.rcParams['font.family'] = data.font_family
     plt.rcParams['font.weight'] = 'bold'
     plt.rcParams['axes.linewidth'] = 1.5
@@ -16,46 +17,70 @@
     num_x = data.get_num_x()
     num_y = data.get_num_y()
 
     # 创建画布和子图对象
     fig, ax = plt.subplots(figsize=data.figure_size)
 
     # 设置 x 轴和 y 轴的范围
-    ax.set_xlim(0, np.max(num_x) + 1)
-    y_min = np.min(num_y) * 1.25 if np.min(num_y) < 0 else np.min(num_y) * 0.75
-    y_max = np.max(num_y) * 1.25 if np.max(num_y) > 0 else np.max(num_y) * 0.75
+    y_min = np.min(num_y)
+    y_max = np.max(num_y)
+    x_max = np.max(num_x)
+    x_min = np.min(num_x)
+    ax.set_xlim(0, x_max + 1)
+    # 处理最小值为 0 时，不扩展 y 轴范围的情况
+    if y_min == 0:
+        y_max *= 1.25 if y_max > 0 else 0.75
+        y_min = -15
+    else:
+        y_min *= 1.25 if y_min < 0 else 0.75
+        y_max *= 1.25 if y_max > 0 else 0.75
+
     ax.set_ylim(y_min, y_max)
 
+    # 更改颜色主题
+    colors = []
+    if data.color_theme == 'normal':
+        colors = ['black', 'black']
+    elif data.color_theme == 'nature':
+        colors = ['#0072B2', '#D55E00']
+    elif data.color_theme == 'science':
+        colors = ["#1b9e77", "#d95f02"]
+
     # 绘制平台
     # 绘制数据点
     # for i in range(len(num_x)):
     #    ax.scatter(num_x[i], num_y[i])
 
-    # 在每个数据点上绘制长度为 0.4 的水平线
+    # 在每个数据点上绘制长度为 0.4 的水平线，并在水平线上显示数字
     for i, (x, y) in enumerate(zip(num_x, num_y)):
-        ax.plot([x - 0.2, x + 0.2], [y, y], color='black', linewidth=3)
+        ax.plot([x - 0.2, x + 0.2], [y, y], color=colors[0], linewidth=3)
         if abs(y) > 100:
-            ax.text(x, y + 2, f"{y:.1f}", ha='center', va='bottom', fontweight='bold', fontsize=10)
+            ax.text(x, y + 2, f"{y:.1f}", ha='center', va='bottom', fontweight='bold', fontsize=10, color=colors[1])
         else:
-            ax.text(x, y + 0.5, f"{y:.1f}", ha='center', va='bottom', fontweight='bold', fontsize=10)
+            ax.text(x, y + 0.5, f"{y:.1f}", ha='center', va='bottom', fontweight='bold', fontsize=10, color=colors[1])
 
-    for i in range(len(num_x) - 1):
-        ax.plot([num_x[i]+0.2, num_x[i+1]-0.2], [num_y[i], num_y[i+1]],  color='black', linewidth=1, linestyle='--')
+    # 修改折线图样式，一种为折线图、另一种为曲线图
+    if data.plot_style == 'line':
+        for i in range(len(num_x) - 1):
+            ax.plot([num_x[i] + 0.2, num_x[i + 1] - 0.2], [num_y[i], num_y[i + 1]], color=colors[0], linewidth=1,
+                    linestyle='--')
+    elif data.plot_style == 'curve':
+        raise ValueError('不支持的绘图样式')
 
     # 设置 x 轴和 y 轴标签
     y_label = "Free Energy" + f" ({data.unit})"
     ax.set_xlabel("Reaction Coordinate", fontweight='bold', fontsize=14)
     ax.set_ylabel(y_label, fontweight='bold', fontsize=14)
 
     # 设置 x 轴和 y 轴坐标
     ax.tick_params(axis='x', color='white')
     ax.tick_params(axis='x', labelcolor='white')
 
     # 设置标题
     ax.set_title("Chemical Energy Profile", fontweight='bold', fontsize=16)
 
     # 保存路径
-    save_fig_url = save_name + "." + data.save_image
-    plt.savefig(save_fig_url, dpi=700)
+    plt.savefig(save_name, dpi=700)
 
     # 显示图像
     plt.show()
+
```

### Comparing `kimariDraw-1.1.5/kimariDraw/main.py` & `kimariDraw-1.2.0/kimariDraw/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from kimariDraw.Parser.kd_parser import KDFileParser
 from kimariDraw.Plot.kd_plot import kd_draw
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Draw energy profile plot using matplotlib')
     parser.add_argument('input_file', type=str, help='path to input data file')
-    parser.add_argument('-s', '--save_name', type=str, default='figure', help='name of the output image file')
+    parser.add_argument('-s', '--save_name', type=str, default='figure.png', help='name of the output image file')
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     # 读取数据    
     data = KDFileParser(args.input_file).parse().get_kd_data()
```

### Comparing `kimariDraw-1.1.5/setup.py` & `kimariDraw-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='kimariDraw',
-    version='1.1.5',
+    version='1.2.0',
     description='The application is used to draw the Energy Profile Map',
     author='kimariyb',
     author_email='kimariyb@163.com',
     url='https://github.com/kimariyb/kimariDraw',
     install_requires=[
         'numpy',
         'matplotlib',
```

