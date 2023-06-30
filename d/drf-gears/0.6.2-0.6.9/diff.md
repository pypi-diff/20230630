# Comparing `tmp/drf_gears-0.6.2.tar.gz` & `tmp/drf-gears-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_gears-0.6.2.tar", last modified: Mon Aug 29 11:58:38 2022, max compression
+gzip compressed data, was "drf-gears-0.6.9.tar", last modified: Wed Aug 31 19:33:46 2022, max compression
```

## Comparing `drf_gears-0.6.2.tar` & `drf-gears-0.6.9.tar`

### file list

```diff
@@ -1,42 +1,37 @@
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-29 11:58:38.644617 drf_gears-0.6.2/
--rw-r--r--   0 alexander   (501) staff       (20)     1073 2020-12-07 15:50:01.000000 drf_gears-0.6.2/LICENSE
--rw-r--r--   0 alexander   (501) staff       (20)       17 2020-12-07 15:39:16.000000 drf_gears-0.6.2/MANIFEST.in
--rw-r--r--   0 alexander   (501) staff       (20)     6699 2022-08-29 11:58:38.644743 drf_gears-0.6.2/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     6124 2022-08-24 14:13:47.000000 drf_gears-0.6.2/README.md
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-29 11:58:38.572327 drf_gears-0.6.2/app/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-22 16:57:16.000000 drf_gears-0.6.2/app/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)       63 2022-08-22 16:57:16.000000 drf_gears-0.6.2/app/admin.py
--rw-r--r--   0 alexander   (501) staff       (20)      138 2022-08-22 16:57:17.000000 drf_gears-0.6.2/app/apps.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-29 11:58:38.578539 drf_gears-0.6.2/app/migrations/
--rw-r--r--   0 alexander   (501) staff       (20)      822 2022-08-22 17:07:37.000000 drf_gears-0.6.2/app/migrations/0001_initial.py
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-22 16:57:16.000000 drf_gears-0.6.2/app/migrations/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      239 2022-08-22 17:05:28.000000 drf_gears-0.6.2/app/models.py
--rw-r--r--   0 alexander   (501) staff       (20)       60 2022-08-22 16:57:16.000000 drf_gears-0.6.2/app/tests.py
--rw-r--r--   0 alexander   (501) staff       (20)      184 2022-08-22 17:05:28.000000 drf_gears-0.6.2/app/views.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-29 11:58:38.633496 drf_gears-0.6.2/config/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 19:37:37.000000 drf_gears-0.6.2/config/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 drf_gears-0.6.2/config/asgi.py
--rw-r--r--   0 alexander   (501) staff       (20)     4231 2022-08-22 17:05:59.000000 drf_gears-0.6.2/config/settings.py
--rw-r--r--   0 alexander   (501) staff       (20)      746 2021-07-13 19:50:10.000000 drf_gears-0.6.2/config/urls.py
--rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 drf_gears-0.6.2/config/wsgi.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-29 11:58:38.635103 drf_gears-0.6.2/drf_gears.egg-info/
--rw-r--r--   0 alexander   (501) staff       (20)     6699 2022-08-29 11:58:38.000000 drf_gears-0.6.2/drf_gears.egg-info/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)      697 2022-08-29 11:58:38.000000 drf_gears-0.6.2/drf_gears.egg-info/SOURCES.txt
--rw-r--r--   0 alexander   (501) staff       (20)        1 2022-08-29 11:58:38.000000 drf_gears-0.6.2/drf_gears.egg-info/dependency_links.txt
--rw-r--r--   0 alexander   (501) staff       (20)       17 2022-08-29 11:58:38.000000 drf_gears-0.6.2/drf_gears.egg-info/top_level.txt
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-29 11:58:38.635983 drf_gears-0.6.2/gears/
--rw-r--r--   0 alexander   (501) staff       (20)      380 2022-08-24 19:36:19.000000 drf_gears-0.6.2/gears/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      523 2022-08-22 18:21:05.000000 drf_gears-0.6.2/gears/mixins.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-29 11:58:38.640478 drf_gears-0.6.2/gears/renderers/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-24 19:26:03.000000 drf_gears-0.6.2/gears/renderers/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     3034 2022-08-29 11:58:03.000000 drf_gears-0.6.2/gears/renderers/exception_handlers.py
--rw-r--r--   0 alexander   (501) staff       (20)      314 2022-08-24 19:36:40.000000 drf_gears-0.6.2/gears/renderers/mapping.py
--rw-r--r--   0 alexander   (501) staff       (20)     1795 2022-08-24 13:49:40.000000 drf_gears-0.6.2/gears/renderers/renderer.py
--rw-r--r--   0 alexander   (501) staff       (20)      385 2022-08-23 17:54:18.000000 drf_gears-0.6.2/gears/renderers/types.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-29 11:58:38.644074 drf_gears-0.6.2/gears/viewsets/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-24 19:26:03.000000 drf_gears-0.6.2/gears/viewsets/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      724 2022-08-22 18:21:05.000000 drf_gears-0.6.2/gears/viewsets/permissions.py
--rw-r--r--   0 alexander   (501) staff       (20)     1096 2022-08-22 18:21:05.000000 drf_gears-0.6.2/gears/viewsets/querysets.py
--rw-r--r--   0 alexander   (501) staff       (20)     1153 2022-08-22 18:21:05.000000 drf_gears-0.6.2/gears/viewsets/serializers.py
--rw-r--r--   0 alexander   (501) staff       (20)       79 2022-08-29 11:58:38.645159 drf_gears-0.6.2/setup.cfg
--rw-r--r--   0 alexander   (501) staff       (20)      934 2022-08-29 11:58:30.000000 drf_gears-0.6.2/setup.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.297888 drf-gears-0.6.9/
+-rw-r--r--   0 alexander   (501) staff       (20)     1069 2022-08-31 14:23:16.000000 drf-gears-0.6.9/LICENSE
+-rw-r--r--   0 alexander   (501) staff       (20)     9864 2022-08-31 19:33:46.297608 drf-gears-0.6.9/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     8080 2022-08-31 06:54:14.000000 drf-gears-0.6.9/README.md
+-rw-r--r--   0 alexander   (501) staff       (20)      552 2022-08-31 19:33:36.000000 drf-gears-0.6.9/pyproject.toml
+-rw-r--r--   0 alexander   (501) staff       (20)       38 2022-08-31 19:33:46.297980 drf-gears-0.6.9/setup.cfg
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.284198 drf-gears-0.6.9/src/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 17:27:37.000000 drf-gears-0.6.9/src/__init__.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.285231 drf-gears-0.6.9/src/drf_gears.egg-info/
+-rw-r--r--   0 alexander   (501) staff       (20)     9864 2022-08-31 19:33:46.000000 drf-gears-0.6.9/src/drf_gears.egg-info/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)      723 2022-08-31 19:33:46.000000 drf-gears-0.6.9/src/drf_gears.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander   (501) staff       (20)        1 2022-08-31 19:33:46.000000 drf-gears-0.6.9/src/drf_gears.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       15 2022-08-31 19:33:46.000000 drf-gears-0.6.9/src/drf_gears.egg-info/top_level.txt
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.286974 drf-gears-0.6.9/src/gears/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 17:27:25.000000 drf-gears-0.6.9/src/gears/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)       43 2022-08-31 14:30:39.000000 drf-gears-0.6.9/src/gears/example.py
+-rw-r--r--   0 alexander   (501) staff       (20)      523 2022-08-22 18:21:05.000000 drf-gears-0.6.9/src/gears/mixins.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.287975 drf-gears-0.6.9/src/gears/models/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.9/src/gears/models/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     3770 2022-08-31 16:38:57.000000 drf-gears-0.6.9/src/gears/models/jwt.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.291837 drf-gears-0.6.9/src/gears/renderers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:39:27.000000 drf-gears-0.6.9/src/gears/renderers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     3034 2022-08-31 16:39:35.000000 drf-gears-0.6.9/src/gears/renderers/exception_handlers.py
+-rw-r--r--   0 alexander   (501) staff       (20)      314 2022-08-31 16:39:41.000000 drf-gears-0.6.9/src/gears/renderers/mapping.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1795 2022-08-31 16:39:48.000000 drf-gears-0.6.9/src/gears/renderers/renderer.py
+-rw-r--r--   0 alexander   (501) staff       (20)      385 2022-08-31 16:39:54.000000 drf-gears-0.6.9/src/gears/renderers/types.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.293178 drf-gears-0.6.9/src/gears/serializers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.9/src/gears/serializers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      481 2022-08-31 16:40:18.000000 drf-gears-0.6.9/src/gears/serializers/jwt.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.294063 drf-gears-0.6.9/src/gears/views/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.9/src/gears/views/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      351 2022-08-31 17:10:11.000000 drf-gears-0.6.9/src/gears/views/jwt.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.296606 drf-gears-0.6.9/src/gears/viewsets/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.9/src/gears/viewsets/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      724 2022-08-31 16:40:43.000000 drf-gears-0.6.9/src/gears/viewsets/permissions.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1096 2022-08-31 16:40:48.000000 drf-gears-0.6.9/src/gears/viewsets/querysets.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1153 2022-08-31 16:40:56.000000 drf-gears-0.6.9/src/gears/viewsets/serializers.py
```

### Comparing `drf_gears-0.6.2/LICENSE` & `drf-gears-0.6.9/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2018 The Python Packaging Authority
+MIT License
+
+Copyright (c) [year] [fullname]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -12,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `drf_gears-0.6.2/PKG-INFO` & `drf-gears-0.6.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: drf_gears
-Version: 0.6.2
-Summary: Some gears ⚙ ⚙ ⚙ collection for getting life a little bit better.
-Home-page: https://github.com/san4ezy/drf-gears
-Author: Alexander Yudkin
-Author-email: san4ezy@gmail.com
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DRF gears ⚙ ⚙ ⚙
 
 Some gears collection for getting life a little bit better.
 
 ## Installation
 
 ```
