# Comparing `tmp/segment-lidar-0.1.5.tar.gz` & `tmp/segment-lidar-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-lidar-0.1.5.tar", last modified: Tue Jun 13 23:59:52 2023, max compression
+gzip compressed data, was "dist\segment-lidar-0.1.6.tar", last modified: Fri Jun 30 18:35:57 2023, max compression
```

## Comparing `segment-lidar-0.1.5.tar` & `segment-lidar-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 23:59:52.776556 segment-lidar-0.1.5/
--rw-rw-rw-   0        0        0     1246 2023-06-09 11:49:11.000000 segment-lidar-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     4885 2023-06-13 23:59:52.774556 segment-lidar-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4341 2023-06-13 23:53:42.000000 segment-lidar-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 23:59:52.724613 segment-lidar-0.1.5/segment_lidar/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.5/segment_lidar/__init__.py
--rw-rw-rw-   0        0        0    19008 2023-06-13 23:44:39.000000 segment-lidar-0.1.5/segment_lidar/samlidar.py
-drwxrwxrwx   0        0        0        0 2023-06-13 23:59:52.772608 segment-lidar-0.1.5/segment_lidar.egg-info/
--rw-rw-rw-   0        0        0     4885 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      170 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 23:59:52.776556 segment-lidar-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-06-13 23:17:14.000000 segment-lidar-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:35:57.456594 segment-lidar-0.1.6/
+-rw-rw-rw-   0        0        0     1608 2023-06-30 18:32:20.000000 segment-lidar-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     6286 2023-06-30 18:35:57.455596 segment-lidar-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5744 2023-06-30 18:32:20.000000 segment-lidar-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 18:35:57.415704 segment-lidar-0.1.6/segment_lidar/
+-rw-rw-rw-   0        0        0        0 2023-06-30 18:32:20.000000 segment-lidar-0.1.6/segment_lidar/__init__.py
+-rw-rw-rw-   0        0        0    19012 2023-06-30 18:33:58.000000 segment-lidar-0.1.6/segment_lidar/samlidar.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:35:57.453628 segment-lidar-0.1.6/segment_lidar.egg-info/
+-rw-rw-rw-   0        0        0     6286 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 18:35:57.456594 segment-lidar-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-06-30 18:33:17.000000 segment-lidar-0.1.6/setup.py
```

### Comparing `segment-lidar-0.1.5/LICENSE` & `segment-lidar-0.1.6/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 BSD 3-Clause License
 
