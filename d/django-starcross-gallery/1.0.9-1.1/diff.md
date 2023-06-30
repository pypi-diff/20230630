# Comparing `tmp/django-starcross-gallery-1.0.9.tar.gz` & `tmp/django-starcross-gallery-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-starcross-gallery-1.0.9.tar", last modified: Sat Sep 12 09:50:34 2020, max compression
+gzip compressed data, was "django-starcross-gallery-1.1.tar", last modified: Fri Jun 30 16:02:29 2023, max compression
```

## Comparing `django-starcross-gallery-1.0.9.tar` & `django-starcross-gallery-1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/
--rw-rw-r--   0 alex      (1000) alex      (1000)     7651 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     8119 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      107 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)     1384 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/django_starcross_gallery.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     8119 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/django_starcross_gallery.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)        8 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/django_starcross_gallery.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)     1866 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/django_starcross_gallery.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/django_starcross_gallery.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       37 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/django_starcross_gallery.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)     6120 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/README.rst
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/
--rw-rw-r--   0 alex      (1000) alex      (1000)      179 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/apps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      914 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/forms.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      376 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/runtests.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5071 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/models.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1208 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/tests/test_settings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/tests/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6287 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/tests/tests.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      125 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/tests/urls.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1272 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/settings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1098 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/admin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4152 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/views.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      325 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/signals.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       50 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/
--rw-rw-r--   0 alex      (1000) alex      (1000)      265 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/image_upload.html
--rw-rw-r--   0 alex      (1000) alex      (1000)     3329 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/image_detail.html
--rw-rw-r--   0 alex      (1000) alex      (1000)     1525 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/gallery_base.html
--rw-rw-r--   0 alex      (1000) alex      (1000)     1007 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/image_list.html
--rw-rw-r--   0 alex      (1000) alex      (1000)      881 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/album_list.html
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/admin/
--rw-r--r--   0 alex      (1000) alex      (1000)      170 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/admin/thumbnail.html
--rw-rw-r--   0 alex      (1000) alex      (1000)     1072 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/album_detail.html
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/partials/
--rw-rw-r--   0 alex      (1000) alex      (1000)      410 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/partials/thumbnail.html
--rw-rw-r--   0 alex      (1000) alex      (1000)      294 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/partials/thumbnail_preview.html
--rw-rw-r--   0 alex      (1000) alex      (1000)      764 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/partials/image_upload_form.html
--rw-rw-r--   0 alex      (1000) alex      (1000)      243 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/partials/justify_images.html
--rw-rw-r--   0 alex      (1000) alex      (1000)      409 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/templates/gallery/partials/thumbnail_empty.html
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/js/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1750 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/js/infinite_scroll.js
--rw-rw-r--   0 alex      (1000) alex      (1000)     3115 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/js/justify_images.js
--rw-rw-r--   0 alex      (1000) alex      (1000)      517 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/js/image_navigation.js
--rw-rw-r--   0 alex      (1000) alex      (1000)      929 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/js/image_upload.js
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/
--rw-rw-r--   0 alex      (1000) alex      (1000)    10241 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/camera.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     3115 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/iso.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    10548 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/exposure.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    12340 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/aperture.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    10889 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/35mm.png
--rw-r--r--   0 alex      (1000) alex      (1000)     3643 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/starcross.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     5249 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/album.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     3653 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/images/lens.png
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/css/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1021 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/css/gallery_template.css
--rw-rw-r--   0 alex      (1000) alex      (1000)     1921 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/css/gallery.css
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/css/themes/
--rw-rw-r--   0 alex      (1000) alex      (1000)      417 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/css/themes/black.css
--rw-rw-r--   0 alex      (1000) alex      (1000)      416 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/css/themes/grey.css
--rw-rw-r--   0 alex      (1000) alex      (1000)      451 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/static/gallery/css/themes/white.css
--rw-rw-r--   0 alex      (1000) alex      (1000)      579 2020-09-12 09:50:34.000000 django-starcross-gallery-1.0.9/gallery/urls.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7651 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)      107 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6976 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6044 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/README.rst
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/django_starcross_gallery.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6976 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/django_starcross_gallery.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1866 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/django_starcross_gallery.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/django_starcross_gallery.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       23 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/django_starcross_gallery.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/django_starcross_gallery.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       50 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1099 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/admin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      181 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/apps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1236 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/forms.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4911 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/models.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      376 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/runtests.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1272 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/settings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      325 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/signals.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/static/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/static/gallery/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/static/gallery/css/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2016 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/css/gallery.css
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1021 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/css/gallery_template.css
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/static/gallery/css/themes/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      498 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/css/themes/black.css
+-rw-rw-r--   0 alex      (1000) alex      (1000)      497 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/css/themes/grey.css
+-rw-rw-r--   0 alex      (1000) alex      (1000)      532 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/css/themes/white.css
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/static/gallery/images/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10889 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/images/35mm.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5249 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/images/album.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12340 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/images/aperture.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10241 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/images/camera.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10548 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/images/exposure.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3115 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/images/iso.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3653 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/images/lens.png
+-rw-r--r--   0 alex      (1000) alex      (1000)     3643 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/images/starcross.png
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/static/gallery/js/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      521 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/js/image_navigation.js
+-rw-rw-r--   0 alex      (1000) alex      (1000)      938 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/js/image_upload.js
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2035 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/js/infinite_scroll.js
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2989 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/static/gallery/js/justify_images.js
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/templates/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/templates/gallery/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/templates/gallery/admin/
+-rw-r--r--   0 alex      (1000) alex      (1000)      194 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/admin/thumbnail.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1072 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/album_detail.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)      881 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/album_list.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1574 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/gallery_base.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3329 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/image_detail.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1007 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/image_list.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)      265 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/image_upload.html
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/templates/gallery/partials/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      773 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/partials/image_upload_form.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)      243 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/partials/justify_images.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)      409 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/partials/thumbnail.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)      409 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/partials/thumbnail_empty.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)      294 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/templates/gallery/partials/thumbnail_preview.html
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/gallery/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/tests/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1207 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/tests/test_settings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6057 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/tests/tests.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      125 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/tests/urls.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      579 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/urls.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4203 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/gallery/views.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-30 16:02:29.379450 django-starcross-gallery-1.1/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-06-30 16:02:29.000000 django-starcross-gallery-1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-starcross-gallery-1.0.9/LICENSE` & `django-starcross-gallery-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/PKG-INFO` & `django-starcross-gallery-1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,158 +1,161 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-starcross-gallery
-Version: 1.0.9
+Version: 1.1
 Summary: A streamlined Django gallery app with justified layout, infinite scrolling, and drag & drop uploading
 Home-page: https://starcross.dev
 Author: Alex Luton
 Author-email: gallery@starcross.dev
 License: GNU LGPLv3
