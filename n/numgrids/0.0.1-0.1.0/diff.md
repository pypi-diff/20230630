# Comparing `tmp/numgrids-0.0.1.tar.gz` & `tmp/numgrids-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/numgrids-0.0.1.tar", last modified: Fri Jul 29 14:05:22 2022, max compression
+gzip compressed data, was "numgrids-0.1.0.tar", last modified: Fri Jun 30 04:59:22 2023, max compression
```

## Comparing `numgrids-0.0.1.tar` & `numgrids-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-07-29 14:05:22.441686 numgrids-0.0.1/
--rw-r--r--   0 mbaer    (671849960) 579947404      351 2022-07-29 14:05:22.441479 numgrids-0.0.1/PKG-INFO
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-07-29 14:05:22.439975 numgrids-0.0.1/numgrids/
--rw-r--r--   0 mbaer    (671849960) 579947404        0 2022-07-29 14:01:47.000000 numgrids-0.0.1/numgrids/__init__.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-07-29 14:05:22.441201 numgrids-0.0.1/numgrids.egg-info/
--rw-r--r--   0 mbaer    (671849960) 579947404      351 2022-07-29 14:05:22.000000 numgrids-0.0.1/numgrids.egg-info/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404      188 2022-07-29 14:05:22.000000 numgrids-0.0.1/numgrids.egg-info/SOURCES.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2022-07-29 14:05:22.000000 numgrids-0.0.1/numgrids.egg-info/dependency_links.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        7 2022-07-29 14:05:22.000000 numgrids-0.0.1/numgrids.egg-info/requires.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        9 2022-07-29 14:05:22.000000 numgrids-0.0.1/numgrids.egg-info/top_level.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       38 2022-07-29 14:05:22.441756 numgrids-0.0.1/setup.cfg
--rw-r--r--   0 mbaer    (671849960) 579947404      871 2022-07-29 14:05:03.000000 numgrids-0.0.1/setup.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-06-30 04:59:22.230669 numgrids-0.1.0/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1069 2023-06-30 04:56:35.000000 numgrids-0.1.0/LICENSE
+-rw-r--r--   0 mbaer    (671849960) 579947404     1181 2023-06-30 04:59:22.230235 numgrids-0.1.0/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      789 2023-06-26 09:43:56.000000 numgrids-0.1.0/README.md
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-06-30 04:59:22.227212 numgrids-0.1.0/numgrids/
+-rw-r--r--   0 mbaer    (671849960) 579947404      110 2023-06-30 04:50:47.000000 numgrids-0.1.0/numgrids/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     4330 2023-06-30 04:50:24.000000 numgrids-0.1.0/numgrids/api.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     6979 2023-06-29 17:28:57.000000 numgrids-0.1.0/numgrids/axes.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     5157 2023-06-28 14:34:51.000000 numgrids-0.1.0/numgrids/diff.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     1564 2023-06-26 10:51:28.000000 numgrids-0.1.0/numgrids/grids.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     1995 2023-06-30 04:55:14.000000 numgrids-0.1.0/numgrids/integration.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      250 2023-06-27 12:40:22.000000 numgrids-0.1.0/numgrids/utils.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-06-30 04:59:22.229530 numgrids-0.1.0/numgrids.egg-info/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1181 2023-06-30 04:59:22.000000 numgrids-0.1.0/numgrids.egg-info/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      316 2023-06-30 04:59:22.000000 numgrids-0.1.0/numgrids.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-06-30 04:59:22.000000 numgrids-0.1.0/numgrids.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       23 2023-06-30 04:59:22.000000 numgrids-0.1.0/numgrids.egg-info/requires.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        9 2023-06-30 04:59:22.000000 numgrids-0.1.0/numgrids.egg-info/top_level.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       38 2023-06-30 04:59:22.230835 numgrids-0.1.0/setup.cfg
+-rw-r--r--   0 mbaer    (671849960) 579947404      925 2023-06-30 04:58:10.000000 numgrids-0.1.0/setup.py
```

### Comparing `numgrids-0.0.1/setup.py` & `numgrids-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from os.path import exists
 from setuptools import setup, find_packages
 
 author = 'Matthias Baer'
 email = 'matthias.r.baer@googlemail.com'
 description = ''
 name = 'numgrids'
-year = '2022'
-url = ''
-version = '0.0.1'
+year = '2023'
+url = 'https://github.com/maroba/numgrids'
+version = '0.1.0'
 
 setup(
     name=name,
     author=author,
     author_email=email,
     url=url,
     version=version,
     packages=find_packages(),
     package_dir={name: name},
     include_package_data=True,
-    license='None',
+    license='MIT',
     description=description,
     long_description=open('README.md').read() if exists('README.md') else '',
     long_description_content_type="text/markdown",
-    install_requires=['sphinx',
+    install_requires=['numpy', 'scipy', 'matplotlib'
                       ],
     python_requires=">=3.6",
     classifiers=['Operating System :: OS Independent',
                  'Programming Language :: Python :: 3',
                  ],
     platforms=['ALL'],
 )
```

