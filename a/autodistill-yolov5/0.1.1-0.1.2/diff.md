# Comparing `tmp/autodistill-yolov5-0.1.1.tar.gz` & `tmp/autodistill-yolov5-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-yolov5-0.1.1.tar", last modified: Thu Jun  8 14:01:43 2023, max compression
+gzip compressed data, was "autodistill-yolov5-0.1.2.tar", last modified: Fri Jun 30 10:05:12 2023, max compression
```

## Comparing `autodistill-yolov5-0.1.1.tar` & `autodistill-yolov5-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:01:43.086652 autodistill-yolov5-0.1.1/
--rw-r--r--   0 james      (501) staff       (20)    34522 2023-06-08 07:47:05.000000 autodistill-yolov5-0.1.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     2260 2023-06-08 14:01:43.086523 autodistill-yolov5-0.1.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1784 2023-06-08 07:46:20.000000 autodistill-yolov5-0.1.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:01:43.085539 autodistill-yolov5-0.1.1/autodistill_yolov5/
--rw-r--r--   0 james      (501) staff       (20)       74 2023-06-08 07:50:41.000000 autodistill-yolov5-0.1.1/autodistill_yolov5/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      904 2023-06-08 06:21:00.000000 autodistill-yolov5-0.1.1/autodistill_yolov5/yolov5_model.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:01:43.086344 autodistill-yolov5-0.1.1/autodistill_yolov5.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2260 2023-06-08 14:01:43.000000 autodistill-yolov5-0.1.1/autodistill_yolov5.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      301 2023-06-08 14:01:43.000000 autodistill-yolov5-0.1.1/autodistill_yolov5.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-08 14:01:43.000000 autodistill-yolov5-0.1.1/autodistill_yolov5.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       97 2023-06-08 14:01:43.000000 autodistill-yolov5-0.1.1/autodistill_yolov5.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       19 2023-06-08 14:01:43.000000 autodistill-yolov5-0.1.1/autodistill_yolov5.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-08 14:01:43.086698 autodistill-yolov5-0.1.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1163 2023-06-08 07:52:21.000000 autodistill-yolov5-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 10:05:12.718771 autodistill-yolov5-0.1.2/
+-rw-r--r--   0 james      (501) staff       (20)    34522 2023-06-08 07:47:05.000000 autodistill-yolov5-0.1.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2334 2023-06-30 10:05:12.718612 autodistill-yolov5-0.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1815 2023-06-30 10:01:48.000000 autodistill-yolov5-0.1.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 10:05:12.716576 autodistill-yolov5-0.1.2/autodistill_yolov5/
+-rw-r--r--   0 james      (501) staff       (20)       74 2023-06-30 10:03:10.000000 autodistill-yolov5-0.1.2/autodistill_yolov5/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      904 2023-06-08 06:21:00.000000 autodistill-yolov5-0.1.2/autodistill_yolov5/yolov5_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 10:05:12.717760 autodistill-yolov5-0.1.2/autodistill_yolov5.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2334 2023-06-30 10:05:12.000000 autodistill-yolov5-0.1.2/autodistill_yolov5.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      330 2023-06-30 10:05:12.000000 autodistill-yolov5-0.1.2/autodistill_yolov5.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-30 10:05:12.000000 autodistill-yolov5-0.1.2/autodistill_yolov5.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       97 2023-06-30 10:05:12.000000 autodistill-yolov5-0.1.2/autodistill_yolov5.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       23 2023-06-30 10:05:12.000000 autodistill-yolov5-0.1.2/autodistill_yolov5.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-30 10:05:12.718819 autodistill-yolov5-0.1.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1207 2023-06-30 10:05:05.000000 autodistill-yolov5-0.1.2/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 10:05:12.718219 autodistill-yolov5-0.1.2/src/
+-rw-r--r--   0 james      (501) staff       (20)       22 2023-06-30 10:01:35.000000 autodistill-yolov5-0.1.2/src/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)       39 2023-06-30 10:01:35.000000 autodistill-yolov5-0.1.2/src/hello.py
```

### Comparing `autodistill-yolov5-0.1.1/LICENSE` & `autodistill-yolov5-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-yolov5-0.1.1/PKG-INFO` & `autodistill-yolov5-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: autodistill-yolov5
-Version: 0.1.1
+Version: 0.1.2
 Summary: YOLOv5 module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-yolov5
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
   <p>
     <a align="center" href="" target="_blank">
       <img
         width="850"
-        src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.png"
+        src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.png?3"
       >
     </a>
   </p>
 </div>
 
 # Autodistill YOLOv5 Module
 
@@ -56,12 +56,12 @@
 
 # run inference on the new model
 pred = target_model.predict("./context_images_labeled/train/images/dog-7.jpg", conf=0.01)
 ```
 
 ## License
 
-The code in this repository is licensed under an 
+The code in this repository is licensed under an [AGPL 3.0 license](LICENSE).
 
 ## 🏆 Contributing
 
 We love your input! Please see the core Autodistill [contributing guide](https://github.com/autodistill/autodistill/blob/main/CONTRIBUTING.md) to get started. Thank you 🙏 to all our contributors!
```

### Comparing `autodistill-yolov5-0.1.1/README.md` & `autodistill-yolov5-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div align="center">
   <p>
     <a align="center" href="" target="_blank">
       <img
         width="850"
-        src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.png"
+        src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.png?3"
       >
     </a>
   </p>
 </div>
 
 # Autodistill YOLOv5 Module
 
@@ -41,12 +41,12 @@
 
 # run inference on the new model
 pred = target_model.predict("./context_images_labeled/train/images/dog-7.jpg", conf=0.01)
 ```
 
 ## License
 
-The code in this repository is licensed under an 
+The code in this repository is licensed under an [AGPL 3.0 license](LICENSE).
 
 ## 🏆 Contributing
 
-We love your input! Please see the core Autodistill [contributing guide](https://github.com/autodistill/autodistill/blob/main/CONTRIBUTING.md) to get started. Thank you 🙏 to all our contributors!
+We love your input! Please see the core Autodistill [contributing guide](https://github.com/autodistill/autodistill/blob/main/CONTRIBUTING.md) to get started. Thank you 🙏 to all our contributors!
```

### Comparing `autodistill-yolov5-0.1.1/autodistill_yolov5/yolov5_model.py` & `autodistill-yolov5-0.1.2/autodistill_yolov5/yolov5_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-yolov5-0.1.1/autodistill_yolov5.egg-info/PKG-INFO` & `autodistill-yolov5-0.1.2/autodistill_yolov5.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: autodistill-yolov5
-Version: 0.1.1
+Version: 0.1.2
 Summary: YOLOv5 module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-yolov5
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
   <p>
     <a align="center" href="" target="_blank">
       <img
         width="850"
-        src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.png"
+        src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.png?3"
       >
     </a>
   </p>
 </div>
 
 # Autodistill YOLOv5 Module
 
@@ -56,12 +56,12 @@
 
 # run inference on the new model
 pred = target_model.predict("./context_images_labeled/train/images/dog-7.jpg", conf=0.01)
 ```
 
 ## License
 
-The code in this repository is licensed under an 
+The code in this repository is licensed under an [AGPL 3.0 license](LICENSE).
 
 ## 🏆 Contributing
 
 We love your input! Please see the core Autodistill [contributing guide](https://github.com/autodistill/autodistill/blob/main/CONTRIBUTING.md) to get started. Thank you 🙏 to all our contributors!
```

### Comparing `autodistill-yolov5-0.1.1/setup.py` & `autodistill-yolov5-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,12 +27,12 @@
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

