# Comparing `tmp/vgetpupil-1.0.3.tar.gz` & `tmp/vgetpupil-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgetpupil-1.0.3.tar", last modified: Thu Feb 16 00:25:06 2023, max compression
+gzip compressed data, was "dist\vgetpupil-1.0.4.tar", last modified: Thu Jun 29 22:49:06 2023, max compression
```

## Comparing `vgetpupil-1.0.3.tar` & `vgetpupil-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/
--rw-rw-rw-   0        0        0    11558 2021-07-25 22:50:49.000000 vgetpupil-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      617 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2022-12-19 20:22:11.000000 vgetpupil-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1026 2023-02-16 00:23:55.000000 vgetpupil-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/vgetpupil/
--rw-rw-rw-   0        0        0     7986 2023-02-16 00:23:55.000000 vgetpupil-1.0.3/vgetpupil/vget.py
--rw-rw-rw-   0        0        0        0 2021-07-25 22:36:52.000000 vgetpupil-1.0.3/vgetpupil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/vgetpupil.egg-info/
--rw-rw-rw-   0        0        0        1 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/vgetpupil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/vgetpupil.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-16 00:24:07.000000 vgetpupil-1.0.3/vgetpupil.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      617 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/vgetpupil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/vgetpupil.egg-info/requires.txt
--rw-rw-rw-   0        0        0      298 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/vgetpupil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-02-16 00:25:06.000000 vgetpupil-1.0.3/vgetpupil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/
+-rw-rw-rw-   0        0        0    11558 2023-03-26 20:13:24.000000 vgetpupil-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      617 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-03-26 20:13:24.000000 vgetpupil-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-06-29 22:48:43.000000 vgetpupil-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil/
+-rw-rw-rw-   0        0        0     8072 2023-06-29 22:47:04.000000 vgetpupil-1.0.4/vgetpupil/vget.py
+-rw-rw-rw-   0        0        0        0 2023-03-26 20:13:24.000000 vgetpupil-1.0.4/vgetpupil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 22:49:01.000000 vgetpupil-1.0.4/vgetpupil.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      617 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      298 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/top_level.txt
```

### Comparing `vgetpupil-1.0.3/LICENSE` & `vgetpupil-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vgetpupil-1.0.3/PKG-INFO` & `vgetpupil-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgetpupil
-Version: 1.0.3
+Version: 1.0.4
 Summary: pupil positions generator program
 Home-page: https://github.com/jtur044/vgetpupil.git
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: pupil positions generator program vgetpupil
 Platform: UNKNOWN
```

### Comparing `vgetpupil-1.0.3/README.md` & `vgetpupil-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vgetpupil-1.0.3/setup.py` & `vgetpupil-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to write the pupil positions data from input videos.'
 
 setup(
     name='vgetpupil',
-    version='1.0.3',
+    version='1.0.4',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/vgetpupil.git',
     description='pupil positions generator program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

### Comparing `vgetpupil-1.0.3/vgetpupil/vget.py` & `vgetpupil-1.0.4/vgetpupil/vget.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 
     done_str = '█' * done
     togo_str = '░' * togo
 
     sys.stdout.write(f'\r{title_input}: [{done_str}{togo_str}] {percent_done_round}% done')
 
 
+# This function is to change from frame count to frame time to be used as pupil time
 def frame_to_time(frame_number, frame_rate):
     return frame_number / frame_rate
 
 
 def main():
     parser = argparse.ArgumentParser(prog='vgetpupil',
                                      description='VGETPUPIL package.')
-    parser.add_argument('--version', action='version', version='1.0.3'),
+    parser.add_argument('--version', action='version', version='1.0.4'),
     parser.add_argument("-i", dest="input_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
                         help="input mp4 file", metavar="filename.mp4")
     parser.add_argument("-o", dest="output_filename", required=True, type=argparse.FileType('w'), default=sys.stdout,
                         help="output csv file", metavar="filename.csv")
     parser.add_argument("-e", dest="eye_id_input", required=False, type=int, default=None, help="eye id input",
                         metavar="0 or 1")
```

### Comparing `vgetpupil-1.0.3/vgetpupil.egg-info/PKG-INFO` & `vgetpupil-1.0.4/vgetpupil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgetpupil
-Version: 1.0.3
+Version: 1.0.4
 Summary: pupil positions generator program
 Home-page: https://github.com/jtur044/vgetpupil.git
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: pupil positions generator program vgetpupil
 Platform: UNKNOWN
```