-Description: .. image:: https://img.shields.io/pypi/v/django-starcross-gallery.svg
-            :target: https://pypi.python.org/pypi/django-starcross-gallery/
-            :alt: PyPI version
-        
-        .. image:: https://travis-ci.org/Starcross/django-starcross-gallery.svg?branch=master
-            :target: https://travis-ci.org/Starcross/django-starcross-gallery
-            :alt: Build Status
-        
-        .. image:: https://coveralls.io/repos/github/Starcross/django-starcross-gallery/badge.svg?branch=master
-            :target: https://coveralls.io/github/Starcross/django-starcross-gallery?branch=master
-            :alt: Code coverage
-        
-        =================
-        Starcross Gallery
-        =================
-        
-        Starcross Gallery is a streamlined photo gallery Django app. Key features are:
-        
-        * Justified image grid display, as used on sites like Flickr
-        * Infinite scroll
-        * Easy drag and drop upload
-        * Straightforward object model - All metadata is pulled from the file including title and exif data
-        
-        Demo at https://starcross.dev/gallery
-        
-        Quick start
-        -----------
-        
-        1. Install Starcross gallery using pip::
-        
-            pip install django-starcross-gallery
-        
-        2. Add "gallery" to your INSTALLED_APPS setting like this::
-        
-            INSTALLED_APPS = [
-                ...
-                'gallery',
-            ]
-        
-        3. Include the gallery URLconf in your project urls.py like this with your preferred location e.g. "gallery/"::
-        
-            path('gallery/', include('gallery.urls')),
-        
-        4. Ensure a `MEDIA directory <https://docs.djangoproject.com/en/2.1/topics/files/>`_ is set up
-        
-        5. Run ``python manage.py makemigrations gallery``, then ``python manage.py migrate gallery`` to create the models.
-        
-        6. Start the development server and create any albums you required in http://127.0.0.1:8000/admin/. It's not necessary to create albums if you prefer just a single image feed
-        
-        7. Visit http://127.0.0.1:8000/gallery/ to access the gallery. Albums can be added through the django admin interface (/admin)
-        
-        
-        Instructions
-        ------------
-        
-        Starcross gallery groups Images into Albums, which enables your to organise your presentation. Add albums via the django admin interface, and drag multiple images into your empty albums in the album page itself. It's also possible to use the gallery as a flat image feed only, which is a view published at <gallery base>/images. All images will be displayed here in descending date order. You can add images here directly as well, but they will not be added to an album.
-        
-        The gallery was designed with simplicity of Image management in mind, so titles are derived from the file name. You only need to add albums and then drag your collection into place. The idea is to avoid the need to manage your collection both on the website and on your disk. If you wish to reorganise, you can delete and easily re-upload
-        
-        Images in albums are ordered by the date the photo was taken if available in the exif data, or failing that the modification date
-        
-        Album order can be specified in the Django admin interface. Support for `django-admin-sortable2 <https://github.com/jrief/django-admin-sortable2>`_ is provided, if you want drag and drop ordering in the admin interface. Just installing the module is all that's required. If you have already added albums you will need to use the `reorder <https://django-admin-sortable2.readthedocs.io/en/latest/usage.html#initial-data>`_ command.
-        
-        Settings
-        --------
-        
-        Override these default settings by adding to your settings.py
-        
-        
-        **GALLERY_LOGO_PATH** -- Default: "gallery/images/starcross.png"
-        
-        Path to the header logo within the static directory. If you do not wish to use a logo, override with a blank string
-        
-        **GALLERY_TITLE** -- Default: "Gallery"
-        
-        The title of the Gallery shown in the header on the main page and image feed
-        
-        **GALLERY_FOOTER_INFO** -- Default: "Starcross Gallery"
-        
-        Information text in the footer
-        
-        **GALLERY_FOOTER_EMAIL** -- Default: "gallery@starcross.dev"
-        
-        Contact email address in the footer. Override with a blank string to hide
-        
-        **GALLERY_THEME_COLOR** -- Default "black"
-        
-        Use a predefined theme color scheme. Options are black, white, or grey
-        
-        **GALLERY_THUMBNAIL_SIZE** -- Default: 200
-        
-        The target thumbnail height in px. This will vary slightly in rendering due to the justified layout
-        
-        **GALLERY_PREVIEW_SIZE** -- Default: 1000
-        
-        The preview size in px - width or height, whichever is largest. The rendered image size will depend on the size of the browser window, so this should be set high enough to not cause a deterioration in quality
-        
-        **GALLERY_RESIZE_QUALITY** -- Default: 80
-        
-        JPEG quality (0-100) of the preview and thumbnail images
-        
-        **GALLERY_HDPI_FACTOR** -- Default: 2
-        
-        The actual preview and thumbnail sizes are multiplied by this number, but rendered according to the quoted value. This enables high dpi displays, such as many mobile devices to show more detail and take advantage of their extra resolution. Some go up to 4x now, so recommended values are 1-4
-        
-        **GALLERY_IMAGE_MARGIN** -- Default: 6
-        
-        Margin between thumbnails in px. Some may prefer a less condensed look, so increase this value if your template requires it
-        
-        
-        Troubleshooting
-        ---------------
-        
-        **Broken image links after upload**
-        
-        Check your MEDIA settings. If the media location on disk is changed, you will need to copy the files in the CACHE directory to the new location, or delete and re-upload the broken images
-        
-        **Errors during upload**
-        
-        Your server may have a limit on maximum request size (e.g. client_max_body_size for nginx). This needs to be larger than the combined total of all the images your are uploading at once. Also the timeout may need to be extended as preview and thumbnail caches are generated at the time of upload
-        
-        **Delay when dragging images into upload box**
-        
-        If you are using Firefox on Linux, there can be a delay before the upload box flashes to acknowledge the pending files, proportional to the number of files. You can use another browser such as Chrome if this is inconvenient.
-        
-        Credits
-        -------
-        
-        Starcross Gallery is by Alex Luton <gallery@starcross.dev>, published under GNU LGPLv3
-        
-        
-        Album icon by Google licensed CC BY 3.0
-        
-        Focal Length icon by Ilaria Bernareggi from the Noun Project
-        
-        Other image data icons made by Freepik www.flaticon.com licensed by CC 3.0 BY
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/django-starcross-gallery.svg
+    :target: https://pypi.python.org/pypi/django-starcross-gallery/
+    :alt: PyPI version
+
+.. image:: https://github.com/Starcross/django-starcross-gallery/actions/workflows/app.yml/badge.svg
+    :target: https://github.com/Starcross/django-starcross-gallery/actions/workflows/app.yml
+    :alt: Build Status
+
+.. image:: https://coveralls.io/repos/github/Starcross/django-starcross-gallery/badge.svg?branch=master
+    :target: https://coveralls.io/github/Starcross/django-starcross-gallery?branch=master
+    :alt: Code coverage
+
+=================
+Starcross Gallery
+=================
+
+Starcross Gallery is a streamlined photo gallery Django app. Key features are:
+
+* Justified image grid display, as used on sites like Flickr
+* Infinite scroll
+* Easy drag and drop upload
+* Straightforward object model - All metadata is pulled from the file including title and exif data
+
+Demo at https://starcross.dev/gallery
+
+Quick start
+-----------
+
+1. Install Starcross gallery using pip::
+
+    pip install django-starcross-gallery
+
+2. Add "gallery" to your INSTALLED_APPS setting like this::
+
+    INSTALLED_APPS = [
+        ...
+        'gallery',
+    ]
+
+3. Include the gallery URLconf in your project urls.py like this with your preferred location e.g. "gallery/"::
+
+    path('gallery/', include('gallery.urls')),
+
+4. Ensure a `MEDIA directory <https://docs.djangoproject.com/en/4.0/topics/files/>`_ is set up
+
+5. Run ``python manage.py makemigrations gallery``, then ``python manage.py migrate gallery`` to create the models.
+
+6. Start the development server and create albums from the admin site http://127.0.0.1:8000/admin/. It's not necessary to create albums if you prefer just a single image feed
+
+7. Visit http://127.0.0.1:8000/gallery/ to access the gallery.
+
+
+Instructions
+------------
+
+Starcross gallery groups Images into Albums, which enables your to organise your presentation. Add albums via the django admin interface, and drag multiple images into your empty albums in the album page itself. It's also possible to use the gallery as a flat image feed only, which is a view published at <gallery base>/images. All images will be displayed here in descending date order. You can add images here directly as well, but they will not be added to an album.
+
+The gallery was designed with simplicity of image management in mind, so titles are derived from the file name. You only need to add albums and then drag your collection into place. The idea is to avoid the need to manage your collection both on the website and on disk. If you wish to reorganise, you can delete and easily re-upload
+
+Images in albums are ordered by the date the photo was taken if available in the exif data, or failing that the modification date
+
+Album order can be specified in the Django admin interface. Support for `django-admin-sortable2 <https://github.com/jrief/django-admin-sortable2>`_ is provided, if you want drag and drop ordering in the admin interface. Just installing the module is all that's required. If you have already added albums you will need to use the `reorder <https://django-admin-sortable2.readthedocs.io/en/latest/usage.html#initial-data>`_ command.
+
+Settings
+--------
+
+Override these default settings by adding to your settings.py
+
+
+**GALLERY_LOGO_PATH** -- Default: "gallery/images/starcross.png"
+
+Path to the header logo within the static directory. If you do not wish to use a logo, override with a blank string
+
+**GALLERY_TITLE** -- Default: "Gallery"
+
+The title of the Gallery shown in the header on the main page and image feed
+
+**GALLERY_FOOTER_INFO** -- Default: "Starcross Gallery"
+
+Information text in the footer
+
+**GALLERY_FOOTER_EMAIL** -- Default: "gallery@starcross.dev"
+
+Contact email address in the footer. Override with a blank string to hide
+
+**GALLERY_THEME_COLOR** -- Default "black"
+
+Use a predefined theme color scheme. Options are black, white, or grey
+
+**GALLERY_THUMBNAIL_SIZE** -- Default: 200
+
+The target thumbnail height in px. This will vary slightly in rendering due to the justified layout
+
+**GALLERY_PREVIEW_SIZE** -- Default: 1000
+
+The preview size in px - width or height, whichever is largest. The rendered image size will depend on the size of the browser window, so this should be set high enough to not cause a deterioration in quality
+
+**GALLERY_RESIZE_QUALITY** -- Default: 80
+
+JPEG quality (0-100) of the preview and thumbnail images
+
+**GALLERY_HDPI_FACTOR** -- Default: 2
+
+The actual preview and thumbnail sizes are multiplied by this number, but rendered according to the quoted value. This enables high dpi displays, such as many mobile devices to show more detail and take advantage of their extra resolution. Some go up to 4x now, so recommended values are 1-4
+
+**GALLERY_IMAGE_MARGIN** -- Default: 6
+
+Margin between thumbnails in px. This can create a more or less condensed look
+
+
+Troubleshooting
+---------------
+
+**Broken image links after upload**
+
+Check your MEDIA settings. If the media location on disk is changed, you will need to copy the files in the CACHE directory to the new location, or delete and re-upload the broken images
+
+**Errors during upload**
+
+Your server may have a limit on maximum request size (e.g. client_max_body_size for nginx). This needs to be larger than the combined total of all the images your are uploading at once. Also the timeout may need to be extended as preview and thumbnail caches are generated at the time of upload
+
+**Delay when dragging images into upload box**
+
+If you are using Firefox on Linux, there can be a delay before the upload box flashes to acknowledge the pending files, proportional to the number of files. You can use another browser such as Chrome if this is inconvenient.
+
+Credits
+-------
+
+Starcross Gallery is by Alex Luton <gallery@starcross.dev>, published under GNU LGPLv3
+
+
+Album icon by Google licensed CC BY 3.0
+
+Focal Length icon by Ilaria Bernareggi from the Noun Project
+
+Other image data icons made by Freepik www.flaticon.com licensed by CC 3.0 BY
+
+
```

### Comparing `django-starcross-gallery-1.0.9/setup.py` & `django-starcross-gallery-1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-requirements = ['django-imagekit==4.0.2', 'Pillow==7.2.0']
+requirements = ['django-imagekit', 'Pillow']
 
 setup(
     name='django-starcross-gallery',
-    version='1.0.9',
+    version='1.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU LGPLv3',
     description='A streamlined Django gallery app with justified layout, infinite scrolling, and drag & drop uploading',
     long_description=README,
     url='https://starcross.dev',
     author='Alex Luton',
     author_email='gallery@starcross.dev',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     install_requires=requirements,
 )
