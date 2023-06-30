# Comparing `tmp/snimpy-1.0.0.tar.gz` & `tmp/snimpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snimpy-1.0.0.tar", last modified: Sat May 29 15:38:02 2021, max compression
+gzip compressed data, was "snimpy-1.0.1.tar", last modified: Fri Jun 30 06:51:27 2023, max compression
```

## Comparing `snimpy-1.0.0.tar` & `snimpy-1.0.1.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.853861 snimpy-1.0.0/
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/.github/
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/.github/workflows/
--rw-r--r--   0 bernat     (500) users      (100)     1324 2021-05-15 10:37:00.000000 snimpy-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 bernat     (500) users      (100)      181 2016-11-15 06:58:49.000000 snimpy-1.0.0/.gitignore
--rw-r--r--   0 bernat     (500) users      (100)      108 2016-11-15 06:58:49.000000 snimpy-1.0.0/.gitmodules
--rw-r--r--   0 bernat     (500) users      (100)      132 2016-11-15 06:58:49.000000 snimpy-1.0.0/AUTHORS.rst
--rw-r--r--   0 bernat     (500) users      (100)     3121 2020-05-03 12:37:08.000000 snimpy-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 bernat     (500) users      (100)     3599 2021-05-29 15:35:38.000000 snimpy-1.0.0/HISTORY.rst
--rw-r--r--   0 bernat     (500) users      (100)      437 2016-11-15 06:58:49.000000 snimpy-1.0.0/MANIFEST.in
--rw-r--r--   0 bernat     (500) users      (100)     1435 2020-05-04 12:32:07.000000 snimpy-1.0.0/Makefile
--rw-r--r--   0 bernat     (500) users      (100)     8043 2021-05-29 15:38:02.853861 snimpy-1.0.0/PKG-INFO
--rw-r--r--   0 bernat     (500) users      (100)     1945 2020-11-06 14:14:55.000000 snimpy-1.0.0/README.rst
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/docs/
--rw-r--r--   0 bernat     (500) users      (100)     6777 2016-11-15 06:58:49.000000 snimpy-1.0.0/docs/Makefile
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/docs/_static/
--rw-r--r--   0 bernat     (500) users      (100)    12067 2016-11-15 06:58:49.000000 snimpy-1.0.0/docs/_static/snimpy.svg
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/docs/_themes/
--rw-r--r--   0 bernat     (500) users      (100)       22 2014-01-31 18:44:32.000000 snimpy-1.0.0/docs/_themes/.gitignore
--rw-r--r--   0 bernat     (500) users      (100)     1789 2014-01-31 18:44:32.000000 snimpy-1.0.0/docs/_themes/LICENSE
--rw-r--r--   0 bernat     (500) users      (100)     1093 2014-01-31 18:44:32.000000 snimpy-1.0.0/docs/_themes/README
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/docs/_themes/flask/
--rw-r--r--   0 bernat     (500) users      (100)      693 2014-01-31 18:45:14.000000 snimpy-1.0.0/docs/_themes/flask/layout.html
--rw-r--r--   0 bernat     (500) users      (100)      590 2014-01-31 18:45:14.000000 snimpy-1.0.0/docs/_themes/flask/relations.html
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/docs/_themes/flask/static/
--rw-r--r--   0 bernat     (500) users      (100)     9062 2014-01-31 18:45:16.000000 snimpy-1.0.0/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 bernat     (500) users      (100)      164 2014-01-31 18:45:14.000000 snimpy-1.0.0/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/docs/_themes/flask_small/
--rw-r--r--   0 bernat     (500) users      (100)      683 2014-01-31 18:45:14.000000 snimpy-1.0.0/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.849861 snimpy-1.0.0/docs/_themes/flask_small/static/
--rw-r--r--   0 bernat     (500) users      (100)     4609 2014-01-31 18:45:16.000000 snimpy-1.0.0/docs/_themes/flask_small/static/flasky.css_t
--rw-r--r--   0 bernat     (500) users      (100)      184 2014-01-31 18:45:14.000000 snimpy-1.0.0/docs/_themes/flask_small/theme.conf
--rw-r--r--   0 bernat     (500) users      (100)     4875 2014-01-31 18:44:32.000000 snimpy-1.0.0/docs/_themes/flask_theme_support.py
--rw-r--r--   0 bernat     (500) users      (100)      797 2016-11-15 06:58:49.000000 snimpy-1.0.0/docs/api.rst
--rw-r--r--   0 bernat     (500) users      (100)     1278 2021-05-15 10:37:00.000000 snimpy-1.0.0/docs/conf.py
--rw-r--r--   0 bernat     (500) users      (100)       32 2016-11-15 06:58:49.000000 snimpy-1.0.0/docs/contributing.rst
--rw-r--r--   0 bernat     (500) users      (100)       27 2016-11-15 06:58:49.000000 snimpy-1.0.0/docs/history.rst
--rw-r--r--   0 bernat     (500) users      (100)     2379 2016-11-15 06:58:49.000000 snimpy-1.0.0/docs/index.rst
--rw-r--r--   0 bernat     (500) users      (100)     1043 2016-11-15 06:58:49.000000 snimpy-1.0.0/docs/installation.rst
--rw-r--r--   0 bernat     (500) users      (100)      997 2016-11-15 06:58:49.000000 snimpy-1.0.0/docs/license.rst
--rw-r--r--   0 bernat     (500) users      (100)     6814 2021-04-09 20:14:39.000000 snimpy-1.0.0/docs/usage.rst
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.853861 snimpy-1.0.0/examples/
--rw-r--r--   0 bernat     (500) users      (100)     1234 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/add-vlan.py
--rw-r--r--   0 bernat     (500) users      (100)      531 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/disable-port-ingress-filtering.py
--rw-r--r--   0 bernat     (500) users      (100)     1769 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/enable-lldp.py
--rw-r--r--   0 bernat     (500) users      (100)      909 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/get-serial.py
--rw-r--r--   0 bernat     (500) users      (100)      114 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/list-interfaces.py
--rw-r--r--   0 bernat     (500) users      (100)      620 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/list-routes.py
--rw-r--r--   0 bernat     (500) users      (100)      585 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/rename-vlan.py
--rwxr-xr-x   0 bernat     (500) users      (100)     2176 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/set-syslog-ntp.py
--rw-r--r--   0 bernat     (500) users      (100)      630 2021-05-15 10:37:00.000000 snimpy-1.0.0/examples/vlan-and-interfaces.py
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.853861 snimpy-1.0.0/man/
--rw-r--r--   0 bernat     (500) users      (100)     1015 2016-11-15 06:58:49.000000 snimpy-1.0.0/man/snimpy.1
--rw-r--r--   0 bernat     (500) users      (100)       38 2021-05-29 15:38:02.853861 snimpy-1.0.0/setup.cfg
--rw-r--r--   0 bernat     (500) users      (100)     2491 2020-05-03 12:37:08.000000 snimpy-1.0.0/setup.py
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.853861 snimpy-1.0.0/snimpy/
--rw-r--r--   0 bernat     (500) users      (100)      197 2018-10-11 20:02:19.000000 snimpy-1.0.0/snimpy/__init__.py
--rw-r--r--   0 bernat     (500) users      (100)      905 2018-10-11 20:02:19.000000 snimpy-1.0.0/snimpy/__main__.py
--rw-r--r--   0 bernat     (500) users      (100)      132 2021-05-29 15:38:02.000000 snimpy-1.0.0/snimpy/_version.py
--rw-r--r--   0 bernat     (500) users      (100)    29843 2021-05-15 10:37:00.000000 snimpy-1.0.0/snimpy/basictypes.py
--rw-r--r--   0 bernat     (500) users      (100)     1757 2021-05-15 10:37:00.000000 snimpy-1.0.0/snimpy/config.py
--rw-r--r--   0 bernat     (500) users      (100)     5810 2021-05-15 10:37:00.000000 snimpy-1.0.0/snimpy/main.py
--rw-r--r--   0 bernat     (500) users      (100)    20966 2021-05-29 14:06:57.000000 snimpy-1.0.0/snimpy/manager.py
--rw-r--r--   0 bernat     (500) users      (100)    23683 2021-05-15 10:37:00.000000 snimpy-1.0.0/snimpy/mib.py
--rw-r--r--   0 bernat     (500) users      (100)     5210 2018-10-11 20:02:19.000000 snimpy-1.0.0/snimpy/smi_build.py
--rw-r--r--   0 bernat     (500) users      (100)    16256 2021-05-15 10:37:00.000000 snimpy-1.0.0/snimpy/snmp.py
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.853861 snimpy-1.0.0/snimpy.egg-info/
--rw-r--r--   0 bernat     (500) users      (100)     8043 2021-05-29 15:38:02.000000 snimpy-1.0.0/snimpy.egg-info/PKG-INFO
--rw-r--r--   0 bernat     (500) users      (100)     1511 2021-05-29 15:38:02.000000 snimpy-1.0.0/snimpy.egg-info/SOURCES.txt
--rw-r--r--   0 bernat     (500) users      (100)        1 2021-05-29 15:38:02.000000 snimpy-1.0.0/snimpy.egg-info/dependency_links.txt
--rw-r--r--   0 bernat     (500) users      (100)       49 2021-05-29 15:38:02.000000 snimpy-1.0.0/snimpy.egg-info/entry_points.txt
--rw-r--r--   0 bernat     (500) users      (100)        1 2015-11-14 17:00:37.000000 snimpy-1.0.0/snimpy.egg-info/not-zip-safe
--rw-r--r--   0 bernat     (500) users      (100)       33 2021-05-29 15:38:02.000000 snimpy-1.0.0/snimpy.egg-info/requires.txt
--rw-r--r--   0 bernat     (500) users      (100)        7 2021-05-29 15:38:02.000000 snimpy-1.0.0/snimpy.egg-info/top_level.txt
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2021-05-29 15:38:02.853861 snimpy-1.0.0/tests/
--rw-r--r--   0 bernat     (500) users      (100)      624 2016-11-15 06:58:49.000000 snimpy-1.0.0/tests/SNIMPY-INVALID-MIB.mib
--rw-r--r--   0 bernat     (500) users      (100)    13822 2017-12-16 13:48:00.000000 snimpy-1.0.0/tests/SNIMPY-MIB.mib
--rw-r--r--   0 bernat     (500) users      (100)    18561 2021-05-15 10:37:00.000000 snimpy-1.0.0/tests/agent.py
--rw-r--r--   0 bernat     (500) users      (100)    26672 2021-05-15 10:37:00.000000 snimpy-1.0.0/tests/test_basictypes.py
--rw-r--r--   0 bernat     (500) users      (100)     1238 2021-05-15 10:37:00.000000 snimpy-1.0.0/tests/test_conf.py
--rw-r--r--   0 bernat     (500) users      (100)     1132 2021-05-15 10:37:00.000000 snimpy-1.0.0/tests/test_main.py
--rw-r--r--   0 bernat     (500) users      (100)    20324 2021-05-15 10:37:00.000000 snimpy-1.0.0/tests/test_manager.py
--rw-r--r--   0 bernat     (500) users      (100)    18875 2021-05-15 10:37:00.000000 snimpy-1.0.0/tests/test_mib.py
--rw-r--r--   0 bernat     (500) users      (100)    15585 2021-05-15 10:37:00.000000 snimpy-1.0.0/tests/test_snmp.py
--rw-r--r--   0 bernat     (500) users      (100)      693 2021-05-15 10:37:00.000000 snimpy-1.0.0/tox.ini
--rw-r--r--   0 bernat     (500) users      (100)       21 2021-05-29 15:38:02.000000 snimpy-1.0.0/version.txt
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/.github/
+-rw-r--r--   0 bernat     (500) users      (100)      157 2022-12-02 17:49:39.000000 snimpy-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/.github/workflows/
+-rw-r--r--   0 bernat     (500) users      (100)     1399 2023-06-24 22:17:32.000000 snimpy-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 bernat     (500) users      (100)      189 2022-12-14 10:15:32.000000 snimpy-1.0.1/.gitignore
+-rw-r--r--   0 bernat     (500) users      (100)      108 2016-11-15 06:58:49.000000 snimpy-1.0.1/.gitmodules
+-rw-r--r--   0 bernat     (500) users      (100)      132 2016-11-15 06:58:49.000000 snimpy-1.0.1/AUTHORS.rst
+-rw-r--r--   0 bernat     (500) users      (100)     3089 2021-10-22 06:02:08.000000 snimpy-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 bernat     (500) users      (100)     3690 2023-06-30 06:47:54.000000 snimpy-1.0.1/HISTORY.rst
+-rw-r--r--   0 bernat     (500) users      (100)      437 2016-11-15 06:58:49.000000 snimpy-1.0.1/MANIFEST.in
+-rw-r--r--   0 bernat     (500) users      (100)     1474 2021-10-22 06:02:08.000000 snimpy-1.0.1/Makefile
+-rw-r--r--   0 bernat     (500) users      (100)     6264 2023-06-30 06:51:27.635898 snimpy-1.0.1/PKG-INFO
+-rw-r--r--   0 bernat     (500) users      (100)     1945 2021-05-29 15:40:24.000000 snimpy-1.0.1/README.rst
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/
+-rw-r--r--   0 bernat     (500) users      (100)     6777 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/Makefile
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_static/
+-rw-r--r--   0 bernat     (500) users      (100)    12067 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/_static/snimpy.svg
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/
+-rw-r--r--   0 bernat     (500) users      (100)       22 2014-01-31 18:44:32.000000 snimpy-1.0.1/docs/_themes/.gitignore
+-rw-r--r--   0 bernat     (500) users      (100)     1789 2014-01-31 18:44:32.000000 snimpy-1.0.1/docs/_themes/LICENSE
+-rw-r--r--   0 bernat     (500) users      (100)     1093 2014-01-31 18:44:32.000000 snimpy-1.0.1/docs/_themes/README
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/flask/
+-rw-r--r--   0 bernat     (500) users      (100)      693 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask/layout.html
+-rw-r--r--   0 bernat     (500) users      (100)      590 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask/relations.html
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/flask/static/
+-rw-r--r--   0 bernat     (500) users      (100)     9062 2014-01-31 18:45:16.000000 snimpy-1.0.1/docs/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 bernat     (500) users      (100)      164 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/flask_small/
+-rw-r--r--   0 bernat     (500) users      (100)      683 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask_small/layout.html
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/flask_small/static/
+-rw-r--r--   0 bernat     (500) users      (100)     4609 2014-01-31 18:45:16.000000 snimpy-1.0.1/docs/_themes/flask_small/static/flasky.css_t
+-rw-r--r--   0 bernat     (500) users      (100)      184 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask_small/theme.conf
+-rw-r--r--   0 bernat     (500) users      (100)     3905 2023-06-30 06:50:57.000000 snimpy-1.0.1/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 bernat     (500) users      (100)      797 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/api.rst
+-rwxr-xr-x   0 bernat     (500) users      (100)     1216 2023-06-30 06:51:10.000000 snimpy-1.0.1/docs/conf.py
+-rw-r--r--   0 bernat     (500) users      (100)       32 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/contributing.rst
+-rw-r--r--   0 bernat     (500) users      (100)       27 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/history.rst
+-rw-r--r--   0 bernat     (500) users      (100)     2372 2023-06-27 20:20:26.000000 snimpy-1.0.1/docs/index.rst
+-rw-r--r--   0 bernat     (500) users      (100)     1043 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/installation.rst
+-rw-r--r--   0 bernat     (500) users      (100)      997 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/license.rst
+-rw-r--r--   0 bernat     (500) users      (100)     6814 2021-04-09 20:14:39.000000 snimpy-1.0.1/docs/usage.rst
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/examples/
+-rw-r--r--   0 bernat     (500) users      (100)     1234 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/add-vlan.py
+-rw-r--r--   0 bernat     (500) users      (100)      531 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/disable-port-ingress-filtering.py
+-rw-r--r--   0 bernat     (500) users      (100)     1769 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/enable-lldp.py
+-rw-r--r--   0 bernat     (500) users      (100)      909 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/get-serial.py
+-rw-r--r--   0 bernat     (500) users      (100)      114 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/list-interfaces.py
+-rw-r--r--   0 bernat     (500) users      (100)      620 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/list-routes.py
+-rw-r--r--   0 bernat     (500) users      (100)      585 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/rename-vlan.py
+-rwxr-xr-x   0 bernat     (500) users      (100)     2178 2023-06-24 22:17:32.000000 snimpy-1.0.1/examples/set-syslog-ntp.py
+-rw-r--r--   0 bernat     (500) users      (100)      630 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/vlan-and-interfaces.py
+-rw-r--r--   0 bernat     (500) users      (100)      966 2022-12-14 10:01:45.000000 snimpy-1.0.1/flake.lock
+-rw-r--r--   0 bernat     (500) users      (100)     1196 2023-06-27 20:38:13.000000 snimpy-1.0.1/flake.nix
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/man/
+-rw-r--r--   0 bernat     (500) users      (100)     1015 2016-11-15 06:58:49.000000 snimpy-1.0.1/man/snimpy.1
+-rw-r--r--   0 bernat     (500) users      (100)       38 2023-06-30 06:51:27.635898 snimpy-1.0.1/setup.cfg
+-rw-r--r--   0 bernat     (500) users      (100)     2140 2023-06-30 06:51:10.000000 snimpy-1.0.1/setup.py
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/snimpy/
+-rw-r--r--   0 bernat     (500) users      (100)      197 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/__init__.py
+-rw-r--r--   0 bernat     (500) users      (100)      905 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/__main__.py
+-rw-r--r--   0 bernat     (500) users      (100)      132 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy/_version.py
+-rw-r--r--   0 bernat     (500) users      (100)    29843 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/basictypes.py
+-rw-r--r--   0 bernat     (500) users      (100)     1781 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/config.py
+-rw-r--r--   0 bernat     (500) users      (100)     5810 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/main.py
+-rw-r--r--   0 bernat     (500) users      (100)    20966 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/manager.py
+-rw-r--r--   0 bernat     (500) users      (100)    23776 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/mib.py
+-rw-r--r--   0 bernat     (500) users      (100)     5210 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/smi_build.py
+-rw-r--r--   0 bernat     (500) users      (100)    16256 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/snmp.py
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/snimpy.egg-info/
+-rw-r--r--   0 bernat     (500) users      (100)     6264 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/PKG-INFO
+-rw-r--r--   0 bernat     (500) users      (100)     1555 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 bernat     (500) users      (100)        1 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 bernat     (500) users      (100)       48 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/entry_points.txt
+-rw-r--r--   0 bernat     (500) users      (100)        1 2015-11-14 17:00:37.000000 snimpy-1.0.1/snimpy.egg-info/not-zip-safe
+-rw-r--r--   0 bernat     (500) users      (100)       42 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/requires.txt
+-rw-r--r--   0 bernat     (500) users      (100)        7 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/top_level.txt
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/tests/
+-rw-r--r--   0 bernat     (500) users      (100)      624 2016-11-15 06:58:49.000000 snimpy-1.0.1/tests/SNIMPY-INVALID-MIB.mib
+-rw-r--r--   0 bernat     (500) users      (100)    13822 2017-12-16 13:48:00.000000 snimpy-1.0.1/tests/SNIMPY-MIB.mib
+-rw-r--r--   0 bernat     (500) users      (100)    18561 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/agent.py
+-rw-r--r--   0 bernat     (500) users      (100)    26698 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_basictypes.py
+-rw-r--r--   0 bernat     (500) users      (100)     1238 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_conf.py
+-rw-r--r--   0 bernat     (500) users      (100)     1149 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_main.py
+-rw-r--r--   0 bernat     (500) users      (100)    20324 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_manager.py
+-rw-r--r--   0 bernat     (500) users      (100)    18875 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_mib.py
+-rw-r--r--   0 bernat     (500) users      (100)    15585 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_snmp.py
+-rw-r--r--   0 bernat     (500) users      (100)      744 2023-06-27 20:38:04.000000 snimpy-1.0.1/tox.ini
+-rw-r--r--   0 bernat     (500) users      (100)       21 2023-06-30 06:51:27.000000 snimpy-1.0.1/version.txt
```

### Comparing `snimpy-1.0.0/.github/workflows/tests.yml` & `snimpy-1.0.1/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 name: Tests
 on:
   push:
