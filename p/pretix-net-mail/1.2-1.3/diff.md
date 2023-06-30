# Comparing `tmp/pretix_net_mail-1.2.tar.gz` & `tmp/pretix_net_mail-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_net_mail-1.2.tar", last modified: Wed Dec 14 14:35:38 2022, max compression
+gzip compressed data, was "pretix_net_mail-1.3.tar", last modified: Fri Jun 30 13:56:51 2023, max compression
```

## Comparing `pretix_net_mail-1.2.tar` & `pretix_net_mail-1.3.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.479672 pretix_net_mail-1.2/
--rw-r--r--   0 bsheqa     (501) staff       (20)    11332 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/LICENSE
--rw-r--r--   0 bsheqa     (501) staff       (20)      171 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/MANIFEST.in
--rw-r--r--   0 bsheqa     (501) staff       (20)      292 2022-12-14 14:35:38.479428 pretix_net_mail-1.2/PKG-INFO
--rw-r--r--   0 bsheqa     (501) staff       (20)     1235 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/README.md
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.466799 pretix_net_mail-1.2/pretix_net_mail/
--rw-r--r--   0 bsheqa     (501) staff       (20)      697 2022-12-14 14:35:01.000000 pretix_net_mail-1.2/pretix_net_mail/__init__.py
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.462804 pretix_net_mail-1.2/pretix_net_mail/locale/
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.462658 pretix_net_mail-1.2/pretix_net_mail/locale/de/
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.469439 pretix_net_mail-1.2/pretix_net_mail/locale/de/LC_MESSAGES/
--rw-r--r--   0 bsheqa     (501) staff       (20)      260 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/pretix_net_mail/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 bsheqa     (501) staff       (20)      302 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/pretix_net_mail/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.469917 pretix_net_mail-1.2/pretix_net_mail/locale/de_Informal/
--rw-r--r--   0 bsheqa     (501) staff       (20)        0 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/pretix_net_mail/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.470629 pretix_net_mail-1.2/pretix_net_mail/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 bsheqa     (501) staff       (20)      260 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/pretix_net_mail/locale/de_Informal/LC_MESSAGES/django.mo
--rw-r--r--   0 bsheqa     (501) staff       (20)      302 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/pretix_net_mail/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 bsheqa     (501) staff       (20)      972 2022-12-14 14:20:18.000000 pretix_net_mail-1.2/pretix_net_mail/renderer.py
--rw-r--r--   0 bsheqa     (501) staff       (20)      445 2022-12-14 14:20:24.000000 pretix_net_mail-1.2/pretix_net_mail/signals.py
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.463173 pretix_net_mail-1.2/pretix_net_mail/static/
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.473939 pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/
--rw-r--r--   0 bsheqa     (501) staff       (20)        0 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/.gitkeep
--rw-r--r--   0 bsheqa     (501) staff       (20)    25406 2022-12-14 14:20:41.000000 pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/ICINGAthumb.png
--rw-r--r--   0 bsheqa     (501) staff       (20)    31594 2022-10-07 12:30:57.000000 pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/NETthumb.png
--rw-r--r--   0 bsheqa     (501) staff       (20)    33431 2022-10-07 12:30:57.000000 pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/OSMCthumb.png
--rw-r--r--   0 bsheqa     (501) staff       (20)    18592 2022-12-14 14:20:47.000000 pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/STACKCONFthumb.png
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.463406 pretix_net_mail-1.2/pretix_net_mail/templates/
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.478246 pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/
--rw-r--r--   0 bsheqa     (501) staff       (20)        0 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/.gitkeep
--rw-r--r--   0 bsheqa     (501) staff       (20)    67645 2022-12-14 14:21:14.000000 pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/ICINGA.html
--rw-r--r--   0 bsheqa     (501) staff       (20)    74035 2022-10-07 12:31:05.000000 pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/NES.html
--rw-r--r--   0 bsheqa     (501) staff       (20)    73928 2022-12-14 14:21:26.000000 pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/OSMC.html
--rw-r--r--   0 bsheqa     (501) staff       (20)    73925 2022-12-14 14:21:20.000000 pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/STACKCONF.html
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2022-12-14 14:35:38.468767 pretix_net_mail-1.2/pretix_net_mail.egg-info/
--rw-r--r--   0 bsheqa     (501) staff       (20)      292 2022-12-14 14:35:37.000000 pretix_net_mail-1.2/pretix_net_mail.egg-info/PKG-INFO
--rw-r--r--   0 bsheqa     (501) staff       (20)     1119 2022-12-14 14:35:38.000000 pretix_net_mail-1.2/pretix_net_mail.egg-info/SOURCES.txt
--rw-r--r--   0 bsheqa     (501) staff       (20)        1 2022-12-14 14:35:37.000000 pretix_net_mail-1.2/pretix_net_mail.egg-info/dependency_links.txt
--rw-r--r--   0 bsheqa     (501) staff       (20)       67 2022-12-14 14:35:37.000000 pretix_net_mail-1.2/pretix_net_mail.egg-info/entry_points.txt
--rw-r--r--   0 bsheqa     (501) staff       (20)       16 2022-12-14 14:35:38.000000 pretix_net_mail-1.2/pretix_net_mail.egg-info/top_level.txt
--rw-r--r--   0 bsheqa     (501) staff       (20)      105 2022-10-07 12:28:35.000000 pretix_net_mail-1.2/pyproject.toml
--rw-r--r--   0 bsheqa     (501) staff       (20)       38 2022-12-14 14:35:38.479821 pretix_net_mail-1.2/setup.cfg
--rw-r--r--   0 bsheqa     (501) staff       (20)     1077 2022-12-14 14:34:48.000000 pretix_net_mail-1.2/setup.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.354563 pretix_net_mail-1.3/
+-rw-r--r--   0 bsheqa     (501) staff       (20)    11332 2022-10-07 12:28:35.000000 pretix_net_mail-1.3/LICENSE
+-rw-r--r--   0 bsheqa     (501) staff       (20)      171 2022-10-07 12:28:35.000000 pretix_net_mail-1.3/MANIFEST.in
+-rw-r--r--   0 bsheqa     (501) staff       (20)      292 2023-06-30 13:56:51.354228 pretix_net_mail-1.3/PKG-INFO
+-rw-r--r--   0 bsheqa     (501) staff       (20)     1235 2022-10-07 12:28:35.000000 pretix_net_mail-1.3/README.md
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.342150 pretix_net_mail-1.3/pretix_net_mail/
+-rw-r--r--   0 bsheqa     (501) staff       (20)      697 2023-06-30 13:50:13.000000 pretix_net_mail-1.3/pretix_net_mail/__init__.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.338233 pretix_net_mail-1.3/pretix_net_mail/locale/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.338086 pretix_net_mail-1.3/pretix_net_mail/locale/de/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.345823 pretix_net_mail-1.3/pretix_net_mail/locale/de/LC_MESSAGES/
+-rw-r--r--   0 bsheqa     (501) staff       (20)      260 2022-12-14 14:35:38.000000 pretix_net_mail-1.3/pretix_net_mail/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 bsheqa     (501) staff       (20)      302 2022-10-07 12:28:35.000000 pretix_net_mail-1.3/pretix_net_mail/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.346399 pretix_net_mail-1.3/pretix_net_mail/locale/de_Informal/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2022-10-07 12:28:35.000000 pretix_net_mail-1.3/pretix_net_mail/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.347167 pretix_net_mail-1.3/pretix_net_mail/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 bsheqa     (501) staff       (20)      260 2022-12-14 14:35:38.000000 pretix_net_mail-1.3/pretix_net_mail/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-r--r--   0 bsheqa     (501) staff       (20)      302 2022-10-07 12:28:35.000000 pretix_net_mail-1.3/pretix_net_mail/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 bsheqa     (501) staff       (20)     1179 2023-06-30 13:26:36.000000 pretix_net_mail-1.3/pretix_net_mail/renderer.py
+-rw-r--r--   0 bsheqa     (501) staff       (20)      481 2023-06-30 13:26:48.000000 pretix_net_mail-1.3/pretix_net_mail/signals.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.338627 pretix_net_mail-1.3/pretix_net_mail/static/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.350440 pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2022-10-07 12:28:35.000000 pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/.gitkeep
+-rw-r--r--   0 bsheqa     (501) staff       (20)    23060 2023-06-30 13:25:40.000000 pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/DOSTthumb.png
+-rw-r--r--   0 bsheqa     (501) staff       (20)    25406 2023-06-30 13:25:40.000000 pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/ICINGAthumb.png
+-rw-r--r--   0 bsheqa     (501) staff       (20)    31594 2023-06-30 13:25:40.000000 pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/NETthumb.png
+-rw-r--r--   0 bsheqa     (501) staff       (20)    33431 2023-06-30 13:25:40.000000 pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/OSMCthumb.png
+-rw-r--r--   0 bsheqa     (501) staff       (20)    18592 2023-06-30 13:25:40.000000 pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/STACKCONFthumb.png
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.338873 pretix_net_mail-1.3/pretix_net_mail/templates/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.353701 pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2022-10-07 12:28:35.000000 pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/.gitkeep
+-rw-r--r--   0 bsheqa     (501) staff       (20)    70879 2023-06-30 13:26:09.000000 pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/DOST.html
+-rw-r--r--   0 bsheqa     (501) staff       (20)    67645 2023-06-30 13:26:09.000000 pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/ICINGA.html
+-rw-r--r--   0 bsheqa     (501) staff       (20)    74035 2023-06-30 13:26:10.000000 pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/NES.html
+-rw-r--r--   0 bsheqa     (501) staff       (20)    73928 2023-06-30 13:26:10.000000 pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/OSMC.html
+-rw-r--r--   0 bsheqa     (501) staff       (20)    73925 2023-06-30 13:26:10.000000 pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/STACKCONF.html
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-06-30 13:56:51.344836 pretix_net_mail-1.3/pretix_net_mail.egg-info/
+-rw-r--r--   0 bsheqa     (501) staff       (20)      292 2023-06-30 13:56:51.000000 pretix_net_mail-1.3/pretix_net_mail.egg-info/PKG-INFO
+-rw-r--r--   0 bsheqa     (501) staff       (20)     1224 2023-06-30 13:56:51.000000 pretix_net_mail-1.3/pretix_net_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)        1 2023-06-30 13:56:51.000000 pretix_net_mail-1.3/pretix_net_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)       67 2023-06-30 13:56:51.000000 pretix_net_mail-1.3/pretix_net_mail.egg-info/entry_points.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)       16 2023-06-30 13:56:51.000000 pretix_net_mail-1.3/pretix_net_mail.egg-info/top_level.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)      119 2023-06-30 13:56:40.000000 pretix_net_mail-1.3/pyproject.toml
+-rw-r--r--   0 bsheqa     (501) staff       (20)       38 2023-06-30 13:56:51.354652 pretix_net_mail-1.3/setup.cfg
+-rw-r--r--   0 bsheqa     (501) staff       (20)     1077 2023-06-30 13:49:59.000000 pretix_net_mail-1.3/setup.py
```

### Comparing `pretix_net_mail-1.2/LICENSE` & `pretix_net_mail-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/README.md` & `pretix_net_mail-1.3/README.md`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail/__init__.py` & `pretix_net_mail-1.3/pretix_net_mail/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     class PretixPluginMeta:
         name = gettext_lazy("NES Mail")
         author = "NETWAYS GmbH"
         description = gettext_lazy("Custom Email Renderer for NETWAYS")
         visible = True
         restricted = False 
-        version = 1.2
+        version = 1.3
         category = "CUSTOMIZATION"
         
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretix_net_mail-1.2/pretix_net_mail/renderer.py` & `pretix_net_mail-1.3/pretix_net_mail/renderer.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,7 +21,13 @@
 
 class ICINGAMailRenderer(TemplateBasedMailRenderer):
     verbose_name = "Icinga"
     identifier = "icinga"
     thumbnail_filename = "pretix_net_mail/ICINGAthumb.png"
     template_name = "pretix_net_mail/ICINGA.html"
 
+class DOSTMailRenderer(TemplateBasedMailRenderer):
+    verbose_name = "DOST"
+    identifier = "dost"
+    thumbnail_filename = "pretix_net_mail/DOSTthumb.png"
+    template_name = "pretix_net_mail/DOST.html"
+
```