```

### Comparing `django-starcross-gallery-1.0.9/django_starcross_gallery.egg-info/PKG-INFO` & `django-starcross-gallery-1.1/django_starcross_gallery.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,158 +1,161 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-starcross-gallery
-Version: 1.0.9
+Version: 1.1
 Summary: A streamlined Django gallery app with justified layout, infinite scrolling, and drag & drop uploading
 Home-page: https://starcross.dev
 Author: Alex Luton
 Author-email: gallery@starcross.dev
 License: GNU LGPLv3
-Description: .. image:: https://img.shields.io/pypi/v/django-starcross-gallery.svg
-            :target: https://pypi.python.org/pypi/django-starcross-gallery/
-            :alt: PyPI version
-        
-        .. image:: https://travis-ci.org/Starcross/django-starcross-gallery.svg?branch=master
-            :target: https://travis-ci.org/Starcross/django-starcross-gallery
-            :alt: Build Status
-        
-        .. image:: https://coveralls.io/repos/github/Starcross/django-starcross-gallery/badge.svg?branch=master
-            :target: https://coveralls.io/github/Starcross/django-starcross-gallery?branch=master
-            :alt: Code coverage
-        
-        =================
-        Starcross Gallery
-        =================
-        
-        Starcross Gallery is a streamlined photo gallery Django app. Key features are:
-        
-        * Justified image grid display, as used on sites like Flickr
-        * Infinite scroll
-        * Easy drag and drop upload
-        * Straightforward object model - All metadata is pulled from the file including title and exif data
-        
-        Demo at https://starcross.dev/gallery
-        
-        Quick start
-        -----------
-        
-        1. Install Starcross gallery using pip::
-        
-            pip install django-starcross-gallery
-        
-        2. Add "gallery" to your INSTALLED_APPS setting like this::
-        
-            INSTALLED_APPS = [
-                ...
-                'gallery',
-            ]
-        
-        3. Include the gallery URLconf in your project urls.py like this with your preferred location e.g. "gallery/"::
-        
-            path('gallery/', include('gallery.urls')),
-        
-        4. Ensure a `MEDIA directory <https://docs.djangoproject.com/en/2.1/topics/files/>`_ is set up
-        
-        5. Run ``python manage.py makemigrations gallery``, then ``python manage.py migrate gallery`` to create the models.
-        
-        6. Start the development server and create any albums you required in http://127.0.0.1:8000/admin/. It's not necessary to create albums if you prefer just a single image feed
-        
-        7. Visit http://127.0.0.1:8000/gallery/ to access the gallery. Albums can be added through the django admin interface (/admin)
-        
-        
-        Instructions
-        ------------
-        
-        Starcross gallery groups Images into Albums, which enables your to organise your presentation. Add albums via the django admin interface, and drag multiple images into your empty albums in the album page itself. It's also possible to use the gallery as a flat image feed only, which is a view published at <gallery base>/images. All images will be displayed here in descending date order. You can add images here directly as well, but they will not be added to an album.
-        
-        The gallery was designed with simplicity of Image management in mind, so titles are derived from the file name. You only need to add albums and then drag your collection into place. The idea is to avoid the need to manage your collection both on the website and on your disk. If you wish to reorganise, you can delete and easily re-upload
-        
-        Images in albums are ordered by the date the photo was taken if available in the exif data, or failing that the modification date
-        
-        Album order can be specified in the Django admin interface. Support for `django-admin-sortable2 <https://github.com/jrief/django-admin-sortable2>`_ is provided, if you want drag and drop ordering in the admin interface. Just installing the module is all that's required. If you have already added albums you will need to use the `reorder <https://django-admin-sortable2.readthedocs.io/en/latest/usage.html#initial-data>`_ command.
-        
-        Settings
-        --------
-        
-        Override these default settings by adding to your settings.py
-        
-        
-        **GALLERY_LOGO_PATH** -- Default: "gallery/images/starcross.png"
-        
-        Path to the header logo within the static directory. If you do not wish to use a logo, override with a blank string
-        
-        **GALLERY_TITLE** -- Default: "Gallery"
-        
-        The title of the Gallery shown in the header on the main page and image feed
-        
-        **GALLERY_FOOTER_INFO** -- Default: "Starcross Gallery"
-        
-        Information text in the footer
-        
-        **GALLERY_FOOTER_EMAIL** -- Default: "gallery@starcross.dev"
-        
-        Contact email address in the footer. Override with a blank string to hide
-        
-        **GALLERY_THEME_COLOR** -- Default "black"
-        
-        Use a predefined theme color scheme. Options are black, white, or grey
-        
-        **GALLERY_THUMBNAIL_SIZE** -- Default: 200
-        
-        The target thumbnail height in px. This will vary slightly in rendering due to the justified layout
-        
-        **GALLERY_PREVIEW_SIZE** -- Default: 1000
-        
-        The preview size in px - width or height, whichever is largest. The rendered image size will depend on the size of the browser window, so this should be set high enough to not cause a deterioration in quality
-        
-        **GALLERY_RESIZE_QUALITY** -- Default: 80
-        
-        JPEG quality (0-100) of the preview and thumbnail images
-        
-        **GALLERY_HDPI_FACTOR** -- Default: 2
-        
-        The actual preview and thumbnail sizes are multiplied by this number, but rendered according to the quoted value. This enables high dpi displays, such as many mobile devices to show more detail and take advantage of their extra resolution. Some go up to 4x now, so recommended values are 1-4
-        
-        **GALLERY_IMAGE_MARGIN** -- Default: 6
-        
-        Margin between thumbnails in px. Some may prefer a less condensed look, so increase this value if your template requires it
-        
-        
-        Troubleshooting
-        ---------------
-        
-        **Broken image links after upload**
-        
-        Check your MEDIA settings. If the media location on disk is changed, you will need to copy the files in the CACHE directory to the new location, or delete and re-upload the broken images
-        
-        **Errors during upload**
-        
-        Your server may have a limit on maximum request size (e.g. client_max_body_size for nginx). This needs to be larger than the combined total of all the images your are uploading at once. Also the timeout may need to be extended as preview and thumbnail caches are generated at the time of upload
-        
-        **Delay when dragging images into upload box**
-        
-        If you are using Firefox on Linux, there can be a delay before the upload box flashes to acknowledge the pending files, proportional to the number of files. You can use another browser such as Chrome if this is inconvenient.
-        
-        Credits
-        -------
-        
-        Starcross Gallery is by Alex Luton <gallery@starcross.dev>, published under GNU LGPLv3
-        
-        
-        Album icon by Google licensed CC BY 3.0
-        
-        Focal Length icon by Ilaria Bernareggi from the Noun Project
-        
-        Other image data icons made by Freepik www.flaticon.com licensed by CC 3.0 BY
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/django-starcross-gallery.svg
+    :target: https://pypi.python.org/pypi/django-starcross-gallery/
+    :alt: PyPI version
+
+.. image:: https://github.com/Starcross/django-starcross-gallery/actions/workflows/app.yml/badge.svg
+    :target: https://github.com/Starcross/django-starcross-gallery/actions/workflows/app.yml
+    :alt: Build Status
+
+.. image:: https://coveralls.io/repos/github/Starcross/django-starcross-gallery/badge.svg?branch=master
+    :target: https://coveralls.io/github/Starcross/django-starcross-gallery?branch=master
+    :alt: Code coverage
+
+=================
+Starcross Gallery
+=================
+
+Starcross Gallery is a streamlined photo gallery Django app. Key features are:
+
+* Justified image grid display, as used on sites like Flickr
+* Infinite scroll
+* Easy drag and drop upload
+* Straightforward object model - All metadata is pulled from the file including title and exif data
+
+Demo at https://starcross.dev/gallery
+
+Quick start
+-----------
+
+1. Install Starcross gallery using pip::
+
+    pip install django-starcross-gallery
+
+2. Add "gallery" to your INSTALLED_APPS setting like this::
+
+    INSTALLED_APPS = [
+        ...
+        'gallery',
+    ]
+
+3. Include the gallery URLconf in your project urls.py like this with your preferred location e.g. "gallery/"::
+
+    path('gallery/', include('gallery.urls')),
+
+4. Ensure a `MEDIA directory <https://docs.djangoproject.com/en/4.0/topics/files/>`_ is set up
+
+5. Run ``python manage.py makemigrations gallery``, then ``python manage.py migrate gallery`` to create the models.
+
+6. Start the development server and create albums from the admin site http://127.0.0.1:8000/admin/. It's not necessary to create albums if you prefer just a single image feed
+
+7. Visit http://127.0.0.1:8000/gallery/ to access the gallery.
+
+
+Instructions
+------------
+
+Starcross gallery groups Images into Albums, which enables your to organise your presentation. Add albums via the django admin interface, and drag multiple images into your empty albums in the album page itself. It's also possible to use the gallery as a flat image feed only, which is a view published at <gallery base>/images. All images will be displayed here in descending date order. You can add images here directly as well, but they will not be added to an album.
+
+The gallery was designed with simplicity of image management in mind, so titles are derived from the file name. You only need to add albums and then drag your collection into place. The idea is to avoid the need to manage your collection both on the website and on disk. If you wish to reorganise, you can delete and easily re-upload
+
+Images in albums are ordered by the date the photo was taken if available in the exif data, or failing that the modification date
+
+Album order can be specified in the Django admin interface. Support for `django-admin-sortable2 <https://github.com/jrief/django-admin-sortable2>`_ is provided, if you want drag and drop ordering in the admin interface. Just installing the module is all that's required. If you have already added albums you will need to use the `reorder <https://django-admin-sortable2.readthedocs.io/en/latest/usage.html#initial-data>`_ command.
+
+Settings
+--------
+
+Override these default settings by adding to your settings.py
+
+
+**GALLERY_LOGO_PATH** -- Default: "gallery/images/starcross.png"
+
+Path to the header logo within the static directory. If you do not wish to use a logo, override with a blank string
+
+**GALLERY_TITLE** -- Default: "Gallery"
+
+The title of the Gallery shown in the header on the main page and image feed
+
+**GALLERY_FOOTER_INFO** -- Default: "Starcross Gallery"
+
+Information text in the footer
+
+**GALLERY_FOOTER_EMAIL** -- Default: "gallery@starcross.dev"
+
+Contact email address in the footer. Override with a blank string to hide
+
+**GALLERY_THEME_COLOR** -- Default "black"
+
+Use a predefined theme color scheme. Options are black, white, or grey
+
+**GALLERY_THUMBNAIL_SIZE** -- Default: 200
+
+The target thumbnail height in px. This will vary slightly in rendering due to the justified layout
+
+**GALLERY_PREVIEW_SIZE** -- Default: 1000
+
+The preview size in px - width or height, whichever is largest. The rendered image size will depend on the size of the browser window, so this should be set high enough to not cause a deterioration in quality
+
+**GALLERY_RESIZE_QUALITY** -- Default: 80
+
+JPEG quality (0-100) of the preview and thumbnail images
+
+**GALLERY_HDPI_FACTOR** -- Default: 2
+
+The actual preview and thumbnail sizes are multiplied by this number, but rendered according to the quoted value. This enables high dpi displays, such as many mobile devices to show more detail and take advantage of their extra resolution. Some go up to 4x now, so recommended values are 1-4
+
+**GALLERY_IMAGE_MARGIN** -- Default: 6
+
+Margin between thumbnails in px. This can create a more or less condensed look
+
+
+Troubleshooting
+---------------
+
+**Broken image links after upload**
+
+Check your MEDIA settings. If the media location on disk is changed, you will need to copy the files in the CACHE directory to the new location, or delete and re-upload the broken images
+
+**Errors during upload**
+
+Your server may have a limit on maximum request size (e.g. client_max_body_size for nginx). This needs to be larger than the combined total of all the images your are uploading at once. Also the timeout may need to be extended as preview and thumbnail caches are generated at the time of upload
+
+**Delay when dragging images into upload box**
+
+If you are using Firefox on Linux, there can be a delay before the upload box flashes to acknowledge the pending files, proportional to the number of files. You can use another browser such as Chrome if this is inconvenient.
+
+Credits
+-------
+
+Starcross Gallery is by Alex Luton <gallery@starcross.dev>, published under GNU LGPLv3
+
+
+Album icon by Google licensed CC BY 3.0
+
+Focal Length icon by Ilaria Bernareggi from the Noun Project
+
+Other image data icons made by Freepik www.flaticon.com licensed by CC 3.0 BY
+
+
```

### Comparing `django-starcross-gallery-1.0.9/django_starcross_gallery.egg-info/SOURCES.txt` & `django-starcross-gallery-1.1/django_starcross_gallery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/README.rst` & `django-starcross-gallery-1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. image:: https://img.shields.io/pypi/v/django-starcross-gallery.svg
     :target: https://pypi.python.org/pypi/django-starcross-gallery/
     :alt: PyPI version
 