+    branches:
+      - master
+    tags:
+      - "*.*"
   pull_request:
   schedule:
     - cron: 30 7 2 * *
 jobs:
   tests:
     name: Run tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version:
-          - 3.6
           - 3.7
           - 3.8
           - 3.9
+          - "3.10"
+          - "3.11"
     steps:
       - uses: actions/checkout@v1
         with:
           submodules: true
       - name: Setup Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install non-Python dependencies
         run: >
           sudo apt -qy update;
           sudo apt -qy install
           pkg-config
```

### Comparing `snimpy-1.0.0/CONTRIBUTING.rst` & `snimpy-1.0.1/CONTRIBUTING.rst`

 * *Files 7% similar despite different names*

```diff
@@ -62,27 +62,26 @@
 
     $ git clone git@github.com:your_name_here/snimpy.git
 
 3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
 
     $ mkvirtualenv snimpy
     $ cd snimpy/
-    $ python setup.py develop
+    $ pip install -e
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
   Now you can make your changes locally.
 
 5. When you're done making changes, check that your changes pass flake8 and the
 tests, including testing other Python versions with tox::
 
     $ flake8 snimpy tests
-	  $ python setup.py test
     $ tox
 
   To get flake8 and tox, just pip install them into your virtualenv. 
 
 6. Commit your changes and push your branch to GitHub::
 
     $ git add .
