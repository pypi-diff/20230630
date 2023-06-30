# Comparing `tmp/apidev-coop_cms-1.6.1.tar.gz` & `tmp/apidev-coop_cms-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidev-coop_cms-1.6.1.tar", last modified: Fri Jun 30 09:04:44 2023, max compression
+gzip compressed data, was "apidev-coop_cms-1.6.2.tar", last modified: Fri Jun 30 12:17:14 2023, max compression
```

## Comparing `apidev-coop_cms-1.6.1.tar` & `apidev-coop_cms-1.6.2.tar`

### file list

```diff
@@ -1,644 +1,629 @@
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.952549 apidev-coop_cms-1.6.1/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      162 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/MANIFEST.in
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11162 2023-06-30 09:04:44.952549 apidev-coop_cms-1.6.1/PKG-INFO
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    10336 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/README.rst
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.852548 apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11162 2023-06-30 09:04:44.000000 apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/PKG-INFO
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    23840 2023-06-30 09:04:44.000000 apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/SOURCES.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-06-30 09:04:44.000000 apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/dependency_links.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-05-22 10:26:48.000000 apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/not-zip-safe
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      177 2023-06-30 09:04:44.000000 apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/requires.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        9 2023-06-30 09:04:44.000000 apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/top_level.txt
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.856548 apidev-coop_cms-1.6.1/coop_cms/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      327 2023-06-30 09:03:25.000000 apidev-coop_cms-1.6.1/coop_cms/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9252 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/admin.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.856548 apidev-coop_cms-1.6.1/coop_cms/apps/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      208 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/__init__.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.856548 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      155 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      206 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/apps.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.860548 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3722 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/0001_initial.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      478 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/0002_auto_20150924_1433.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      680 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/0003_auto_20160129_1524.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      470 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/0004_auto_20161031_1401.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2092 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/0005_auto_20190719_1408.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      411 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/models.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.844548 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/templates/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.844548 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/templates/admin/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.844548 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/templates/admin/basic_cms/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.860548 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/templates/admin/basic_cms/navtree/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       55 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/templates/admin/basic_cms/navtree/change_form.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       54 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/tests.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      427 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/translation.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.860548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      164 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      257 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/apps.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      378 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/forms.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.844548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.844548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.860548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    22608 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap-theme.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    19963 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap-theme.min.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   141622 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   117305 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap.min.css
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.864548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    20127 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   108738 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    45404 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    23424 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.woff
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.864548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/js/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    67546 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/js/bootstrap.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    35951 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/js/bootstrap.min.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      484 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/js/npm.js
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.844548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.864548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1035 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/carousel.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1874 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/form.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1257 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/headline_carousel.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      642 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/li_node.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.864548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_cms/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      851 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_cms/article_list_item.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       43 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_cms/navigation_node.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.864548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_cms/widgets/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       15 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_cms/widgets/_imageedit_cssclass.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       52 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_cms/widgets/_img_logo.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.864548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/pagination/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      998 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/pagination/pagination.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.864548 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templatetags/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       53 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templatetags/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      723 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templatetags/coop_bs.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.868548 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      434 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      481 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/admin.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      186 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/apps.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      978 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/coop_cms_settings.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1238 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/forms.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.868548 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/migrations/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3603 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/migrations/0001_initial.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/migrations/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1462 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/models.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      841 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/my_coop_bar.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/static/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.868548 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/static/css/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4845 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/static/css/demo-style.css
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.868548 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/static/js/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1931 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/static/js/jquery.sortElements.js
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.868548 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      340 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/404.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      689 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/500.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1144 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/base.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      195 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/basic_newsletter.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      964 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/blog.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      185 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/homepage.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1522 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/sortable_newsletter.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      499 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/special_newsletter.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      824 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/standard.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      390 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/standard_en.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4984 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/tests.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.868548 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      158 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      411 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/admin.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      218 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/apps.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1448 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/auth_backends.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3462 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/forms.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.868548 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/management/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       23 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/management/__init__.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.872548 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/management/commands/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       23 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/management/commands/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      707 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/management/commands/invalidate_passwords.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.872548 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/migrations/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      732 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/migrations/0001_initial.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/migrations/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      430 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/models.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.872548 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/registration_backend/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/registration_backend/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1084 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/registration_backend/forms.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1247 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/registration_backend/urls.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2362 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/registration_backend/views.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/templates/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.872548 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/templates/email_auth/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       85 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/templates/email_auth/activation_notification.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       73 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/templates/email_auth/registration_notification.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    25018 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/tests.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      924 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/urls.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.872548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       89 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1709 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/admin.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      216 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/apps.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      811 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/coop_bar_cfg.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.872548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/files/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      178 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/files/email-tracking.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      342 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/forms.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.872548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/management/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/management/__init__.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.876548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/management/commands/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/management/commands/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1459 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/management/commands/send_newsletters.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.876548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/migrations/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6018 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/migrations/0001_initial.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/migrations/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6393 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/models.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      552 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/settings.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.876548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      871 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/_link_bar.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       47 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/_linkbar_link_style.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       72 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/_linkbar_style.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      410 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/newsletter.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.876548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/public/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      846 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/public/base.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       86 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/public/base_custom.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      489 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/public/unregister_confirm.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      483 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/public/unregister_done.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.876548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/test/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      850 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/test/newsletter_contact.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      302 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/test/newsletter_contact_lang.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      706 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/test/newsletter_no_link.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.876548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templatetags/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templatetags/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      707 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templatetags/newsletters_utils.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.880548 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2525 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_customize_content.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      949 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_magic_links.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3913 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_max_length.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      655 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_newsletter.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    23608 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_sending.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6672 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_tracking.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5453 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_unregister.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8041 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_view_online.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      863 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/urls.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9219 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/utils.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4202 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/views.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.880548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      146 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1516 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/admin.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      214 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/apps.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      931 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/forms.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/en/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.880548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/en/LC_MESSAGES/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      380 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1936 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/fr/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.880548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1375 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2263 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.880548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/management/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       51 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/management/__init__.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.880548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/management/commands/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       49 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/management/commands/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      356 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/management/commands/collect_rss.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/migrations/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1861 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/migrations/0001_initial.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/migrations/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1351 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/models.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/static/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/static/css/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/static/css/rss_sync/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       93 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/static/css/rss_sync/admin-cust.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7462 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/tests.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      333 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/urls.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2272 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/utils.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1823 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/views.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1983 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/widgets.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      160 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      177 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/admin.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      220 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/apps.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1084 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/forms.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/migrations/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1278 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/migrations/0001_initial.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/migrations/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1458 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/models.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      600 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/base.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      674 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/custom_tag_template.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      887 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/detail.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      387 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/formset.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      217 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/list.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templatetags/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       23 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templatetags/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      358 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templatetags/coop_unit_test.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    32394 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/tests.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      617 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/urls.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1017 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/apps/test_app/views.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1598 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/bs_forms.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/ci/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/en/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/en/LC_MESSAGES/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      380 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5293 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/fr/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.884549 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      379 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5293 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.888548 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/public/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/public/dummy.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       74 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/requirements.txt
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.888548 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/static/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/static/dummy.js
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.888548 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      252 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/_field.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2082 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/base.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.888548 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/django_registration/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      146 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/django_registration/activate.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      345 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/django_registration/activation_complete.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      488 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/django_registration/activation_email_body.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       59 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/django_registration/activation_email_subject.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      276 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/django_registration/registration_complete.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1377 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/django_registration/registration_form.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.888548 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      136 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/base.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      478 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/logged_out.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1107 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/login.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       46 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/logout.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      268 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/password_change_done.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      386 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/password_change_form.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      250 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/password_reset_complete.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      424 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      237 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/password_reset_done.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      500 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/password_reset_form.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      393 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/standard.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      675 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/context_processors.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16929 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/coop_bar_cfg.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       79 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/exceptions.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      658 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/feeds.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.892548 apidev-coop_cms-1.6.1/coop_cms/forms/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      426 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8180 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/articles.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1019 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/base.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4528 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/content.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      360 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/fields.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4586 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/fragments.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3702 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/navigation.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7234 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/newsletters.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      365 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/forms/webutils.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12471 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/generic_views.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/locale/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/locale/en/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.892548 apidev-coop_cms-1.6.1/coop_cms/locale/en/LC_MESSAGES/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      337 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    26559 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.848548 apidev-coop_cms-1.6.1/coop_cms/locale/fr/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.892548 apidev-coop_cms-1.6.1/coop_cms/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    24224 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    36263 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       92 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/logger.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.892548 apidev-coop_cms-1.6.1/coop_cms/management/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       49 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/management/__init__.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.892548 apidev-coop_cms-1.6.1/coop_cms/management/commands/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       46 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/management/commands/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      409 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/management/commands/create_db_password.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1046 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/management/commands/create_newsletter_items.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1013 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/management/commands/migrate.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1753 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/management/commands/migrate_coop_cms_dump.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1608 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/management/commands/patch_alias_translation.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1401 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/management/commands/send_newsletter.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      712 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/middleware.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.896549 apidev-coop_cms-1.6.1/coop_cms/migrations/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16604 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0001_initial.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1528 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0002_auto_20160108_1628.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      885 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0003_auto_20160204_1540.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1079 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0004_auto_20160620_1310.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      495 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0005_articlecategory_pagination_size.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      428 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0006_image_copyright.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      425 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0007_newsletter_newsletter_date.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      442 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0008_alias_redirect_code.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      830 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0009_auto_20170301_1621.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1068 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0010_auto_20170320_1349.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      413 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0011_auto_20170502_1124.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      830 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0012_auto_20170502_1125.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      211 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0013_auto_20170607_1508.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      353 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0014_auto_20171006_1040.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3508 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0015_auto_20170608_1600.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      719 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0016_auto_20190509_2158.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      600 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0017_auto_20200124_1341.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      628 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0018_auto_20201209_0944.py
--rw-r--r--   0 lucjean   (1001) lucjean   (1001)      455 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/0019_alter_navtree_types.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/migrations/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    53670 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/models.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1302 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/moves.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      625 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/optionals.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1020 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/perms_backends.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1449 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/secrets.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16681 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/settings.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4362 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/shortcuts.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3418 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/sitemap.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.852548 apidev-coop_cms-1.6.1/coop_cms/static/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.900549 apidev-coop_cms-1.6.1/coop_cms/static/chosen/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4621 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen-bootstrap.css
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      646 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen-sprite.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      872 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen-sprite@2x.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    13586 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.css
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    40437 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.jquery.js
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    25688 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.jquery.min.js
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    11634 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.min.css
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    40895 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.proto.js
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    26064 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.proto.min.js
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.900549 apidev-coop_cms-1.6.1/coop_cms/static/css/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/admin-tricks.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1431 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/coop_cms.css
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.900549 apidev-coop_cms-1.6.1/coop_cms/static/css/images/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      112 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/border.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2893 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/controls.png
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.900549 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/borderBottomCenter.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      215 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/borderBottomLeft.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      217 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/borderBottomRight.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      108 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/borderMiddleLeft.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      108 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/borderMiddleRight.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/borderTopCenter.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      216 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/borderTopLeft.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      214 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/ie6/borderTopRight.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9427 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/loading.gif
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      157 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/loading_background.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      182 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/images/overlay.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2986 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/mediatheque.css
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.900549 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.904549 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      180 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      178 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      120 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      105 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      110 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      119 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      101 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_222222_256x240.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_454545_256x240.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_888888_256x240.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    33378 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/jquery-ui-1.8.14.custom.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2108 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/css/tree.css
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.904549 apidev-coop_cms-1.6.1/coop_cms/static/img/
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      473 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/cross.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1109 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/default-logo.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      382 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/facebook.png
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.852548 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.908549 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6066 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/avi.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4896 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/default.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5573 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/doc.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5573 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/docx.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5634 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/gif.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5958 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/html.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5634 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/jpg.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6066 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/mov.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5789 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/mp3.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6066 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/mp4.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5789 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/ogg.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5598 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/pdf.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5634 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/png.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5507 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/pps.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5507 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/ppt.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5573 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/rtf.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5625 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/xls.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5625 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/xlsx.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6155 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/zip.png
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.912549 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2269 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/avi.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      621 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/default.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1237 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/doc.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1237 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/docx.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1548 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/gif.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     2154 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/html.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1548 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/jpg.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2269 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/mov.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1378 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/mp3.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2269 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/mp4.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1378 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/ogg.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1294 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/pdf.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1548 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/png.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1142 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/pps.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1142 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/ppt.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1237 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/rtf.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      621 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/txt.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1270 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/xls.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1270 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/xlsx.png
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1746 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/zip.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2025 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/gplus.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3343 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/in_nav.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3272 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/out_nav.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1221 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/img/twitter.png
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.916549 apidev-coop_cms-1.6.1/coop_cms/static/js/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.916549 apidev-coop_cms-1.6.1/coop_cms/static/js/_lib/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4246 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/_lib/jquery.cookie.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3080 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/_lib/jquery.hotkeys.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    91341 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/_lib/jquery.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   284393 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.11.3.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    95956 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.11.3.min.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    93867 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.7.1.min.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   266057 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.8.3.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    93636 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.8.3.min.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   280364 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-3.4.1.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1589 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-ajax-csrf.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16620 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-migrate-1.2.1.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7199 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-migrate-1.2.1.min.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   210246 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-ui-1.8.14.custom.min.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   180213 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery.jstree.js
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6956 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/jquery.pageslide.js
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.852548 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.916549 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      331 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/bg.jpg
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7765 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/d.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       43 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/dot_for_ie.gif
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3987 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/style.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1849 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/throbber.gif
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.920549 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3003 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/d.gif
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7535 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/d.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       43 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/dot_for_ie.gif
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4997 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/style.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1849 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/throbber.gif
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.920549 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2944 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/d.gif
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7635 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/d.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4723 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/style.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1849 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/throbber.gif
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.920549 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2872 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/d.gif
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7459 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/d.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      132 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/dots.gif
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5811 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/style.css
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1849 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/throbber.gif
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1340 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/js/utils.coop.js
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.920549 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.924549 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      300 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/L1-center.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      305 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/L1-left.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      295 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/L1-right.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      353 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/L3-bottom.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      326 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/L3-center.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3019 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/L3-li-top.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      201 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/L3-ul-top.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      152 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/vertical-line.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      189 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/white-highlight.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5235 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/static/slickmap/slickmap.css
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.852548 apidev-coop_cms-1.6.1/coop_cms/templates/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.852548 apidev-coop_cms-1.6.1/coop_cms/templates/admin/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.852548 apidev-coop_cms-1.6.1/coop_cms/templates/admin/coop_cms/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.924549 apidev-coop_cms-1.6.1/coop_cms/templates/admin/coop_cms/navnode/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      782 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/admin/coop_cms/navnode/change_form.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      282 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/admin/coop_cms/navnode/change_list.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.924549 apidev-coop_cms-1.6.1/coop_cms/templates/admin/coop_cms/navtree/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12274 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/admin/coop_cms/navtree/change_form.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.924549 apidev-coop_cms-1.6.1/coop_cms/templates/bs/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      676 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/bs/form_fields.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      718 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/bs/horizontal_form_fields.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.936549 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1149 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_accept_cookies_message.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      210 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_article_form.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      570 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_article_publication.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      487 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_change_language.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3531 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_coop_bar_js.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      886 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_csrf_failure_message.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      532 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_facebook_like.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      150 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_field.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      124 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_form_error.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1204 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_js_includes.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      544 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_messages.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      439 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_newsletter_articles.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      854 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_newsletter_categories.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      354 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_newsletter_categories_index.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2115 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_pagination.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      975 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_pagination_js.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1164 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_social_share.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      382 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/article.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/article_list.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      498 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/article_list_item.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      449 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/articles_category.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       26 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/base.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.936549 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/categories/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      520 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/categories/only-for-unit-testing.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      275 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/csrf_403.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/dropdown_li.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       54 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/dropdown_li_class.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       97 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/dropdown_ul.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.936549 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/medialib/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4384 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/medialib/slide_base.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      506 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/medialib/slide_docs_content.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1155 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/medialib/slide_images_content.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1286 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/medialib/slide_photologue_content.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      538 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/navigation_node.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.936549 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/navtree_content/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      502 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/navtree_content/article.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      958 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/navtree_content/default.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2546 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/newsletter.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2090 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/newsletter_base.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1149 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_add_fragment.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      299 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_article_settings.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_change_newsletter_template.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      217 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_change_template.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2684 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_edit_fragments.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      278 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_new_article.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      180 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_new_link.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      494 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_newsletter_settings.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      946 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_publish_article.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_schedule_newsletter_sending.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      184 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_set_homepage.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      200 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_swicth_language.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      400 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_test_newsletter.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      205 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_update_logo.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_upload_doc.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      238 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_upload_image.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       45 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/test_li.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2570 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/view_all_articles.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.940549 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/widgets/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/widgets/_imageedit_cssclass.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      507 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/widgets/chosen.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      170 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/widgets/imageedit.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      195 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/widgets/readonlyinput.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.944549 apidev-coop_cms-1.6.1/coop_cms/templates/test/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       14 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/_accept_cookies_message.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      233 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/_fragment.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       54 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      460 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_li_node.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      316 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_no_logo_size.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      443 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_blocks.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      354 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_blocks_parent.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      495 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_fragments.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      539 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_fragments_extra_id.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      564 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_fragments_template.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      334 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_logo_size.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      350 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_logo_size_and_crop.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2082 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/base.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      378 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/base_article.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1035 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/carousel.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      173 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/nav_tag_in_edit_tag.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      645 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/navigation_li_node.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      575 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/navigation_node.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      147 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/newsletter_blue.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      483 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/newsletter_red.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      394 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/standard.html
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      148 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templates/test/test_send_email.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.944549 apidev-coop_cms-1.6.1/coop_cms/templatetags/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       43 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/templatetags/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2233 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/templatetags/article_tags.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    21043 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/templatetags/coop_edition.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7258 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/templatetags/coop_navigation.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16166 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/templatetags/coop_utils.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      396 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/test_runners.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.948549 apidev-coop_cms-1.6.1/coop_cms/tests/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6329 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/__init__.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.948549 apidev-coop_cms-1.6.1/coop_cms/tests/fixtures/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      221 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/tests/fixtures/unittest1.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       60 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/tests/fixtures/unittest1.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      215 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/tests/fixtures/unittest2.png
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3719 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_admin.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8437 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_alias.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    33962 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_articles.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4513 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_cache.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12612 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_categories.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8767 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_edition.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    63456 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_fragments.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      761 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_generic_views.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    33312 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_homepage.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7678 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_link.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    23485 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_localization.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    41138 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_media.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      637 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_middleware.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8965 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_multisites.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    64715 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_navigation.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    69167 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_newsletter.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2160 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_permissions.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1363 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_settings.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8190 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_sitemap.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5039 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_slugs.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3048 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_special_pages.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2814 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_templates.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    22100 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_templatetags.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1927 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/tests/test_utils.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1022 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/thumbnail_backend.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2937 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/translation.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5352 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/urls.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.952549 apidev-coop_cms-1.6.1/coop_cms/utils/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      543 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/utils/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5948 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/utils/emails.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1839 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/utils/i18n.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      969 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/utils/loaders.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      658 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/utils/pagination.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1583 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/utils/requests.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      257 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/utils/settings.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2523 2023-06-30 09:01:25.000000 apidev-coop_cms-1.6.1/coop_cms/utils/text.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2261 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/utils/xsendfile.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 09:04:44.952549 apidev-coop_cms-1.6.1/coop_cms/views/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.1/coop_cms/views/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11773 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/views/articles.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2467 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/views/fragments.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2239 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/views/homepage.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1513 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/views/links.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7225 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/views/medialib.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    13211 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/views/navigation.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8233 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/views/newsletters.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4933 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/views/webutils.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5774 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/coop_cms/widgets.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       38 2023-06-30 09:04:44.952549 apidev-coop_cms-1.6.1/setup.cfg
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1723 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.1/setup.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.285429 apidev-coop_cms-1.6.2/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      162 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/MANIFEST.in
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11162 2023-06-30 12:17:14.285429 apidev-coop_cms-1.6.2/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    10336 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/README.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.237429 apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11162 2023-06-30 12:17:14.000000 apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    23220 2023-06-30 12:17:14.000000 apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-06-30 12:17:14.000000 apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-05-22 10:26:48.000000 apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/not-zip-safe
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      177 2023-06-30 12:17:14.000000 apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/requires.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        9 2023-06-30 12:17:14.000000 apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/top_level.txt
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      327 2023-06-30 12:16:07.000000 apidev-coop_cms-1.6.2/coop_cms/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9252 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/admin.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/apps/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      208 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/__init__.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      155 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      206 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/apps.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3722 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/0001_initial.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      478 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/0002_auto_20150924_1433.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      680 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/0003_auto_20160129_1524.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      470 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/0004_auto_20161031_1401.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2092 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/0005_auto_20190719_1408.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      411 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/models.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.229429 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.229429 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/templates/admin/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.229429 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/templates/admin/basic_cms/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/templates/admin/basic_cms/navtree/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       55 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/templates/admin/basic_cms/navtree/change_form.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       54 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/tests.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      427 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/translation.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      164 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      257 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      378 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.229429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.229429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    22608 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap-theme.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    19963 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap-theme.min.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   141622 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   117305 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap.min.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    20127 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   108738 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    45404 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    23424 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.woff
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.241429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/js/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    67546 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/js/bootstrap.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    35951 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/js/bootstrap.min.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      484 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/js/npm.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.229429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1035 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/carousel.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1874 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/form.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1257 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/headline_carousel.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      642 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/li_node.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_cms/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      851 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_cms/article_list_item.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       43 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_cms/navigation_node.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_cms/widgets/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       15 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_cms/widgets/_imageedit_cssclass.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       52 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_cms/widgets/_img_logo.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/pagination/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      998 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/pagination/pagination.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templatetags/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       53 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templatetags/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      723 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templatetags/coop_bs.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      434 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      481 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/admin.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      186 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      978 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/coop_cms_settings.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1238 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/migrations/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3603 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/migrations/0001_initial.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/migrations/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1462 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/models.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      841 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/my_coop_bar.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/static/css/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4845 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/static/css/demo-style.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/static/js/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1931 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/static/js/jquery.sortElements.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      340 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/404.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      689 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/500.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1144 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/base.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      195 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/basic_newsletter.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      964 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/blog.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      185 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/homepage.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1522 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/sortable_newsletter.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      499 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/special_newsletter.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      824 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/standard.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      390 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/standard_en.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4984 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/tests.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      158 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      411 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/admin.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      218 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1448 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/auth_backends.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3462 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/management/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       23 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/management/__init__.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/management/commands/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       23 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/management/commands/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      707 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/management/commands/invalidate_passwords.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.245429 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/migrations/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      732 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/migrations/0001_initial.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/migrations/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      430 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/models.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/registration_backend/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/registration_backend/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1084 2023-06-30 09:37:28.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/registration_backend/forms.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1247 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/registration_backend/urls.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2362 2023-06-30 09:37:34.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/registration_backend/views.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/templates/email_auth/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       85 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/templates/email_auth/activation_notification.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       73 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/templates/email_auth/registration_notification.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    25018 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/tests.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      924 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/urls.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       89 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1709 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/admin.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      216 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      811 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/coop_bar_cfg.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/files/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      178 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/files/email-tracking.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      342 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/management/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/management/__init__.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/management/commands/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/management/commands/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1459 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/management/commands/send_newsletters.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/migrations/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6018 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/migrations/0001_initial.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/migrations/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6393 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/models.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      552 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/settings.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      871 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/_link_bar.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       47 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/_linkbar_link_style.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       72 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/_linkbar_style.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      410 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/newsletter.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/public/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      846 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/public/base.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       86 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/public/base_custom.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      489 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/public/unregister_confirm.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      483 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/public/unregister_done.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/test/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      850 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/test/newsletter_contact.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      302 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/test/newsletter_contact_lang.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      706 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/test/newsletter_no_link.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templatetags/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templatetags/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      707 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templatetags/newsletters_utils.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.249429 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2525 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_customize_content.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      949 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_magic_links.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3913 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_max_length.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      655 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_newsletter.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    23608 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_sending.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6672 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_tracking.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5453 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_unregister.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8041 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_view_online.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      863 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/urls.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9219 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4202 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/views.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      146 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1516 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/admin.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      214 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      931 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/en/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      380 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1936 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/fr/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1375 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2263 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/management/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       51 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/management/__init__.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/management/commands/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       49 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/management/commands/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      356 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/management/commands/collect_rss.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/migrations/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1861 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/migrations/0001_initial.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/migrations/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1351 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/models.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/static/css/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/static/css/rss_sync/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       93 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/static/css/rss_sync/admin-cust.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7462 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/tests.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      333 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/urls.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2272 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1823 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/views.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1983 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/widgets.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      160 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      177 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/admin.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      220 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1084 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/migrations/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1278 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/migrations/0001_initial.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/migrations/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1458 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/models.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      600 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/base.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      674 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/custom_tag_template.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      887 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/detail.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      387 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/formset.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      217 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/list.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templatetags/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       23 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templatetags/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      358 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templatetags/coop_unit_test.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    32394 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/tests.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      617 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/urls.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1017 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/apps/test_app/views.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1598 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/bs_forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/ci/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/en/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      380 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5293 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/fr/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.253429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      379 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5293 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/public/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/public/dummy.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       74 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/requirements.txt
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/static/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/static/dummy.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      252 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/_field.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2082 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/base.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/django_registration/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      146 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/django_registration/activate.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      345 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/django_registration/activation_complete.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      488 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/django_registration/activation_email_body.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       59 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/django_registration/activation_email_subject.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      276 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/django_registration/registration_complete.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1377 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/django_registration/registration_form.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      136 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/base.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      478 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/logged_out.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1107 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/login.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       46 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/logout.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      268 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/password_change_done.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      386 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/password_change_form.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      250 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      424 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      237 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/password_reset_done.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      500 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/password_reset_form.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      393 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/standard.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      675 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/context_processors.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16929 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/coop_bar_cfg.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       79 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/exceptions.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      658 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/feeds.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/forms/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      426 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8180 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/articles.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1019 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/base.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4528 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/content.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      360 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/fields.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4586 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/fragments.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3702 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/navigation.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7234 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/newsletters.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      365 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/forms/webutils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12471 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/generic_views.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/locale/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/locale/en/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      337 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    26559 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.233429 apidev-coop_cms-1.6.2/coop_cms/locale/fr/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    24224 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    36263 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       92 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/logger.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/management/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       49 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/management/__init__.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.257429 apidev-coop_cms-1.6.2/coop_cms/management/commands/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       46 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/management/commands/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      409 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/management/commands/create_db_password.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1046 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/management/commands/create_newsletter_items.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1013 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/management/commands/migrate.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1753 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/management/commands/migrate_coop_cms_dump.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1608 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/management/commands/patch_alias_translation.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1401 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/management/commands/send_newsletter.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      712 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/middleware.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.261429 apidev-coop_cms-1.6.2/coop_cms/migrations/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16604 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0001_initial.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1528 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0002_auto_20160108_1628.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      885 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0003_auto_20160204_1540.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1079 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0004_auto_20160620_1310.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      495 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0005_articlecategory_pagination_size.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      428 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0006_image_copyright.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      425 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0007_newsletter_newsletter_date.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      442 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0008_alias_redirect_code.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      830 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0009_auto_20170301_1621.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1068 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0010_auto_20170320_1349.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      413 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0011_auto_20170502_1124.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      830 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0012_auto_20170502_1125.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      211 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0013_auto_20170607_1508.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      353 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0014_auto_20171006_1040.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3508 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0015_auto_20170608_1600.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      719 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0016_auto_20190509_2158.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      600 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0017_auto_20200124_1341.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      628 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0018_auto_20201209_0944.py
+-rw-r--r--   0 lucjean   (1001) lucjean   (1001)      455 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/0019_alter_navtree_types.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/migrations/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    53670 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/models.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1302 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/moves.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      625 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/optionals.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1020 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/perms_backends.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1449 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/secrets.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16681 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/settings.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4362 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/shortcuts.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3418 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/sitemap.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.237429 apidev-coop_cms-1.6.2/coop_cms/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.261429 apidev-coop_cms-1.6.2/coop_cms/static/chosen/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4621 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen-bootstrap.css
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      646 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen-sprite.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      872 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen-sprite@2x.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    13586 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.css
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    40437 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.jquery.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    25688 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.jquery.min.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    11634 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.min.css
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    40895 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.proto.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    26064 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.proto.min.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.261429 apidev-coop_cms-1.6.2/coop_cms/static/css/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/admin-tricks.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1431 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/coop_cms.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2986 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/mediatheque.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.261429 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.261429 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      180 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      178 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      120 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      105 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      110 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      119 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      101 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_222222_256x240.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_454545_256x240.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_888888_256x240.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4369 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    33378 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/jquery-ui-1.8.14.custom.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2108 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/css/tree.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.265429 apidev-coop_cms-1.6.2/coop_cms/static/img/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      473 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/cross.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1109 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/default-logo.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      382 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/facebook.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.237429 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.265429 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6066 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/avi.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4896 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/default.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5573 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/doc.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5573 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/docx.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5634 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/gif.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5958 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/html.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5634 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/jpg.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6066 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/mov.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5789 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/mp3.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6066 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/mp4.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5789 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/ogg.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5598 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/pdf.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5634 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/png.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5507 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/pps.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5507 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/ppt.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5573 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/rtf.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5625 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/xls.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5625 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/xlsx.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6155 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/zip.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.269429 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2269 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/avi.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      621 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/default.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1237 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/doc.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1237 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/docx.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1548 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/gif.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     2154 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/html.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1548 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/jpg.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2269 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/mov.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1378 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/mp3.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2269 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/mp4.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1378 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/ogg.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1294 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/pdf.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1548 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/png.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1142 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/pps.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1142 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/ppt.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1237 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/rtf.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      621 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/txt.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1270 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/xls.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1270 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/xlsx.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1746 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/zip.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2025 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/gplus.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3343 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/in_nav.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3272 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/out_nav.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1221 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/img/twitter.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.269429 apidev-coop_cms-1.6.2/coop_cms/static/js/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.269429 apidev-coop_cms-1.6.2/coop_cms/static/js/_lib/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4246 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/_lib/jquery.cookie.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3080 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/_lib/jquery.hotkeys.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    91341 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/_lib/jquery.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   284393 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.11.3.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    95956 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.11.3.min.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    93867 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.7.1.min.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   266057 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.8.3.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    93636 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.8.3.min.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   280364 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-3.4.1.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1589 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-ajax-csrf.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16620 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-migrate-1.2.1.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7199 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-migrate-1.2.1.min.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   210246 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-ui-1.8.14.custom.min.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   180213 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery.jstree.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6956 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/jquery.pageslide.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.237429 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.269429 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      331 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/bg.jpg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7765 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/d.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       43 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/dot_for_ie.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3987 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/style.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1849 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/throbber.gif
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.269429 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3003 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/d.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7535 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/d.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       43 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/dot_for_ie.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4997 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/style.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1849 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/throbber.gif
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.273429 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2944 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/d.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7635 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/d.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4723 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/style.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1849 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/throbber.gif
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.273429 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2872 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/d.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7459 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/d.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      132 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/dots.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5811 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/style.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1849 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/throbber.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1340 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/js/utils.coop.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.273429 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.273429 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      300 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/L1-center.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      305 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/L1-left.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      295 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/L1-right.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      353 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/L3-bottom.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      326 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/L3-center.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3019 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/L3-li-top.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      201 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/L3-ul-top.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      152 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/vertical-line.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      189 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/white-highlight.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5235 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/static/slickmap/slickmap.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.237429 apidev-coop_cms-1.6.2/coop_cms/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.237429 apidev-coop_cms-1.6.2/coop_cms/templates/admin/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.237429 apidev-coop_cms-1.6.2/coop_cms/templates/admin/coop_cms/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.273429 apidev-coop_cms-1.6.2/coop_cms/templates/admin/coop_cms/navnode/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      782 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/admin/coop_cms/navnode/change_form.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      282 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/admin/coop_cms/navnode/change_list.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.273429 apidev-coop_cms-1.6.2/coop_cms/templates/admin/coop_cms/navtree/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12274 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/admin/coop_cms/navtree/change_form.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.273429 apidev-coop_cms-1.6.2/coop_cms/templates/bs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      676 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/bs/form_fields.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      718 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/bs/horizontal_form_fields.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.277429 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1149 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_accept_cookies_message.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      210 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_article_form.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      570 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_article_publication.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      487 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_change_language.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3531 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_coop_bar_js.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      886 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_csrf_failure_message.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      532 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_facebook_like.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      150 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_field.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      124 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_form_error.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1204 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_js_includes.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      544 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_messages.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      439 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_newsletter_articles.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      854 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_newsletter_categories.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      354 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_newsletter_categories_index.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2115 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_pagination.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      975 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_pagination_js.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1164 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_social_share.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      382 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/article.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/article_list.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      498 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/article_list_item.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      449 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/articles_category.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       26 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/base.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.277429 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/categories/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      520 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/categories/only-for-unit-testing.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      275 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/csrf_403.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/dropdown_li.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       54 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/dropdown_li_class.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       97 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/dropdown_ul.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.277429 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/medialib/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4384 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/medialib/slide_base.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      506 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/medialib/slide_docs_content.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1155 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/medialib/slide_images_content.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1286 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/medialib/slide_photologue_content.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      538 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/navigation_node.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.277429 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/navtree_content/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      502 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/navtree_content/article.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      958 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/navtree_content/default.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2546 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/newsletter.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2090 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/newsletter_base.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1149 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_add_fragment.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      299 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_article_settings.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_change_newsletter_template.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      217 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_change_template.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2684 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_edit_fragments.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      278 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_new_article.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      180 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_new_link.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      494 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_newsletter_settings.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      946 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_publish_article.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_schedule_newsletter_sending.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      184 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_set_homepage.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      200 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_swicth_language.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      400 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_test_newsletter.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      205 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_update_logo.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_upload_doc.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      238 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_upload_image.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       45 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/test_li.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2570 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/view_all_articles.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.277429 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/widgets/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/widgets/_imageedit_cssclass.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      507 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/widgets/chosen.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      170 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/widgets/imageedit.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      195 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/widgets/readonlyinput.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.281429 apidev-coop_cms-1.6.2/coop_cms/templates/test/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       14 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/_accept_cookies_message.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      233 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/_fragment.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       54 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      460 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_li_node.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      316 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_no_logo_size.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      443 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_blocks.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      354 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_blocks_parent.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      495 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_fragments.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      539 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_fragments_extra_id.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      564 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_fragments_template.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      334 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_logo_size.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      350 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_logo_size_and_crop.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2082 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/base.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      378 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/base_article.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1035 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/carousel.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      173 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/nav_tag_in_edit_tag.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      645 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/navigation_li_node.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      575 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/navigation_node.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      147 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/newsletter_blue.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      483 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/newsletter_red.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      394 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/standard.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      148 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templates/test/test_send_email.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.281429 apidev-coop_cms-1.6.2/coop_cms/templatetags/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       43 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/templatetags/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2233 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/templatetags/article_tags.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    21043 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/templatetags/coop_edition.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7258 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/templatetags/coop_navigation.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16166 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/templatetags/coop_utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      396 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/test_runners.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.281429 apidev-coop_cms-1.6.2/coop_cms/tests/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6292 2023-06-30 09:39:50.000000 apidev-coop_cms-1.6.2/coop_cms/tests/__init__.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.281429 apidev-coop_cms-1.6.2/coop_cms/tests/fixtures/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      221 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/tests/fixtures/unittest1.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       60 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/tests/fixtures/unittest1.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      215 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/tests/fixtures/unittest2.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3719 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_admin.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8437 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_alias.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    33962 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_articles.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4513 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_cache.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12612 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_categories.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8767 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_edition.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    63456 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_fragments.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      761 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_generic_views.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    33312 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_homepage.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7678 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_link.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    23485 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_localization.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    41138 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_media.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      637 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_middleware.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8965 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_multisites.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    64715 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_navigation.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    69167 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_newsletter.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2160 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_permissions.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1363 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_settings.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8190 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_sitemap.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5039 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_slugs.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3048 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_special_pages.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2814 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_templates.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    22100 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_templatetags.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1927 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/tests/test_utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1022 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/thumbnail_backend.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2937 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/translation.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5352 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/urls.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.285429 apidev-coop_cms-1.6.2/coop_cms/utils/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      543 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/utils/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5948 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/utils/emails.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1839 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/utils/i18n.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      969 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/utils/loaders.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      658 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/utils/pagination.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1583 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/utils/requests.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      257 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/utils/settings.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2523 2023-06-30 09:01:25.000000 apidev-coop_cms-1.6.2/coop_cms/utils/text.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2261 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/utils/xsendfile.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-30 12:17:14.285429 apidev-coop_cms-1.6.2/coop_cms/views/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       24 2023-05-22 06:59:48.000000 apidev-coop_cms-1.6.2/coop_cms/views/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11773 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/views/articles.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2467 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/views/fragments.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2239 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/views/homepage.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1513 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/views/links.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7225 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/views/medialib.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    13211 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/views/navigation.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8233 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/views/newsletters.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4933 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/views/webutils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5774 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/coop_cms/widgets.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       38 2023-06-30 12:17:14.285429 apidev-coop_cms-1.6.2/setup.cfg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1723 2023-06-12 12:47:18.000000 apidev-coop_cms-1.6.2/setup.py
```

### Comparing `apidev-coop_cms-1.6.1/PKG-INFO` & `apidev-coop_cms-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidev-coop_cms
-Version: 1.6.1
+Version: 1.6.2
 Summary: Small CMS built around a tree navigation open to any django models
 Home-page: https://github.com/ljean/coop_cms/
 Download-URL: https://github.com/ljean/coop_cms/tarball/master
 Author: Luc Jean
 Author-email: ljean@apidev.fr
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apidev-coop_cms-1.6.1/README.rst` & `apidev-coop_cms-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/PKG-INFO` & `apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidev-coop-cms
-Version: 1.6.1
+Version: 1.6.2
 Summary: Small CMS built around a tree navigation open to any django models
 Home-page: https://github.com/ljean/coop_cms/
 Download-URL: https://github.com/ljean/coop_cms/tarball/master
 Author: Luc Jean
 Author-email: ljean@apidev.fr
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apidev-coop_cms-1.6.1/apidev_coop_cms.egg-info/SOURCES.txt` & `apidev-coop_cms-1.6.2/apidev_coop_cms.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -260,27 +260,14 @@
 coop_cms/static/chosen/chosen.min.css
 coop_cms/static/chosen/chosen.proto.js
 coop_cms/static/chosen/chosen.proto.min.js
 coop_cms/static/css/admin-tricks.css
 coop_cms/static/css/coop_cms.css
 coop_cms/static/css/mediatheque.css
 coop_cms/static/css/tree.css