-.. image:: https://travis-ci.org/Starcross/django-starcross-gallery.svg?branch=master
-    :target: https://travis-ci.org/Starcross/django-starcross-gallery
+.. image:: https://github.com/Starcross/django-starcross-gallery/actions/workflows/app.yml/badge.svg
+    :target: https://github.com/Starcross/django-starcross-gallery/actions/workflows/app.yml
     :alt: Build Status
 
 .. image:: https://coveralls.io/repos/github/Starcross/django-starcross-gallery/badge.svg?branch=master
     :target: https://coveralls.io/github/Starcross/django-starcross-gallery?branch=master
     :alt: Code coverage
 
 =================
@@ -37,29 +37,29 @@
         'gallery',
     ]
 
 3. Include the gallery URLconf in your project urls.py like this with your preferred location e.g. "gallery/"::
 
     path('gallery/', include('gallery.urls')),
 
-4. Ensure a `MEDIA directory <https://docs.djangoproject.com/en/2.1/topics/files/>`_ is set up
+4. Ensure a `MEDIA directory <https://docs.djangoproject.com/en/4.0/topics/files/>`_ is set up
 
 5. Run ``python manage.py makemigrations gallery``, then ``python manage.py migrate gallery`` to create the models.
 
-6. Start the development server and create any albums you required in http://127.0.0.1:8000/admin/. It's not necessary to create albums if you prefer just a single image feed
+6. Start the development server and create albums from the admin site http://127.0.0.1:8000/admin/. It's not necessary to create albums if you prefer just a single image feed
 
