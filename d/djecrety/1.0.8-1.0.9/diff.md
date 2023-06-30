# Comparing `tmp/djecrety-1.0.8.tar.gz` & `tmp/djecrety-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djecrety-1.0.8.tar", last modified: Fri Aug  2 17:23:14 2019, max compression
+gzip compressed data, was "dist/djecrety-1.0.9.tar", last modified: Fri Aug 23 08:49:07 2019, max compression
```

## Comparing `djecrety-1.0.8.tar` & `djecrety-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-02 17:23:14.000000 djecrety-1.0.8/
-drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-02 17:23:14.000000 djecrety-1.0.8/docs/
--rw-rw-r--   0 mython    (1000) mython    (1000)      518 2019-08-02 16:55:13.000000 djecrety-1.0.8/docs/getting_started.rst
--rw-rw-r--   0 mython    (1000) mython    (1000)      452 2019-08-02 16:55:13.000000 djecrety-1.0.8/docs/introduction.rst
--rw-rw-r--   0 mython    (1000) mython    (1000)      864 2019-08-02 16:55:13.000000 djecrety-1.0.8/docs/usage.rst
--rw-rw-r--   0 mython    (1000) mython    (1000)      358 2019-02-12 21:35:08.000000 djecrety-1.0.8/docs/index.rst
--rw-rw-r--   0 mython    (1000) mython    (1000)     1289 2019-08-02 16:55:13.000000 djecrety-1.0.8/README.rst
--rw-rw-r--   0 mython    (1000) mython    (1000)       38 2019-08-02 17:23:14.000000 djecrety-1.0.8/setup.cfg
--rw-rw-r--   0 mython    (1000) mython    (1000)     2696 2019-08-02 17:23:14.000000 djecrety-1.0.8/PKG-INFO
-drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety/
-drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety/management/
-drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety/management/commands/
--rw-rw-r--   0 mython    (1000) mython    (1000)     1903 2019-02-12 20:35:06.000000 djecrety-1.0.8/djecrety/management/commands/djecrety.py
--rw-rw-r--   0 mython    (1000) mython    (1000)        0 2019-01-24 07:26:50.000000 djecrety-1.0.8/djecrety/management/commands/__init__.py
--rw-rw-r--   0 mython    (1000) mython    (1000)        0 2019-01-24 07:26:39.000000 djecrety-1.0.8/djecrety/management/__init__.py
--rw-rw-r--   0 mython    (1000) mython    (1000)       22 2019-08-02 17:22:22.000000 djecrety-1.0.8/djecrety/__init__.py
--rw-rw-r--   0 mython    (1000) mython    (1000)     1763 2019-04-25 08:07:41.000000 djecrety-1.0.8/djecrety/utils.py
--rwxrwxrwx   0 mython    (1000) mython    (1000)    35147 2018-08-13 18:35:43.000000 djecrety-1.0.8/LICENSE
--rwxrwxr-x   0 mython    (1000) mython    (1000)     1650 2019-08-02 17:23:02.000000 djecrety-1.0.8/setup.py
--rw-r--r--   0 mython    (1000) mython    (1000)       60 2019-01-25 11:50:59.000000 djecrety-1.0.8/MANIFEST.in
-drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety.egg-info/
--rw-rw-r--   0 mython    (1000) mython    (1000)       12 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety.egg-info/requires.txt
--rw-rw-r--   0 mython    (1000) mython    (1000)     2696 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety.egg-info/PKG-INFO
--rw-rw-r--   0 mython    (1000) mython    (1000)        1 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety.egg-info/dependency_links.txt
--rw-rw-r--   0 mython    (1000) mython    (1000)        9 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety.egg-info/top_level.txt
--rw-rw-r--   0 mython    (1000) mython    (1000)      459 2019-08-02 17:23:14.000000 djecrety-1.0.8/djecrety.egg-info/SOURCES.txt
--rw-rw-r--   0 mython    (1000) mython    (1000)        1 2019-08-02 17:22:45.000000 djecrety-1.0.8/djecrety.egg-info/not-zip-safe
+drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-23 08:49:07.000000 djecrety-1.0.9/
+drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-23 08:49:07.000000 djecrety-1.0.9/docs/
+-rw-rw-r--   0 mython    (1000) mython    (1000)      505 2019-08-23 08:48:36.000000 djecrety-1.0.9/docs/getting_started.rst
+-rw-rw-r--   0 mython    (1000) mython    (1000)      452 2019-08-02 16:55:13.000000 djecrety-1.0.9/docs/introduction.rst
+-rw-rw-r--   0 mython    (1000) mython    (1000)      853 2019-08-23 08:48:36.000000 djecrety-1.0.9/docs/usage.rst
+-rw-rw-r--   0 mython    (1000) mython    (1000)      358 2019-02-12 21:35:08.000000 djecrety-1.0.9/docs/index.rst
+-rw-rw-r--   0 mython    (1000) mython    (1000)     1289 2019-08-02 16:55:13.000000 djecrety-1.0.9/README.rst
+-rw-rw-r--   0 mython    (1000) mython    (1000)       38 2019-08-23 08:49:07.000000 djecrety-1.0.9/setup.cfg
+-rw-rw-r--   0 mython    (1000) mython    (1000)     2680 2019-08-23 08:49:07.000000 djecrety-1.0.9/PKG-INFO
+drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety/
+drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety/management/
+drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety/management/commands/
+-rw-rw-r--   0 mython    (1000) mython    (1000)     2299 2019-08-23 08:48:36.000000 djecrety-1.0.9/djecrety/management/commands/djecrety.py
+-rw-rw-r--   0 mython    (1000) mython    (1000)        0 2019-01-24 07:26:50.000000 djecrety-1.0.9/djecrety/management/commands/__init__.py
+-rw-rw-r--   0 mython    (1000) mython    (1000)        0 2019-01-24 07:26:39.000000 djecrety-1.0.9/djecrety/management/__init__.py
+-rw-rw-r--   0 mython    (1000) mython    (1000)       22 2019-08-23 08:48:36.000000 djecrety-1.0.9/djecrety/__init__.py
+-rw-rw-r--   0 mython    (1000) mython    (1000)     1664 2019-08-23 08:48:36.000000 djecrety-1.0.9/djecrety/utils.py
+-rwxrwxrwx   0 mython    (1000) mython    (1000)    35147 2018-08-13 18:35:43.000000 djecrety-1.0.9/LICENSE
+-rwxrwxr-x   0 mython    (1000) mython    (1000)     1650 2019-08-23 08:48:36.000000 djecrety-1.0.9/setup.py
+-rw-r--r--   0 mython    (1000) mython    (1000)       60 2019-01-25 11:50:59.000000 djecrety-1.0.9/MANIFEST.in
+drwxrwxr-x   0 mython    (1000) mython    (1000)        0 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety.egg-info/
+-rw-rw-r--   0 mython    (1000) mython    (1000)       12 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety.egg-info/requires.txt
+-rw-rw-r--   0 mython    (1000) mython    (1000)     2680 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety.egg-info/PKG-INFO
+-rw-rw-r--   0 mython    (1000) mython    (1000)        1 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety.egg-info/dependency_links.txt
+-rw-rw-r--   0 mython    (1000) mython    (1000)        9 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety.egg-info/top_level.txt
+-rw-rw-r--   0 mython    (1000) mython    (1000)      459 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety.egg-info/SOURCES.txt
+-rw-rw-r--   0 mython    (1000) mython    (1000)        1 2019-08-23 08:49:07.000000 djecrety-1.0.9/djecrety.egg-info/not-zip-safe
```

### Comparing `djecrety-1.0.8/docs/usage.rst` & `djecrety-1.0.9/docs/usage.rst`

 * *Files 13% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 * With ``-s`` argument, save the generated secret key to ``settings.py``:
 
 .. code-block:: text
 
     $ ./manage.py djecrety -s
 
-* With ``-p`` argument, display the generated secret key when saving to the file:
+* With ``-p`` argument, display the generated secret key while saving to the file:
 
 .. note::
 
-    ``-p`` argument work when saving the secret key to the file.
+    ``-p`` argument work with ``-s`` argument.
 
 .. code-block:: text
 
     $ ./manage.py djecrety -sp
 
 * With ``-d`` argument, specify settings directory name:
 
 .. note::
 
-    By default, we try to detect your project directory and ``settings.py`` location, if ``settings.py`` not in default location you can specify the directory.
+    By default, Djecrety try to detect your project directory and ``settings.py`` location, if ``settings.py`` not in default location you can specify the directory.
 
 .. code-block:: text
 
     $ ./manage.py djecrety -sp
```