-coop_cms/static/css/images/border.png
-coop_cms/static/css/images/controls.png
-coop_cms/static/css/images/loading.gif
-coop_cms/static/css/images/loading_background.png
-coop_cms/static/css/images/overlay.png
-coop_cms/static/css/images/ie6/borderBottomCenter.png
-coop_cms/static/css/images/ie6/borderBottomLeft.png
-coop_cms/static/css/images/ie6/borderBottomRight.png
-coop_cms/static/css/images/ie6/borderMiddleLeft.png
-coop_cms/static/css/images/ie6/borderMiddleRight.png
-coop_cms/static/css/images/ie6/borderTopCenter.png
-coop_cms/static/css/images/ie6/borderTopLeft.png
-coop_cms/static/css/images/ie6/borderTopRight.png
 coop_cms/static/css/smoothness/jquery-ui-1.8.14.custom.css
 coop_cms/static/css/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
 coop_cms/static/css/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
 coop_cms/static/css/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
 coop_cms/static/css/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
 coop_cms/static/css/smoothness/images/ui-bg_glass_75_dadada_1x400.png
 coop_cms/static/css/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
```

### Comparing `apidev-coop_cms-1.6.1/coop_cms/admin.py` & `apidev-coop_cms-1.6.2/coop_cms/admin.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/0001_initial.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/0003_auto_20160129_1524.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/0003_auto_20160129_1524.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/basic_cms/migrations/0005_auto_20190719_1408.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/basic_cms/migrations/0005_auto_20190719_1408.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap-theme.css` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap-theme.min.css` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap.css` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap.min.css` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.eot` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.svg` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.ttf` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.woff` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/js/bootstrap.js` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/static/bs/js/bootstrap.min.js` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/static/bs/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/carousel.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/carousel.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/form.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/form.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/headline_carousel.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/headline_carousel.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/li_node.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_bootstrap/li_node.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/coop_cms/article_list_item.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/coop_cms/article_list_item.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templates/pagination/pagination.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templates/pagination/pagination.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/coop_bootstrap/templatetags/coop_bs.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/coop_bootstrap/templatetags/coop_bs.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/coop_cms_settings.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/coop_cms_settings.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/forms.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/forms.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/migrations/0001_initial.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/models.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/models.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/my_coop_bar.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/my_coop_bar.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/static/css/demo-style.css` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/static/css/demo-style.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/static/js/jquery.sortElements.js` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/static/js/jquery.sortElements.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/500.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/500.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/base.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/base.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/blog.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/blog.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/sortable_newsletter.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/sortable_newsletter.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/templates/standard.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/templates/standard.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/demo_cms/tests.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/demo_cms/tests.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/auth_backends.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/auth_backends.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/forms.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/forms.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/management/commands/invalidate_passwords.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/management/commands/invalidate_passwords.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/migrations/0001_initial.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/registration_backend/forms.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/registration_backend/forms.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/registration_backend/urls.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/registration_backend/urls.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/registration_backend/views.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/registration_backend/views.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/tests.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/tests.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/email_auth/urls.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/email_auth/urls.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/admin.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/admin.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/coop_bar_cfg.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/coop_bar_cfg.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/management/commands/send_newsletters.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/management/commands/send_newsletters.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/migrations/0001_initial.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/models.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/models.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/settings.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/settings.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/_link_bar.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/_link_bar.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/newsletters/public/base.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/newsletters/public/base.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/test/newsletter_contact.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/test/newsletter_contact.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templates/test/newsletter_no_link.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templates/test/newsletter_no_link.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/templatetags/newsletters_utils.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/templatetags/newsletters_utils.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_customize_content.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_customize_content.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_magic_links.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_magic_links.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_max_length.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_max_length.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_newsletter.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_newsletter.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_sending.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_sending.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_tracking.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_tracking.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_unregister.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_unregister.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/tests/test_view_online.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/tests/test_view_online.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/urls.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/urls.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/utils.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/utils.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/newsletters/views.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/newsletters/views.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/admin.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/admin.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/forms.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/forms.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/en/LC_MESSAGES/django.po` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/django.mo` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/django.po` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/migrations/0001_initial.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/models.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/models.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/tests.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/tests.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/utils.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/utils.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/views.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/views.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/rss_sync/widgets.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/rss_sync/widgets.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/forms.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/forms.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/migrations/0001_initial.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/models.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/models.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/base.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/base.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/custom_tag_template.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/custom_tag_template.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/templates/coop_cms/test_app/detail.html` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/templates/coop_cms/test_app/detail.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/tests.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/tests.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/urls.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/urls.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/apps/test_app/views.py` & `apidev-coop_cms-1.6.2/coop_cms/apps/test_app/views.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/bs_forms.py` & `apidev-coop_cms-1.6.2/coop_cms/bs_forms.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/en/LC_MESSAGES/django.po` & `apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/locale/fr/LC_MESSAGES/django.po` & `apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/base.html` & `apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/base.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/django_registration/registration_form.html` & `apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/ci/semaphore_project/templates/registration/login.html` & `apidev-coop_cms-1.6.2/coop_cms/ci/semaphore_project/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/context_processors.py` & `apidev-coop_cms-1.6.2/coop_cms/context_processors.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/coop_bar_cfg.py` & `apidev-coop_cms-1.6.2/coop_cms/coop_bar_cfg.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/feeds.py` & `apidev-coop_cms-1.6.2/coop_cms/feeds.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/forms/articles.py` & `apidev-coop_cms-1.6.2/coop_cms/forms/articles.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/forms/base.py` & `apidev-coop_cms-1.6.2/coop_cms/forms/base.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/forms/content.py` & `apidev-coop_cms-1.6.2/coop_cms/forms/content.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/forms/fragments.py` & `apidev-coop_cms-1.6.2/coop_cms/forms/fragments.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/forms/navigation.py` & `apidev-coop_cms-1.6.2/coop_cms/forms/navigation.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/forms/newsletters.py` & `apidev-coop_cms-1.6.2/coop_cms/forms/newsletters.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/generic_views.py` & `apidev-coop_cms-1.6.2/coop_cms/generic_views.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/locale/en/LC_MESSAGES/django.po` & `apidev-coop_cms-1.6.2/coop_cms/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/locale/fr/LC_MESSAGES/django.mo` & `apidev-coop_cms-1.6.2/coop_cms/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/locale/fr/LC_MESSAGES/django.po` & `apidev-coop_cms-1.6.2/coop_cms/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/management/commands/create_newsletter_items.py` & `apidev-coop_cms-1.6.2/coop_cms/management/commands/create_newsletter_items.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/management/commands/migrate.py` & `apidev-coop_cms-1.6.2/coop_cms/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/management/commands/migrate_coop_cms_dump.py` & `apidev-coop_cms-1.6.2/coop_cms/management/commands/migrate_coop_cms_dump.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/management/commands/patch_alias_translation.py` & `apidev-coop_cms-1.6.2/coop_cms/management/commands/patch_alias_translation.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/management/commands/send_newsletter.py` & `apidev-coop_cms-1.6.2/coop_cms/management/commands/send_newsletter.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/middleware.py` & `apidev-coop_cms-1.6.2/coop_cms/middleware.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0001_initial.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0002_auto_20160108_1628.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0002_auto_20160108_1628.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0003_auto_20160204_1540.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0003_auto_20160204_1540.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0004_auto_20160620_1310.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0004_auto_20160620_1310.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0009_auto_20170301_1621.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0009_auto_20170301_1621.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0010_auto_20170320_1349.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0010_auto_20170320_1349.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0012_auto_20170502_1125.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0012_auto_20170502_1125.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0015_auto_20170608_1600.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0015_auto_20170608_1600.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0016_auto_20190509_2158.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0016_auto_20190509_2158.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0017_auto_20200124_1341.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0017_auto_20200124_1341.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/migrations/0018_auto_20201209_0944.py` & `apidev-coop_cms-1.6.2/coop_cms/migrations/0018_auto_20201209_0944.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/models.py` & `apidev-coop_cms-1.6.2/coop_cms/models.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/moves.py` & `apidev-coop_cms-1.6.2/coop_cms/moves.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/optionals.py` & `apidev-coop_cms-1.6.2/coop_cms/optionals.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/perms_backends.py` & `apidev-coop_cms-1.6.2/coop_cms/perms_backends.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/secrets.py` & `apidev-coop_cms-1.6.2/coop_cms/secrets.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/settings.py` & `apidev-coop_cms-1.6.2/coop_cms/settings.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/shortcuts.py` & `apidev-coop_cms-1.6.2/coop_cms/shortcuts.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/sitemap.py` & `apidev-coop_cms-1.6.2/coop_cms/sitemap.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen-bootstrap.css` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen-bootstrap.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen-sprite.png` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen-sprite@2x.png` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.css` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.jquery.js` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.jquery.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.jquery.min.js` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.min.css` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.min.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.proto.js` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.proto.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/chosen/chosen.proto.min.js` & `apidev-coop_cms-1.6.2/coop_cms/static/chosen/chosen.proto.min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/coop_cms.css` & `apidev-coop_cms-1.6.2/coop_cms/static/css/coop_cms.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/mediatheque.css` & `apidev-coop_cms-1.6.2/coop_cms/static/css/mediatheque.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_222222_256x240.png` & `apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_2e83ff_256x240.png` & `apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_454545_256x240.png` & `apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_888888_256x240.png` & `apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/images/ui-icons_cd0a0a_256x240.png` & `apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/smoothness/jquery-ui-1.8.14.custom.css` & `apidev-coop_cms-1.6.2/coop_cms/static/css/smoothness/jquery-ui-1.8.14.custom.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/css/tree.css` & `apidev-coop_cms-1.6.2/coop_cms/static/css/tree.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/default-logo.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/default-logo.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/avi.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/avi.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/default.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/default.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/doc.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/doc.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/docx.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/docx.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/gif.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/gif.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/html.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/html.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/jpg.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/jpg.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/mov.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/mov.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/mp3.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/mp3.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/mp4.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/mp4.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/ogg.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/ogg.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/pdf.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/pdf.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/png.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/png.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/pps.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/pps.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/ppt.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/ppt.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/rtf.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/rtf.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/xls.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/xls.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/xlsx.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/xlsx.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/bloc/zip.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/bloc/zip.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/avi.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/avi.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/default.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/default.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/doc.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/doc.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/docx.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/docx.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/gif.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/gif.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/html.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/html.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/jpg.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/jpg.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/mov.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/mov.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/mp3.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/mp3.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/mp4.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/mp4.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/ogg.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/ogg.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/pdf.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/pdf.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/png.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/png.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/pps.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/pps.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/ppt.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/ppt.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/rtf.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/rtf.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/txt.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/txt.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/xls.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/xls.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/xlsx.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/xlsx.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/filetypes/icon/zip.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/filetypes/icon/zip.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/gplus.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/gplus.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/in_nav.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/in_nav.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/out_nav.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/out_nav.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/img/twitter.png` & `apidev-coop_cms-1.6.2/coop_cms/static/img/twitter.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/_lib/jquery.cookie.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/_lib/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/_lib/jquery.hotkeys.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/_lib/jquery.hotkeys.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/_lib/jquery.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/_lib/jquery.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.11.3.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.11.3.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.11.3.min.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.11.3.min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.7.1.min.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.7.1.min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.8.3.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.8.3.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-1.8.3.min.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-1.8.3.min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-3.4.1.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-ajax-csrf.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-ajax-csrf.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-migrate-1.2.1.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-migrate-1.2.1.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-migrate-1.2.1.min.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-migrate-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery-ui-1.8.14.custom.min.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery-ui-1.8.14.custom.min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery.jstree.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery.jstree.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/jquery.pageslide.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/jquery.pageslide.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/d.png` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/d.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/style.css` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/style.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/apple/throbber.gif` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/apple/throbber.gif`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/d.gif` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/d.gif`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/d.png` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/d.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/style.css` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/style.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/classic/throbber.gif` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/classic/throbber.gif`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/d.gif` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/d.gif`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/d.png` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/d.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/style.css` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default/throbber.gif` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/d.gif` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/d.gif`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/d.png` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/d.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/style.css` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/style.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/themes/default-rtl/throbber.gif` & `apidev-coop_cms-1.6.2/coop_cms/static/js/themes/default-rtl/throbber.gif`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/js/utils.coop.js` & `apidev-coop_cms-1.6.2/coop_cms/static/js/utils.coop.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/slickmap/images/L3-li-top.png` & `apidev-coop_cms-1.6.2/coop_cms/static/slickmap/images/L3-li-top.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/static/slickmap/slickmap.css` & `apidev-coop_cms-1.6.2/coop_cms/static/slickmap/slickmap.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/admin/coop_cms/navnode/change_form.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/admin/coop_cms/navnode/change_form.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/admin/coop_cms/navtree/change_form.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/admin/coop_cms/navtree/change_form.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/bs/form_fields.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/bs/form_fields.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/bs/horizontal_form_fields.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/bs/horizontal_form_fields.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_accept_cookies_message.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_accept_cookies_message.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_article_publication.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_article_publication.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_coop_bar_js.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_coop_bar_js.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_csrf_failure_message.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_csrf_failure_message.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_facebook_like.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_facebook_like.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_js_includes.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_js_includes.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_messages.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_messages.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_newsletter_categories.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_newsletter_categories.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_pagination.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_pagination.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_pagination_js.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_pagination_js.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/_social_share.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/_social_share.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/categories/only-for-unit-testing.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/categories/only-for-unit-testing.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/medialib/slide_base.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/medialib/slide_base.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/medialib/slide_images_content.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/medialib/slide_images_content.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/medialib/slide_photologue_content.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/medialib/slide_photologue_content.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/navigation_node.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/navigation_node.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/navtree_content/default.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/navtree_content/default.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/newsletter.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/newsletter.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/newsletter_base.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/newsletter_base.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_add_fragment.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_add_fragment.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_edit_fragments.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_edit_fragments.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/popup_publish_article.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/popup_publish_article.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/coop_cms/view_all_articles.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/coop_cms/view_all_articles.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_fragments_extra_id.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_fragments_extra_id.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/test/article_with_fragments_template.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/test/article_with_fragments_template.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/test/base.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/test/base.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/test/carousel.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/test/carousel.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/test/navigation_li_node.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/test/navigation_li_node.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templates/test/navigation_node.html` & `apidev-coop_cms-1.6.2/coop_cms/templates/test/navigation_node.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templatetags/article_tags.py` & `apidev-coop_cms-1.6.2/coop_cms/templatetags/article_tags.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templatetags/coop_edition.py` & `apidev-coop_cms-1.6.2/coop_cms/templatetags/coop_edition.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templatetags/coop_navigation.py` & `apidev-coop_cms-1.6.2/coop_cms/templatetags/coop_navigation.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/templatetags/coop_utils.py` & `apidev-coop_cms-1.6.2/coop_cms/templatetags/coop_utils.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/__init__.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,14 @@
             self.editor.is_active = True
             self.editor.save()
 
             self.editor.user_permissions.add(self.can_edit_newsletter_permission())
 
             ct = ContentType.objects.get_for_model(get_article_class())
             codename = 'change_{0}'.format(ct.model)
