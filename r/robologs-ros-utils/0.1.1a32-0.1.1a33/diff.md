# Comparing `tmp/robologs_ros_utils-0.1.1a32.tar.gz` & `tmp/robologs_ros_utils-0.1.1a33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robologs_ros_utils-0.1.1a32.tar", max compression
+gzip compressed data, was "robologs_ros_utils-0.1.1a33.tar", max compression
```

## Comparing `robologs_ros_utils-0.1.1a32.tar` & `robologs_ros_utils-0.1.1a33.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a32/README.md
--rw-r--r--   0        0        0     1608 2023-06-30 14:34:09.194708 robologs_ros_utils-0.1.1a32/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a32/robologs_ros_utils/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-30 14:08:53.448134 robologs_ros_utils-0.1.1a32/robologs_ros_utils/cli.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/__init__.py
--rw-r--r--   0        0        0      523 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/argument_parsers.py
--rw-r--r--   0        0        0     2590 2023-06-29 10:14:57.985160 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/clip_rosbag.py
--rw-r--r--   0        0        0      399 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/commands.py
--rw-r--r--   0        0        0     1075 2023-06-30 14:34:00.582649 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/get_csv_data_from_bag.py
--rw-r--r--   0        0        0     2698 2023-06-27 11:55:58.437675 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/get_images_from_bag.py
--rw-r--r--   0        0        0     1052 2023-06-27 11:55:36.549553 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/get_summary_from_bag.py
--rw-r--r--   0        0        0     3029 2023-06-27 11:56:05.773716 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/get_videos_from_bag.py
--rw-r--r--   0        0        0     2669 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/ros_img_tools.py
--rw-r--r--   0        0        0    18021 2023-06-30 14:23:32.998278 robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/ros_utils.py
--rw-r--r--   0        0        0        0 2023-06-27 11:36:54.527450 robologs_ros_utils-0.1.1a32/robologs_ros_utils/utils/__init__.py
--rw-r--r--   0        0        0     4615 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a32/robologs_ros_utils/utils/file_utils.py
--rw-r--r--   0        0        0     1147 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a32/robologs_ros_utils/utils/img_utils.py
--rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a32/setup.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a32/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a33/README.md
+-rw-r--r--   0        0        0     1608 2023-06-30 14:42:43.038215 robologs_ros_utils-0.1.1a33/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a33/robologs_ros_utils/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-30 14:08:53.448134 robologs_ros_utils-0.1.1a33/robologs_ros_utils/cli.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/__init__.py
+-rw-r--r--   0        0        0      523 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/argument_parsers.py
+-rw-r--r--   0        0        0     2590 2023-06-29 10:14:57.985160 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/clip_rosbag.py
+-rw-r--r--   0        0        0      399 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/commands.py
+-rw-r--r--   0        0        0     1123 2023-06-30 14:42:29.962126 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/get_csv_data_from_bag.py
+-rw-r--r--   0        0        0     2698 2023-06-27 11:55:58.437675 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/get_images_from_bag.py
+-rw-r--r--   0        0        0     1052 2023-06-27 11:55:36.549553 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/get_summary_from_bag.py
+-rw-r--r--   0        0        0     3029 2023-06-27 11:56:05.773716 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/get_videos_from_bag.py
+-rw-r--r--   0        0        0     2669 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/ros_img_tools.py
+-rw-r--r--   0        0        0    18021 2023-06-30 14:23:32.998278 robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/ros_utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:36:54.527450 robologs_ros_utils-0.1.1a33/robologs_ros_utils/utils/__init__.py
+-rw-r--r--   0        0        0     4615 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a33/robologs_ros_utils/utils/file_utils.py
+-rw-r--r--   0        0        0     1147 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a33/robologs_ros_utils/utils/img_utils.py
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a33/setup.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a33/PKG-INFO
```

### Comparing `robologs_ros_utils-0.1.1a32/pyproject.toml` & `robologs_ros_utils-0.1.1a33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robologs-ros-utils"
-version = "0.1.1a32"
+version = "0.1.1a33"
 description = "robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities"
 authors = ["roboto.ai <info@roboto.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.2"
```

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/cli.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/cli.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/argument_parsers.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/argument_parsers.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/clip_rosbag.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/clip_rosbag.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/get_csv_data_from_bag.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/get_csv_data_from_bag.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 
 from robologs_ros_utils.sources.ros1 import ros_utils
 from robologs_ros_utils.utils import file_utils
 
 
 def process_topics(ctx, param, value):
     """Callback function to process topics input."""
-    return [topic.strip() for topic in value.split(',')]
+    if value:
+        return [topic.strip() for topic in value.split(',')]
+    else:
+        return None
 
 
 @click.command()
 @click.option("--input", "-i", type=str, required=True, help="A single rosbag, or directory containing rosbags")
 @click.option("--output", "-o", type=str, required=True, help="Output directory for CSV files")
 @click.option("--topics", "-t", type=str, default=None, callback=process_topics, help="Comma-separated list of topics to extract")
 def get_csv_data_from_bag(input, output, topics):
```

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/get_images_from_bag.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/get_images_from_bag.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/get_summary_from_bag.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/get_summary_from_bag.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/get_videos_from_bag.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/get_videos_from_bag.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/ros_img_tools.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/ros_img_tools.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/sources/ros1/ros_utils.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/sources/ros1/ros_utils.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/utils/file_utils.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/robologs_ros_utils/utils/img_utils.py` & `robologs_ros_utils-0.1.1a33/robologs_ros_utils/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a32/setup.py` & `robologs_ros_utils-0.1.1a33/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'types-tqdm>=4.64.7.9,<5.0.0.0']
 
 entry_points = \
 {'console_scripts': ['robologs-ros-utils = robologs_ros_utils.cli:main']}
 
 setup_kwargs = {
     'name': 'robologs-ros-utils',
-    'version': '0.1.1a32',
+    'version': '0.1.1a33',
     'description': 'robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities',
     'long_description': '',
     'author': 'roboto.ai',
     'author_email': 'info@roboto.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `robologs_ros_utils-0.1.1a32/PKG-INFO` & `robologs_ros_utils-0.1.1a33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robologs-ros-utils
-Version: 0.1.1a32
+Version: 0.1.1a33
 Summary: robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities
 License: Apache-2.0
 Author: roboto.ai
 Author-email: info@roboto.ai
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

