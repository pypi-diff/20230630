# Comparing `tmp/mayfpayapi-1.3.0.tar.gz` & `tmp/mayfpayapi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayfpayapi-1.3.0.tar", last modified: Mon Apr 10 18:25:00 2023, max compression
+gzip compressed data, was "mayfpayapi-1.4.0.tar", last modified: Fri Jun 30 09:34:14 2023, max compression
```

## Comparing `mayfpayapi-1.3.0.tar` & `mayfpayapi-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-04-10 18:25:00.183618 mayfpayapi-1.3.0/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     2065 2023-04-10 18:25:00.183382 mayfpayapi-1.3.0/PKG-INFO
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     1512 2023-04-10 17:47:22.000000 mayfpayapi-1.3.0/README.md
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-04-10 18:25:00.181751 mayfpayapi-1.3.0/mayfpayapi/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       26 2023-04-10 18:23:23.000000 mayfpayapi-1.3.0/mayfpayapi/__init__.py
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     1656 2023-04-10 17:47:23.000000 mayfpayapi-1.3.0/mayfpayapi/mayfpayapi.py
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-04-10 18:25:00.183055 mayfpayapi-1.3.0/mayfpayapi.egg-info/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     2065 2023-04-10 18:25:00.000000 mayfpayapi-1.3.0/mayfpayapi.egg-info/PKG-INFO
--rw-r--r--   0 dimamayfeed   (502) staff       (20)      235 2023-04-10 18:25:00.000000 mayfpayapi-1.3.0/mayfpayapi.egg-info/SOURCES.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)        1 2023-04-10 18:25:00.000000 mayfpayapi-1.3.0/mayfpayapi.egg-info/dependency_links.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)        9 2023-04-10 18:25:00.000000 mayfpayapi-1.3.0/mayfpayapi.egg-info/requires.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       11 2023-04-10 18:25:00.000000 mayfpayapi-1.3.0/mayfpayapi.egg-info/top_level.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       38 2023-04-10 18:25:00.183699 mayfpayapi-1.3.0/setup.cfg
--rw-r--r--   0 dimamayfeed   (502) staff       (20)      892 2023-04-10 18:23:37.000000 mayfpayapi-1.3.0/setup.py
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-06-30 09:34:14.950790 mayfpayapi-1.4.0/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)      642 2023-06-30 09:34:14.950606 mayfpayapi-1.4.0/PKG-INFO
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)        0 2023-06-30 09:26:33.000000 mayfpayapi-1.4.0/README.md
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-06-30 09:34:14.949201 mayfpayapi-1.4.0/mayfpayapi/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     3757 2023-06-30 09:28:15.000000 mayfpayapi-1.4.0/mayfpayapi/__init__.py
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     3757 2023-06-30 09:29:58.000000 mayfpayapi-1.4.0/mayfpayapi/mayfpayapi.py
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-06-30 09:34:14.950290 mayfpayapi-1.4.0/mayfpayapi.egg-info/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)      642 2023-06-30 09:34:14.000000 mayfpayapi-1.4.0/mayfpayapi.egg-info/PKG-INFO
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)      235 2023-06-30 09:34:14.000000 mayfpayapi-1.4.0/mayfpayapi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)        1 2023-06-30 09:34:14.000000 mayfpayapi-1.4.0/mayfpayapi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)        9 2023-06-30 09:34:14.000000 mayfpayapi-1.4.0/mayfpayapi.egg-info/requires.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)       11 2023-06-30 09:34:14.000000 mayfpayapi-1.4.0/mayfpayapi.egg-info/top_level.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)       38 2023-06-30 09:34:14.950858 mayfpayapi-1.4.0/setup.cfg
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)      979 2023-06-30 09:33:53.000000 mayfpayapi-1.4.0/setup.py
```

### Comparing `mayfpayapi-1.3.0/setup.py` & `mayfpayapi-1.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mayfpayapi',
-    version='1.3.0',
-    author='MayfPay',
+    version='1.4.0',
+    author='MayfPay.top',
     author_email='support@mayfpay.top',
-    description='MayfPayApi is a Python library for interacting with the MayfPay payment system API. It provides methods for retrieving kassa balances, creating and checking invoices.',
+    description='MayfPayApi is a Python library for interacting with the MayfPay payment system API.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/MAYFPAY/MayfPayApi',
     packages=find_packages(),
-    py_modules=['mayfpayapi'],
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
     project_urls={
         'Source': 'https://github.com/MAYFPAY/MayfPayApi',
         'Documentation': 'https://mayfpay.top/docs',
         'Bug Reports': 'https://github.com/MAYFPAY/MayfPayApi/issues',
     },
-    long_description=long_description,
-    long_description_content_type="text/markdown",
+    python_requires='>=3.6',
     install_requires=[
         'requests',
     ],
 )
```

