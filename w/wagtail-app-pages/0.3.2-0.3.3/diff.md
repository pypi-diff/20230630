# Comparing `tmp/wagtail_app_pages-0.3.2.tar.gz` & `tmp/wagtail_app_pages-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_app_pages-0.3.2.tar", last modified: Tue Jun 27 11:32:33 2023, max compression
+gzip compressed data, was "wagtail_app_pages-0.3.3.tar", last modified: Fri Jun 30 07:50:44 2023, max compression
```

## Comparing `wagtail_app_pages-0.3.2.tar` & `wagtail_app_pages-0.3.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.479250 wagtail_app_pages-0.3.2/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      166 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/AUTHORS.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3376 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/CONTRIBUTING.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1834 2023-06-27 11:29:24.000000 wagtail_app_pages-0.3.2/HISTORY.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1074 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/LICENSE
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      315 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/MANIFEST.in
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3700 2023-06-27 11:32:33.479348 wagtail_app_pages-0.3.2/PKG-INFO
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1142 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/README.md
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.462495 wagtail_app_pages-0.3.2/docs/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      618 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/Makefile
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       28 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/authors.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4465 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/caveats.rst
--rwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4955 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/conf.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       33 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/contributing.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3108 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/examples.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       28 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/history.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      344 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/index.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1201 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/installation.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      779 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/make.bat
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      918 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/readme.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1238 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/docs/usage.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      422 2023-06-27 11:32:33.480283 wagtail_app_pages-0.3.2/setup.cfg
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1386 2023-06-27 11:29:42.000000 wagtail_app_pages-0.3.2/setup.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.462761 wagtail_app_pages-0.3.2/tests/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       72 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/__init__.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.463050 wagtail_app_pages-0.3.2/tests/testproject/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.464336 wagtail_app_pages-0.3.2/tests/testproject/home/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/__init__.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.465428 wagtail_app_pages-0.3.2/tests/testproject/home/migrations/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      604 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/migrations/0001_initial.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1673 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/migrations/0002_create_homepage.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/migrations/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      149 2023-02-06 14:17:03.000000 wagtail_app_pages-0.3.2/tests/testproject/home/models.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.451413 wagtail_app_pages-0.3.2/tests/testproject/home/templates/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.466254 wagtail_app_pages-0.3.2/tests/testproject/home/templates/home/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      507 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/templates/home/home_page.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      142 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/templates/home/test_a.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      142 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/templates/home/test_b.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      212 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/urls.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      356 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/home/views.py
--rwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      254 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/manage.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.467646 wagtail_app_pages-0.3.2/tests/testproject/testproject/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3613 2023-06-27 11:07:04.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/settings.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.452360 wagtail_app_pages-0.3.2/tests/testproject/testproject/static/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.468114 wagtail_app_pages-0.3.2/tests/testproject/testproject/static/css/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/static/css/testproject.css
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.468368 wagtail_app_pages-0.3.2/tests/testproject/testproject/static/js/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/static/js/testproject.js
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.469367 wagtail_app_pages-0.3.2/tests/testproject/testproject/templates/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      191 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/templates/404.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      680 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/templates/500.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1622 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/templates/base.html
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.469920 wagtail_app_pages-0.3.2/tests/testproject/testproject/tests/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/tests/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      794 2023-02-06 14:18:24.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/tests/test_wagtail_app_pages.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1147 2022-09-30 08:41:15.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/urls.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      403 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/tests/testproject/testproject/wsgi.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.473315 wagtail_app_pages-0.3.2/wagtail_app_pages/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      170 2023-06-27 11:29:53.000000 wagtail_app_pages-0.3.2/wagtail_app_pages/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      100 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/wagtail_app_pages/apps.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      772 2023-02-06 14:18:04.000000 wagtail_app_pages-0.3.2/wagtail_app_pages/compatibility.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      423 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/wagtail_app_pages/context_processors.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3196 2022-09-29 09:59:13.000000 wagtail_app_pages-0.3.2/wagtail_app_pages/models.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.479042 wagtail_app_pages-0.3.2/wagtail_app_pages/templatetags/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/wagtail_app_pages/templatetags/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      406 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/wagtail_app_pages/templatetags/app_pages_tags.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      133 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.2/wagtail_app_pages/utils.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-27 11:32:33.478477 wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3700 2023-06-27 11:32:33.000000 wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/PKG-INFO
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1825 2023-06-27 11:32:33.000000 wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/SOURCES.txt
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-06-27 11:32:33.000000 wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/dependency_links.txt
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-06-27 11:32:33.000000 wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/not-zip-safe
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       18 2023-06-27 11:32:33.000000 wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/requires.txt
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       18 2023-06-27 11:32:33.000000 wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/top_level.txt
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.124316 wagtail_app_pages-0.3.3/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      166 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/AUTHORS.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3376 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1882 2023-06-30 07:49:01.000000 wagtail_app_pages-0.3.3/HISTORY.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1074 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/LICENSE
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      315 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/MANIFEST.in
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3748 2023-06-30 07:50:44.124406 wagtail_app_pages-0.3.3/PKG-INFO
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1142 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/README.md
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.111209 wagtail_app_pages-0.3.3/docs/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      618 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/Makefile
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       28 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/authors.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4465 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/caveats.rst
+-rwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4955 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/conf.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       33 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/contributing.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3108 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/examples.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       28 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/history.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      344 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/index.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1201 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/installation.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      779 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/make.bat
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      918 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/readme.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1238 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/docs/usage.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      422 2023-06-30 07:50:44.125941 wagtail_app_pages-0.3.3/setup.cfg
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1386 2023-06-30 07:48:42.000000 wagtail_app_pages-0.3.3/setup.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.111529 wagtail_app_pages-0.3.3/tests/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       72 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/__init__.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.111881 wagtail_app_pages-0.3.3/tests/testproject/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.113077 wagtail_app_pages-0.3.3/tests/testproject/home/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/__init__.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.113979 wagtail_app_pages-0.3.3/tests/testproject/home/migrations/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      604 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/migrations/0001_initial.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1673 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/migrations/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      149 2023-02-06 14:17:03.000000 wagtail_app_pages-0.3.3/tests/testproject/home/models.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.100620 wagtail_app_pages-0.3.3/tests/testproject/home/templates/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.114891 wagtail_app_pages-0.3.3/tests/testproject/home/templates/home/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      507 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/templates/home/home_page.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      142 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/templates/home/test_a.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      142 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/templates/home/test_b.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      212 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/urls.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      356 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/home/views.py
+-rwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      254 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/manage.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.116066 wagtail_app_pages-0.3.3/tests/testproject/testproject/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3613 2023-06-27 11:07:04.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/settings.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.101907 wagtail_app_pages-0.3.3/tests/testproject/testproject/static/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.116469 wagtail_app_pages-0.3.3/tests/testproject/testproject/static/css/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/static/css/testproject.css
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.116708 wagtail_app_pages-0.3.3/tests/testproject/testproject/static/js/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/static/js/testproject.js
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.117442 wagtail_app_pages-0.3.3/tests/testproject/testproject/templates/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      191 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/templates/404.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      680 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/templates/500.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1622 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/templates/base.html
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.118108 wagtail_app_pages-0.3.3/tests/testproject/testproject/tests/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/tests/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      794 2023-02-06 14:18:24.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/tests/test_wagtail_app_pages.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1147 2022-09-30 08:41:15.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/urls.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      403 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/tests/testproject/testproject/wsgi.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.119765 wagtail_app_pages-0.3.3/wagtail_app_pages/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      170 2023-06-30 07:49:09.000000 wagtail_app_pages-0.3.3/wagtail_app_pages/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      100 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/wagtail_app_pages/apps.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      772 2023-02-06 14:18:04.000000 wagtail_app_pages-0.3.3/wagtail_app_pages/compatibility.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      423 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/wagtail_app_pages/context_processors.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3196 2022-09-29 09:59:13.000000 wagtail_app_pages-0.3.3/wagtail_app_pages/models.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.124179 wagtail_app_pages-0.3.3/wagtail_app_pages/templatetags/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/wagtail_app_pages/templatetags/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      406 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/wagtail_app_pages/templatetags/app_pages_tags.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      133 2022-02-25 09:06:32.000000 wagtail_app_pages-0.3.3/wagtail_app_pages/utils.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-06-30 07:50:44.123665 wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3748 2023-06-30 07:50:43.000000 wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/PKG-INFO
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1825 2023-06-30 07:50:44.000000 wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-06-30 07:50:43.000000 wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-06-30 07:50:43.000000 wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/not-zip-safe
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       18 2023-06-30 07:50:43.000000 wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/requires.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       18 2023-06-30 07:50:43.000000 wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/top_level.txt
```

### Comparing `wagtail_app_pages-0.3.2/CONTRIBUTING.rst` & `wagtail_app_pages-0.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/HISTORY.rst` & `wagtail_app_pages-0.3.3/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 =======
 History
 =======