@@ -282,7 +266,68 @@
 from gears import Error
 
 RESPONSE_ERROR_MAPPING = {
     'required': Error(code='value_required'),
     ...
 }
 ```
+
+### JWT helpers
+
+Before we start. We assumed you use Django Rest Framework and djangorestframework-simplejwt packages for handling the JWT authorisation process.
+
+There are some gears which want to help you fill tokens with an additional payload.
+
+Firstly, add the `JWTUserModelMixin` to your user model. It delivers a set of methods for extending the tokens.
+
+```python
+from gears import JWTUserModelMixin
+
+class User(JWTUserModelMixin, BaseUserModel):
+    ...
+    def get_public_jwt_data(self):
+        return {
+            'name': self.name,
+        }
+
+    def get_private_jwt_data(self):
+        return {
+            'address': self.address,
+        }
+```
+
+You should override these two method. The first one must return a dictionary with an open data.
+The second one must return a dictionary with a sensitive data, which must be closed for anyone.
+
+Keep on mind, JWT tokens could be unpacked by any person, so the information inside the token available for anyone who has this token.
+If you need to fill JWT token with a sensitive data, please put it to the `get_private_jwt_data`. The entire data in this method will be encrypted with a secret symmetric key you will generate on the next step.
+
+Now we should generate a secret key and put it into the settings:
+
+```python
+from gears import TokenEncryption
+
+secret_key = TokenEncryption.generate_key()
+```
+
+The value of the `secret_key` you must put to the project's settings.
+It would be better to keep it in the virtual environment variable.
+
+```python
+import os
+
+JWT_PAYLOAD_ENCRYPTION_KEY = os.environ.get('JWT_PAYLOAD_ENCRYPTION_KEY')
+```
+
+#### Details
+
+There was used the symmetric Fernet algorithm. Anyone, who has a secret key could decrypt data.
+
+An example how to do it on python:
+
+```python
+from gears import TokenEncryption
+
+decrypted_data = TokenEncryption.decrypt_data(encrypted_data, secret_key)
+```
+
+Google help you if you need similar functionality for another programming language.
```