@@ -105,8 +104,8 @@
    sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
 
-	$ python -m nose tests/test_snmp.py
+	$ python3 -m pytest tests/test_snmp.py
```

### Comparing `snimpy-1.0.0/HISTORY.rst` & `snimpy-1.0.1/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+1.0.1 (2023-06-30)
+++++++++++++++++++
+
+* Switch to pysnmp-lextudio, a maintained fork of PySNMP.
+
 1.0.0 (2021-05-29)
 ++++++++++++++++++
 
 * Drop compatibility with Python 2.
 
 0.8.14 (2020-04-26)
 +++++++++++++++++++
@@ -108,15 +113,15 @@
 
 * Major rewrite.
 * SNMP support is now provided through PySNMP_.
 * MIB parsing is still done with ``libsmi`` but through CFFI instead of a
   C module.
 * More unittests. Many bugfixes.
 
-.. _PySNMP: http://pysnmp.sourceforge.net/
+.. _PySNMP: https://www.pysnmp.com/
 
 0.6.4 (2013-03-21)
 ++++++++++++++++++
 
 * GETBULK support.
 * MacAddress SMI type support.
```

### Comparing `snimpy-1.0.0/Makefile` & `snimpy-1.0.1/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .PHONY: clean-pyc clean-build docs
 
 open := $(shell { which xdg-open || which open; } 2>/dev/null)