### Comparing `djecrety-1.0.8/README.rst` & `djecrety-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `djecrety-1.0.8/PKG-INFO` & `djecrety-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: djecrety
-Version: 1.0.8
-Summary: Djecrety package provides a command to generate a new secret key for your project and                 save it to settings.py file.
+Version: 1.0.9
+Summary: Djecrety package provides a command to generate a new secret key for your project and save it to settings.py file.
 Home-page: https://djecrety.ir/
 Author: Majid Rouhi
 Author-email: mrouhi13@gmail.com
 License: GNU Version 3 License
 Description: Djecrety
         ========
         .. image:: https://img.shields.io/pypi/v/djecrety.svg
```

### Comparing `djecrety-1.0.8/djecrety/utils.py` & `djecrety-1.0.9/djecrety/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,56 +5,48 @@
 
 from django.conf import settings
 from django.utils.crypto import get_random_string
 
 
 def generate_secret_key(length=50):
     """
-        Return a 50 character random string usable as a SECRET_KEY setting value.
+    Return a 50 character random string
+    usable as a `SECRET_KEY` setting value.
     """
-    try:
-        length = int(length)
-    except ValueError:
-        length = 50
-    except TypeError:
-        length = 50
-
     chars = 'abcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*(-_=+)'
-
+    if not isinstance(length, int):
+        raise TypeError(
+            f'invalid literal for int() with base 10: {length}')
     return get_random_string(length, chars)
 
 
 def save_to_settings(value, parameter_name, settings_dir_name=''):
     """
-        Save the value to the given parameter in settings.py file.
+    Save the value to the given parameter in `settings.py` file.
     """