-7. Visit http://127.0.0.1:8000/gallery/ to access the gallery. Albums can be added through the django admin interface (/admin)
+7. Visit http://127.0.0.1:8000/gallery/ to access the gallery.
 
 
 Instructions
 ------------
 
 Starcross gallery groups Images into Albums, which enables your to organise your presentation. Add albums via the django admin interface, and drag multiple images into your empty albums in the album page itself. It's also possible to use the gallery as a flat image feed only, which is a view published at <gallery base>/images. All images will be displayed here in descending date order. You can add images here directly as well, but they will not be added to an album.
 
-The gallery was designed with simplicity of Image management in mind, so titles are derived from the file name. You only need to add albums and then drag your collection into place. The idea is to avoid the need to manage your collection both on the website and on your disk. If you wish to reorganise, you can delete and easily re-upload
+The gallery was designed with simplicity of image management in mind, so titles are derived from the file name. You only need to add albums and then drag your collection into place. The idea is to avoid the need to manage your collection both on the website and on disk. If you wish to reorganise, you can delete and easily re-upload
 
 Images in albums are ordered by the date the photo was taken if available in the exif data, or failing that the modification date
 
 Album order can be specified in the Django admin interface. Support for `django-admin-sortable2 <https://github.com/jrief/django-admin-sortable2>`_ is provided, if you want drag and drop ordering in the admin interface. Just installing the module is all that's required. If you have already added albums you will need to use the `reorder <https://django-admin-sortable2.readthedocs.io/en/latest/usage.html#initial-data>`_ command.
 
 Settings
 --------
@@ -101,15 +101,15 @@
 
 **GALLERY_HDPI_FACTOR** -- Default: 2
 
 The actual preview and thumbnail sizes are multiplied by this number, but rendered according to the quoted value. This enables high dpi displays, such as many mobile devices to show more detail and take advantage of their extra resolution. Some go up to 4x now, so recommended values are 1-4
 
 **GALLERY_IMAGE_MARGIN** -- Default: 6
 
-Margin between thumbnails in px. Some may prefer a less condensed look, so increase this value if your template requires it
+Margin between thumbnails in px. This can create a more or less condensed look
 
 
 Troubleshooting
 ---------------
 
 **Broken image links after upload**
```

### Comparing `django-starcross-gallery-1.0.9/gallery/models.py` & `django-starcross-gallery-1.1/gallery/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,37 +11,43 @@
 from datetime import datetime
 import os
 
 
 class Image(models.Model):
 
     data = models.ImageField(upload_to='images')
-    data_thumbnail = ImageSpecField(source='data',
-                                    processors=[ResizeToFit(
-                                        height=settings.GALLERY_THUMBNAIL_SIZE * settings.GALLERY_HDPI_FACTOR)],
-                                    format='JPEG',
-                                    options={'quality': settings.GALLERY_RESIZE_QUALITY})
-    data_preview = ImageSpecField(source='data',
-                                  processors=[ResizeToFit(width=settings.GALLERY_PREVIEW_SIZE * settings.GALLERY_HDPI_FACTOR,
-                                                          height=settings.GALLERY_PREVIEW_SIZE * settings.GALLERY_HDPI_FACTOR)],
-                                  format='JPEG',
-                                  options={'quality': settings.GALLERY_RESIZE_QUALITY})
+    data_thumbnail = ImageSpecField(
+        source='data',
+        processors=[ResizeToFit(height=settings.GALLERY_THUMBNAIL_SIZE * settings.GALLERY_HDPI_FACTOR)],
+        format='JPEG',
+        options={'quality': settings.GALLERY_RESIZE_QUALITY}
+    )
+    data_preview = ImageSpecField(
+        source='data',
+        processors=[ResizeToFit(
+            width=settings.GALLERY_PREVIEW_SIZE * settings.GALLERY_HDPI_FACTOR,
+            height=settings.GALLERY_PREVIEW_SIZE * settings.GALLERY_HDPI_FACTOR
+        )],
+        format='JPEG',
+        options={'quality': settings.GALLERY_RESIZE_QUALITY}
+    )
     date_uploaded = models.DateTimeField(auto_now_add=True)
 
     @cached_property
     def slug(self):
         return slugify(self.title, allow_unicode=True)
 
     @cached_property
     def exif(self):