+python = python3
 
 help:
 	@echo "Please use \`make <target>' where <target> is one of"
 	@echo "  clean-build   to remove build artifacts"
 	@echo "  clean-pyc     to remove Python file artifacts"
 	@echo "  lint          to check style with flake8"
 	@echo "  test          to run tests quickly with the default Python"
@@ -28,29 +29,30 @@
 	find . -name '__pycache__' -type d -exec rm -rf {} +
 
 lint:
 	flake8 snimpy tests
 	interrogate --fail-under 50 -v snimpy tests
 
 test:
-	python -m nose
+	$(python) -m pytest
 
 test-all:
 	tox
 
 coverage:
-	coverage run --source snimpy setup.py test
+	coverage run --source snimpy -m unittest discover -s tests
 	coverage report -m
 	coverage html
 	$(open) htmlcov/index.html
 
 docs:
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
 	$(open) docs/_build/html/index.html
 
 release: clean
-	python setup.py sdist upload
+	$(python) -m build
+	twine upload
 
 sdist: clean
-	python setup.py sdist
+	$(python) -m build
 	ls -l dist
```

### Comparing `snimpy-1.0.0/README.rst` & `snimpy-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ===============================
 snimpy
 ===============================
 
-.. image:: https://badge.fury.io/py/snimpy.png
+.. image:: https://badge.fury.io/py/snimpy.svg
     :target: http://badge.fury.io/py/snimpy
     
 .. image:: https://github.com/vincentbernat/snimpy/workflows/Tests/badge.svg
 
