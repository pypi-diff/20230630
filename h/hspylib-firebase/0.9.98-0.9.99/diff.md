# Comparing `tmp/hspylib-firebase-0.9.98.tar.gz` & `tmp/hspylib-firebase-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-firebase-0.9.98.tar", last modified: Wed May 17 17:34:27 2023, max compression
+gzip compressed data, was "hspylib-firebase-0.9.99.tar", last modified: Wed May 17 18:23:04 2023, max compression
```

## Comparing `hspylib-firebase-0.9.98.tar` & `hspylib-firebase-0.9.99.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.710077 hspylib-firebase-0.9.98/
--rw-r--r--   0 hjunior    (504) staff       (20)       95 2022-06-17 15:16:57.000000 hspylib-firebase-0.9.98/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-05-17 17:34:27.707313 hspylib-firebase-0.9.98/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      708 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.666035 hspylib-firebase-0.9.98/firebase/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      722 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.98/firebase/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      186 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4427 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.98/firebase/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.677038 hspylib-firebase-0.9.98/firebase/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      226 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6370 2023-04-25 19:05:44.000000 hspylib-firebase-0.9.98/firebase/core/agent_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4926 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.98/firebase/core/file_processor.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2923 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.98/firebase/core/firebase.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2644 2023-04-25 19:05:08.000000 hspylib-firebase-0.9.98/firebase/core/firebase_auth.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.682533 hspylib-firebase-0.9.98/firebase/domain/
--rw-r--r--   0 hjunior    (504) staff       (20)      172 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/domain/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3136 2023-05-17 17:32:46.000000 hspylib-firebase-0.9.98/firebase/domain/firebase_dto.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.687370 hspylib-firebase-0.9.98/firebase/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      173 2023-05-17 17:34:26.000000 hspylib-firebase-0.9.98/firebase/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      765 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.98/firebase/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.689740 hspylib-firebase-0.9.98/firebase/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)      130 2022-11-12 19:14:41.000000 hspylib-firebase-0.9.98/firebase/resources/application.properties
--rw-r--r--   0 hjunior    (504) staff       (20)      237 2022-02-18 20:00:37.000000 hspylib-firebase-0.9.98/firebase/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 17:34:27.704953 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      647 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-05-17 17:34:27.000000 hspylib-firebase-0.9.98/hspylib_firebase.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-05-17 17:34:27.710322 hspylib-firebase-0.9.98/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1864 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.98/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 18:23:04.623913 hspylib-firebase-0.9.99/
+-rw-r--r--   0 hjunior    (504) staff       (20)       95 2022-06-17 15:16:57.000000 hspylib-firebase-0.9.99/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-05-17 18:23:04.622780 hspylib-firebase-0.9.99/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      708 2023-05-17 18:23:03.000000 hspylib-firebase-0.9.99/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 18:23:04.592233 hspylib-firebase-0.9.99/firebase/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-05-17 18:23:03.000000 hspylib-firebase-0.9.99/firebase/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      722 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.99/firebase/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      186 2023-05-17 18:23:03.000000 hspylib-firebase-0.9.99/firebase/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4427 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.99/firebase/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 18:23:04.601205 hspylib-firebase-0.9.99/firebase/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      226 2023-05-17 18:23:03.000000 hspylib-firebase-0.9.99/firebase/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6370 2023-04-25 19:05:44.000000 hspylib-firebase-0.9.99/firebase/core/agent_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4918 2023-05-17 18:22:46.000000 hspylib-firebase-0.9.99/firebase/core/file_processor.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2943 2023-05-17 18:15:15.000000 hspylib-firebase-0.9.99/firebase/core/firebase.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2644 2023-04-25 19:05:08.000000 hspylib-firebase-0.9.99/firebase/core/firebase_auth.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 18:23:04.605361 hspylib-firebase-0.9.99/firebase/domain/
+-rw-r--r--   0 hjunior    (504) staff       (20)      172 2023-05-17 18:23:03.000000 hspylib-firebase-0.9.99/firebase/domain/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3136 2023-05-17 17:32:46.000000 hspylib-firebase-0.9.99/firebase/domain/firebase_dto.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 18:23:04.610081 hspylib-firebase-0.9.99/firebase/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      173 2023-05-17 18:23:03.000000 hspylib-firebase-0.9.99/firebase/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      765 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.99/firebase/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 18:23:04.611553 hspylib-firebase-0.9.99/firebase/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)      130 2022-11-12 19:14:41.000000 hspylib-firebase-0.9.99/firebase/resources/application.properties
+-rw-r--r--   0 hjunior    (504) staff       (20)      237 2022-02-18 20:00:37.000000 hspylib-firebase-0.9.99/firebase/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-17 18:23:04.621442 hspylib-firebase-0.9.99/hspylib_firebase.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-05-17 18:23:04.000000 hspylib-firebase-0.9.99/hspylib_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      647 2023-05-17 18:23:04.000000 hspylib-firebase-0.9.99/hspylib_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-05-17 18:23:04.000000 hspylib-firebase-0.9.99/hspylib_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-05-17 18:23:04.000000 hspylib-firebase-0.9.99/hspylib_firebase.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-05-17 18:23:04.000000 hspylib-firebase-0.9.99/hspylib_firebase.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-05-17 18:23:04.624094 hspylib-firebase-0.9.99/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1864 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.99/setup.py
```

### Comparing `hspylib-firebase-0.9.98/PKG-INFO` & `hspylib-firebase-0.9.99/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-firebase
-Version: 0.9.98
+Version: 0.9.99
 Summary: HsPyLib - Firebase integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-firebase/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.99/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.98/README.md` & `hspylib-firebase-0.9.99/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.99/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.98/firebase/__classpath__.py` & `hspylib-firebase-0.9.99/firebase/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.98/firebase/__main__.py` & `hspylib-firebase-0.9.99/firebase/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.98/firebase/core/agent_config.py` & `hspylib-firebase-0.9.99/firebase/core/agent_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.98/firebase/core/file_processor.py` & `hspylib-firebase-0.9.99/firebase/core/file_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         for f_path in file_paths:
             if os.path.exists(f_path):
                 if os.path.isfile(f_path):
                     sysout(f'%BLUE%Uploading file "{f_path}" to Firebase ...')
                     dto = FileProcessor._read_and_encode(f_path)
                     data.append(dto)
                 else:
-                    sysout(f'%BLUE%Uploading files from "{f_path}" to Firebase ...')
+                    sysout(f'%BLUE%Uploading files from directory "{f_path}" to Firebase ...')
                     all_files = next(os.walk(f_path))[2]
                     log.debug("\nGlob: %s \nFiles: %s", glob_exp, all_files)
                     for file in all_files:
                         filename = os.path.join(f_path, file)
                         if os.path.isfile(filename) and fnmatch(file, glob_exp or "*.*"):
                             dto = FileProcessor._read_and_encode(filename)
                             data.append(dto)
@@ -58,20 +58,18 @@
         if data:
             payload = FileProcessor._create_request(data)
             response = put(url, payload)
             check_not_none(response)
             if response.status_code != HttpCode.OK:
                 raise HTTPError(f"{response.status_code} - Unable to upload into={url} with json_string={payload}")
             paths = ", \n  |- ".join([f.path for f in data])
-
-            sysout(f"%EOL%%GREEN%File(s) [\n  |- {paths}\n] successfully uploaded to: {url}%NC%")
-
+            sysout(f"%EOL%%GREEN%File(s) [\n  |- {paths}\n] successfully uploaded to Firebase!%NC%")
             return len(data)
 
-        sysout(f"%ORANGE%No files were uploaded from {file_paths} %NC%")
+        syserr(f"No file has been uploaded from ${file_paths}!")
 
         return 0
 
     @staticmethod
     def download_files(url: str, dest_dir: str) -> int:
         """Download files from URL.
         :param url: the URL to download the files.
@@ -85,15 +83,15 @@
         if response.status_code != HttpCode.OK:
             raise HTTPError(f"{response.status_code} - Unable to download from={url} with response={response}")
         dto_list = FirebaseDto.from_json(response.body)
         if dto_list and len(dto_list) > 0:
             FileProcessor._decode_and_write(dest_dir, *dto_list)
             return len(dto_list)
 
-        sysout(f"%ORANGE%Database alias was not found in: {url} %NC%")
+        syserr(f"Database alias was not found in: {url} !")
 
         return 0
 
     @staticmethod
     def _read_and_encode(file_path: str) -> FirebaseDto:
         """Read and B64-encode a text file.
         :param file_path: the path to the encoding file.
```

### Comparing `hspylib-firebase-0.9.98/firebase/core/firebase.py` & `hspylib-firebase-0.9.99/firebase/core/firebase.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,25 +47,25 @@
         :param file_paths: the file paths to be uploaded. File paths will be filtered by glob expressions.
         :param glob_exp: the GLOB expressions to filter the input files/folders.
         """
         self._authenticate()
         url = f"{self.agent_config.url(db_alias)}.json"
         check_argument(len(file_paths) > 0, "Unable to upload file_paths (zero size).")
         log.debug("Uploading files  alias=%s  files=[%s]", db_alias, ",".join(file_paths))
-        return self.processor.upload_files(url, file_paths, glob_exp) > 0
+        return self.processor.upload_files(db_alias, url, file_paths, glob_exp) > 0
 
     def download(self, db_alias: str, dest_dir: str) -> bool:
         """Download specified aliased files from firebase.
         :param db_alias: the database alias to download from.
         :param dest_dir: the destination directory.
         """
         self._authenticate()
         url = f"{self.agent_config.url(db_alias)}.json"
         log.debug("Downloading files  alias=%s  dest_dir=%s", db_alias, dest_dir)
-        return self.processor.download_files(url, dest_dir or os.environ.get("HOME")) > 0
+        return self.processor.download_files(db_alias, url, dest_dir or os.environ.get("HOME")) > 0
 
     def is_configured(self) -> bool:
         """Checks whether firebase is properly configured or not."""
         return self.agent_config is not None and self.agent_config.firebase_configs is not None
 
     def _authenticate(self) -> None:
         """Authenticate to Firebase using the user UID."""
```

### Comparing `hspylib-firebase-0.9.98/firebase/core/firebase_auth.py` & `hspylib-firebase-0.9.99/firebase/core/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.98/firebase/domain/firebase_dto.py` & `hspylib-firebase-0.9.99/firebase/domain/firebase_dto.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.98/firebase/exception/exceptions.py` & `hspylib-firebase-0.9.99/firebase/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.98/hspylib_firebase.egg-info/PKG-INFO` & `hspylib-firebase-0.9.99/hspylib_firebase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-firebase
-Version: 0.9.98
+Version: 0.9.99
 Summary: HsPyLib - Firebase integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-firebase/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.99/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.98/hspylib_firebase.egg-info/SOURCES.txt` & `hspylib-firebase-0.9.99/hspylib_firebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.98/setup.py` & `hspylib-firebase-0.9.99/setup.py`

 * *Files identical despite different names*