-Copyright (c) 2023 Anass Yarroudh
+Copyright (c) 2023, University of Liège - Author: Anass Yarroudh (ayarroudh@uliege.be), Geomatics Unit of ULiege
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice,
    this list of conditions and the following disclaimer in the documentation
    and/or other materials provided with the distribution.
 
 3. Neither the name of the copyright holder nor the names of its
    contributors may be used to endorse or promote products derived from
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `segment-lidar-0.1.5/PKG-INFO` & `segment-lidar-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,19 @@
-Metadata-Version: 2.1
-Name: segment-lidar
-Version: 0.1.5
-Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
-Home-page: https://github.com/Yarroudh/segment-lidar
-Author: Anass Yarroudh
-Author-email: ayarroudh@uliege.be
-License: BSD 3-Clause "New" or "Revised" License
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
+[![read - documentation](https://img.shields.io/static/v1?label=read&message=documentation&color=orange)](https://yarroudh.gitbook.io/segment-lidar/)
 
-*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
+*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
-![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/1ed9c405-a305-46ff-827b-a70275733371)
-
+![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/089a603b-697e-4483-af1e-3687a79adcc1)
 
 ## Installation
 
 We recommand using `Python 3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
 
 Then, you can easily install `segment-lidar` from [PyPI](https://pypi.org/project/segment-lidar/):
 
@@ -39,53 +25,71 @@
 
 ```bash
 git clone https://github.com/Yarroudh/segment-lidar
 cd segment-lidar
 python setup.py install
 ```
 
-Please, note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
-
+Please, note that the actual version is always under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version should implement more advanced features and fonctionalities.
 
 ## Documentation
 
-If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](segment-lidar.readthedocs.io). The documentation is an essential resource that will help you understand the features and functionality of our software, as well as provide guidance on how to use it effectively.
+If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](https://yarroudh.gitbook.io/segment-lidar/). The documentation is an essential resource that will help you understand the features of the package, as well as provide guidance on how to use it effectively.
 
 ## Basic tutorial
 
-A basic tutorial is available [here]().
+A basic tutorial is available [here](https://yarroudh.gitbook.io/segment-lidar/tutorial/basic-usage).
 You can also refer to API for more information about different parameters.
 
 ```python
 from segment_lidar import samlidar
 
 model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
 points = model.read("pointcloud.las")
 cloud, non_ground, ground = model.csf(points)
-labels, *_ = instance.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
+labels, *_ = model.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
 model.write(points=points, non_ground=non_ground, ground=ground, segment_ids=labels, save_path="segmented.las")
 ```
 
 ## Sample data
 
 For testing purposes, you can download a sample here: [pointcloud.las](https://drive.google.com/file/d/16EF2aRSvo8u0pXvwtaQ6sjhP5h0sWw3o/view?usp=sharing).
 
-This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/)
-
+This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/).
 
 ## Related repositories
 
 We would like to express our acknowledgments to the creators of:
 
 - [segment-anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
-Please, visit these repositories for more information about image automatic segmentation using SAM from Meta AI.
+Please, visit these repositories for more information about image raster automatic segmentation using SAM from Meta AI.
 
 ## License
 
 This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
+## Citation
+
+The use of open-source software repositories has become increasingly prevalent in scientific research. If you use this repository for your research, please make sure to cite it appropriately in your work. The recommended citation format for this repository is provided in the accompanying [BibTeX citation](https://github.com/Yarroudh/segment-lidar/blob/main/CITATION.bib). Additionally, please make sure to comply with any licensing terms and conditions associated with the use of this repository.
+
+```bib
+@misc{yarroudh:2023:samlidar,
+  author = {Yarroudh, Anass},
+  title = {LiDAR Automatic Unsupervised Segmentation using Segment-Anything Model (SAM) from Meta AI},
+  year = {2023},
+  howpublished = {GitHub Repository},
+  url = {https://github.com/Yarroudh/segment-lidar}
+}
+```
+
+Yarroudh, A. (2023). *LiDAR Automatic Unsupervised Segmentation using Segment-Anything Model (SAM) from Meta AI* [GitHub repository]. Retrieved from https://github.com/Yarroudh/segment-lidar
+
 ## Author
 
-This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
+This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
 For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
+
+-----
+
+Copyright © 2023, [Geomatics Unit of ULiège](http://geomatics.ulg.ac.be/fr/home.php). Released under [BSD-3 Clause License](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `segment-lidar-0.1.5/README.md` & `segment-lidar-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,33 @@
+Metadata-Version: 2.1
+Name: segment-lidar
+Version: 0.1.6
+Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
+Home-page: https://github.com/Yarroudh/segment-lidar
+Author: Anass Yarroudh
+Author-email: ayarroudh@uliege.be
+License: BSD 3-Clause "New" or "Revised" License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
+[![read - documentation](https://img.shields.io/static/v1?label=read&message=documentation&color=orange)](https://yarroudh.gitbook.io/segment-lidar/)
 
-*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
+*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
-![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/1ed9c405-a305-46ff-827b-a70275733371)
-
+![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/089a603b-697e-4483-af1e-3687a79adcc1)
 
 ## Installation
 
 We recommand using `Python 3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
 
 Then, you can easily install `segment-lidar` from [PyPI](https://pypi.org/project/segment-lidar/):
 
@@ -25,53 +39,71 @@
 
 ```bash
 git clone https://github.com/Yarroudh/segment-lidar
 cd segment-lidar
 python setup.py install
 ```
 
-Please, note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
-
+Please, note that the actual version is always under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version should implement more advanced features and fonctionalities.
 
 ## Documentation
 
-If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](segment-lidar.readthedocs.io). The documentation is an essential resource that will help you understand the features and functionality of our software, as well as provide guidance on how to use it effectively.
+If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](https://yarroudh.gitbook.io/segment-lidar/). The documentation is an essential resource that will help you understand the features of the package, as well as provide guidance on how to use it effectively.
 
 ## Basic tutorial
 
-A basic tutorial is available [here]().
+A basic tutorial is available [here](https://yarroudh.gitbook.io/segment-lidar/tutorial/basic-usage).
 You can also refer to API for more information about different parameters.
 
 ```python
 from segment_lidar import samlidar
 
 model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
 points = model.read("pointcloud.las")
 cloud, non_ground, ground = model.csf(points)
-labels, *_ = instance.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
+labels, *_ = model.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
 model.write(points=points, non_ground=non_ground, ground=ground, segment_ids=labels, save_path="segmented.las")
 ```
 
 ## Sample data
 
 For testing purposes, you can download a sample here: [pointcloud.las](https://drive.google.com/file/d/16EF2aRSvo8u0pXvwtaQ6sjhP5h0sWw3o/view?usp=sharing).
 
-This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/)
-
+This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/).
 
 ## Related repositories
 
 We would like to express our acknowledgments to the creators of:
 
 - [segment-anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
-Please, visit these repositories for more information about image automatic segmentation using SAM from Meta AI.
+Please, visit these repositories for more information about image raster automatic segmentation using SAM from Meta AI.
 
 ## License
 
 This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
+## Citation
+
+The use of open-source software repositories has become increasingly prevalent in scientific research. If you use this repository for your research, please make sure to cite it appropriately in your work. The recommended citation format for this repository is provided in the accompanying [BibTeX citation](https://github.com/Yarroudh/segment-lidar/blob/main/CITATION.bib). Additionally, please make sure to comply with any licensing terms and conditions associated with the use of this repository.
+
+```bib
+@misc{yarroudh:2023:samlidar,
+  author = {Yarroudh, Anass},
+  title = {LiDAR Automatic Unsupervised Segmentation using Segment-Anything Model (SAM) from Meta AI},
+  year = {2023},
+  howpublished = {GitHub Repository},
+  url = {https://github.com/Yarroudh/segment-lidar}
+}
+```
+
+Yarroudh, A. (2023). *LiDAR Automatic Unsupervised Segmentation using Segment-Anything Model (SAM) from Meta AI* [GitHub repository]. Retrieved from https://github.com/Yarroudh/segment-lidar
+
 ## Author
 
-This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
-For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
+This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
+For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
+
+-----
+
+Copyright © 2023, [Geomatics Unit of ULiège](http://geomatics.ulg.ac.be/fr/home.php). Released under [BSD-3 Clause License](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `segment-lidar-0.1.5/segment_lidar/samlidar.py` & `segment-lidar-0.1.6/segment_lidar/samlidar.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,25 +383,26 @@
             lines = message.split('\n')
             print(lines[-2])
             print(lines[-1])
             exit()
 
         print(f'Writing the segmented point cloud to {save_path}...')
 
+        header = laspy.LasHeader(point_format=3, version="1.3")
+        lidar = laspy.LasData(header=header)
+        
         if ground is not None:
-            header = laspy.LasHeader(point_format=3, version="1.3")
-            lidar = laspy.LasData(header=header)
             indices = np.concatenate((non_ground, ground))
             lidar.xyz = points[indices]
             segment_ids = np.append(segment_ids, np.full(len(ground), -1))
             lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
             lidar.segment_id = segment_ids
         else:
             lidar.points = points
             lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
             lidar.segment_id = segment_ids
 
         lidar.write(save_path)
 
         end = time.time()
         print(f'Writing is completed in {end - start:.2f} seconds.\n')
-        return None
+        return None
```

### Comparing `segment-lidar-0.1.5/segment_lidar.egg-info/PKG-INFO` & `segment-lidar-0.1.6/segment_lidar.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -13,21 +13,21 @@
 License-File: LICENSE
 
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
+[![read - documentation](https://img.shields.io/static/v1?label=read&message=documentation&color=orange)](https://yarroudh.gitbook.io/segment-lidar/)
 
-*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
+*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
-![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/1ed9c405-a305-46ff-827b-a70275733371)
-
+![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/089a603b-697e-4483-af1e-3687a79adcc1)
 
 ## Installation
 
 We recommand using `Python 3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
 
 Then, you can easily install `segment-lidar` from [PyPI](https://pypi.org/project/segment-lidar/):
 
@@ -39,53 +39,71 @@
 
 ```bash
 git clone https://github.com/Yarroudh/segment-lidar
 cd segment-lidar
 python setup.py install
 ```
 
-Please, note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
-
+Please, note that the actual version is always under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version should implement more advanced features and fonctionalities.
 
 ## Documentation
 
-If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](segment-lidar.readthedocs.io). The documentation is an essential resource that will help you understand the features and functionality of our software, as well as provide guidance on how to use it effectively.
+If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](https://yarroudh.gitbook.io/segment-lidar/). The documentation is an essential resource that will help you understand the features of the package, as well as provide guidance on how to use it effectively.
 
 ## Basic tutorial
 
-A basic tutorial is available [here]().
+A basic tutorial is available [here](https://yarroudh.gitbook.io/segment-lidar/tutorial/basic-usage).
 You can also refer to API for more information about different parameters.
 
 ```python
 from segment_lidar import samlidar
 
 model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
 points = model.read("pointcloud.las")
 cloud, non_ground, ground = model.csf(points)
-labels, *_ = instance.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
+labels, *_ = model.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
 model.write(points=points, non_ground=non_ground, ground=ground, segment_ids=labels, save_path="segmented.las")
 ```
 
 ## Sample data
 
 For testing purposes, you can download a sample here: [pointcloud.las](https://drive.google.com/file/d/16EF2aRSvo8u0pXvwtaQ6sjhP5h0sWw3o/view?usp=sharing).
 
-This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/)
-
+This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/).
 
 ## Related repositories
 
 We would like to express our acknowledgments to the creators of:
 
 - [segment-anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
-Please, visit these repositories for more information about image automatic segmentation using SAM from Meta AI.
+Please, visit these repositories for more information about image raster automatic segmentation using SAM from Meta AI.
 
 ## License
 
 This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
+## Citation
+
+The use of open-source software repositories has become increasingly prevalent in scientific research. If you use this repository for your research, please make sure to cite it appropriately in your work. The recommended citation format for this repository is provided in the accompanying [BibTeX citation](https://github.com/Yarroudh/segment-lidar/blob/main/CITATION.bib). Additionally, please make sure to comply with any licensing terms and conditions associated with the use of this repository.
+
+```bib
+@misc{yarroudh:2023:samlidar,
+  author = {Yarroudh, Anass},
+  title = {LiDAR Automatic Unsupervised Segmentation using Segment-Anything Model (SAM) from Meta AI},
+  year = {2023},
+  howpublished = {GitHub Repository},
+  url = {https://github.com/Yarroudh/segment-lidar}
+}
+```
+
+Yarroudh, A. (2023). *LiDAR Automatic Unsupervised Segmentation using Segment-Anything Model (SAM) from Meta AI* [GitHub repository]. Retrieved from https://github.com/Yarroudh/segment-lidar
+
 ## Author
 
-This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
+This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
 For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
+
+-----
+
+Copyright © 2023, [Geomatics Unit of ULiège](http://geomatics.ulg.ac.be/fr/home.php). Released under [BSD-3 Clause License](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `segment-lidar-0.1.5/setup.py` & `segment-lidar-0.1.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from setuptools import setup, find_packages
-from setuptools.command.install import install
-import subprocess
-
-with open("requirements.txt", "r") as file:
-    requirements = file.read().splitlines()
-
-class CustomInstallCommand(install):
-    def run(self):
-        subprocess.call(['pip', 'install', '-r', 'requirements.txt'])
-        install.run(self)
-        try:
-            import CSF
-        except ImportError:
-            subprocess.call(['pip', 'install', 'git+https://github.com/jianboqi/CSF.git'])
-        from samgeo import SamGeo
-        from samgeo.text_sam import LangSAM
-
-setup(
-    name="segment-lidar",
-    version='0.1.5',
-    description="A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.",
-    long_description=open('README.md', encoding='utf-8').read(),
-    long_description_content_type='text/markdown',
-    license='BSD 3-Clause "New" or "Revised" License',
-    author='Anass Yarroudh',
-    author_email='ayarroudh@uliege.be',
-    url='https://github.com/Yarroudh/segment-lidar',
-    packages=find_packages(),
-    install_requires=requirements,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: BSD License",
-        "Operating System :: OS Independent",
-    ],
-    cmdclass={
-        'install': CustomInstallCommand,
-    }
-)
+from setuptools import setup, find_packages
+from setuptools.command.install import install
+import subprocess
+
+with open("requirements.txt", "r") as file:
+    requirements = file.read().splitlines()
+
+class CustomInstallCommand(install):
+    def run(self):
+        subprocess.call(['pip', 'install', '-r', 'requirements.txt'])
+        install.run(self)
+        try:
+            import CSF
+        except ImportError:
+            subprocess.call(['pip', 'install', 'git+https://github.com/jianboqi/CSF.git'])
+        from samgeo import SamGeo
+        from samgeo.text_sam import LangSAM
+
+setup(
+    name="segment-lidar",
+    version='0.1.6',
+    description="A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.",
+    long_description=open('README.md', encoding='utf-8').read(),
+    long_description_content_type='text/markdown',
+    license='BSD 3-Clause "New" or "Revised" License',
+    author='Anass Yarroudh',
+    author_email='ayarroudh@uliege.be',
+    url='https://github.com/Yarroudh/segment-lidar',
+    packages=find_packages(),
+    install_requires=requirements,
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+    ],
+    cmdclass={
+        'install': CustomInstallCommand,
+    }
+)
```