-.. image:: https://coveralls.io/repos/vincentbernat/snimpy/badge.png
+.. image:: https://coveralls.io/repos/vincentbernat/snimpy/badge.svg
         :target: https://coveralls.io/r/vincentbernat/snimpy
 
 ---
 
  Interactive SNMP tool.
 
 *Snimpy* is a Python-based tool providing a simple interface to build
```

### Comparing `snimpy-1.0.0/docs/Makefile` & `snimpy-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_static/snimpy.svg` & `snimpy-1.0.1/docs/_static/snimpy.svg`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_themes/LICENSE` & `snimpy-1.0.1/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_themes/README` & `snimpy-1.0.1/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_themes/flask/layout.html` & `snimpy-1.0.1/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_themes/flask/relations.html` & `snimpy-1.0.1/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_themes/flask/static/flasky.css_t` & `snimpy-1.0.1/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_themes/flask_small/layout.html` & `snimpy-1.0.1/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_themes/flask_small/static/flasky.css_t` & `snimpy-1.0.1/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/_themes/flask_theme_support.py` & `snimpy-1.0.1/docs/_themes/flask_theme_support.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 # flasky extensions.  flasky pygments style based on tango style
 from pygments.style import Style
-from pygments.token import Keyword, Name, Comment, String, Error, \
-     Number, Operator, Generic, Whitespace, Punctuation, Other, Literal
+from pygments.token import (
+    Keyword,
+    Name,
+    Comment,
+    String,
+    Error,
+    Number,
+    Operator,
+    Generic,
+    Whitespace,
+    Punctuation,
+    Other,
+    Literal,
+)
 
 
 class FlaskyStyle(Style):
     background_color = "#f8f8f8"
     default_style = ""
 
     styles = {
         # No corresponding class for the following:
-        #Text:                     "", # class:  ''
-        Whitespace:                "underline #f8f8f8",      # class: 'w'
-        Error:                     "#a40000 border:#ef2929", # class: 'err'
-        Other:                     "#000000",                # class 'x'
-
-        Comment:                   "italic #8f5902", # class: 'c'
-        Comment.Preproc:           "noitalic",       # class: 'cp'
-
-        Keyword:                   "bold #004461",   # class: 'k'
-        Keyword.Constant:          "bold #004461",   # class: 'kc'
-        Keyword.Declaration:       "bold #004461",   # class: 'kd'
-        Keyword.Namespace:         "bold #004461",   # class: 'kn'
-        Keyword.Pseudo:            "bold #004461",   # class: 'kp'
-        Keyword.Reserved:          "bold #004461",   # class: 'kr'
-        Keyword.Type:              "bold #004461",   # class: 'kt'
-
-        Operator:                  "#582800",   # class: 'o'
-        Operator.Word:             "bold #004461",   # class: 'ow' - like keywords
-
-        Punctuation:               "bold #000000",   # class: 'p'
-
+        # Text:                     "", # class:  ''
+        Whitespace: "underline #f8f8f8",  # class: 'w'
+        Error: "#a40000 border:#ef2929",  # class: 'err'
+        Other: "#000000",  # class 'x'
+        Comment: "italic #8f5902",  # class: 'c'
+        Comment.Preproc: "noitalic",  # class: 'cp'
+        Keyword: "bold #004461",  # class: 'k'
+        Keyword.Constant: "bold #004461",  # class: 'kc'
+        Keyword.Declaration: "bold #004461",  # class: 'kd'
+        Keyword.Namespace: "bold #004461",  # class: 'kn'
+        Keyword.Pseudo: "bold #004461",  # class: 'kp'
+        Keyword.Reserved: "bold #004461",  # class: 'kr'
+        Keyword.Type: "bold #004461",  # class: 'kt'
+        Operator: "#582800",  # class: 'o'
+        Operator.Word: "bold #004461",  # class: 'ow' - like keywords
+        Punctuation: "bold #000000",  # class: 'p'
         # because special names such as Name.Class, Name.Function, etc.
         # are not recognized as such later in the parsing, we choose them
         # to look the same as ordinary variables.
-        Name:                      "#000000",        # class: 'n'
-        Name.Attribute:            "#c4a000",        # class: 'na' - to be revised
-        Name.Builtin:              "#004461",        # class: 'nb'
-        Name.Builtin.Pseudo:       "#3465a4",        # class: 'bp'
-        Name.Class:                "#000000",        # class: 'nc' - to be revised
-        Name.Constant:             "#000000",        # class: 'no' - to be revised
-        Name.Decorator:            "#888",           # class: 'nd' - to be revised
-        Name.Entity:               "#ce5c00",        # class: 'ni'
-        Name.Exception:            "bold #cc0000",   # class: 'ne'
-        Name.Function:             "#000000",        # class: 'nf'
-        Name.Property:             "#000000",        # class: 'py'
-        Name.Label:                "#f57900",        # class: 'nl'
-        Name.Namespace:            "#000000",        # class: 'nn' - to be revised
-        Name.Other:                "#000000",        # class: 'nx'
-        Name.Tag:                  "bold #004461",   # class: 'nt' - like a keyword
-        Name.Variable:             "#000000",        # class: 'nv' - to be revised
-        Name.Variable.Class:       "#000000",        # class: 'vc' - to be revised
-        Name.Variable.Global:      "#000000",        # class: 'vg' - to be revised
-        Name.Variable.Instance:    "#000000",        # class: 'vi' - to be revised
-
-        Number:                    "#990000",        # class: 'm'
-
-        Literal:                   "#000000",        # class: 'l'
-        Literal.Date:              "#000000",        # class: 'ld'
-
-        String:                    "#4e9a06",        # class: 's'
-        String.Backtick:           "#4e9a06",        # class: 'sb'
-        String.Char:               "#4e9a06",        # class: 'sc'
-        String.Doc:                "italic #8f5902", # class: 'sd' - like a comment
-        String.Double:             "#4e9a06",        # class: 's2'
-        String.Escape:             "#4e9a06",        # class: 'se'
-        String.Heredoc:            "#4e9a06",        # class: 'sh'
-        String.Interpol:           "#4e9a06",        # class: 'si'
-        String.Other:              "#4e9a06",        # class: 'sx'
-        String.Regex:              "#4e9a06",        # class: 'sr'
-        String.Single:             "#4e9a06",        # class: 's1'
-        String.Symbol:             "#4e9a06",        # class: 'ss'
-
-        Generic:                   "#000000",        # class: 'g'
-        Generic.Deleted:           "#a40000",        # class: 'gd'
-        Generic.Emph:              "italic #000000", # class: 'ge'
-        Generic.Error:             "#ef2929",        # class: 'gr'
-        Generic.Heading:           "bold #000080",   # class: 'gh'
-        Generic.Inserted:          "#00A000",        # class: 'gi'
-        Generic.Output:            "#888",           # class: 'go'
-        Generic.Prompt:            "#745334",        # class: 'gp'
-        Generic.Strong:            "bold #000000",   # class: 'gs'
-        Generic.Subheading:        "bold #800080",   # class: 'gu'
-        Generic.Traceback:         "bold #a40000",   # class: 'gt'
+        Name: "#000000",  # class: 'n'
+        Name.Attribute: "#c4a000",  # class: 'na' - to be revised
+        Name.Builtin: "#004461",  # class: 'nb'
+        Name.Builtin.Pseudo: "#3465a4",  # class: 'bp'
+        Name.Class: "#000000",  # class: 'nc' - to be revised
+        Name.Constant: "#000000",  # class: 'no' - to be revised
+        Name.Decorator: "#888",  # class: 'nd' - to be revised
+        Name.Entity: "#ce5c00",  # class: 'ni'
+        Name.Exception: "bold #cc0000",  # class: 'ne'
+        Name.Function: "#000000",  # class: 'nf'
+        Name.Property: "#000000",  # class: 'py'
+        Name.Label: "#f57900",  # class: 'nl'
+        Name.Namespace: "#000000",  # class: 'nn' - to be revised
+        Name.Other: "#000000",  # class: 'nx'
+        Name.Tag: "bold #004461",  # class: 'nt' - like a keyword
+        Name.Variable: "#000000",  # class: 'nv' - to be revised
+        Name.Variable.Class: "#000000",  # class: 'vc' - to be revised
+        Name.Variable.Global: "#000000",  # class: 'vg' - to be revised
+        Name.Variable.Instance: "#000000",  # class: 'vi' - to be revised
+        Number: "#990000",  # class: 'm'
+        Literal: "#000000",  # class: 'l'
+        Literal.Date: "#000000",  # class: 'ld'
+        String: "#4e9a06",  # class: 's'
+        String.Backtick: "#4e9a06",  # class: 'sb'
+        String.Char: "#4e9a06",  # class: 'sc'
+        String.Doc: "italic #8f5902",  # class: 'sd' - like a comment
+        String.Double: "#4e9a06",  # class: 's2'
+        String.Escape: "#4e9a06",  # class: 'se'
+        String.Heredoc: "#4e9a06",  # class: 'sh'
+        String.Interpol: "#4e9a06",  # class: 'si'
+        String.Other: "#4e9a06",  # class: 'sx'
+        String.Regex: "#4e9a06",  # class: 'sr'
+        String.Single: "#4e9a06",  # class: 's1'
+        String.Symbol: "#4e9a06",  # class: 'ss'
+        Generic: "#000000",  # class: 'g'
+        Generic.Deleted: "#a40000",  # class: 'gd'
+        Generic.Emph: "italic #000000",  # class: 'ge'
+        Generic.Error: "#ef2929",  # class: 'gr'
+        Generic.Heading: "bold #000080",  # class: 'gh'
+        Generic.Inserted: "#00A000",  # class: 'gi'
+        Generic.Output: "#888",  # class: 'go'
+        Generic.Prompt: "#745334",  # class: 'gp'
+        Generic.Strong: "bold #000000",  # class: 'gs'
+        Generic.Subheading: "bold #800080",  # class: 'gu'
+        Generic.Traceback: "bold #a40000",  # class: 'gt'
     }
```