### Comparing `drf_gears-0.6.2/README.md` & `drf-gears-0.6.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: drf-gears
+Version: 0.6.9
+Summary: Some gears collection for getting life a little bit better.
+Author-email: Alexander Yudkin <san4ezy@gmail.com>
+License: MIT License
+        
+        Copyright (c) [year] [fullname]
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DRF gears ⚙ ⚙ ⚙
 
 Some gears collection for getting life a little bit better.
 
 ## Installation
 
 ```
@@ -266,7 +302,68 @@
 from gears import Error
 
 RESPONSE_ERROR_MAPPING = {
     'required': Error(code='value_required'),
     ...
 }
 ```
+
+### JWT helpers
+
+Before we start. We assumed you use Django Rest Framework and djangorestframework-simplejwt packages for handling the JWT authorisation process.
+
+There are some gears which want to help you fill tokens with an additional payload.
+
+Firstly, add the `JWTUserModelMixin` to your user model. It delivers a set of methods for extending the tokens.
+
+```python
+from gears import JWTUserModelMixin
+
+class User(JWTUserModelMixin, BaseUserModel):
+    ...
+    def get_public_jwt_data(self):
+        return {
+            'name': self.name,
+        }
+
+    def get_private_jwt_data(self):
+        return {
+            'address': self.address,
+        }
+```
+
+You should override these two method. The first one must return a dictionary with an open data.
+The second one must return a dictionary with a sensitive data, which must be closed for anyone.
+
+Keep on mind, JWT tokens could be unpacked by any person, so the information inside the token available for anyone who has this token.
+If you need to fill JWT token with a sensitive data, please put it to the `get_private_jwt_data`. The entire data in this method will be encrypted with a secret symmetric key you will generate on the next step.
+
+Now we should generate a secret key and put it into the settings:
+
+```python
+from gears import TokenEncryption
+
+secret_key = TokenEncryption.generate_key()
+```
+
+The value of the `secret_key` you must put to the project's settings.
+It would be better to keep it in the virtual environment variable.
+
+```python
+import os
+
+JWT_PAYLOAD_ENCRYPTION_KEY = os.environ.get('JWT_PAYLOAD_ENCRYPTION_KEY')
+```
+
+#### Details
+
+There was used the symmetric Fernet algorithm. Anyone, who has a secret key could decrypt data.
+
+An example how to do it on python:
+
+```python
+from gears import TokenEncryption
+
+decrypted_data = TokenEncryption.decrypt_data(encrypted_data, secret_key)
+```
+
+Google help you if you need similar functionality for another programming language.
```

### Comparing `drf_gears-0.6.2/drf_gears.egg-info/PKG-INFO` & `drf-gears-0.6.9/src/drf_gears.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,40 @@
 Metadata-Version: 2.1
 Name: drf-gears