+        """ Retrieve exif data using PIL as a dictionary """
         exif_data = {}
         self.data.open()
         with pImage.open(self.data) as img:
             if hasattr(img, '_getexif'):
-                info = img.getexif()
+                info = img._getexif()
                 if not info:
                     return {}
                 for tag, value in info.items():
                     decoded = TAGS.get(tag, tag)
                     exif_data[decoded] = value
                 # Process some data for easy rendering in template
                 exif_data['Camera'] = exif_data.get('Model', '')
@@ -53,37 +59,37 @@
                     exif_data['Exposure'] = "{0}/{1}".format(exif_data['ExposureTime'].numerator,
                                                              exif_data['ExposureTime'].denominator)
             img.close()
         return exif_data
 
     @cached_property
     def date_taken(self):
+        """ Use the date taken from the exif data, otherwise file modification time """
         original_exif = self.exif.get('DateTimeOriginal')
         if not original_exif:
             return self.mtime
         try:
             return datetime.strptime(original_exif, "%Y:%m:%d %H:%M:%S")
         except ValueError:  # Fall back to file modification time
             return self.mtime
 
     @cached_property
     def mtime(self):
         return datetime.fromtimestamp(os.path.getmtime(self.data.path))
 
     @property
     def title(self):
+        """ Derive a title from the original filename """
         if hasattr(self, '_title'):
             return self._title
-        """ Derive a title from the original filename """
+        name = Path(self.data.name)
         # remove extension
-        filename = Path(self.data.name).with_suffix('').name
+        name = name.with_suffix('').name
         # convert spacing characters to whitespaces
-        name = filename.translate(str.maketrans('_', ' '))
-        # return with first letter caps
-        return name.title()
+        return name.translate(str.maketrans('_', ' '))
 
     # Temporary override for album highlights
     @title.setter
     def title(self, name):
         self._title = name
 
     def get_absolute_url(self):
@@ -92,30 +98,32 @@
     def __str__(self):
         return self.title
 
 
 class Album(models.Model):
     title = models.CharField(max_length=250)
     images = models.ManyToManyField(Image, blank=True, related_name='image_albums')
-    highlight = models.OneToOneField(Image,
-                                     related_name='album_highlight',
-                                     null=True, blank=True,
-                                     on_delete=models.SET_NULL,
-                                     )
+    highlight = models.OneToOneField(
+        Image,
+        related_name='album_highlight',
+        null=True, blank=True,
+        on_delete=models.SET_NULL,
+    )
     order = models.PositiveIntegerField(default=0, blank=False, null=False)
 
     class Meta(object):
         ordering = ['order', '-pk']
 
     @property
     def slug(self):
         return slugify(self.title, allow_unicode=True)
 
     @property
     def display_highlight(self):
+        """ User selectable thumbnail for the album """
         # if there is no highlight but there are images in the album, use the first
         if not self.highlight and self.images.count():
             image = self.images.earliest('id')
         else:
             image = self.highlight
         if image:
             image.title = self.title  # use the album title instead of the highlight title