### Comparing `snimpy-1.0.0/docs/api.rst` & `snimpy-1.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/conf.py` & `snimpy-1.0.1/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 import sys
 import os
+from unittest.mock import Mock
 
-rtd = os.environ.get('READTHEDOCS', None) == 'True'
 cwd = os.getcwd()
 project_root = os.path.dirname(cwd)
 sys.path.insert(0, project_root)
 
 # -- Don't try to load CFFI (doesn't work on RTD) -----------------------------
 
-if rtd:
-    from mock import Mock
-    sys.modules['cffi'] = Mock()
-    sys.modules['cffi.verifier'] = Mock()
+sys.modules['cffi'] = Mock()
+sys.modules['cffi.verifier'] = Mock()
 import snimpy
 
 # -- General configuration ----------------------------------------------------
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
 templates_path = ['_templates']
 source_suffix = '.rst'
```

### Comparing `snimpy-1.0.0/docs/index.rst` & `snimpy-1.0.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 For Python, there are other bindings. For example, pysnmp_ provides a
 pure Python implementation. However, MIBs need to be
 compiled. Moreover, the exposed interface is still low-level. Sending
 a simple SNMP GET can either take 10 lines or one line wrapped into 10
 lines.
 
-.. _pysnmp: http://pysnmp.sourceforge.net/
+.. _pysnmp: https://www.pysnmp.com/
 
 The two main points of *Snimpy* are:
 
 * very high-level interface relying on MIBs
 * raise exceptions when something goes wrong
 
 Meantime, another Pythonic SNMP library based on Net-SNMP has been
