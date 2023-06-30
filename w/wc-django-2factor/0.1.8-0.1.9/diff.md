# Comparing `tmp/wc-django-2factor-0.1.8.tar.gz` & `tmp/wc-django-2factor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-2factor-0.1.8.tar", last modified: Wed Jul 20 05:47:41 2022, max compression
+gzip compressed data, was "wc-django-2factor-0.1.9.tar", last modified: Fri Jun 30 07:53:34 2023, max compression
```

## Comparing `wc-django-2factor-0.1.8.tar` & `wc-django-2factor-0.1.9.tar`

### file list

```diff
@@ -1,335 +1,445 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.302380 wc-django-2factor-0.1.8/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      660 2022-06-21 09:08:36.000000 wc-django-2factor-0.1.8/CHANGELOG.md
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1072 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/LICENSE
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      153 2022-05-06 14:15:00.000000 wc-django-2factor-0.1.8/MANIFEST.in
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1250 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5378 2022-07-20 05:47:41.302380 wc-django-2factor-0.1.8/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4111 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/README.md
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       79 2022-07-20 05:47:41.302380 wc-django-2factor-0.1.8/setup.cfg
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1596 2022-07-20 05:44:45.000000 wc-django-2factor-0.1.8/setup.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      556 2022-07-12 15:13:12.000000 wc-django-2factor-0.1.8/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.186354 wc-django-2factor-0.1.8/wc_django_2factor.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5378 2022-07-20 05:47:40.000000 wc-django-2factor-0.1.8/wc_django_2factor.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5337 2022-07-20 05:47:40.000000 wc-django-2factor-0.1.8/wc_django_2factor.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2022-07-20 05:47:40.000000 wc-django-2factor-0.1.8/wc_django_2factor.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      153 2022-07-20 05:47:40.000000 wc-django-2factor-0.1.8/wc_django_2factor.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2022-07-20 05:47:40.000000 wc-django-2factor-0.1.8/wc_django_2factor.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.202358 wc-django-2factor-0.1.8/wcd_2factor/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      120 2022-07-20 05:47:07.000000 wc-django-2factor-0.1.8/wcd_2factor/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      398 2022-05-18 09:34:27.000000 wc-django-2factor-0.1.8/wcd_2factor/admin.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      323 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1594 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/conf.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.202358 wc-django-2factor-0.1.8/wcd_2factor/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.202358 wc-django-2factor-0.1.8/wcd_2factor/contrib/drf/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/contrib/drf/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1766 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/contrib/drf/serializers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1659 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/contrib/drf/views.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.202358 wc-django-2factor-0.1.8/wcd_2factor/contrib/graphene/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/contrib/graphene/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1747 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/contrib/graphene/mutations.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.202358 wc-django-2factor-0.1.8/wcd_2factor/contrib/wcd_jwt/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/contrib/wcd_jwt/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      797 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/contrib/wcd_jwt/serializers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       57 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/discovery.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      400 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.142344 wc-django-2factor-0.1.8/wcd_2factor/locale/af/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.202358 wc-django-2factor-0.1.8/wcd_2factor/locale/af/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/af/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.146345 wc-django-2factor-0.1.8/wcd_2factor/locale/ar/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.210359 wc-django-2factor-0.1.8/wcd_2factor/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ar/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.142344 wc-django-2factor-0.1.8/wcd_2factor/locale/ar-dz/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.202358 wc-django-2factor-0.1.8/wcd_2factor/locale/ar-dz/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ar-dz/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.146345 wc-django-2factor-0.1.8/wcd_2factor/locale/ast/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.210359 wc-django-2factor-0.1.8/wcd_2factor/locale/ast/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ast/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.146345 wc-django-2factor-0.1.8/wcd_2factor/locale/az/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.210359 wc-django-2factor-0.1.8/wcd_2factor/locale/az/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/az/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/be/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.214360 wc-django-2factor-0.1.8/wcd_2factor/locale/be/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/be/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/bg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.218361 wc-django-2factor-0.1.8/wcd_2factor/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/bg/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/bn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.218361 wc-django-2factor-0.1.8/wcd_2factor/locale/bn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/bn/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/br/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.218361 wc-django-2factor-0.1.8/wcd_2factor/locale/br/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/br/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/bs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.218361 wc-django-2factor-0.1.8/wcd_2factor/locale/bs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/bs/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/ca/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.218361 wc-django-2factor-0.1.8/wcd_2factor/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ca/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/cs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.222362 wc-django-2factor-0.1.8/wcd_2factor/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/cs/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/cy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.230364 wc-django-2factor-0.1.8/wcd_2factor/locale/cy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/cy/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/da/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.230364 wc-django-2factor-0.1.8/wcd_2factor/locale/da/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/da/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.150346 wc-django-2factor-0.1.8/wcd_2factor/locale/de/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.230364 wc-django-2factor-0.1.8/wcd_2factor/locale/de/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/de/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.154347 wc-django-2factor-0.1.8/wcd_2factor/locale/dsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.230364 wc-django-2factor-0.1.8/wcd_2factor/locale/dsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/dsb/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.154347 wc-django-2factor-0.1.8/wcd_2factor/locale/el/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.230364 wc-django-2factor-0.1.8/wcd_2factor/locale/el/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/el/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.154347 wc-django-2factor-0.1.8/wcd_2factor/locale/en/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.234365 wc-django-2factor-0.1.8/wcd_2factor/locale/en/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      400 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/en/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.154347 wc-django-2factor-0.1.8/wcd_2factor/locale/en-au/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.230364 wc-django-2factor-0.1.8/wcd_2factor/locale/en-au/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/en-au/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.154347 wc-django-2factor-0.1.8/wcd_2factor/locale/en-gb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.230364 wc-django-2factor-0.1.8/wcd_2factor/locale/en-gb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/en-gb/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.158348 wc-django-2factor-0.1.8/wcd_2factor/locale/eo/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.234365 wc-django-2factor-0.1.8/wcd_2factor/locale/eo/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/eo/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.158348 wc-django-2factor-0.1.8/wcd_2factor/locale/es/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.238366 wc-django-2factor-0.1.8/wcd_2factor/locale/es/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/es/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.158348 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ar/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.234365 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ar/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ar/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.158348 wc-django-2factor-0.1.8/wcd_2factor/locale/es-co/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.234365 wc-django-2factor-0.1.8/wcd_2factor/locale/es-co/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/es-co/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.158348 wc-django-2factor-0.1.8/wcd_2factor/locale/es-mx/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.234365 wc-django-2factor-0.1.8/wcd_2factor/locale/es-mx/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/es-mx/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.158348 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ni/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.234365 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ni/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ni/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.158348 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ve/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.238366 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ve/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/es-ve/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.158348 wc-django-2factor-0.1.8/wcd_2factor/locale/et/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.238366 wc-django-2factor-0.1.8/wcd_2factor/locale/et/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/et/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.162349 wc-django-2factor-0.1.8/wcd_2factor/locale/eu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.238366 wc-django-2factor-0.1.8/wcd_2factor/locale/eu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/eu/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.162349 wc-django-2factor-0.1.8/wcd_2factor/locale/fa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.238366 wc-django-2factor-0.1.8/wcd_2factor/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/fa/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.162349 wc-django-2factor-0.1.8/wcd_2factor/locale/fi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.238366 wc-django-2factor-0.1.8/wcd_2factor/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/fi/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.162349 wc-django-2factor-0.1.8/wcd_2factor/locale/fr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.238366 wc-django-2factor-0.1.8/wcd_2factor/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/fr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.162349 wc-django-2factor-0.1.8/wcd_2factor/locale/fy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.246368 wc-django-2factor-0.1.8/wcd_2factor/locale/fy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/fy/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/ga/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.246368 wc-django-2factor-0.1.8/wcd_2factor/locale/ga/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ga/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/gd/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.246368 wc-django-2factor-0.1.8/wcd_2factor/locale/gd/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/gd/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/gl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.246368 wc-django-2factor-0.1.8/wcd_2factor/locale/gl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/gl/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/he/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.246368 wc-django-2factor-0.1.8/wcd_2factor/locale/he/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/he/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/hi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.246368 wc-django-2factor-0.1.8/wcd_2factor/locale/hi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/hi/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/hr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/hr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/hsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/hsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/hsb/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/hu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/hu/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/hy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/hy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/hy/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/ia/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/ia/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ia/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.166350 wc-django-2factor-0.1.8/wcd_2factor/locale/id/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/id/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/id/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/ig/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/ig/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ig/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/io/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/io/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/io/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/is/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/is/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/is/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/it/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/it/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/it/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/ja/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ja/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/ka/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/ka/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ka/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/kab/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.250368 wc-django-2factor-0.1.8/wcd_2factor/locale/kab/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/kab/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/kk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.254369 wc-django-2factor-0.1.8/wcd_2factor/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/kk/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/km/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.254369 wc-django-2factor-0.1.8/wcd_2factor/locale/km/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/km/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/kn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.254369 wc-django-2factor-0.1.8/wcd_2factor/locale/kn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/kn/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/ko/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.254369 wc-django-2factor-0.1.8/wcd_2factor/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ko/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/ky/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.262371 wc-django-2factor-0.1.8/wcd_2factor/locale/ky/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ky/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/lb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.262371 wc-django-2factor-0.1.8/wcd_2factor/locale/lb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/lb/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/lt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.262371 wc-django-2factor-0.1.8/wcd_2factor/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/lt/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/lv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.262371 wc-django-2factor-0.1.8/wcd_2factor/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/lv/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/mk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.262371 wc-django-2factor-0.1.8/wcd_2factor/locale/mk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/mk/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/ml/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.266372 wc-django-2factor-0.1.8/wcd_2factor/locale/ml/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ml/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/mn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.270373 wc-django-2factor-0.1.8/wcd_2factor/locale/mn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/mn/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/mr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.270373 wc-django-2factor-0.1.8/wcd_2factor/locale/mr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/mr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.170350 wc-django-2factor-0.1.8/wcd_2factor/locale/ms/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.274374 wc-django-2factor-0.1.8/wcd_2factor/locale/ms/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ms/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.174351 wc-django-2factor-0.1.8/wcd_2factor/locale/my/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.274374 wc-django-2factor-0.1.8/wcd_2factor/locale/my/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/my/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.174351 wc-django-2factor-0.1.8/wcd_2factor/locale/nb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.274374 wc-django-2factor-0.1.8/wcd_2factor/locale/nb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/nb/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.174351 wc-django-2factor-0.1.8/wcd_2factor/locale/ne/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.274374 wc-django-2factor-0.1.8/wcd_2factor/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ne/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.174351 wc-django-2factor-0.1.8/wcd_2factor/locale/nl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.278375 wc-django-2factor-0.1.8/wcd_2factor/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/nl/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.174351 wc-django-2factor-0.1.8/wcd_2factor/locale/nn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.278375 wc-django-2factor-0.1.8/wcd_2factor/locale/nn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/nn/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/os/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.282376 wc-django-2factor-0.1.8/wcd_2factor/locale/os/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/os/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/pa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.282376 wc-django-2factor-0.1.8/wcd_2factor/locale/pa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/pa/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/pt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.282376 wc-django-2factor-0.1.8/wcd_2factor/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/pt/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/pt-br/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.282376 wc-django-2factor-0.1.8/wcd_2factor/locale/pt-br/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/pt-br/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/ro/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.282376 wc-django-2factor-0.1.8/wcd_2factor/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ro/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/sk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.282376 wc-django-2factor-0.1.8/wcd_2factor/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/sk/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/sl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.282376 wc-django-2factor-0.1.8/wcd_2factor/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/sl/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/sq/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.282376 wc-django-2factor-0.1.8/wcd_2factor/locale/sq/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/sq/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/sr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.286377 wc-django-2factor-0.1.8/wcd_2factor/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/sr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/sr-latn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.286377 wc-django-2factor-0.1.8/wcd_2factor/locale/sr-latn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/sr-latn/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/sv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.286377 wc-django-2factor-0.1.8/wcd_2factor/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/sv/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.178352 wc-django-2factor-0.1.8/wcd_2factor/locale/sw/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.286377 wc-django-2factor-0.1.8/wcd_2factor/locale/sw/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/sw/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/ta/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.294378 wc-django-2factor-0.1.8/wcd_2factor/locale/ta/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ta/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/te/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.294378 wc-django-2factor-0.1.8/wcd_2factor/locale/te/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/te/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/tg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.294378 wc-django-2factor-0.1.8/wcd_2factor/locale/tg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/tg/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/th/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.294378 wc-django-2factor-0.1.8/wcd_2factor/locale/th/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/th/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/tk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.294378 wc-django-2factor-0.1.8/wcd_2factor/locale/tk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/tk/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/tr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.298379 wc-django-2factor-0.1.8/wcd_2factor/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/tr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/tt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.298379 wc-django-2factor-0.1.8/wcd_2factor/locale/tt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/tt/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/udm/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.298379 wc-django-2factor-0.1.8/wcd_2factor/locale/udm/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/udm/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/ur/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.298379 wc-django-2factor-0.1.8/wcd_2factor/locale/ur/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/ur/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/uz/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.298379 wc-django-2factor-0.1.8/wcd_2factor/locale/uz/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/uz/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/vi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.298379 wc-django-2factor-0.1.8/wcd_2factor/locale/vi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/vi/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/zh-hans/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.298379 wc-django-2factor-0.1.8/wcd_2factor/locale/zh-hans/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/zh-hans/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.182353 wc-django-2factor-0.1.8/wcd_2factor/locale/zh-hant/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.298379 wc-django-2factor-0.1.8/wcd_2factor/locale/zh-hant/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/locale/zh-hant/LC_MESSAGES/django.mo
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.302380 wc-django-2factor-0.1.8/wcd_2factor/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      957 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      725 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/migrations/0002_auto_20220406_1436.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/migrations/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1892 2022-06-21 09:08:36.000000 wc-django-2factor-0.1.8/wcd_2factor/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      131 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/query.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.302380 wc-django-2factor-0.1.8/wcd_2factor/sender/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/sender/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1661 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/sender/backend.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      233 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/sender/config.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      494 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/sender/resolver.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-20 05:47:41.302380 wc-django-2factor-0.1.8/wcd_2factor/services/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1362 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/services/confirmer.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      595 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/services/sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      206 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/signals.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      167 2022-04-19 13:41:05.000000 wc-django-2factor-0.1.8/wcd_2factor/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      660 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/CHANGELOG.md
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1072 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/LICENSE
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      153 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/MANIFEST.in
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1250 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5339 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/PKG-INFO
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     4111 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/README.md
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       79 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/setup.cfg
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1596 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/setup.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      556 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wc_django_2factor.egg-info/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     5339 2023-06-30 07:53:34.000000 wc-django-2factor-0.1.9/wc_django_2factor.egg-info/PKG-INFO
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     9878 2023-06-30 07:53:34.000000 wc-django-2factor-0.1.9/wc_django_2factor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        1 2023-06-30 07:53:34.000000 wc-django-2factor-0.1.9/wc_django_2factor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      153 2023-06-30 07:53:34.000000 wc-django-2factor-0.1.9/wc_django_2factor.egg-info/requires.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       12 2023-06-30 07:53:34.000000 wc-django-2factor-0.1.9/wc_django_2factor.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      120 2023-06-30 07:33:34.000000 wc-django-2factor-0.1.9/wcd_2factor/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      448 2023-06-30 07:32:26.000000 wc-django-2factor-0.1.9/wcd_2factor/admin.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      323 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/apps.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1594 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/conf.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/contrib/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/contrib/drf/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/contrib/drf/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1766 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/contrib/drf/serializers.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1659 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/contrib/drf/views.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/contrib/graphene/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/contrib/graphene/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1747 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/contrib/graphene/mutations.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/contrib/wcd_jwt/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/contrib/wcd_jwt/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      797 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/contrib/wcd_jwt/serializers.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       57 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/discovery.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      400 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/locale/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/af/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/locale/af/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/af/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/af/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/ar/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/locale/ar/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      463 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2115 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/ar-dz/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/locale/ar-dz/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ar-dz/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ar-dz/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/ast/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/ast/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ast/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ast/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/az/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/az/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/az/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/az/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/be/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/be/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      518 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/be/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2173 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/be/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/bg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/bg/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/bg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/bn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/bn/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/bn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/bn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/br/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/br/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      671 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/br/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2332 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/br/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/bs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/bs/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      454 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/bs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2106 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/bs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/ca/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/ca/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/cs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/cs/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      460 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2112 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/cy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/cy/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      425 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/cy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2077 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/cy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/da/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/da/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/de/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/de/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/dsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/dsb/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      432 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/dsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2084 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/dsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/el/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/el/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/el/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/en/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/en/LC_MESSAGES/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      400 2022-12-23 11:01:26.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/en-au/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/en-au/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/en-au/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/en-au/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.204860 wc-django-2factor-0.1.9/wcd_2factor/locale/en-gb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/en-gb/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/en-gb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/en-gb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/eo/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/eo/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/eo/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/eo/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/es/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/es/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ar/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ar/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/es-co/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/es-co/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-co/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-co/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/es-mx/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/es-mx/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-mx/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-mx/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ni/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.220859 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ni/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ni/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ni/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ve/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ve/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ve/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/es-ve/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/et/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/et/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/et/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/eu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/eu/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/eu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/eu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/fa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/fa/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      379 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2028 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/fi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/fi/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/fr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/fr/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      379 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2028 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/fy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/fy/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/fy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/fy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/ga/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/ga/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      418 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ga/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2070 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ga/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/gd/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/gd/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      441 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/gd/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2093 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/gd/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/gl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/gl/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/gl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/gl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/he/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/he/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      474 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/he/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2126 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/he/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/hi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/hi/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/hr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/hr/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      452 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2104 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/hsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/hsb/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      432 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2084 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/hu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/hu/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/hy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/hy/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/hy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/ia/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/ia/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ia/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ia/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/id/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/id/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/ig/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/ig/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ig/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ig/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/io/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/io/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/io/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/io/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/is/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.224859 wc-django-2factor-0.1.9/wcd_2factor/locale/is/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      402 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/is/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2051 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/is/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/it/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/it/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/ja/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/ja/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/ka/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/ka/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      378 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ka/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2027 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ka/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/kab/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/kab/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/kab/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/kab/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/kk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/kk/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/km/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/km/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/km/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/km/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/kn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/kn/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/kn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/kn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/ko/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/ko/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/ky/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/ky/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ky/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ky/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/lb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/lb/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/lb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/lb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/lt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/lt/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      511 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2166 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/lv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/lv/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      415 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/lv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2067 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/lv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/mk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/mk/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      410 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/mk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2059 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/mk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.208860 wc-django-2factor-0.1.9/wcd_2factor/locale/ml/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/ml/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ml/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ml/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/mn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/mn/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/mn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/mn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/mr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/mr/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/mr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/mr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/ms/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/ms/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ms/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ms/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/my/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/my/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/my/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/my/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/nb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/nb/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/nb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/ne/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/ne/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ne/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ne/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/nl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/nl/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/nn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/nn/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/nn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/nn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/os/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/os/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/os/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/os/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/pa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.228859 wc-django-2factor-0.1.9/wcd_2factor/locale/pa/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/pa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/pa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/pl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2181 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/pt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/pt/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/pt-br/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/pt-br/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/pt-br/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/pt-br/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/ro/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/ro/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      421 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ro/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2073 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ro/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/ru/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2173 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/ru_RU/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/ru_RU/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2023-02-07 14:27:16.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2388 2023-02-07 14:22:08.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ru_RU/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/sk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/sk/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      455 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2107 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/sl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/sl/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      432 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2084 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/sq/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/sq/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sq/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sq/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/sr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/sr/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      454 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2106 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/sr-latn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/sr-latn/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sr-latn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sr-latn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/sv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/sv/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/sw/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/sw/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sw/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/sw/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/ta/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/ta/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ta/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ta/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/te/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/te/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/te/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/te/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/tg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/tg/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/tg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/tg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/th/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/th/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/th/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/th/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/tk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/tk/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/tk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/tk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/tr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/tr/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      379 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2028 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/tt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/tt/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/tt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/tt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/udm/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/udm/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/udm/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/udm/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/uk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2260 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/ur/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.232859 wc-django-2factor-0.1.9/wcd_2factor/locale/ur/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      380 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ur/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/ur/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.212859 wc-django-2factor-0.1.9/wcd_2factor/locale/uz/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/wcd_2factor/locale/uz/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/uz/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/uz/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/locale/vi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/wcd_2factor/locale/vi/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      373 2022-12-22 15:27:03.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/vi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2022 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/vi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/locale/zh-hans/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/wcd_2factor/locale/zh-hans/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/zh-hans/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/zh-hans/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.216859 wc-django-2factor-0.1.9/wcd_2factor/locale/zh-hant/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/wcd_2factor/locale/zh-hant/LC_MESSAGES/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      337 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/zh-hant/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1983 2022-12-22 15:27:02.000000 wc-django-2factor-0.1.9/wcd_2factor/locale/zh-hant/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/wcd_2factor/migrations/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      957 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/migrations/0001_initial.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      725 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/migrations/0002_auto_20220406_1436.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/migrations/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1892 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/models.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      131 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/query.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/wcd_2factor/sender/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       69 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/sender/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1661 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/sender/backend.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      233 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/sender/config.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      494 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/sender/resolver.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-30 07:53:34.236859 wc-django-2factor-0.1.9/wcd_2factor/services/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/services/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1362 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/services/confirmer.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      595 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/services/sender.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      206 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/signals.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      167 2022-09-20 08:50:23.000000 wc-django-2factor-0.1.9/wcd_2factor/utils.py
```

### Comparing `wc-django-2factor-0.1.8/CHANGELOG.md` & `wc-django-2factor-0.1.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/LICENSE` & `wc-django-2factor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/Makefile` & `wc-django-2factor-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/PKG-INFO` & `wc-django-2factor-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: wc-django-2factor
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package to create general API for 2factor checkers.
-Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -207,9 +205,7 @@
 
 ## [0.1.1]
 ### Added
 - `DEBUG_CODE_RESPONSE` setting. It adds generated 'code' field to a request confirmation response for easier debug.
 
 ## [0.1.0]
 Initial version.
