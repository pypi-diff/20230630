# Comparing `tmp/llvd-3.0.4.tar.gz` & `tmp/llvd-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llvd-3.0.4.tar", last modified: Fri Jun 30 12:30:41 2023, max compression
+gzip compressed data, was "llvd-3.0.5.tar", last modified: Fri Jun 30 14:09:38 2023, max compression
```

## Comparing `llvd-3.0.4.tar` & `llvd-3.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-06-30 12:30:41.429427 llvd-3.0.4/
--rw-r--r--   0 df-4       (501) staff       (20)     1093 2023-03-16 10:32:53.000000 llvd-3.0.4/LICENSE
--rw-r--r--   0 df-4       (501) staff       (20)     5316 2023-06-30 12:30:41.429313 llvd-3.0.4/PKG-INFO
--rw-r--r--   0 df-4       (501) staff       (20)     4766 2023-03-16 10:32:53.000000 llvd-3.0.4/README.md
-drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-06-30 12:30:41.428517 llvd-3.0.4/llvd/
--rwxr-xr-x   0 df-4       (501) staff       (20)       90 2023-06-30 12:29:51.000000 llvd-3.0.4/llvd/__init__.py
--rw-r--r--   0 df-4       (501) staff       (20)    13880 2023-06-30 12:29:51.000000 llvd-3.0.4/llvd/app.py
--rw-r--r--   0 df-4       (501) staff       (20)     3200 2023-03-16 10:32:53.000000 llvd-3.0.4/llvd/cli.py
--rw-r--r--   0 df-4       (501) staff       (20)      555 2023-03-16 10:32:53.000000 llvd-3.0.4/llvd/config.py
--rw-r--r--   0 df-4       (501) staff       (20)     3572 2023-06-30 12:29:51.000000 llvd-3.0.4/llvd/downloader.py
--rw-r--r--   0 df-4       (501) staff       (20)      136 2023-03-16 10:32:53.000000 llvd-3.0.4/llvd/exceptions.py
--rw-r--r--   0 df-4       (501) staff       (20)      642 2023-06-30 12:07:01.000000 llvd-3.0.4/llvd/process_io.py
--rw-r--r--   0 df-4       (501) staff       (20)     1601 2023-03-16 10:32:53.000000 llvd-3.0.4/llvd/utils.py
-drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-06-30 12:30:41.429160 llvd-3.0.4/llvd.egg-info/
--rw-r--r--   0 df-4       (501) staff       (20)     5316 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/PKG-INFO
--rw-r--r--   0 df-4       (501) staff       (20)      323 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/SOURCES.txt
--rw-r--r--   0 df-4       (501) staff       (20)        1 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/dependency_links.txt
--rw-r--r--   0 df-4       (501) staff       (20)       39 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/entry_points.txt
--rw-r--r--   0 df-4       (501) staff       (20)      166 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/requires.txt
--rw-r--r--   0 df-4       (501) staff       (20)        5 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/top_level.txt
--rw-r--r--   0 df-4       (501) staff       (20)       38 2023-06-30 12:30:41.429467 llvd-3.0.4/setup.cfg
--rw-r--r--   0 df-4       (501) staff       (20)     1269 2023-03-16 10:32:53.000000 llvd-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:09:38.768085 llvd-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-30 14:09:22.000000 llvd-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-30 14:09:38.768085 llvd-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-30 14:09:22.000000 llvd-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:09:38.764085 llvd-3.0.5/llvd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14169 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/process_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:09:38.768085 llvd-3.0.5/llvd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:09:38.768085 llvd-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 14:09:22.000000 llvd-3.0.5/setup.py
```

### Comparing `llvd-3.0.4/LICENSE` & `llvd-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llvd-3.0.4/PKG-INFO` & `llvd-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: llvd
-Version: 3.0.4
+Version: 3.0.5
 Summary: Linkedin Learning Video Downloader CLI Tool
 Home-page: https://github.com/knowbee/llvd.git
 Author: Igwaneza Bruce
 Author-email: knowbeeinc@gmail.com
-License: UNKNOWN
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -184,9 +183,7 @@
     <img src="https://raw.githubusercontent.com/knowbee/hosting/master/assets/progress_llvd.png" width="auto" height="auto"/>
 </p>
 
 <a name="author"/>
 
 # Author
 Igwaneza Bruce
-
-
```

### Comparing `llvd-3.0.4/README.md` & `llvd-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `llvd-3.0.4/llvd/app.py` & `llvd-3.0.5/llvd/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,14 +369,22 @@
         except requests.exceptions.ConnectionError:
             click.echo(
                 click.style(
                     f"ConnectionError: There is a connection error. Please check your connectivity.\n",
                     fg="red",
                 )
             )
+        except json.decoder.JSONDecodeError: 
+            click.echo(
+               click.style(
+                            f"The course is locked, you probably"
+                            f"need a premium account",
+                            fg="red",
+                )
+            )
         except Exception as e:
             if os.path.exists(
                 f"{self.chapter_path}/{self.current_video_index:0=2d}. {clean_name(self.current_video_name)}.mp4"
             ):
                 os.remove(
                     f"{self.chapter_path}/{self.current_video_index:0=2d}. {clean_name(self.current_video_name)}.mp4"
                 )
```

### Comparing `llvd-3.0.4/llvd/cli.py` & `llvd-3.0.5/llvd/cli.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.4/llvd/config.py` & `llvd-3.0.5/llvd/config.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.4/llvd/downloader.py` & `llvd-3.0.5/llvd/downloader.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.4/llvd/process_io.py` & `llvd-3.0.5/llvd/process_io.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.4/llvd/utils.py` & `llvd-3.0.5/llvd/utils.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.4/llvd.egg-info/PKG-INFO` & `llvd-3.0.5/llvd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: llvd
-Version: 3.0.4
+Version: 3.0.5
 Summary: Linkedin Learning Video Downloader CLI Tool
 Home-page: https://github.com/knowbee/llvd.git
 Author: Igwaneza Bruce
 Author-email: knowbeeinc@gmail.com
-License: UNKNOWN
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -184,9 +183,7 @@
     <img src="https://raw.githubusercontent.com/knowbee/hosting/master/assets/progress_llvd.png" width="auto" height="auto"/>
 </p>
 
 <a name="author"/>
 
 # Author
 Igwaneza Bruce
-
-
```

### Comparing `llvd-3.0.4/setup.py` & `llvd-3.0.5/setup.py`

 * *Files identical despite different names*