+
+0.3.3
+-------------------
+
+* fix requirements
+
 0.3.2
 -------------------
 
 * Wagtail support for 5.0, dropping support for 3
 
 0.3.1
 -------------------
```

### Comparing `wagtail_app_pages-0.3.2/LICENSE` & `wagtail_app_pages-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/PKG-INFO` & `wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_app_pages
-Version: 0.3.2
+Name: wagtail-app-pages
+Version: 0.3.3
 Summary: Full MVC support for wagtail pages
 Home-page: https://github.com/mwesterhof/wagtail_app_pages
 Author: Marco Westerhof
 Author-email: westerhof.marco@gmail.com
 License: MIT license
 Keywords: wagtail_app_pages
 Platform: UNKNOWN
@@ -43,14 +43,20 @@
 
 [![Build Status](https://api.travis-ci.com/mwesterhof/wagtail_app_pages.svg?branch=master)](https://travis-ci.com/mwesterhof/wagtail_app_pages)
 
 
 =======
 History
 =======
+
+0.3.3
+-------------------
+
+* fix requirements
+
 0.3.2
 -------------------
 
 * Wagtail support for 5.0, dropping support for 3
 
 0.3.1
 -------------------
```

### Comparing `wagtail_app_pages-0.3.2/README.md` & `wagtail_app_pages-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/docs/Makefile` & `wagtail_app_pages-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/docs/caveats.rst` & `wagtail_app_pages-0.3.3/docs/caveats.rst`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/docs/conf.py` & `wagtail_app_pages-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/docs/examples.rst` & `wagtail_app_pages-0.3.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/docs/installation.rst` & `wagtail_app_pages-0.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/docs/make.bat` & `wagtail_app_pages-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/docs/readme.rst` & `wagtail_app_pages-0.3.3/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/docs/usage.rst` & `wagtail_app_pages-0.3.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/setup.py` & `wagtail_app_pages-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 requirements = [
-    "wagtail>=3.0,<4.3",
+    "wagtail>=4.0,<5.1",
 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
@@ -40,10 +40,10 @@
     keywords="wagtail_app_pages",
     name="wagtail_app_pages",
     packages=find_packages(include=["wagtail_app_pages"]),
     setup_requires=setup_requirements,
     test_suite="tests.testproject.testproject.tests",
     tests_require=test_requirements,
     url="https://github.com/mwesterhof/wagtail_app_pages",
-    version="0.3.2",
+    version="0.3.3",
     zip_safe=False,
 )
```

### Comparing `wagtail_app_pages-0.3.2/tests/testproject/home/migrations/0001_initial.py` & `wagtail_app_pages-0.3.3/tests/testproject/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/tests/testproject/home/migrations/0002_create_homepage.py` & `wagtail_app_pages-0.3.3/tests/testproject/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/tests/testproject/testproject/settings.py` & `wagtail_app_pages-0.3.3/tests/testproject/testproject/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/tests/testproject/testproject/templates/500.html` & `wagtail_app_pages-0.3.3/tests/testproject/testproject/templates/500.html`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/tests/testproject/testproject/templates/base.html` & `wagtail_app_pages-0.3.3/tests/testproject/testproject/templates/base.html`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/tests/testproject/testproject/tests/test_wagtail_app_pages.py` & `wagtail_app_pages-0.3.3/tests/testproject/testproject/tests/test_wagtail_app_pages.py`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/tests/testproject/testproject/urls.py` & `wagtail_app_pages-0.3.3/tests/testproject/testproject/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/wagtail_app_pages/compatibility.py` & `wagtail_app_pages-0.3.3/wagtail_app_pages/compatibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/wagtail_app_pages/models.py` & `wagtail_app_pages-0.3.3/wagtail_app_pages/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/PKG-INFO` & `wagtail_app_pages-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail-app-pages
-Version: 0.3.2
+Name: wagtail_app_pages
+Version: 0.3.3
 Summary: Full MVC support for wagtail pages
 Home-page: https://github.com/mwesterhof/wagtail_app_pages
 Author: Marco Westerhof
 Author-email: westerhof.marco@gmail.com
 License: MIT license
 Keywords: wagtail_app_pages
 Platform: UNKNOWN
@@ -43,14 +43,20 @@
 
 [![Build Status](https://api.travis-ci.com/mwesterhof/wagtail_app_pages.svg?branch=master)](https://travis-ci.com/mwesterhof/wagtail_app_pages)
 
 
 =======
 History
 =======
+
+0.3.3
+-------------------
+
+* fix requirements
+
 0.3.2
 -------------------
 
 * Wagtail support for 5.0, dropping support for 3
 
 0.3.1
 -------------------
```

### Comparing `wagtail_app_pages-0.3.2/wagtail_app_pages.egg-info/SOURCES.txt` & `wagtail_app_pages-0.3.3/wagtail_app_pages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