### Comparing `pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/ICINGAthumb.png` & `pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/ICINGAthumb.png`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/NETthumb.png` & `pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/NETthumb.png`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/OSMCthumb.png` & `pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/OSMCthumb.png`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail/static/pretix_net_mail/STACKCONFthumb.png` & `pretix_net_mail-1.3/pretix_net_mail/static/pretix_net_mail/STACKCONFthumb.png`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/ICINGA.html` & `pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/ICINGA.html`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/NES.html` & `pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/NES.html`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/OSMC.html` & `pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/OSMC.html`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail/templates/pretix_net_mail/STACKCONF.html` & `pretix_net_mail-1.3/pretix_net_mail/templates/pretix_net_mail/STACKCONF.html`

 * *Files identical despite different names*

### Comparing `pretix_net_mail-1.2/pretix_net_mail.egg-info/SOURCES.txt` & `pretix_net_mail-1.3/pretix_net_mail.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 pretix_net_mail.egg-info/top_level.txt
 pretix_net_mail/locale/de/LC_MESSAGES/django.mo
 pretix_net_mail/locale/de/LC_MESSAGES/django.po
 pretix_net_mail/locale/de_Informal/.gitkeep
 pretix_net_mail/locale/de_Informal/LC_MESSAGES/django.mo
 pretix_net_mail/locale/de_Informal/LC_MESSAGES/django.po
 pretix_net_mail/static/pretix_net_mail/.gitkeep
+pretix_net_mail/static/pretix_net_mail/DOSTthumb.png
 pretix_net_mail/static/pretix_net_mail/ICINGAthumb.png
 pretix_net_mail/static/pretix_net_mail/NETthumb.png
 pretix_net_mail/static/pretix_net_mail/OSMCthumb.png
 pretix_net_mail/static/pretix_net_mail/STACKCONFthumb.png
 pretix_net_mail/templates/pretix_net_mail/.gitkeep
+pretix_net_mail/templates/pretix_net_mail/DOST.html
 pretix_net_mail/templates/pretix_net_mail/ICINGA.html
 pretix_net_mail/templates/pretix_net_mail/NES.html
 pretix_net_mail/templates/pretix_net_mail/OSMC.html
 pretix_net_mail/templates/pretix_net_mail/STACKCONF.html
```

### Comparing `pretix_net_mail-1.2/setup.py` & `pretix_net_mail-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 cmdclass = {"build": CustomBuild}
 
 
 setup(
     name="pretix_net_mail",
-    version='1.2',
+    version='1.3',
     description="Custom HTML Email Renderer for NETWAYS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NETWAYS/pretix-email-net",
     author="NETWAYS GmbH",
     author_email="support@netways.de",
     license="Apache",
```

