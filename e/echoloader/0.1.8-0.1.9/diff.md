# Comparing `tmp/echoloader-0.1.8.tar.gz` & `tmp/echoloader-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoloader-0.1.8.tar", max compression
+gzip compressed data, was "echoloader-0.1.9.tar", max compression
```

## Comparing `echoloader-0.1.8.tar` & `echoloader-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       23 2022-01-11 17:35:35.818016 echoloader-0.1.8/echoloader/__init__.py
--rw-r--r--   0        0        0       79 2022-01-02 19:46:54.788914 echoloader-0.1.8/echoloader/__main__.py
--rw-r--r--   0        0        0    13627 2022-01-11 17:35:35.831013 echoloader-0.1.8/echoloader/watcher.py
--rw-r--r--   0        0        0      578 2022-01-11 17:35:35.824014 echoloader-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      927 2022-01-11 17:36:21.189915 echoloader-0.1.8/setup.py
--rw-r--r--   0        0        0      721 2022-01-11 17:36:21.189915 echoloader-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       23 2022-03-17 04:59:39.323495 echoloader-0.1.9/echoloader/__init__.py
+-rw-r--r--   0        0        0       79 2022-02-16 06:38:08.433882 echoloader-0.1.9/echoloader/__main__.py
+-rw-r--r--   0        0        0    13687 2022-03-17 04:56:44.633659 echoloader-0.1.9/echoloader/watcher.py
+-rw-r--r--   0        0        0      578 2022-03-17 04:59:39.316349 echoloader-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      927 2022-03-17 04:59:53.317504 echoloader-0.1.9/setup.py
+-rw-r--r--   0        0        0      721 2022-03-17 04:59:53.317504 echoloader-0.1.9/PKG-INFO
```

### Comparing `echoloader-0.1.8/echoloader/watcher.py` & `echoloader-0.1.9/echoloader/watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
 def anonymize_dicom(ds):
     # Populate required values for file meta information
     ds.remove_private_tags()
     ds.walk(person_data_callback)
     media = parse_dicom_pixel(ds)
     video = is_video(media)
-    ds.file_meta.TransferSyntaxUID = uid.JPEGExtended
+    ds.file_meta.TransferSyntaxUID = uid.JPEGBaseline8Bit
 
     ds.is_little_endian = True
     ds.is_implicit_VR = False
 
     ds.BitsStored = 8
     ds.BitsAllocated = 8
     ds.HighBit = 7
@@ -214,15 +214,15 @@
 
     def file_params(self, ds):
         customer = getattr(self.args, 'customer', '')
         return {
             'customer': customer,
             'trial': customer,
             'patient_id': ds.PatientID,
-            'visit_id': ds.StudyID,
+            'visit_id': ds.StudyID or ds.StudyInstanceUID or ds.StudyDate or 'No Study ID',
             'filename': f"{ds.SOPInstanceUID}.dcm",
         }
 
     def upload(self, ds, params):
         content_type = 'application/dicom'
         params['content_type'] = content_type
         headers = self.args.cognito.get_headers()
```

### Comparing `echoloader-0.1.8/pyproject.toml` & `echoloader-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "echoloader"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["mathias <mathias@us2.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7.5,<3.11"
 requests = "^2.26.0"
 watchdog = "^2.1.5"
```

### Comparing `echoloader-0.1.8/setup.py` & `echoloader-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'watchdog>=2.1.5,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['echoloader = echoloader.watcher:main']}
 
 setup_kwargs = {
     'name': 'echoloader',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'mathias',
     'author_email': 'mathias@us2.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `echoloader-0.1.8/PKG-INFO` & `echoloader-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoloader
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: mathias
 Author-email: mathias@us2.ai
 Requires-Python: >=3.7.5,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

