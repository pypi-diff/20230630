# Comparing `tmp/robologs_ros_utils-0.1.1a29.tar.gz` & `tmp/robologs_ros_utils-0.1.1a30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robologs_ros_utils-0.1.1a29.tar", max compression
+gzip compressed data, was "robologs_ros_utils-0.1.1a30.tar", max compression
```

## Comparing `robologs_ros_utils-0.1.1a29.tar` & `robologs_ros_utils-0.1.1a30.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a29/README.md
--rw-r--r--   0        0        0     1608 2023-06-28 13:12:26.395066 robologs_ros_utils-0.1.1a29/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a29/robologs_ros_utils/__init__.py
--rw-r--r--   0        0        0     1156 2023-06-28 13:12:04.166783 robologs_ros_utils-0.1.1a29/robologs_ros_utils/cli.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/__init__.py
--rw-r--r--   0        0        0      523 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/argument_parsers.py
--rw-r--r--   0        0        0     2578 2023-06-27 11:55:49.889627 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/clip_rosbag.py
--rw-r--r--   0        0        0      399 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/commands.py
--rw-r--r--   0        0        0     2698 2023-06-27 11:55:58.437675 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/get_images_from_bag.py
--rw-r--r--   0        0        0     1052 2023-06-27 11:55:36.549553 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/get_summary_from_bag.py
--rw-r--r--   0        0        0     3029 2023-06-27 11:56:05.773716 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/get_videos_from_bag.py
--rw-r--r--   0        0        0     2669 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/ros_img_tools.py
--rw-r--r--   0        0        0    15655 2023-06-27 13:51:44.266140 robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/ros_utils.py
--rw-r--r--   0        0        0        0 2023-06-27 11:36:54.527450 robologs_ros_utils-0.1.1a29/robologs_ros_utils/utils/__init__.py
--rw-r--r--   0        0        0     4615 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a29/robologs_ros_utils/utils/file_utils.py
--rw-r--r--   0        0        0     1147 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a29/robologs_ros_utils/utils/img_utils.py
--rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a29/setup.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a29/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a30/README.md
+-rw-r--r--   0        0        0     1608 2023-06-30 14:12:15.433489 robologs_ros_utils-0.1.1a30/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a30/robologs_ros_utils/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-30 14:08:53.448134 robologs_ros_utils-0.1.1a30/robologs_ros_utils/cli.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/__init__.py
+-rw-r--r--   0        0        0      523 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/argument_parsers.py
+-rw-r--r--   0        0        0     2590 2023-06-29 10:14:57.985160 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/clip_rosbag.py
+-rw-r--r--   0        0        0      399 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/commands.py
+-rw-r--r--   0        0        0      884 2023-06-30 14:07:28.171561 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/get_csv_data_from_bag.py
+-rw-r--r--   0        0        0     2698 2023-06-27 11:55:58.437675 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/get_images_from_bag.py
+-rw-r--r--   0        0        0     1052 2023-06-27 11:55:36.549553 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/get_summary_from_bag.py
+-rw-r--r--   0        0        0     3029 2023-06-27 11:56:05.773716 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/get_videos_from_bag.py
+-rw-r--r--   0        0        0     2669 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/ros_img_tools.py
+-rw-r--r--   0        0        0    18132 2023-06-30 14:04:45.530465 robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/ros_utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:36:54.527450 robologs_ros_utils-0.1.1a30/robologs_ros_utils/utils/__init__.py
+-rw-r--r--   0        0        0     4615 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a30/robologs_ros_utils/utils/file_utils.py
+-rw-r--r--   0        0        0     1147 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a30/robologs_ros_utils/utils/img_utils.py
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a30/setup.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a30/PKG-INFO
```

### Comparing `robologs_ros_utils-0.1.1a29/pyproject.toml` & `robologs_ros_utils-0.1.1a30/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robologs-ros-utils"
-version = "0.1.1a29"
+version = "0.1.1a30"
 description = "robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities"
 authors = ["roboto.ai <info@roboto.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.2"
```

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/cli.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from inspect import getmembers
 
 import click
 
-#from robologs_ros_utils.sources.ros1.commands import ros
-from robologs_ros_utils.sources.ros1 import clip_rosbag, get_images_from_bag, get_summary_from_bag, get_videos_from_bag
+from robologs_ros_utils.sources.ros1 import clip_rosbag, get_images_from_bag, get_summary_from_bag, get_videos_from_bag, \
+    get_csv_data_from_bag
 
 
 @click.group(invoke_without_command=True)
 @click.pass_context
 def cli(ctx):
     if ctx.invoked_subcommand is None:
         click.echo(
@@ -26,14 +26,15 @@
         click.echo("")
 
 
 cli.add_command(get_images_from_bag.get_images)
 cli.add_command(get_videos_from_bag.get_videos)
 cli.add_command(get_summary_from_bag.get_summary)
 cli.add_command(clip_rosbag.clip_rosbag)
+cli.add_command(get_csv_data_from_bag.get_csv_data_from_bag)
 
 
 def main():
     cli()
 
 
 if __name__ == "__main__":
```

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/argument_parsers.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/argument_parsers.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/clip_rosbag.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/clip_rosbag.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 @click.option("--output", "-o", type=str, required=True, help="Output directory")
 @click.option("--topics", type=str, help="Topic names used for extraction, comma-separated list")
 @click.option("--start-time", type=float, help="Only extract from start time")
 @click.option("--end-time", type=float, help="Only extract until end time")
 @click.option("--name", type=str, help="Output name of rosbag, only is used when there is a single input bag")
 @click.option("--timestamp_type", type=str, help="valid values are [rosbag_ns, offset_s]", default="rosbag_ns")
 def clip_rosbag(input, output, topics, start_time, end_time, name, timestamp_type):
-    """Get images from Rosbag1 format"""
-
+    """Clip rosbags based on topics and timestamps"""
     input_path = input
     output_path = output
     topics = topics.split(",") if topics is not None else topics
     start_time = start_time if start_time is not None else start_time
     end_time = end_time if end_time is not None else end_time
     timestamp_type = timestamp_type
```

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/get_images_from_bag.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/get_images_from_bag.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/get_summary_from_bag.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/get_summary_from_bag.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/get_videos_from_bag.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/get_videos_from_bag.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/ros_img_tools.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/ros_img_tools.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/sources/ros1/ros_utils.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/sources/ros1/ros_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import glob
 import logging
 import os
 from typing import Optional, Union, Tuple
 
 import cv2
 import numpy as np
+import pandas as pd
+import shutil
+import click
 from bagpy import bagreader
 from PIL import Image
 from rosbag import Bag
 from rosbags.rosbag1 import Reader
 from rosbags.serde import deserialize_cdr, ros1_to_cdr
 from tqdm import tqdm
 
@@ -482,39 +485,113 @@
     if timestamp_type not in ["rosbag_ns", "offset_s"]:
         raise Exception(f"Robologs: invalid timestamp_type parameter: {timestamp_type}")
 
     with Bag(output_bag_path, "w") as outbag:
         msg_counter = 0
         first_time_stamp = -1
         for topic, msg, t in Bag(input_bag_path).read_messages():
-
             if first_time_stamp < 0:
                 first_time_stamp = t.to_nsec()
                 if timestamp_type == "offset_s":
                     if start_time:
                         start_time = convert_offset_s_to_rosbag_ns(
                             offset_s=start_time, first_rosbag_time_ns=first_time_stamp
                         )
+
                     if end_time:
                         end_time = convert_offset_s_to_rosbag_ns(
                             offset_s=end_time, first_rosbag_time_ns=first_time_stamp
                         )
 
             if topic_list:
                 if topic not in topic_list:
                     continue
 
             in_time_range, past_end_time = is_message_within_time_range(time_ns=t.to_nsec(),
                                                                         start_time_rosbag_ns=start_time,
                                                                         end_time_rosbag_ns=end_time)
 
-            # stop iterating over rosbag if we're past the user specified ent-time
+            # stop iterating over rosbag if we're past the user specified end-time
             if past_end_time:
                 break
 
             if not in_time_range:
                 continue
 
             msg_counter += 1
             outbag.write(topic, msg, t)
 
     return
+
+
+def get_all_topics(rosbag_list):
+    topic_list = list()
+    for rosbag_file in rosbag_list:
+        summary_dict = get_bag_info_from_file(rosbag_file)
+        if summary_dict:
+            if "topics" in summary_dict.keys():
+                topic_dict = get_topic_dict(summary_dict)
+                for key in topic_dict.keys():
+                    topic_list.append(key)
+    return topic_list
+
+
+def get_csv_data_from_bag(input_dir_or_file: str, output_dir: str, topic_list: list = None) -> None:
+    """
+    Extract CSV data from rosbag files and move the CSV files to the specified output directory.
+
+    This function can accept either a directory of rosbag files or a single rosbag file.
+
+    Parameters
+    ----------
+    input_dir_or_file : str
+        The directory containing the rosbag files or a path to a single rosbag file.
+    output_dir : str
+        The directory where the extracted CSV files should be moved.
+    topic_list : list, optional
+        List of topics to be extracted. If not provided, all topics will be extracted.
+
+    Returns
+    -------
+    None
+
+    """
+
+    if os.path.isfile(input_dir_or_file):
+        rosbag_files = [input_dir_or_file]
+    else:
+        # List of rosbag files
+        rosbag_files = glob.glob(os.path.join(input_dir_or_file, '*.bag'))
+
+    # Loop over each rosbag file
+    for rosbag_file in rosbag_files:    # List of rosbag files
+        bag = bagreader(rosbag_file)
+
+        # Get all topics
+        all_topics = get_all_topics([rosbag_file])
+
+        # If a topic list is specified, filter the topics
+        if topic_list is not None:
+            all_topics = [topic for topic in all_topics if topic in topic_list]
+
+        # Create subfolder in output directory with rosbag name (without .bag)
+        rosbag_name = os.path.basename(rosbag_file).replace('.bag', '')
+        rosbag_dir = os.path.join(output_dir, rosbag_name)
+        os.makedirs(rosbag_dir, exist_ok=True)
+
+        # Loop over each topic
+        for topic in all_topics:
+            data = bag.message_by_topic(topic)
+
+            if data:
+                # construct the full destination path, including the file name
+                destination = os.path.join(rosbag_dir, os.path.basename(data))
+
+                # move the file
+                shutil.move(data, destination)
+
+    return
+
+
+if __name__ == "__main__":
+    get_csv_data_from_bag('/home/yves/ros_data/', '/home/yves/ros_data/output/')
+
```

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/utils/file_utils.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a29/robologs_ros_utils/utils/img_utils.py` & `robologs_ros_utils-0.1.1a30/robologs_ros_utils/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a29/setup.py` & `robologs_ros_utils-0.1.1a30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'types-tqdm>=4.64.7.9,<5.0.0.0']
 
 entry_points = \
 {'console_scripts': ['robologs-ros-utils = robologs_ros_utils.cli:main']}
 
 setup_kwargs = {
     'name': 'robologs-ros-utils',
-    'version': '0.1.1a29',
+    'version': '0.1.1a30',
     'description': 'robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities',
     'long_description': '',
     'author': 'roboto.ai',
     'author_email': 'info@roboto.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `robologs_ros_utils-0.1.1a29/PKG-INFO` & `robologs_ros_utils-0.1.1a30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robologs-ros-utils
-Version: 0.1.1a29
+Version: 0.1.1a30
 Summary: robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities
 License: Apache-2.0
 Author: roboto.ai
 Author-email: info@roboto.ai
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

