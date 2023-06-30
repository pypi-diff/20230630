# Comparing `tmp/webint_media-0.0.53.tar.gz` & `tmp/webint_media-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_media-0.0.53.tar", max compression
+gzip compressed data, was "webint_media-0.0.54.tar", max compression
```

## Comparing `webint_media-0.0.53.tar` & `webint_media-0.0.54.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      819 2023-06-29 03:28:40.141094 webint_media-0.0.53/pyproject.toml
--rw-r--r--   0        0        0     5554 2023-06-29 03:01:15.571573 webint_media-0.0.53/webint_media/__init__.py
--rw-r--r--   0        0        0       37 2023-01-27 00:43:31.371967 webint_media-0.0.53/webint_media/templates/__init__.py
--rw-r--r--   0        0        0    10406 2023-06-25 03:18:21.573370 webint_media-0.0.53/webint_media/templates/index.html
--rw-r--r--   0        0        0       96 2023-01-27 00:43:31.367967 webint_media-0.0.53/webint_media/templates/media_added.html
--rw-r--r--   0        0        0       70 2023-01-27 00:43:31.367967 webint_media-0.0.53/webint_media/templates/media_deleted.html
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 webint_media-0.0.53/setup.py
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 webint_media-0.0.53/PKG-INFO
+-rw-r--r--   0        0        0      819 2023-06-30 20:35:20.833345 webint_media-0.0.54/pyproject.toml
+-rw-r--r--   0        0        0     5554 2023-06-29 03:01:15.571573 webint_media-0.0.54/webint_media/__init__.py
+-rw-r--r--   0        0        0       37 2023-01-27 00:43:31.371967 webint_media-0.0.54/webint_media/templates/__init__.py
+-rw-r--r--   0        0        0    10406 2023-06-30 20:35:11.849208 webint_media-0.0.54/webint_media/templates/index.html
+-rw-r--r--   0        0        0       96 2023-01-27 00:43:31.367967 webint_media-0.0.54/webint_media/templates/media_added.html
+-rw-r--r--   0        0        0       70 2023-01-27 00:43:31.367967 webint_media-0.0.54/webint_media/templates/media_deleted.html
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 webint_media-0.0.54/setup.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 webint_media-0.0.54/PKG-INFO
```

### Comparing `webint_media-0.0.53/pyproject.toml` & `webint_media-0.0.54/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-media"
-version = "0.0.53"
+version = "0.0.54"
 description = "manage media on your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 packages = [{include = "webint_media"}]
 
 [tool.poetry.plugins."webapps"]
 media = "webint_media:app"
```

### Comparing `webint_media-0.0.53/webint_media/__init__.py` & `webint_media-0.0.54/webint_media/__init__.py`

 * *Files identical despite different names*

### Comparing `webint_media-0.0.53/webint_media/templates/index.html` & `webint_media-0.0.54/webint_media/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         <div><a href=/$file.name><img src=/$file.name></a></div>
     $elif file.name.endswith((".mp4", ".webm", ".mov", ".flv")):
         $if file.name.endswith(".mp4"):
             $ type = "mp4"
         $elif file.name.endswith(".webm"):
             $ type = "webm"
         $elif file.name.endswith(".mov"):
-            $ type = "mov"
+            $ type = "mp4"
         $elif file.name.endswith(".flv"):
             $ type = "x-flv"
         <div>
         <video id=player class="video-js vjs-default-skin" controls style=height:360px;width:100%>
         <source src="/$file.name" type=video/$type>
         </video>
         </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 $#
 $for file in files:
 $if tx.user.is_owner:
  $if file.name.endswith((".png", ".jpg", ".jpeg", ".gif", ".webp")):
 [/$file.name]
 $elif file.name.endswith((".mp4", ".webm", ".mov", ".flv")): $if
 file.name.endswith(".mp4"): $ type = "mp4" $elif file.name.endswith(".webm"): $
-type = "webm" $elif file.name.endswith(".mov"): $ type = "mov" $elif
+type = "webm" $elif file.name.endswith(".mov"): $ type = "mp4" $elif
 file.name.endswith(".flv"): $ type = "x-flv"
 
  $elif file.name.endswith((".m4a",)):
 $file.name $round(file.stat().st_size / 1024 / 1024, 2)mb
 $if tx.user.is_owner: Delete
 $#
  $#
```

### Comparing `webint_media-0.0.53/setup.py` & `webint_media-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0', 'yt-dlp>=2023.3.4,<2024.0.0']
 
 entry_points = \
 {'webapps': ['media = webint_media:app']}
 
 setup_kwargs = {
     'name': 'webint-media',
-    'version': '0.0.53',
+    'version': '0.0.54',
     'description': 'manage media on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