```

### Comparing `snimpy-1.0.0/docs/installation.rst` & `snimpy-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/license.rst` & `snimpy-1.0.1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/docs/usage.rst` & `snimpy-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/examples/add-vlan.py` & `snimpy-1.0.1/examples/add-vlan.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/examples/disable-port-ingress-filtering.py` & `snimpy-1.0.1/examples/disable-port-ingress-filtering.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/examples/enable-lldp.py` & `snimpy-1.0.1/examples/enable-lldp.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/examples/get-serial.py` & `snimpy-1.0.1/examples/get-serial.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/examples/list-routes.py` & `snimpy-1.0.1/examples/list-routes.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/examples/rename-vlan.py` & `snimpy-1.0.1/examples/rename-vlan.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/examples/set-syslog-ntp.py` & `snimpy-1.0.1/examples/set-syslog-ntp.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 host = sys.argv[2]
 targets = sys.argv[4:]
 operation = sys.argv[1]
 
 try:
     s = M(host=host, community=sys.argv[3])
     sid = str(s.sysObjectID)
-except snmp.SNMPException, e:
+except snmp.SNMPException as e:
     print("%s: %s" % (host, e))
     sys.exit(1)
 
 if sid.startswith("1.3.6.1.4.1.45.3."):
     # Nortel
     print("%s is Nortel 55xx" % host)
     load(os.path.expanduser("~/.snmp/mibs/SYNOPTICS-ROOT-MIB"))
```

### Comparing `snimpy-1.0.0/examples/vlan-and-interfaces.py` & `snimpy-1.0.1/examples/vlan-and-interfaces.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/man/snimpy.1` & `snimpy-1.0.1/man/snimpy.1`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/setup.py` & `snimpy-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 from setuptools import setup
 from setuptools.command.test import test
 import snimpy
 
 rtd = os.environ.get('READTHEDOCS', None) == 'True'
 
 
@@ -45,22 +44,16 @@
               'console_scripts': [
                   'snimpy = snimpy.main:interact',
               ],
           },
           data_files=[('share/man/man1', ['man/snimpy.1'])],
           zip_safe=False,
           cffi_modules=(not rtd and ["snimpy/smi_build.py:ffi"] or []),
-          install_requires=["cffi >= 1.0.0", "pysnmp >= 4", "setuptools"],
+          install_requires=["cffi >= 1.0.0", "pysnmp-lextudio >= 4", "setuptools"],
           setup_requires=["cffi >= 1.0.0", "vcversioner"],
-          tests_require=list(filter(None, ["cffi >= 1.0.0",
-                                           "pysnmp >= 4",
-                                           "nose",
-                                           sys.version_info < (3, 6) and
-                                           "mock < 4" or "mock"])),
-          test_suite="nose.collector",
           cmdclass={
               "test": SnimpyTestCommand
           },
           pbr=False,
           vcversioner={
               'version_module_paths': ['snimpy/_version.py'],
           },
```

### Comparing `snimpy-1.0.0/snimpy/__main__.py` & `snimpy-1.0.1/snimpy/__main__.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/snimpy/basictypes.py` & `snimpy-1.0.1/snimpy/basictypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
             value = [value]
         for v in value:
             if not isinstance(v, int):
                 raise NotImplementedError(
                     "on string, bit-operation are limited to integers")
             if len(nvalue) < (v >> 3) + 1:
                 return False
