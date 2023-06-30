# Comparing `tmp/rest-api-supporter-0.0.8.tar.gz` & `tmp/rest-api-supporter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest-api-supporter-0.0.8.tar", last modified: Tue Jun 27 03:30:43 2023, max compression
+gzip compressed data, was "rest-api-supporter-0.0.9.tar", last modified: Tue Jun 27 10:03:59 2023, max compression
```

## Comparing `rest-api-supporter-0.0.8.tar` & `rest-api-supporter-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 03:30:43.513266 rest-api-supporter-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      817 2023-06-27 03:30:43.512266 rest-api-supporter-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      553 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 03:30:43.507266 rest-api-supporter-0.0.8/rest_api_supporter/
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/rest_api_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 03:30:43.510266 rest-api-supporter-0.0.8/rest_api_supporter/servers/
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/rest_api_supporter/servers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/rest_api_supporter/servers/flask_rest_api_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 03:30:43.511266 rest-api-supporter-0.0.8/rest_api_supporter/utils/
--rw-r--r--   0 root         (0) root         (0)      220 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/rest_api_supporter/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/rest_api_supporter/utils/base64_decode.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/rest_api_supporter/utils/base64_encode.py
--rw-r--r--   0 root         (0) root         (0)      387 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/rest_api_supporter/utils/get.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/rest_api_supporter/utils/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 03:30:43.509266 rest-api-supporter-0.0.8/rest_api_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      817 2023-06-27 03:30:43.000000 rest-api-supporter-0.0.8/rest_api_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      576 2023-06-27 03:30:43.000000 rest-api-supporter-0.0.8/rest_api_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 03:30:43.000000 rest-api-supporter-0.0.8/rest_api_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 03:30:43.000000 rest-api-supporter-0.0.8/rest_api_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-27 03:30:43.000000 rest-api-supporter-0.0.8/rest_api_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-27 03:30:43.000000 rest-api-supporter-0.0.8/rest_api_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 03:30:43.513266 rest-api-supporter-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-06-27 03:30:42.000000 rest-api-supporter-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:03:59.599592 rest-api-supporter-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      614 2023-06-27 10:03:59.598591 rest-api-supporter-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-27 10:03:58.000000 rest-api-supporter-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:03:59.596591 rest-api-supporter-0.0.9/rest_api_supporter/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-27 10:03:58.000000 rest-api-supporter-0.0.9/rest_api_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:03:59.598591 rest-api-supporter-0.0.9/rest_api_supporter/utils/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-06-27 10:03:58.000000 rest-api-supporter-0.0.9/rest_api_supporter/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-06-27 10:03:58.000000 rest-api-supporter-0.0.9/rest_api_supporter/utils/base64_decode.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-06-27 10:03:58.000000 rest-api-supporter-0.0.9/rest_api_supporter/utils/base64_encode.py
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-27 10:03:58.000000 rest-api-supporter-0.0.9/rest_api_supporter/utils/get.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-06-27 10:03:58.000000 rest-api-supporter-0.0.9/rest_api_supporter/utils/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:03:59.597591 rest-api-supporter-0.0.9/rest_api_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      614 2023-06-27 10:03:59.000000 rest-api-supporter-0.0.9/rest_api_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-27 10:03:59.000000 rest-api-supporter-0.0.9/rest_api_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 10:03:59.000000 rest-api-supporter-0.0.9/rest_api_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 10:03:59.000000 rest-api-supporter-0.0.9/rest_api_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-27 10:03:59.000000 rest-api-supporter-0.0.9/rest_api_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-27 10:03:59.000000 rest-api-supporter-0.0.9/rest_api_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 10:03:59.599592 rest-api-supporter-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-06-27 10:03:58.000000 rest-api-supporter-0.0.9/setup.py
```

### Comparing `rest-api-supporter-0.0.8/rest_api_supporter/utils/base64_decode.py` & `rest-api-supporter-0.0.9/rest_api_supporter/utils/base64_decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
                      #/9j/4AAQSkZJRgABAQ...2qjR37P/2Q==
 base64_decoded = base64_decode(full_encoded)
 print(type(base64_decoded)) #<class 'PIL.JpegImagePlugin.JpegImageFile'>
                             #<class 'bytes'>
                             #<class 'PIL.JpegImagePlugin.JpegImageFile'>
 '''
 def base64_decode(full_encoded):
-    if "base64," in full_encoded:
+    if isinstance(full_encoded, str) and "base64," in full_encoded:
         #print(full_encoded) #data:image/png;base64,/9j/4AAQSkZJRgABAQ...2qjR37P/2Q==
                              #data:audio/wav;base64,UklGRiTuAgBXQVZFZm...At84WACNZGwA=
         front = full_encoded.split('base64,')[0]
         encoded = full_encoded.split('base64,')[1]
         decoded = base64.b64decode(encoded)
         if "image" in front:
             image = Image.open(io.BytesIO(decoded))
```

### Comparing `rest-api-supporter-0.0.8/setup.py` & `rest-api-supporter-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='rest-api-supporter',
-	version='0.0.8',
+	version='0.0.9',
 	description='Rest api supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/rest-api-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