-
-
```

### Comparing `wc-django-2factor-0.1.8/README.md` & `wc-django-2factor-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/setup.py` & `wc-django-2factor-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/tox.ini` & `wc-django-2factor-0.1.9/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wc_django_2factor.egg-info/PKG-INFO` & `wc-django-2factor-0.1.9/wc_django_2factor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: wc-django-2factor
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package to create general API for 2factor checkers.
-Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -207,9 +205,7 @@
 
 ## [0.1.1]
 ### Added
 - `DEBUG_CODE_RESPONSE` setting. It adds generated 'code' field to a request confirmation response for easier debug.
 
 ## [0.1.0]
 Initial version.
-
-
```

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/conf.py` & `wc-django-2factor-0.1.9/wcd_2factor/conf.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/contrib/drf/serializers.py` & `wc-django-2factor-0.1.9/wcd_2factor/contrib/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/contrib/drf/views.py` & `wc-django-2factor-0.1.9/wcd_2factor/contrib/drf/views.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/contrib/graphene/mutations.py` & `wc-django-2factor-0.1.9/wcd_2factor/contrib/graphene/mutations.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/contrib/wcd_jwt/serializers.py` & `wc-django-2factor-0.1.9/wcd_2factor/contrib/wcd_jwt/serializers.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/locale/be/LC_MESSAGES/django.mo` & `wc-django-2factor-0.1.9/wcd_2factor/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/locale/br/LC_MESSAGES/django.mo` & `wc-django-2factor-0.1.9/wcd_2factor/locale/br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/migrations/0001_initial.py` & `wc-django-2factor-0.1.9/wcd_2factor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/migrations/0002_auto_20220406_1436.py` & `wc-django-2factor-0.1.9/wcd_2factor/migrations/0002_auto_20220406_1436.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/models.py` & `wc-django-2factor-0.1.9/wcd_2factor/models.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/sender/backend.py` & `wc-django-2factor-0.1.9/wcd_2factor/sender/backend.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/services/confirmer.py` & `wc-django-2factor-0.1.9/wcd_2factor/services/confirmer.py`

 * *Files identical despite different names*

### Comparing `wc-django-2factor-0.1.8/wcd_2factor/services/sender.py` & `wc-django-2factor-0.1.9/wcd_2factor/services/sender.py`

 * *Files identical despite different names*