```

### Comparing `django-starcross-gallery-1.0.9/gallery/tests/test_settings.py` & `django-starcross-gallery-1.1/gallery/tests/test_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 DATABASES = {
     'default': {'ENGINE': 'django.db.backends.sqlite3'}
 }
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [os.path.join(BASE_DIR,  'templates')],
+        'DIRS': [os.path.join(BASE_DIR, 'templates')],
         'APP_DIRS': True,
         'OPTIONS': {
             'context_processors': [
                 'django.template.context_processors.debug',
                 'django.template.context_processors.request',
                 'django.contrib.auth.context_processors.auth',
                 'django.contrib.messages.context_processors.messages',
```

### Comparing `django-starcross-gallery-1.0.9/gallery/tests/tests.py` & `django-starcross-gallery-1.1/gallery/tests/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,129 +9,118 @@
 from datetime import datetime
 
 from gallery.models import Album, Image
 from gallery.forms import ImageCreateForm
 
 
 class ImageTests(TestCase):
+    """ Test case for starcross-django-gallery """
 
     test_image_title = "Antibes Marina"
     test_slug = "antibes-marina"
     test_album_title = "My First Album"
     test_image_title_unicode = "Паровоз"
 
-    image_filenames = ['antibes_marina.jpg', 'castle_combe.jpg', 'паровоз.jpg']
+    image_filenames = ['Antibes_Marina.jpg', 'Castle_Combe.jpg', 'Паровоз.jpg']
 
     exif_data = ['Sony  DSLR-A700', 'F/11.0', '1/500s', '16mm', 'ISO 200']
 
     username = 'admin'
     password = 'yj4KlZ6N'
 
     def setUp(self):
 
         # Find the local directory and add the test media location
-        TEST_ROOT = os.path.abspath(os.path.dirname(__file__))
-        settings.MEDIA_ROOT = os.path.join(TEST_ROOT, 'media/')
+        test_root = os.path.abspath(os.path.dirname(__file__))
+        settings.MEDIA_ROOT = os.path.join(test_root, 'media/')
 
         # Create test album with test images inside
         self.album = Album.objects.create(title=self.test_album_title)
         self.images = []
         for filename in self.image_filenames:
             self.images += [self.album.images.create(data=filename)]
         self.image = self.images[0]  # Set main set image
         self.unicode_image = self.images[2]  # Set unicode image
 
         User.objects.create_superuser(self.username, 'user@email.com', self.password)
+        self.client.login(username=self.username, password=self.password)
 
-    # Test global image list
     def test_image_list(self):
+        """ Test global image list """
 
         response = self.client.get(reverse('gallery:image_list'))
         self.assertContains(response, self.test_image_title, msg_prefix="Image title missing from image feed")
         self.assertContains(response, self.test_image_title_unicode,
                             msg_prefix="Unicode image title missing from image feed")
 
-    # Test image preview
     def test_image_detail(self):
+        """ Test image preview """
 
         response = self.client.get(reverse('gallery:image_detail',
                                            kwargs={'pk': self.image.pk, 'slug': self.image.title}))
         self.assertContains(response, self.test_image_title, msg_prefix="Image preview does not contain image title")
         # Check exif data present
         for data in self.exif_data:
             self.assertContains(response, data, msg_prefix="Exif data missing")
         # Check image's album appears in this context
         self.assertContains(response, self.test_album_title, count=2,
                             msg_prefix="Image preview does not contain related album")
 
-    # Test image preview with album context. Should contain previews to any other images in the same album
     def test_album_image_detail(self):
+        """ Test image preview with album context. Should contain previews to any other images in the same album """
         response = self.client.get(reverse('gallery:album_image_detail',
                                            kwargs={'pk': self.image.pk, 'slug': self.image.title,
                                                    'apk': self.album.pk}))
         self.assertContains(response, self.test_album_title, count=2, msg_prefix="Image preview incorrect")
 
-    # Test album and auto highlight
     def test_album_list(self):
-
+        """ Test album and auto highlight """
         response = self.client.get(reverse('gallery:album_list'))
 
         self.assertContains(response, self.test_album_title, msg_prefix="Album data missing from album list")
         image = self.album.images.earliest('id')
         self.assertContains(response, image.data_thumbnail.url, msg_prefix="Album list missing album url")
 
-    # Check empty albums do not cause errors
     def test_empty_album(self):
+        """ Check empty albums do not cause errors """
 
         self.empty_album = Album.objects.create(title='Empty album')
         response = self.client.get(reverse('gallery:album_list'))
         self.assertEqual(response.status_code, 200, "Error displaying empty album")
         Album.objects.all().last().delete()
 
-    # Test albums contain images
     def test_album_view(self):
+        """ Test albums contain images """
 
         response = self.client.get(reverse('gallery:album_detail',
                                    kwargs={'pk': self.album.pk, 'slug': self.album.title}))
         self.assertEqual(response.status_code, 200, "Error testing album view")
         self.assertContains(response, self.image.title, count=2, msg_prefix="Error testing image in album view")
 
     def test_image_properties(self):
-
         image = Image.objects.all()[0]
         self.assertEqual(image.title, ImageTests.test_image_title, "Incorrect title in image object")
         self.assertEqual(image.date_taken, datetime.strptime("2013-03-21 15:04:53", "%Y-%m-%d %H:%M:%S"),
                          "Incorrect date in image object")
         self.assertEqual(image.slug, self.test_slug, "Incorrect slug in image object")
 
-    def test_image_form_validation(self):
-        data = {'apk': self.album.pk}
-        image_path = os.path.join(settings.MEDIA_ROOT, self.image_filenames[0])
-        image_files = MultiValueDict({'data': [image_path]})
-        form = ImageCreateForm(data, files=image_files)
-        form.clean()
-
-    def test_image_upload(self):
+    def test_valid_image_upload(self):
         album_size = len(self.album.images.all())
         image_path = os.path.join(settings.MEDIA_ROOT, self.image_filenames[0])
-        self.client.login(username=self.username, password=self.password)
-
-        # No data
-        response = self.client.post(reverse('gallery:image_upload'))
-        self.assertEqual(response.status_code, 200, "Error testing empty image upload")
 
-        # Invalid file
-        data = {'data': SimpleUploadedFile('text.txt', b'text')}
-        response = self.client.post(reverse('gallery:image_upload'), data=data)
-        self.assertContains(response, "Unable to add invalid images", msg_prefix="Error testing invalid image data")
-
-        # Valid data
         with open(image_path, 'rb') as image_file:
             data = {'apk': self.album.pk,
                     'data': image_file}
             response = self.client.post(reverse('gallery:image_upload'), data=data)
         self.assertRedirects(response, reverse('gallery:image_list'), msg_prefix="Error uploading image")
         self.assertEqual(album_size + 1, len(self.album.images.all()), "Error uploading image to album")
         self.album.images.last().delete()
         self.assertEqual(album_size, len(self.album.images.all()), "Error removing image")
 
-        self.client.logout()
+    def test_empty_image_upload(self):
+        response = self.client.post(reverse('gallery:image_upload'))
+        self.assertContains(response, "Unable to add")
+
+    def test_invalid_image_upload(self):
+        data = {'data': SimpleUploadedFile('text.txt', b'text')}
+        response = self.client.post(reverse('gallery:image_upload'), data=data)
+        self.assertContains(response, "Unable to add invalid image", msg_prefix="Error testing invalid image data")
```

### Comparing `django-starcross-gallery-1.0.9/gallery/settings.py` & `django-starcross-gallery-1.1/gallery/settings.py`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/admin.py` & `django-starcross-gallery-1.1/gallery/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,7 +28,8 @@
     filter_horizontal = ('images',)
     raw_id_fields = ('highlight',)
 
 
 admin.site.register(Image, ImageAdmin)
 admin.site.register(Album, AlbumAdmin)
 
+
```

### Comparing `django-starcross-gallery-1.0.9/gallery/views.py` & `django-starcross-gallery-1.1/gallery/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,40 +61,41 @@
 
     def get_queryset(self):
         # Order by newest first
         return super(ImageList, self).get_queryset().order_by('-pk')
 
 
 class ImageCreate(GallerySettingsMixin, LoginRequiredMixin, FormView):
-    """ Embedded drag and drop image upload"""
+    """ Embedded drag and drop image upload """
     login_url = '/admin/login/'
     form_class = ImageCreateForm
     template_name = 'gallery/image_upload.html'
 
     def form_valid(self, form):
         """ Bulk create images based on form data """
         image_data = form.files.getlist('data')
         for data in image_data:
             image = Image.objects.create(data=data)
-            image.image_albums.add(form.data['apk'])
+            if form.data.get('apk'):
+                image.image_albums.add(form.data['apk'])
         messages.success(self.request, "Images added successfully")
         return super().form_valid(form)
 
     def get_success_url(self):
         next_url = self.request.POST.get('next')
         return_url = reverse('gallery:image_list')
         if next_url:
             return_url = next_url
         return return_url
 
     def form_invalid(self, form):
         response = super().form_invalid(form)
         next_url = self.request.POST.get('next')
         if next_url:
-            # TODO: Preserve error message
+            messages.error(self.request, form.errors)
             return redirect(next_url)
         else:
             return response
 
 
 class AlbumView(GallerySettingsMixin, DetailView):
     model = Album
@@ -109,9 +110,7 @@
         context['images'] = sorted(images, key=lambda i: i.date_taken)
         return context
 
 
 class AlbumList(GallerySettingsMixin, ListView):
     model = Album
     template_name = 'gallery/album_list.html'
-
-
```

### Comparing `django-starcross-gallery-1.0.9/gallery/templates/gallery/image_detail.html` & `django-starcross-gallery-1.1/gallery/templates/gallery/image_detail.html`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/templates/gallery/gallery_base.html` & `django-starcross-gallery-1.1/gallery/templates/gallery/gallery_base.html`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 <body>
 
 <div id="top_bar">
 
     {% if logo_path %}
         <div id="logo">
-            <a href="/gallery"><img src="{% static logo_path %}" style="height: auto; max-width:100%;"></a>
+            <a href="/gallery">
+                <img src="{% static logo_path %}" alt="Gallery logo" style="height: auto; max-width:100%;">
+            </a>
         </div>
     {%  endif %}
     <div id="detail">
         {% block bar_detail %}
         {%  endblock %}
     </div>
     {% block bar_title %}
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
  {% block header %} {% endblock %}
 {% if logo_path %}
-[{%_static_logo_path_%}]
+[Gallery_logo]
 {% endif %}
 {% block bar_detail %} {% endblock %}
 {% block bar_title %}
 {{ gallery_title }}
 {% endblock %}
 {% block content %} {% endblock %}
 {{ footer_info }}
```

### Comparing `django-starcross-gallery-1.0.9/gallery/templates/gallery/image_list.html` & `django-starcross-gallery-1.1/gallery/templates/gallery/image_list.html`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/templates/gallery/album_list.html` & `django-starcross-gallery-1.1/gallery/templates/gallery/album_list.html`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/templates/gallery/album_detail.html` & `django-starcross-gallery-1.1/gallery/templates/gallery/album_detail.html`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/templates/gallery/partials/image_upload_form.html` & `django-starcross-gallery-1.1/gallery/templates/gallery/partials/image_upload_form.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-{% if form.non_field_errors %}
+{% if form.errors %}
     <div class="alert alert-warning">
-        {{ form.non_field_errors }}
+        {{ form.errors }}
     </div>
 {% endif %}
 
 {% if messages %}
     <div class="alert alert-info">
         {% for message in messages %}
             <p>{{ message }}</p>
@@ -19,12 +19,13 @@
 
     <input id="data" type="file" name="data" data-url="{% url 'gallery:image_upload' %}" multiple>
 
     <!--
     <div id="progress">
         <div class="progressbar"></div>
     </div>-->
+    <input type="submit"/>
 
-   <input type="hidden" name="apk" value="{{ album.pk }}"/>
-   <input type="hidden" name="next" value="{{ request.path }}"/>
+    <input type="hidden" name="apk" value="{{ album.pk }}"/>
+    <input type="hidden" name="next" value="{{ request.path }}"/>
 
 </form>
```

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/js/justify_images.js` & `django-starcross-gallery-1.1/gallery/static/gallery/js/justify_images.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,52 +1,50 @@
 /** Justify image grid based on thumbnail class
 
-    These global vars should be present
+    These global values should be present
 
     hdpi_factor e.g. 2
     image_margin e.g 6.0
 
 */
 
 
 
 function justify_images() {
     /** Fix the width each image in a container to fully justify each row */
 
-    var container = document.getElementById('image_container');
+    const container = document.getElementById('image_container');
     // Get exact width of container - 1 to allow for rounding error
-    var container_width = container.getBoundingClientRect()['width'] - 1;
+    const container_width = container.getBoundingClientRect()['width'] - 1;
 
     // Find the images in the thumbnail container
-    var images = document.querySelectorAll('.image');
+    const images = document.querySelectorAll('.image');
     if (images == []) {
         return;
     }
-    // Assume all images have the same height from the ImageSpecField resize
-    // var target_height = images[0].naturalHeight / hdpi_factor;
 
-    // Build an array of images for the current row and it's width
-    var row_width = 0;
-    var row_images = [];
-    for (var i = 0; i < images.length; i++) {
+    // Build an array of images for the current row, and it's width
+    let row_width = 0;
+    let row_images = [];
+    for (let i = 0; i < images.length; i++) {
         // Add the current image and it's width
         row_images.push(images[i]);
         row_width += (images[i].naturalWidth / hdpi_factor);
         // Look ahead to see how wide the next image is
-        var next_half_width = 0;
+        let next_half_width = 0;
         if (i < images.length - 1) {
             next_half_width = images[i + 1].naturalWidth / hdpi_factor / 2;
         }
-        // See if the we have exceed the size of the row, including half the next image
+        // See if we have exceeded the size of the row, including half the next image
         // This keeps us closer to the target height
         if ((row_width + next_half_width) >= container_width) {
             // Account for the total width of all margins on this row
-            var margin_total = image_margin * (row_images.length - 1);
+            const margin_total = image_margin * (row_images.length - 1);
             // Find the factor required to shrink or enlarge the images in this row
-            var resize_factor = (container_width - margin_total) / (row_width - margin_total);
+            const resize_factor = (container_width - margin_total) / (row_width - margin_total);
             resize_row(row_images, resize_factor);
             // Reset values for new row
             row_width = 0;
             row_images = [];
         } else {
             // Add the margin to the running row width
             row_width += image_margin;
@@ -59,20 +57,20 @@
     }
 
 }
 
 function resize_row(images, factor) {
     /** Set each item in the image array according to the given factor */
 
-    for (var i = 0; i < images.length; i++) {
+    for (let i = 0; i < images.length; i++) {
 
-        var overlay = images[i].nextElementSibling;
-        var width = ((images[i].naturalWidth / hdpi_factor) * factor);
+        const overlay = images[i].nextElementSibling;
+        const width = ((images[i].naturalWidth / hdpi_factor) * factor);
         images[i].style.width = width + "px";
-        var height = ((images[i].naturalHeight / hdpi_factor) * factor);
+        const height = ((images[i].naturalHeight / hdpi_factor) * factor);
         images[i].style.height = height + "px";
         // Add a margin to image and overlay if this is not the last image
         if (i < (images.length - 1)) {
             images[i].classList.add('image_spacer');
             overlay.classList.add('image_spacer');
 
         } else {
```

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/js/image_navigation.js` & `django-starcross-gallery-1.1/gallery/static/gallery/js/image_navigation.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /** Provide navigation keys to change the current image */
 
-var left = 37;
-var right = 39;
+const left = 37;
+const right = 39;
 
 document.addEventListener("keydown", function(event) {
     switch (event.which) {
         case left:
             if (previous_image_url) {
                 window.location.href = previous_image_url;
             }
```

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/js/image_upload.js` & `django-starcross-gallery-1.1/gallery/static/gallery/js/image_upload.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 /**
 Provide drag and drop support on image display pages
 */
 
 document.addEventListener('drop', function(event) {
-    var drop_container = document.getElementById('image_container');
-    var image_form = document.getElementById('image_upload_form');
-    var data_input = image_form.elements['data'];
+    const drop_container = document.getElementById('image_container');
+    const image_form = document.getElementById('image_upload_form');
+    const data_input = image_form.elements['data'];
 
     drop_container.classList.remove('highlight');
 
     data_input.files = event.dataTransfer.files;
     image_form.submit();
 
     event.preventDefault();
 });
 
 document.addEventListener('dragover', function(event) {
     event.preventDefault();
 });
 
 document.addEventListener('dragenter', function(event) {
-    var drop_container = document.getElementById('image_container');
+    const drop_container = document.getElementById('image_container');
     drop_container.classList.add('highlight');
     event.preventDefault();
 });
 
 document.addEventListener('dragexit', function() {
-    var drop_container = document.getElementById('image_container');
+    const drop_container = document.getElementById('image_container');
     drop_container.classList.remove('highlight');
 });
```

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/images/camera.png` & `django-starcross-gallery-1.1/gallery/static/gallery/images/camera.png`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/images/iso.png` & `django-starcross-gallery-1.1/gallery/static/gallery/images/iso.png`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/images/exposure.png` & `django-starcross-gallery-1.1/gallery/static/gallery/images/exposure.png`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/images/aperture.png` & `django-starcross-gallery-1.1/gallery/static/gallery/images/aperture.png`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/images/35mm.png` & `django-starcross-gallery-1.1/gallery/static/gallery/images/35mm.png`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/images/starcross.png` & `django-starcross-gallery-1.1/gallery/static/gallery/images/starcross.png`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/images/album.png` & `django-starcross-gallery-1.1/gallery/static/gallery/images/album.png`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/images/lens.png` & `django-starcross-gallery-1.1/gallery/static/gallery/images/lens.png`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/css/gallery_template.css` & `django-starcross-gallery-1.1/gallery/static/gallery/css/gallery_template.css`

 * *Files identical despite different names*

### Comparing `django-starcross-gallery-1.0.9/gallery/static/gallery/css/gallery.css` & `django-starcross-gallery-1.1/gallery/static/gallery/css/gallery.css`

 * *Files 13% similar despite different names*

```diff
@@ -87,8 +87,15 @@
     height: 76.5vh;
     object-fit: contain;
 }
 .exif_icon {
     width: 1em;
     vertical-align: sub;
     padding: 0 0.2em 0 0.5em;
+}
+.alert {
+    border: 0.15em solid;
+    margin: 1em 0;
+}
+.alert ul li {
+    list-style: none;
 }
```

### Comparing `django-starcross-gallery-1.0.9/gallery/urls.py` & `django-starcross-gallery-1.1/gallery/urls.py`

 * *Files identical despite different names*