-    settings_dir = os.path.join(settings.BASE_DIR, settings_dir_name, 'settings.py')
+    if not settings_dir_name:
+        settings_dir_name = ''
 
+    settings_dir = os.path.join(settings.BASE_DIR, settings_dir_name,
+                                'settings.py')
     if not os.path.exists(settings_dir):
-        return False, f'Not found: {settings_dir}\n\nCan\'t find \'settings.py\' file,' \
-            ' please specify settings file directory name using -p argument.'
-
-    result, message = _replace_line(value, parameter_name, settings_dir)
-
-    return result, message
+        raise FileNotFoundError("Can't find `settings.py` file: "
+                                f"{settings_dir}")
+    return _replace_line(value, parameter_name, settings_dir)
 
 
 def _replace_line(value, parameter_name, settings_file):
     parameter_is_exist = False
-
-    if not parameter_name:
-        return False, f'Can\'t find passed parameter name. (parameter: {parameter_name})'
-
-    new_line = f'{parameter_name} = {value}'
-    line_pattern = fr'^{parameter_name} = .*'
-
-    for line in fileinput.input(settings_file, inplace=True):
-        if re.match(line_pattern, line):
-            parameter_is_exist = True
-            line = re.sub(line_pattern, new_line, line)
-
-        sys.stdout.write(line)
-
-    if not parameter_is_exist:
-        return False, f'Can\'t find passed parameter name. (parameter: {parameter_name})'
-
-    return True, f'{parameter_name} updated successfully.'
+    if parameter_name:
+        new_line = f'{parameter_name} = {value}'
+        line_pattern = fr'^{parameter_name} = .*'
+
+        for line in fileinput.input(settings_file, inplace=True):
+            if re.match(line_pattern, line):
+                parameter_is_exist = True
+                line = re.sub(line_pattern, new_line, line)
+            sys.stdout.write(line)
+
+        if not parameter_is_exist:
+            raise NameError(f"Can't find parameter name: {parameter_name}")
+        return True
+    return False
```

### Comparing `djecrety-1.0.8/LICENSE` & `djecrety-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djecrety-1.0.8/setup.py` & `djecrety-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 setup(
     name='djecrety',
     version=version,
     python_requires='>=3.5',
     packages=find_packages(exclude=['testproject']),
     include_package_data=True,
     license='GNU Version 3 License',
-    description='Djecrety package provides a command to generate a new secret key for your project and \
-                save it to settings.py file.',
+    description='Djecrety package provides a command to generate a new secret '
+                'key for your project and save it to settings.py file.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://djecrety.ir/',
     author='Majid Rouhi',
     author_email='mrouhi13@gmail.com',
     zip_safe=False,
     install_requires=[
@@ -40,9 +40,9 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Topic :: Security :: Cryptography',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Utilities'
-    ],
+    ]
 )
```

### Comparing `djecrety-1.0.8/djecrety.egg-info/PKG-INFO` & `djecrety-1.0.9/djecrety.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: djecrety
-Version: 1.0.8
-Summary: Djecrety package provides a command to generate a new secret key for your project and                 save it to settings.py file.
+Version: 1.0.9
+Summary: Djecrety package provides a command to generate a new secret key for your project and save it to settings.py file.
 Home-page: https://djecrety.ir/
 Author: Majid Rouhi
 Author-email: mrouhi13@gmail.com
 License: GNU Version 3 License
 Description: Djecrety
         ========
         .. image:: https://img.shields.io/pypi/v/djecrety.svg
```