-            print('#', ct, codename)
             can_edit_article = Permission.objects.get(content_type__app_label=ct.app_label, codename=codename)
             self.editor.user_permissions.add(can_edit_article)
 
             if can_add:
                 codename = 'add_{0}'.format(ct.model)
                 can_add_article = Permission.objects.get(content_type__app_label=ct.app_label, codename=codename)
                 self.editor.user_permissions.add(can_add_article)
```

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_admin.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_alias.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_articles.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_articles.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_cache.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_categories.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_edition.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_edition.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_fragments.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_fragments.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_generic_views.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_generic_views.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_homepage.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_homepage.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_link.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_localization.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_localization.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_media.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_middleware.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_multisites.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_multisites.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_navigation.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_newsletter.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_newsletter.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_permissions.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_settings.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_sitemap.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_slugs.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_slugs.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_special_pages.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_special_pages.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_templates.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_templatetags.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/tests/test_utils.py` & `apidev-coop_cms-1.6.2/coop_cms/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/thumbnail_backend.py` & `apidev-coop_cms-1.6.2/coop_cms/thumbnail_backend.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/translation.py` & `apidev-coop_cms-1.6.2/coop_cms/translation.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/urls.py` & `apidev-coop_cms-1.6.2/coop_cms/urls.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/utils/__init__.py` & `apidev-coop_cms-1.6.2/coop_cms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/utils/emails.py` & `apidev-coop_cms-1.6.2/coop_cms/utils/emails.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/utils/i18n.py` & `apidev-coop_cms-1.6.2/coop_cms/utils/i18n.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/utils/loaders.py` & `apidev-coop_cms-1.6.2/coop_cms/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/utils/pagination.py` & `apidev-coop_cms-1.6.2/coop_cms/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/utils/requests.py` & `apidev-coop_cms-1.6.2/coop_cms/utils/requests.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/utils/text.py` & `apidev-coop_cms-1.6.2/coop_cms/utils/text.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/utils/xsendfile.py` & `apidev-coop_cms-1.6.2/coop_cms/utils/xsendfile.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/views/articles.py` & `apidev-coop_cms-1.6.2/coop_cms/views/articles.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/views/fragments.py` & `apidev-coop_cms-1.6.2/coop_cms/views/fragments.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/views/homepage.py` & `apidev-coop_cms-1.6.2/coop_cms/views/homepage.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/views/links.py` & `apidev-coop_cms-1.6.2/coop_cms/views/links.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/views/medialib.py` & `apidev-coop_cms-1.6.2/coop_cms/views/medialib.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/views/navigation.py` & `apidev-coop_cms-1.6.2/coop_cms/views/navigation.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/views/newsletters.py` & `apidev-coop_cms-1.6.2/coop_cms/views/newsletters.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/views/webutils.py` & `apidev-coop_cms-1.6.2/coop_cms/views/webutils.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/coop_cms/widgets.py` & `apidev-coop_cms-1.6.2/coop_cms/widgets.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_cms-1.6.1/setup.py` & `apidev-coop_cms-1.6.2/setup.py`

 * *Files identical despite different names*