-Version: 0.6.2
-Summary: Some gears ⚙ ⚙ ⚙ collection for getting life a little bit better.
-Home-page: https://github.com/san4ezy/drf-gears
-Author: Alexander Yudkin
-Author-email: san4ezy@gmail.com
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
+Version: 0.6.9
+Summary: Some gears collection for getting life a little bit better.
+Author-email: Alexander Yudkin <san4ezy@gmail.com>
+License: MIT License
+        
+        Copyright (c) [year] [fullname]
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DRF gears ⚙ ⚙ ⚙
 
 Some gears collection for getting life a little bit better.
 
@@ -282,7 +302,68 @@
 from gears import Error
 
 RESPONSE_ERROR_MAPPING = {
     'required': Error(code='value_required'),
     ...
 }
 ```
+
+### JWT helpers
+
+Before we start. We assumed you use Django Rest Framework and djangorestframework-simplejwt packages for handling the JWT authorisation process.
+
+There are some gears which want to help you fill tokens with an additional payload.
+
+Firstly, add the `JWTUserModelMixin` to your user model. It delivers a set of methods for extending the tokens.
+
+```python
+from gears import JWTUserModelMixin
+
+class User(JWTUserModelMixin, BaseUserModel):
+    ...
+    def get_public_jwt_data(self):
+        return {
+            'name': self.name,
+        }
+
+    def get_private_jwt_data(self):
+        return {
+            'address': self.address,
+        }
+```
+
+You should override these two method. The first one must return a dictionary with an open data.
+The second one must return a dictionary with a sensitive data, which must be closed for anyone.
+
+Keep on mind, JWT tokens could be unpacked by any person, so the information inside the token available for anyone who has this token.
+If you need to fill JWT token with a sensitive data, please put it to the `get_private_jwt_data`. The entire data in this method will be encrypted with a secret symmetric key you will generate on the next step.
+
+Now we should generate a secret key and put it into the settings:
+
+```python
+from gears import TokenEncryption
+
+secret_key = TokenEncryption.generate_key()
+```
+
+The value of the `secret_key` you must put to the project's settings.
+It would be better to keep it in the virtual environment variable.
+
+```python
+import os
+
+JWT_PAYLOAD_ENCRYPTION_KEY = os.environ.get('JWT_PAYLOAD_ENCRYPTION_KEY')
+```
+
+#### Details
+
+There was used the symmetric Fernet algorithm. Anyone, who has a secret key could decrypt data.
+
+An example how to do it on python:
+
+```python
+from gears import TokenEncryption
+
+decrypted_data = TokenEncryption.decrypt_data(encrypted_data, secret_key)
+```
+
+Google help you if you need similar functionality for another programming language.
```

### Comparing `drf_gears-0.6.2/gears/mixins.py` & `drf-gears-0.6.9/src/gears/mixins.py`

 * *Files identical despite different names*

### Comparing `drf_gears-0.6.2/gears/renderers/exception_handlers.py` & `drf-gears-0.6.9/src/gears/renderers/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `drf_gears-0.6.2/gears/renderers/renderer.py` & `drf-gears-0.6.9/src/gears/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `drf_gears-0.6.2/gears/viewsets/permissions.py` & `drf-gears-0.6.9/src/gears/viewsets/permissions.py`

 * *Files identical despite different names*

### Comparing `drf_gears-0.6.2/gears/viewsets/querysets.py` & `drf-gears-0.6.9/src/gears/viewsets/querysets.py`

 * *Files identical despite different names*

### Comparing `drf_gears-0.6.2/gears/viewsets/serializers.py` & `drf-gears-0.6.9/src/gears/viewsets/serializers.py`

 * *Files identical despite different names*