-            if not(nvalue[v >> 3] & (1 << (7 - v % 8))):
+            if not (nvalue[v >> 3] & (1 << (7 - v % 8))):
                 return False
         return True
 
 
 class String(StringOrOctetString, str):
 
     """Class for a display string. Such a string is an unicode string and
@@ -632,15 +632,15 @@
             try:
                 other = self.__class__(self.entity, other)
             except Exception:
                 raise NotImplementedError  # pragma: no cover
         return self._value == other._value
 
     def __ne__(self, other):
-        return not(self.__eq__(other))
+        return not self.__eq__(other)
 
     def __str__(self):
         if self._value in self.entity.enum:
             return (
                 "{}({:d})".format(self.entity.enum[self._value], self._value)
             )
         else:
```

### Comparing `snimpy-1.0.0/snimpy/main.py` & `snimpy-1.0.1/snimpy/main.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/snimpy/manager.py` & `snimpy-1.0.1/snimpy/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         self.flush()
         return value
 
     def get(self, *args):
         return self.getorwalk("get", *args)
 
     def walk(self, *args):
-        assert(len(args) == 1)  # we should ony walk one oid at a time
+        assert len(args) == 1  # we should ony walk one oid at a time
         return self.getorwalk("walkmore", *args)
 
     def flush(self):
         keys = list(self.cache.keys())
         for k in keys:
             if time() - self.cache[k][0] > self.timeout:
                 del self.cache[k]
@@ -452,15 +452,15 @@
 
         walk_oid = oid
         for noid, result in self.session.walk(oid):
             if noid <= oid:
                 noid = None
                 break
             oid = noid
-            if not(len(oid) >= len(walk_oid) and
+            if not (len(oid) >= len(walk_oid) and
                     oid[:len(walk_oid)] ==
                     walk_oid[:len(walk_oid)]):
                 noid = None
                 break
 
             # oid should be turned into index
             index = tuple(oid[len(self.proxy.oid):])
```

### Comparing `snimpy-1.0.0/snimpy/mib.py` & `snimpy-1.0.1/snimpy/mib.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,16 +457,19 @@
     else:
         _lastError = None
 
 
 def reset():
     """Reset libsmi to its initial state."""
     _smi.smiExit()
-    if _smi.smiInit(b"snimpy") < 0:
-        raise SMIException("unable to init libsmi")
+    try:
+        if _smi.smiInit(b"snimpy") < 0:
+            raise SMIException("unable to init libsmi")
+    except TypeError:
+        pass                    # We are being mocked
     _smi.smiSetErrorLevel(1)
     _smi.smiSetErrorHandler(_logError)
     try:
         _smi.smiSetFlags(_smi.SMI_FLAG_ERRORS | _smi.SMI_FLAG_RECURSIVE)
     except TypeError:
         pass                    # We are being mocked
```

### Comparing `snimpy-1.0.0/snimpy/smi_build.py` & `snimpy-1.0.1/snimpy/smi_build.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/snimpy/snmp.py` & `snimpy-1.0.1/snimpy/snmp.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/snimpy.egg-info/SOURCES.txt` & `snimpy-1.0.1/snimpy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 .gitmodules
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 MANIFEST.in
 Makefile
 README.rst
+flake.lock
+flake.nix
 setup.py
 tox.ini
 version.txt
+.github/dependabot.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
```

### Comparing `snimpy-1.0.0/tests/SNIMPY-INVALID-MIB.mib` & `snimpy-1.0.1/tests/SNIMPY-INVALID-MIB.mib`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/tests/SNIMPY-MIB.mib` & `snimpy-1.0.1/tests/SNIMPY-MIB.mib`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/tests/agent.py` & `snimpy-1.0.1/tests/agent.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/tests/test_basictypes.py` & `snimpy-1.0.1/tests/test_basictypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
+import unittest.mock as mock
 import os
 import re
 import socket
-import mock
 import ipaddress
 from datetime import timedelta
 from snimpy import mib, basictypes
 from pysnmp.proto import rfc1902
 
 
 class TestBasicTypes(unittest.TestCase):
@@ -175,16 +175,16 @@
 
     def testBoolean(self):
         """Test boolean basic type"""
         a = basictypes.build("SNIMPY-MIB", "snimpyBoolean", True)
         self.assertTrue(isinstance(a, basictypes.Boolean))
         self.assertEqual(a, True)
         self.assertTrue(a)
-        self.assertTrue(not(not(a)))
-        self.assertEqual(not(a), False)
+        self.assertTrue(not not a)
+        self.assertEqual(not a, False)
         a = basictypes.build("SNIMPY-MIB", "snimpyBoolean", "false")
         self.assertEqual(a, False)
         b = basictypes.build("SNIMPY-MIB", "snimpyBoolean", True)
         self.assertEqual(a or b, True)
         self.assertEqual(a and b, False)
 
     def testTimeticks(self):
@@ -261,22 +261,22 @@
             b"\x17\x00\x01")
         self.assertTrue(isinstance(a, basictypes.OctetString))
         b = [7, 6, 5, 3, 23]
         for i in range(30):
             if i in b:
                 self.assertTrue(a & i)
             else:
-                self.assertTrue(not(a & i))
+                self.assertTrue(not (a & i))
         self.assertTrue(a & [5, 7])
-        self.assertTrue(not(a & [5, 9]))
+        self.assertTrue(not (a & [5, 9]))
         a |= [2, 10]
         a -= 22
         a -= [23, 22]
         self.assertTrue(a & [2, 10])
-        self.assertTrue(not(a & 23))
+        self.assertTrue(not (a & 23))
         self.assertEqual(a, b"\x37\x20\x00")
         a |= 31
         self.assertEqual(a, b"\x37\x20\x00\x01")
 
     def testPacking(self):
         """Test pack() function"""
         self.assertEqual(basictypes.build("SNIMPY-MIB",
@@ -337,17 +337,19 @@
                              tt[key])
             # Test double conversion
             self.assertEqual(mib.get("SNIMPY-MIB", t).type.fromOid(
                 mib.get("SNIMPY-MIB", t), oid, implied),
                 (len(tt[key]), v))
 
     def testTooLargeOid(self):
-        """Handle the special case of octet string as OID with too large octets.
+        """Handle the special case of octet string as OID with too
+        large octets.
 
         See: https://github.com/vincentbernat/snimpy/pull/14
+
         """
         self.assertEqual(mib.get("SNIMPY-MIB",
                                  "snimpyIndexImplied").type.fromOid(
                                      mib.get("SNIMPY-MIB",
                                              "snimpyIndexImplied"),
                                      (104, 0xff00 | 101, 108, 108, 111),
                                      implied=True),
```

### Comparing `snimpy-1.0.0/tests/test_conf.py` & `snimpy-1.0.1/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/tests/test_main.py` & `snimpy-1.0.1/tests/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import tempfile
 import code  # noqa: F401
-import mock
 import platform
 from snimpy.main import interact
 from multiprocessing import Process
 import agent
 import unittest
+import unittest.mock as mock
 
 
 class TestMain(unittest.TestCase):
 
     """Test the main shell"""
 
     @classmethod
```

### Comparing `snimpy-1.0.0/tests/test_manager.py` & `snimpy-1.0.1/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/tests/test_mib.py` & `snimpy-1.0.1/tests/test_mib.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/tests/test_snmp.py` & `snimpy-1.0.1/tests/test_snmp.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.0/tox.ini` & `snimpy-1.0.1/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 [tox]
-envlist = py{34,35,36,37,38,39}{,-ipython},lint,doc
+envlist = py{34,35,36,37,38,39,310,311}{,-ipython},lint,doc
 skip_missing_interpreters = True
 
 [gh-actions]
 python =
   3.6: py36
   3.7: py37
   3.8: py38, lint, doc
   3.9: py39
+  3.10: py310
+  3.11: py311
 
 [testenv]
+allowlist_externals = make
 deps =
     coverage
     ipython: ipython
-commands = {envpython} {envbindir}/coverage run --source=snimpy setup.py test
+    pytest
+commands = coverage run --source=snimpy -m pytest {posargs}
 
 [testenv:lint]
 basepython = python3
 deps =
     flake8
     twine
     interrogate
+    build
 whitelist_externals = make
 commands =
     make lint
-    python setup.py sdist
+    python -m build
     twine check dist/*
 
 [testenv:doc]
 basepython = python3
 changedir = docs
 deps =
-    mock
     sphinx
     sphinx-rtd-theme
 whitelist_externals = make
 commands =
     make html READTHEDOCS=True
 
 [coverage:run]
```

