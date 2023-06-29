# Comparing `tmp/wafer-0.9.3.tar.gz` & `tmp/wafer-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wafer-0.9.3.tar", last modified: Sat Sep 19 17:31:07 2020, max compression
+gzip compressed data, was "dist/wafer-0.9.4.tar", last modified: Sat Sep 19 19:00:16 2020, max compression
```

## Comparing `wafer-0.9.3.tar` & `wafer-0.9.4.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/
--rw-r-----   0 neil      (1000) neil      (1000)      420 2018-10-14 08:22:43.000000 wafer-0.9.3/.gitignore
--rw-r-----   0 neil      (1000) neil      (1000)     2006 2020-04-18 11:20:50.000000 wafer-0.9.3/.travis.yml
--rw-r-----   0 neil      (1000) neil      (1000)      776 2020-03-20 20:20:38.000000 wafer-0.9.3/LICENSE
--rw-r-----   0 neil      (1000) neil      (1000)     4986 2020-09-19 17:31:07.000000 wafer-0.9.3/PKG-INFO
--rw-r-----   0 neil      (1000) neil      (1000)     3213 2020-04-18 11:20:50.000000 wafer-0.9.3/README.rst
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/docs/
--rw-r-----   0 neil      (1000) neil      (1000)     5559 2020-04-13 10:30:47.000000 wafer-0.9.3/docs/Makefile
--rw-r-----   0 neil      (1000) neil      (1000)     7758 2020-09-19 17:30:16.000000 wafer-0.9.3/docs/conf.py
--rw-r-----   0 neil      (1000) neil      (1000)      287 2018-05-03 14:13:58.000000 wafer-0.9.3/docs/index.rst
--rw-r-----   0 neil      (1000) neil      (1000)     2313 2020-04-18 11:20:50.000000 wafer-0.9.3/docs/install.rst
--rw-r-----   0 neil      (1000) neil      (1000)     5103 2014-10-15 15:48:24.000000 wafer-0.9.3/docs/make.bat
--rw-r-----   0 neil      (1000) neil      (1000)     3118 2018-05-03 14:14:11.000000 wafer-0.9.3/docs/menus.rst
--rw-r-----   0 neil      (1000) neil      (1000)     2683 2019-12-04 11:38:56.000000 wafer-0.9.3/docs/pages.rst
--rw-r-----   0 neil      (1000) neil      (1000)     4172 2020-04-18 11:20:50.000000 wafer-0.9.3/docs/schedule.rst
--rw-r-----   0 neil      (1000) neil      (1000)     5283 2020-06-04 14:42:52.000000 wafer-0.9.3/docs/settings.rst
--rw-r-----   0 neil      (1000) neil      (1000)     1162 2018-10-14 08:22:43.000000 wafer-0.9.3/docs/sponsors.rst
--rw-r-----   0 neil      (1000) neil      (1000)      737 2018-10-14 08:22:43.000000 wafer-0.9.3/docs/static.rst
--rw-r-----   0 neil      (1000) neil      (1000)     5920 2018-05-03 14:14:11.000000 wafer-0.9.3/docs/talks.rst
--rwxr-x---   0 neil      (1000) neil      (1000)      136 2013-07-29 09:20:38.000000 wafer-0.9.3/install_requirements
--rwxr-x---   0 neil      (1000) neil      (1000)      248 2014-09-03 11:56:53.000000 wafer-0.9.3/manage.py
--rw-r-----   0 neil      (1000) neil      (1000)      315 2018-05-03 14:13:58.000000 wafer-0.9.3/package.json
--rw-r-----   0 neil      (1000) neil      (1000)       35 2018-05-03 14:13:58.000000 wafer-0.9.3/requirements-dev.txt
--rw-r-----   0 neil      (1000) neil      (1000)       56 2014-10-04 12:13:30.000000 wafer-0.9.3/requirements.txt
--rw-r-----   0 neil      (1000) neil      (1000)       67 2020-09-19 17:31:07.000000 wafer-0.9.3/setup.cfg
--rw-r-----   0 neil      (1000) neil      (1000)     2130 2020-09-19 17:30:16.000000 wafer-0.9.3/setup.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/utils/
--rwxr-x---   0 neil      (1000) neil      (1000)      722 2014-10-15 15:48:59.000000 wafer-0.9.3/utils/bump-version.sh
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/
--rw-r-----   0 neil      (1000) neil      (1000)       93 2020-09-19 17:30:16.000000 wafer-0.9.3/wafer/__init__.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/compare/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2016-08-17 12:10:46.000000 wafer-0.9.3/wafer/compare/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     7193 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/compare/admin.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/compare/templates/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/compare/templates/admin/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/compare/templates/admin/wafer.compare/
--rw-r-----   0 neil      (1000) neil      (1000)      591 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/compare/templates/admin/wafer.compare/change_form.html
--rw-r-----   0 neil      (1000) neil      (1000)      585 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/compare/templates/admin/wafer.compare/compare.html
--rw-r-----   0 neil      (1000) neil      (1000)     2206 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/compare/templates/admin/wafer.compare/compare_list.html
--rw-r-----   0 neil      (1000) neil      (1000)     1287 2019-10-15 10:30:54.000000 wafer-0.9.3/wafer/context_processors.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/kv/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2016-08-17 12:10:46.000000 wafer-0.9.3/wafer/kv/__init__.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/kv/migrations/
--rw-r-----   0 neil      (1000) neil      (1000)      827 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/kv/migrations/0001_initial.py
--rw-r-----   0 neil      (1000) neil      (1000)        0 2016-08-17 12:10:46.000000 wafer-0.9.3/wafer/kv/migrations/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      381 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/kv/models.py
--rw-r-----   0 neil      (1000) neil      (1000)     1009 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/kv/permissions.py
--rw-r-----   0 neil      (1000) neil      (1000)     1312 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/kv/serializers.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/kv/tests/
--rw-r-----   0 neil      (1000) neil      (1000)     9649 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/kv/tests/test_kv_api.py
--rw-r-----   0 neil      (1000) neil      (1000)      256 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/kv/urls.py
--rw-r-----   0 neil      (1000) neil      (1000)      537 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/kv/utils.py
--rw-r-----   0 neil      (1000) neil      (1000)      879 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/kv/views.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/locale/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/locale/pt_BR/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/locale/pt_BR/LC_MESSAGES/
--rw-r-----   0 neil      (1000) neil      (1000)    27050 2020-09-16 17:15:44.000000 wafer-0.9.3/wafer/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r-----   0 neil      (1000) neil      (1000)    42066 2020-07-12 12:40:38.000000 wafer-0.9.3/wafer/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/locale/ru/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/locale/ru/LC_MESSAGES/
--rw-r-----   0 neil      (1000) neil      (1000)     7142 2020-09-16 17:15:44.000000 wafer-0.9.3/wafer/locale/ru/LC_MESSAGES/django.mo
--rw-r-----   0 neil      (1000) neil      (1000)    17371 2019-10-15 10:30:54.000000 wafer-0.9.3/wafer/locale/ru/LC_MESSAGES/django.po
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/management/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2013-10-06 13:47:00.000000 wafer-0.9.3/wafer/management/__init__.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/management/commands/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2013-03-09 09:13:17.000000 wafer-0.9.3/wafer/management/commands/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     2175 2020-07-27 09:12:38.000000 wafer-0.9.3/wafer/management/commands/wafer_add_default_groups.py
--rw-r-----   0 neil      (1000) neil      (1000)     3107 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/management/commands/wafer_emails.py
--rw-r-----   0 neil      (1000) neil      (1000)     1798 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/management/commands/wafer_registered_attendees.py
--rw-r-----   0 neil      (1000) neil      (1000)     1492 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/management/commands/wafer_speaker_contact_details.py
--rw-r-----   0 neil      (1000) neil      (1000)     1984 2018-05-03 14:13:35.000000 wafer-0.9.3/wafer/management/commands/wafer_speaker_tickets.py
--rw-r-----   0 neil      (1000) neil      (1000)      502 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/management/commands/wafer_stats.py
--rw-r-----   0 neil      (1000) neil      (1000)     4806 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/menu.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/pages/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2013-07-29 09:48:59.000000 wafer-0.9.3/wafer/pages/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      551 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/pages/admin.py
--rw-r-----   0 neil      (1000) neil      (1000)      606 2019-04-09 14:40:44.000000 wafer-0.9.3/wafer/pages/forms.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/pages/management/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/pages/management/__init__.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/pages/management/commands/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/pages/management/commands/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     2338 2019-11-08 09:50:20.000000 wafer-0.9.3/wafer/pages/management/commands/load_pages.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/pages/management/tests/
--rw-r-----   0 neil      (1000) neil      (1000)     1395 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/pages/management/tests/test_load_pages.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/pages/migrations/
--rw-r-----   0 neil      (1000) neil      (1000)     1985 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/pages/migrations/0001_initial.py
--rw-r-----   0 neil      (1000) neil      (1000)      693 2015-11-20 18:19:02.000000 wafer-0.9.3/wafer/pages/migrations/0002_page_people.py
--rw-r-----   0 neil      (1000) neil      (1000)      853 2016-08-17 12:10:46.000000 wafer-0.9.3/wafer/pages/migrations/0003_non-null_people+files.py
--rw-r-----   0 neil      (1000) neil      (1000)      403 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/pages/migrations/0004_allow_blank_files_description.py
--rw-r-----   0 neil      (1000) neil      (1000)      650 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/pages/migrations/0005_page_cache_time.py
--rw-r-----   0 neil      (1000) neil      (1000)      567 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/pages/migrations/0006_menu_order.py
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.3/wafer/pages/migrations/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     6401 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/pages/models.py
--rw-r-----   0 neil      (1000) neil      (1000)     1072 2016-08-17 12:10:46.000000 wafer-0.9.3/wafer/pages/serializers.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/pages/templates/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/pages/templates/wafer.pages/
--rw-r-----   0 neil      (1000) neil      (1000)      569 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/pages/templates/wafer.pages/page.html
--rw-r-----   0 neil      (1000) neil      (1000)     1352 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/pages/templates/wafer.pages/page_compare.html
--rw-r-----   0 neil      (1000) neil      (1000)      397 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/pages/templates/wafer.pages/page_form.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/pages/tests/
--rw-r-----   0 neil      (1000) neil      (1000)     1083 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/pages/tests/test_menu.py
--rw-r-----   0 neil      (1000) neil      (1000)     5350 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/pages/tests/test_pages.py
--rw-r-----   0 neil      (1000) neil      (1000)      614 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/pages/tests/test_views.py
--rw-r-----   0 neil      (1000) neil      (1000)      524 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/pages/urls.py
--rw-r-----   0 neil      (1000) neil      (1000)     4224 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/pages/views.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/registration/
--rw-r-----   0 neil      (1000) neil      (1000)       66 2014-10-04 08:49:07.000000 wafer-0.9.3/wafer/registration/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      196 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/registration/apps.py
--rw-r-----   0 neil      (1000) neil      (1000)      844 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/registration/forms.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/registration/migrations/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-10-04 08:49:07.000000 wafer-0.9.3/wafer/registration/migrations/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     6586 2020-06-04 14:42:52.000000 wafer-0.9.3/wafer/registration/sso.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/registration/templates/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/registration/templates/registration/
--rw-r-----   0 neil      (1000) neil      (1000)      481 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/registration/templates/registration/activate.html
--rw-r-----   0 neil      (1000) neil      (1000)      553 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/registration/templates/registration/activation_complete.html
--rw-r-----   0 neil      (1000) neil      (1000)      642 2020-01-30 07:30:18.000000 wafer-0.9.3/wafer/registration/templates/registration/activation_email.txt
--rw-r-----   0 neil      (1000) neil      (1000)      174 2015-08-14 21:06:04.000000 wafer-0.9.3/wafer/registration/templates/registration/activation_email_subject.txt
--rw-r-----   0 neil      (1000) neil      (1000)     1144 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/registration/templates/registration/login.html
--rw-r-----   0 neil      (1000) neil      (1000)      337 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/registration/templates/registration/logout.html
--rw-r-----   0 neil      (1000) neil      (1000)       32 2015-11-28 16:33:11.000000 wafer-0.9.3/wafer/registration/templates/registration/registration_base.html
--rw-r-----   0 neil      (1000) neil      (1000)      572 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/registration/templates/registration/registration_complete.html
--rw-r-----   0 neil      (1000) neil      (1000)      291 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/registration/templates/registration/registration_form.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/registration/templatetags/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-03 11:44:10.000000 wafer-0.9.3/wafer/registration/templatetags/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      536 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/registration/templatetags/wafer_crispy.py
--rw-r-----   0 neil      (1000) neil      (1000)      521 2019-07-30 14:28:03.000000 wafer-0.9.3/wafer/registration/templatetags/wafer_sso.py
--rw-r-----   0 neil      (1000) neil      (1000)      392 2020-06-04 14:42:52.000000 wafer-0.9.3/wafer/registration/urls.py
--rw-r-----   0 neil      (1000) neil      (1000)     3196 2020-06-04 14:42:52.000000 wafer-0.9.3/wafer/registration/views.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/schedule/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-06-11 12:55:14.000000 wafer-0.9.3/wafer/schedule/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)    17804 2020-04-22 11:34:09.000000 wafer-0.9.3/wafer/schedule/admin.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/schedule/migrations/
--rw-r-----   0 neil      (1000) neil      (1000)     4442 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/schedule/migrations/0001_initial.py
--rw-r-----   0 neil      (1000) neil      (1000)      374 2016-08-17 12:10:46.000000 wafer-0.9.3/wafer/schedule/migrations/0002_auto_20140909_1403.py
--rw-r-----   0 neil      (1000) neil      (1000)      745 2016-08-17 12:10:46.000000 wafer-0.9.3/wafer/schedule/migrations/0003_protect_scheduleitems_from_deletion.py
--rw-r-----   0 neil      (1000) neil      (1000)      427 2016-08-17 12:10:46.000000 wafer-0.9.3/wafer/schedule/migrations/0004_drop_order_with_respect_to.py
--rw-r-----   0 neil      (1000) neil      (1000)      494 2016-10-09 11:19:28.000000 wafer-0.9.3/wafer/schedule/migrations/0005_scheduleitem_expand.py
--rw-r-----   0 neil      (1000) neil      (1000)      595 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/schedule/migrations/0006_schedule_item_update_timestamp.py
--rw-r-----   0 neil      (1000) neil      (1000)      519 2018-10-14 08:22:43.000000 wafer-0.9.3/wafer/schedule/migrations/0007_venue_add_video.py
--rw-r-----   0 neil      (1000) neil      (1000)     2344 2019-10-16 08:40:41.000000 wafer-0.9.3/wafer/schedule/migrations/0008_add_schedule_block_and_datetimes.py
--rw-r-----   0 neil      (1000) neil      (1000)     4486 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/schedule/migrations/0009_migrate_to_datetimes.py
--rw-r-----   0 neil      (1000) neil      (1000)      881 2019-10-16 08:40:41.000000 wafer-0.9.3/wafer/schedule/migrations/0010_cleanup_old_data.py
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.3/wafer/schedule/migrations/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)    15163 2020-09-17 06:23:19.000000 wafer-0.9.3/wafer/schedule/models.py
--rw-r-----   0 neil      (1000) neil      (1000)     2085 2018-05-28 20:25:08.000000 wafer-0.9.3/wafer/schedule/serializers.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/schedule/templates/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/schedule/templates/admin/
--rw-r-----   0 neil      (1000) neil      (1000)     2122 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/schedule/templates/admin/scheduleitem_list.html
--rw-r-----   0 neil      (1000) neil      (1000)      643 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/schedule/templates/admin/slot_list.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/schedule/templates/wafer.schedule/
--rw-r-----   0 neil      (1000) neil      (1000)     4043 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/schedule/templates/wafer.schedule/current.html
--rw-r-----   0 neil      (1000) neil      (1000)     6713 2020-08-13 07:18:53.000000 wafer-0.9.3/wafer/schedule/templates/wafer.schedule/edit_schedule.html
--rw-r-----   0 neil      (1000) neil      (1000)     3474 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/schedule/templates/wafer.schedule/full_schedule.html
--rw-r-----   0 neil      (1000) neil      (1000)     7290 2019-10-16 08:40:41.000000 wafer-0.9.3/wafer/schedule/templates/wafer.schedule/penta_schedule.xml
--rw-r-----   0 neil      (1000) neil      (1000)      535 2018-10-14 08:22:43.000000 wafer-0.9.3/wafer/schedule/templates/wafer.schedule/schedule_item.html
--rw-r-----   0 neil      (1000) neil      (1000)      291 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/schedule/templates/wafer.schedule/venue.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/schedule/tests/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-06-11 12:55:14.000000 wafer-0.9.3/wafer/schedule/tests/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)    36434 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/schedule/tests/test_admin.py
--rw-r-----   0 neil      (1000) neil      (1000)    22658 2020-09-17 06:23:19.000000 wafer-0.9.3/wafer/schedule/tests/test_models.py
--rw-r-----   0 neil      (1000) neil      (1000)    72170 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/schedule/tests/test_views.py
--rw-r-----   0 neil      (1000) neil      (1000)      732 2018-11-04 13:39:20.000000 wafer-0.9.3/wafer/schedule/urls.py
--rw-r-----   0 neil      (1000) neil      (1000)    15945 2020-02-23 17:35:31.000000 wafer-0.9.3/wafer/schedule/views.py
--rw-r-----   0 neil      (1000) neil      (1000)    10183 2020-07-27 09:12:38.000000 wafer-0.9.3/wafer/settings.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/snippets/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2013-07-29 09:20:38.000000 wafer-0.9.3/wafer/snippets/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     2486 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/snippets/markdown_field.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/sponsors/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2013-07-29 09:20:38.000000 wafer-0.9.3/wafer/sponsors/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      539 2018-10-14 08:22:43.000000 wafer-0.9.3/wafer/sponsors/admin.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/sponsors/migrations/
--rw-r-----   0 neil      (1000) neil      (1000)     3152 2014-10-25 18:38:10.000000 wafer-0.9.3/wafer/sponsors/migrations/0001_initial.py
--rw-r-----   0 neil      (1000) neil      (1000)      810 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/sponsors/migrations/0002_non-null_files.py
--rw-r-----   0 neil      (1000) neil      (1000)      405 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/sponsors/migrations/0003_add_ordering_option.py
--rw-r-----   0 neil      (1000) neil      (1000)      752 2016-10-09 11:19:28.000000 wafer-0.9.3/wafer/sponsors/migrations/0004_auto_20160813_1328.py
--rw-r-----   0 neil      (1000) neil      (1000)      552 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/sponsors/migrations/0005_sponsorshippackage_symbol.py
--rw-r-----   0 neil      (1000) neil      (1000)      410 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/sponsors/migrations/0006_allow_blank_files_description.py
--rw-r-----   0 neil      (1000) neil      (1000)     1179 2018-10-14 08:22:43.000000 wafer-0.9.3/wafer/sponsors/migrations/0007_tagged_file_support.py
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.3/wafer/sponsors/migrations/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     5177 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/sponsors/models.py
--rw-r-----   0 neil      (1000) neil      (1000)     1585 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/sponsors/serializers.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/sponsors/templates/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/
--rw-r-----   0 neil      (1000) neil      (1000)     1192 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/packages.html
--rw-r-----   0 neil      (1000) neil      (1000)      702 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/sponsor.html
--rw-r-----   0 neil      (1000) neil      (1000)     1526 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/sponsors.html
--rw-r-----   0 neil      (1000) neil      (1000)      833 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/sponsors_block.html
--rw-r-----   0 neil      (1000) neil      (1000)      690 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/sponsors_footer.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/sponsors/templatetags/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/sponsors/templatetags/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     1275 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/sponsors/templatetags/sponsors.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/sponsors/tests/
--rw-r-----   0 neil      (1000) neil      (1000)     8632 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/sponsors/tests/test_models.py
--rw-r-----   0 neil      (1000) neil      (1000)      611 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/sponsors/urls.py
--rw-r-----   0 neil      (1000) neil      (1000)     1312 2018-10-14 08:22:43.000000 wafer-0.9.3/wafer/sponsors/views.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/static/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/static/css/
--rw-r-----   0 neil      (1000) neil      (1000)      291 2019-10-15 10:30:54.000000 wafer-0.9.3/wafer/static/css/markitup_styling.css
--rw-r-----   0 neil      (1000) neil      (1000)     1638 2020-08-02 09:05:35.000000 wafer-0.9.3/wafer/static/css/wafer.css
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/static/img/
--rw-r-----   0 neil      (1000) neil      (1000)     8777 2018-03-02 08:47:41.000000 wafer-0.9.3/wafer/static/img/glyphicons-halflings-white.png
--rw-r-----   0 neil      (1000) neil      (1000)    12799 2018-03-02 08:47:41.000000 wafer-0.9.3/wafer/static/img/glyphicons-halflings.png
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/static/js/
--rw-r-----   0 neil      (1000) neil      (1000)     9149 2020-08-02 09:05:35.000000 wafer-0.9.3/wafer/static/js/edit_schedule.js
--rw-r-----   0 neil      (1000) neil      (1000)     1322 2020-04-22 11:34:09.000000 wafer-0.9.3/wafer/static/js/scheduledatetime.js
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2018-08-13 19:35:00.000000 wafer-0.9.3/wafer/talks/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     5631 2020-07-12 12:40:38.000000 wafer-0.9.3/wafer/talks/admin.py
--rw-r-----   0 neil      (1000) neil      (1000)     7087 2020-04-18 11:22:39.000000 wafer-0.9.3/wafer/talks/forms.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/migrations/
--rw-r-----   0 neil      (1000) neil      (1000)     3207 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/talks/migrations/0001_initial.py
--rw-r-----   0 neil      (1000) neil      (1000)      383 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/talks/migrations/0002_auto_20150813_2327.py
--rw-r-----   0 neil      (1000) neil      (1000)      527 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/talks/migrations/0003_talk_private_notes.py
--rw-r-----   0 neil      (1000) neil      (1000)      454 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/talks/migrations/0004_edit_private_notes_permission.py
--rw-r-----   0 neil      (1000) neil      (1000)      441 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/talks/migrations/0005_add_kv.py
--rw-r-----   0 neil      (1000) neil      (1000)      963 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/talks/migrations/0006_author_helptext.py
--rw-r-----   0 neil      (1000) neil      (1000)      404 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/talks/migrations/0007_add_ordering_option.py
--rw-r-----   0 neil      (1000) neil      (1000)      527 2016-10-09 11:19:28.000000 wafer-0.9.3/wafer/talks/migrations/0008_auto_20160629_1404.py
--rw-r-----   0 neil      (1000) neil      (1000)      757 2016-10-09 11:19:28.000000 wafer-0.9.3/wafer/talks/migrations/0009_auto_20160813_1819.py
--rw-r-----   0 neil      (1000) neil      (1000)      583 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/talks/migrations/0010_auto_20161121_2134.py
--rw-r-----   0 neil      (1000) neil      (1000)      632 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/talks/migrations/0011_talk_status_data_migration.py
--rw-r-----   0 neil      (1000) neil      (1000)     1108 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/talks/migrations/0012_add_tracks.py
--rw-r-----   0 neil      (1000) neil      (1000)      599 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/talks/migrations/0013_talk_types_optional.py
--rw-r-----   0 neil      (1000) neil      (1000)     1033 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/talks/migrations/0014_video.py
--rw-r-----   0 neil      (1000) neil      (1000)      644 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/talks/migrations/0015_add_withdrawn_status.py
--rw-r-----   0 neil      (1000) neil      (1000)     4151 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/talks/migrations/0016_add_reviews.py
--rw-r-----   0 neil      (1000) neil      (1000)      701 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/talks/migrations/0017_talk_submission_time.py
--rw-r-----   0 neil      (1000) neil      (1000)      809 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/talks/migrations/0018_talk_type_submission_details.py
--rw-r-----   0 neil      (1000) neil      (1000)      396 2020-09-19 17:28:03.000000 wafer-0.9.3/wafer/talks/migrations/0019_talk_url_public.py
--rw-r-----   0 neil      (1000) neil      (1000)      539 2020-08-28 06:57:41.000000 wafer-0.9.3/wafer/talks/migrations/0019_talkurl_length.py
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.3/wafer/talks/migrations/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)    14749 2020-09-19 17:28:03.000000 wafer-0.9.3/wafer/talks/models.py
--rw-r-----   0 neil      (1000) neil      (1000)     2173 2020-09-19 17:28:03.000000 wafer-0.9.3/wafer/talks/serializers.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/static/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/static/wafer/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/static/wafer/talks/
--rw-r-----   0 neil      (1000) neil      (1000)      736 2020-04-18 11:22:39.000000 wafer-0.9.3/wafer/talks/static/wafer/talks/talk-categorization.js
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/templates/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/
--rw-r-----   0 neil      (1000) neil      (1000)      245 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/review_talk.html
--rw-r-----   0 neil      (1000) neil      (1000)      463 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/reviewed-badge.html
--rw-r-----   0 neil      (1000) neil      (1000)      967 2018-05-03 14:13:35.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/speakers.html
--rw-r-----   0 neil      (1000) neil      (1000)     5872 2020-09-19 17:28:03.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/talk.html
--rw-r-----   0 neil      (1000) neil      (1000)     1561 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/talk_form.html
--rw-r-----   0 neil      (1000) neil      (1000)      574 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/talk_tracks.html
--rw-r-----   0 neil      (1000) neil      (1000)      608 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/talk_types.html
--rw-r-----   0 neil      (1000) neil      (1000)      667 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/talk_withdraw.html
--rw-r-----   0 neil      (1000) neil      (1000)     2960 2020-07-02 10:28:47.000000 wafer-0.9.3/wafer/talks/templates/wafer.talks/talks.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/templatetags/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/talks/templatetags/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      510 2020-02-10 16:46:01.000000 wafer-0.9.3/wafer/talks/templatetags/review.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/talks/tests/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2013-03-09 14:18:26.000000 wafer-0.9.3/wafer/talks/tests/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     1278 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/talks/tests/test_talk_type.py
--rw-r-----   0 neil      (1000) neil      (1000)    32996 2020-09-19 17:28:03.000000 wafer-0.9.3/wafer/talks/tests/test_views.py
--rw-r-----   0 neil      (1000) neil      (1000)     4342 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/talks/tests/test_wafer_basic_talks.py
--rw-r-----   0 neil      (1000) neil      (1000)     1357 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/talks/urls.py
--rw-r-----   0 neil      (1000) neil      (1000)    11367 2020-08-17 06:55:38.000000 wafer-0.9.3/wafer/talks/views.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/templates/
--rw-r-----   0 neil      (1000) neil      (1000)      206 2020-02-04 13:01:55.000000 wafer-0.9.3/wafer/templates/403.html
--rw-r-----   0 neil      (1000) neil      (1000)      206 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/templates/404.html
--rw-r-----   0 neil      (1000) neil      (1000)      239 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/templates/500.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/templates/markitup/
--rw-r-----   0 neil      (1000) neil      (1000)      290 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/templates/markitup/preview.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/templates/wafer/
--rw-r-----   0 neil      (1000) neil      (1000)     1714 2020-09-10 09:16:06.000000 wafer-0.9.3/wafer/templates/wafer/base.html
--rw-r-----   0 neil      (1000) neil      (1000)      271 2020-04-18 11:25:23.000000 wafer-0.9.3/wafer/templates/wafer/base_form.html
--rw-r-----   0 neil      (1000) neil      (1000)      222 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/templates/wafer/index.html
--rw-r-----   0 neil      (1000) neil      (1000)     3460 2020-09-10 09:16:06.000000 wafer-0.9.3/wafer/templates/wafer/nav.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/tests/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2013-07-29 09:48:59.000000 wafer-0.9.3/wafer/tests/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      746 2017-12-16 14:33:09.000000 wafer-0.9.3/wafer/tests/api_utils.py
--rw-r-----   0 neil      (1000) neil      (1000)     3984 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/tests/test_menu.py
--rw-r-----   0 neil      (1000) neil      (1000)      679 2020-09-10 09:16:06.000000 wafer-0.9.3/wafer/tests/utils.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/tickets/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-07-02 13:08:39.000000 wafer-0.9.3/wafer/tickets/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      147 2014-07-02 13:08:39.000000 wafer-0.9.3/wafer/tickets/admin.py
--rw-r-----   0 neil      (1000) neil      (1000)     1131 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/tickets/forms.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/tickets/management/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-07-02 13:08:39.000000 wafer-0.9.3/wafer/tickets/management/__init__.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/tickets/management/commands/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-07-02 13:08:39.000000 wafer-0.9.3/wafer/tickets/management/commands/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     1196 2014-07-02 13:08:39.000000 wafer-0.9.3/wafer/tickets/management/commands/import_quicket_guest_list.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/tickets/migrations/
--rw-r-----   0 neil      (1000) neil      (1000)     1555 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/tickets/migrations/0001_initial.py
--rw-r-----   0 neil      (1000) neil      (1000)      394 2015-08-14 13:57:48.000000 wafer-0.9.3/wafer/tickets/migrations/0002_auto_20150813_1926.py
--rw-r-----   0 neil      (1000) neil      (1000)      415 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/tickets/migrations/0003_longer_email_field.py
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.3/wafer/tickets/migrations/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)      729 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/tickets/models.py
--rw-r-----   0 neil      (1000) neil      (1000)     1961 2020-09-10 09:16:06.000000 wafer-0.9.3/wafer/tickets/serializers.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/tickets/templates/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/tickets/templates/wafer.tickets/
--rw-r-----   0 neil      (1000) neil      (1000)      766 2019-12-04 11:38:56.000000 wafer-0.9.3/wafer/tickets/templates/wafer.tickets/claim.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/tickets/tests/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2015-08-14 13:57:48.000000 wafer-0.9.3/wafer/tickets/tests/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)    14217 2020-09-10 09:16:06.000000 wafer-0.9.3/wafer/tickets/tests/test_views.py
--rw-r-----   0 neil      (1000) neil      (1000)      589 2020-09-10 09:16:06.000000 wafer-0.9.3/wafer/tickets/urls.py
--rw-r-----   0 neil      (1000) neil      (1000)     5392 2020-09-10 09:16:06.000000 wafer-0.9.3/wafer/tickets/views.py
--rw-r-----   0 neil      (1000) neil      (1000)      939 2019-04-09 12:39:28.000000 wafer-0.9.3/wafer/urls.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/users/
--rw-r-----   0 neil      (1000) neil      (1000)        0 2013-03-09 15:46:47.000000 wafer-0.9.3/wafer/users/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     1867 2020-04-18 11:22:55.000000 wafer-0.9.3/wafer/users/admin.py
--rw-r-----   0 neil      (1000) neil      (1000)     1820 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/users/forms.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/users/migrations/
--rw-r-----   0 neil      (1000) neil      (1000)     1547 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/users/migrations/0001_initial.py
--rw-r-----   0 neil      (1000) neil      (1000)      426 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/users/migrations/0002_userprofile_kv.py
--rw-r-----   0 neil      (1000) neil      (1000)      366 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/users/migrations/0003_auto_20160329_2003.py
--rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.3/wafer/users/migrations/__init__.py
--rw-r-----   0 neil      (1000) neil      (1000)     4238 2020-07-27 09:12:38.000000 wafer-0.9.3/wafer/users/models.py
--rw-r-----   0 neil      (1000) neil      (1000)      394 2016-08-17 12:10:47.000000 wafer-0.9.3/wafer/users/serializers.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/users/templates/
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/users/templates/wafer.users/
--rw-r-----   0 neil      (1000) neil      (1000)      172 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/users/templates/wafer.users/edit_profile.html
--rw-r-----   0 neil      (1000) neil      (1000)      431 2020-01-30 07:30:18.000000 wafer-0.9.3/wafer/users/templates/wafer.users/edit_user.html
--rw-r-----   0 neil      (1000) neil      (1000)     7658 2020-01-30 07:30:18.000000 wafer-0.9.3/wafer/users/templates/wafer.users/profile.html
--rw-r-----   0 neil      (1000) neil      (1000)     1313 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/users/templates/wafer.users/users.html
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer/users/tests/
--rw-r-----   0 neil      (1000) neil      (1000)      610 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/users/tests/test_models.py
--rw-r-----   0 neil      (1000) neil      (1000)     5893 2020-04-13 10:03:36.000000 wafer-0.9.3/wafer/users/tests/test_views.py
--rw-r-----   0 neil      (1000) neil      (1000)      823 2018-05-03 14:13:58.000000 wafer-0.9.3/wafer/users/urls.py
--rw-r-----   0 neil      (1000) neil      (1000)     5349 2020-04-18 11:20:50.000000 wafer-0.9.3/wafer/users/views.py
--rw-r-----   0 neil      (1000) neil      (1000)     3158 2018-10-14 08:22:44.000000 wafer-0.9.3/wafer/utils.py
--rw-r-----   0 neil      (1000) neil      (1000)     1416 2013-03-09 09:13:17.000000 wafer-0.9.3/wafer/wsgi.py
-drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 17:31:07.000000 wafer-0.9.3/wafer.egg-info/
--rw-r-----   0 neil      (1000) neil      (1000)     4986 2020-09-19 17:31:06.000000 wafer-0.9.3/wafer.egg-info/PKG-INFO
--rw-r-----   0 neil      (1000) neil      (1000)     9414 2020-09-19 17:31:06.000000 wafer-0.9.3/wafer.egg-info/SOURCES.txt
--rw-r-----   0 neil      (1000) neil      (1000)        1 2020-09-19 17:31:06.000000 wafer-0.9.3/wafer.egg-info/dependency_links.txt
--rw-r-----   0 neil      (1000) neil      (1000)      287 2020-09-19 17:31:06.000000 wafer-0.9.3/wafer.egg-info/requires.txt
--rw-r-----   0 neil      (1000) neil      (1000)        6 2020-09-19 17:31:06.000000 wafer-0.9.3/wafer.egg-info/top_level.txt
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/
+-rw-r-----   0 neil      (1000) neil      (1000)      420 2018-10-14 08:22:43.000000 wafer-0.9.4/.gitignore
+-rw-r-----   0 neil      (1000) neil      (1000)     2006 2020-04-18 11:20:50.000000 wafer-0.9.4/.travis.yml
+-rw-r-----   0 neil      (1000) neil      (1000)      776 2020-03-20 20:20:38.000000 wafer-0.9.4/LICENSE
+-rw-r-----   0 neil      (1000) neil      (1000)     4986 2020-09-19 19:00:16.000000 wafer-0.9.4/PKG-INFO
+-rw-r-----   0 neil      (1000) neil      (1000)     3213 2020-04-18 11:20:50.000000 wafer-0.9.4/README.rst
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/docs/
+-rw-r-----   0 neil      (1000) neil      (1000)     5559 2020-04-13 10:30:47.000000 wafer-0.9.4/docs/Makefile
+-rw-r-----   0 neil      (1000) neil      (1000)     7758 2020-09-19 19:00:01.000000 wafer-0.9.4/docs/conf.py
+-rw-r-----   0 neil      (1000) neil      (1000)      287 2018-05-03 14:13:58.000000 wafer-0.9.4/docs/index.rst
+-rw-r-----   0 neil      (1000) neil      (1000)     2313 2020-04-18 11:20:50.000000 wafer-0.9.4/docs/install.rst
+-rw-r-----   0 neil      (1000) neil      (1000)     5103 2014-10-15 15:48:24.000000 wafer-0.9.4/docs/make.bat
+-rw-r-----   0 neil      (1000) neil      (1000)     3118 2018-05-03 14:14:11.000000 wafer-0.9.4/docs/menus.rst
+-rw-r-----   0 neil      (1000) neil      (1000)     2683 2019-12-04 11:38:56.000000 wafer-0.9.4/docs/pages.rst
+-rw-r-----   0 neil      (1000) neil      (1000)     4172 2020-04-18 11:20:50.000000 wafer-0.9.4/docs/schedule.rst
+-rw-r-----   0 neil      (1000) neil      (1000)     5283 2020-06-04 14:42:52.000000 wafer-0.9.4/docs/settings.rst
+-rw-r-----   0 neil      (1000) neil      (1000)     1162 2018-10-14 08:22:43.000000 wafer-0.9.4/docs/sponsors.rst
+-rw-r-----   0 neil      (1000) neil      (1000)      737 2018-10-14 08:22:43.000000 wafer-0.9.4/docs/static.rst
+-rw-r-----   0 neil      (1000) neil      (1000)     5920 2018-05-03 14:14:11.000000 wafer-0.9.4/docs/talks.rst
+-rwxr-x---   0 neil      (1000) neil      (1000)      136 2013-07-29 09:20:38.000000 wafer-0.9.4/install_requirements
+-rwxr-x---   0 neil      (1000) neil      (1000)      248 2014-09-03 11:56:53.000000 wafer-0.9.4/manage.py
+-rw-r-----   0 neil      (1000) neil      (1000)      315 2018-05-03 14:13:58.000000 wafer-0.9.4/package.json
+-rw-r-----   0 neil      (1000) neil      (1000)       35 2018-05-03 14:13:58.000000 wafer-0.9.4/requirements-dev.txt
+-rw-r-----   0 neil      (1000) neil      (1000)       56 2014-10-04 12:13:30.000000 wafer-0.9.4/requirements.txt
+-rw-r-----   0 neil      (1000) neil      (1000)       67 2020-09-19 19:00:16.000000 wafer-0.9.4/setup.cfg
+-rw-r-----   0 neil      (1000) neil      (1000)     2130 2020-09-19 19:00:01.000000 wafer-0.9.4/setup.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/utils/
+-rwxr-x---   0 neil      (1000) neil      (1000)      722 2014-10-15 15:48:59.000000 wafer-0.9.4/utils/bump-version.sh
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/
+-rw-r-----   0 neil      (1000) neil      (1000)       93 2020-09-19 19:00:01.000000 wafer-0.9.4/wafer/__init__.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/compare/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2016-08-17 12:10:46.000000 wafer-0.9.4/wafer/compare/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     7193 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/compare/admin.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/compare/templates/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/compare/templates/admin/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/compare/templates/admin/wafer.compare/
+-rw-r-----   0 neil      (1000) neil      (1000)      591 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/compare/templates/admin/wafer.compare/change_form.html
+-rw-r-----   0 neil      (1000) neil      (1000)      585 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/compare/templates/admin/wafer.compare/compare.html
+-rw-r-----   0 neil      (1000) neil      (1000)     2206 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/compare/templates/admin/wafer.compare/compare_list.html
+-rw-r-----   0 neil      (1000) neil      (1000)     1287 2019-10-15 10:30:54.000000 wafer-0.9.4/wafer/context_processors.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/kv/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2016-08-17 12:10:46.000000 wafer-0.9.4/wafer/kv/__init__.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/kv/migrations/
+-rw-r-----   0 neil      (1000) neil      (1000)      827 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/kv/migrations/0001_initial.py
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2016-08-17 12:10:46.000000 wafer-0.9.4/wafer/kv/migrations/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      381 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/kv/models.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1009 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/kv/permissions.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1312 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/kv/serializers.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/kv/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)     9649 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/kv/tests/test_kv_api.py
+-rw-r-----   0 neil      (1000) neil      (1000)      256 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/kv/urls.py
+-rw-r-----   0 neil      (1000) neil      (1000)      537 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/kv/utils.py
+-rw-r-----   0 neil      (1000) neil      (1000)      879 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/kv/views.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/locale/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/locale/pt_BR/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/locale/pt_BR/LC_MESSAGES/
+-rw-r-----   0 neil      (1000) neil      (1000)    27050 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r-----   0 neil      (1000) neil      (1000)    42066 2020-07-12 12:40:38.000000 wafer-0.9.4/wafer/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/locale/ru/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/locale/ru/LC_MESSAGES/
+-rw-r-----   0 neil      (1000) neil      (1000)     7142 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/locale/ru/LC_MESSAGES/django.mo
+-rw-r-----   0 neil      (1000) neil      (1000)    17371 2019-10-15 10:30:54.000000 wafer-0.9.4/wafer/locale/ru/LC_MESSAGES/django.po
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/management/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2013-10-06 13:47:00.000000 wafer-0.9.4/wafer/management/__init__.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/management/commands/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2013-03-09 09:13:17.000000 wafer-0.9.4/wafer/management/commands/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     2175 2020-07-27 09:12:38.000000 wafer-0.9.4/wafer/management/commands/wafer_add_default_groups.py
+-rw-r-----   0 neil      (1000) neil      (1000)     3107 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/management/commands/wafer_emails.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1798 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/management/commands/wafer_registered_attendees.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1492 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/management/commands/wafer_speaker_contact_details.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1984 2018-05-03 14:13:35.000000 wafer-0.9.4/wafer/management/commands/wafer_speaker_tickets.py
+-rw-r-----   0 neil      (1000) neil      (1000)      502 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/management/commands/wafer_stats.py
+-rw-r-----   0 neil      (1000) neil      (1000)     4806 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/menu.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/pages/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2013-07-29 09:48:59.000000 wafer-0.9.4/wafer/pages/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      551 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/pages/admin.py
+-rw-r-----   0 neil      (1000) neil      (1000)      606 2019-04-09 14:40:44.000000 wafer-0.9.4/wafer/pages/forms.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/pages/management/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/pages/management/__init__.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/pages/management/commands/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/pages/management/commands/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     2338 2019-11-08 09:50:20.000000 wafer-0.9.4/wafer/pages/management/commands/load_pages.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/pages/management/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)     1395 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/pages/management/tests/test_load_pages.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/pages/migrations/
+-rw-r-----   0 neil      (1000) neil      (1000)     1985 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/pages/migrations/0001_initial.py
+-rw-r-----   0 neil      (1000) neil      (1000)      693 2015-11-20 18:19:02.000000 wafer-0.9.4/wafer/pages/migrations/0002_page_people.py
+-rw-r-----   0 neil      (1000) neil      (1000)      853 2016-08-17 12:10:46.000000 wafer-0.9.4/wafer/pages/migrations/0003_non-null_people+files.py
+-rw-r-----   0 neil      (1000) neil      (1000)      403 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/pages/migrations/0004_allow_blank_files_description.py
+-rw-r-----   0 neil      (1000) neil      (1000)      650 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/pages/migrations/0005_page_cache_time.py
+-rw-r-----   0 neil      (1000) neil      (1000)      567 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/pages/migrations/0006_menu_order.py
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.4/wafer/pages/migrations/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     6401 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/pages/models.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1072 2016-08-17 12:10:46.000000 wafer-0.9.4/wafer/pages/serializers.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/pages/templates/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/pages/templates/wafer.pages/
+-rw-r-----   0 neil      (1000) neil      (1000)      569 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/pages/templates/wafer.pages/page.html
+-rw-r-----   0 neil      (1000) neil      (1000)     1352 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/pages/templates/wafer.pages/page_compare.html
+-rw-r-----   0 neil      (1000) neil      (1000)      397 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/pages/templates/wafer.pages/page_form.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/pages/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)     1083 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/pages/tests/test_menu.py
+-rw-r-----   0 neil      (1000) neil      (1000)     5350 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/pages/tests/test_pages.py
+-rw-r-----   0 neil      (1000) neil      (1000)      614 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/pages/tests/test_views.py
+-rw-r-----   0 neil      (1000) neil      (1000)      524 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/pages/urls.py
+-rw-r-----   0 neil      (1000) neil      (1000)     4224 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/pages/views.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/registration/
+-rw-r-----   0 neil      (1000) neil      (1000)       66 2014-10-04 08:49:07.000000 wafer-0.9.4/wafer/registration/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      196 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/registration/apps.py
+-rw-r-----   0 neil      (1000) neil      (1000)      844 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/registration/forms.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/registration/migrations/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-10-04 08:49:07.000000 wafer-0.9.4/wafer/registration/migrations/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     6586 2020-06-04 14:42:52.000000 wafer-0.9.4/wafer/registration/sso.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/registration/templates/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/registration/templates/registration/
+-rw-r-----   0 neil      (1000) neil      (1000)      481 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/registration/templates/registration/activate.html
+-rw-r-----   0 neil      (1000) neil      (1000)      553 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/registration/templates/registration/activation_complete.html
+-rw-r-----   0 neil      (1000) neil      (1000)      642 2020-01-30 07:30:18.000000 wafer-0.9.4/wafer/registration/templates/registration/activation_email.txt
+-rw-r-----   0 neil      (1000) neil      (1000)      174 2015-08-14 21:06:04.000000 wafer-0.9.4/wafer/registration/templates/registration/activation_email_subject.txt
+-rw-r-----   0 neil      (1000) neil      (1000)     1144 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/registration/templates/registration/login.html
+-rw-r-----   0 neil      (1000) neil      (1000)      337 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/registration/templates/registration/logout.html
+-rw-r-----   0 neil      (1000) neil      (1000)       32 2015-11-28 16:33:11.000000 wafer-0.9.4/wafer/registration/templates/registration/registration_base.html
+-rw-r-----   0 neil      (1000) neil      (1000)      572 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/registration/templates/registration/registration_complete.html
+-rw-r-----   0 neil      (1000) neil      (1000)      291 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/registration/templates/registration/registration_form.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/registration/templatetags/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-03 11:44:10.000000 wafer-0.9.4/wafer/registration/templatetags/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      536 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/registration/templatetags/wafer_crispy.py
+-rw-r-----   0 neil      (1000) neil      (1000)      521 2019-07-30 14:28:03.000000 wafer-0.9.4/wafer/registration/templatetags/wafer_sso.py
+-rw-r-----   0 neil      (1000) neil      (1000)      392 2020-06-04 14:42:52.000000 wafer-0.9.4/wafer/registration/urls.py
+-rw-r-----   0 neil      (1000) neil      (1000)     3196 2020-06-04 14:42:52.000000 wafer-0.9.4/wafer/registration/views.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/schedule/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-06-11 12:55:14.000000 wafer-0.9.4/wafer/schedule/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)    17804 2020-04-22 11:34:09.000000 wafer-0.9.4/wafer/schedule/admin.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/schedule/migrations/
+-rw-r-----   0 neil      (1000) neil      (1000)     4442 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/schedule/migrations/0001_initial.py
+-rw-r-----   0 neil      (1000) neil      (1000)      374 2016-08-17 12:10:46.000000 wafer-0.9.4/wafer/schedule/migrations/0002_auto_20140909_1403.py
+-rw-r-----   0 neil      (1000) neil      (1000)      745 2016-08-17 12:10:46.000000 wafer-0.9.4/wafer/schedule/migrations/0003_protect_scheduleitems_from_deletion.py
+-rw-r-----   0 neil      (1000) neil      (1000)      427 2016-08-17 12:10:46.000000 wafer-0.9.4/wafer/schedule/migrations/0004_drop_order_with_respect_to.py
+-rw-r-----   0 neil      (1000) neil      (1000)      494 2016-10-09 11:19:28.000000 wafer-0.9.4/wafer/schedule/migrations/0005_scheduleitem_expand.py
+-rw-r-----   0 neil      (1000) neil      (1000)      595 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/schedule/migrations/0006_schedule_item_update_timestamp.py
+-rw-r-----   0 neil      (1000) neil      (1000)      519 2018-10-14 08:22:43.000000 wafer-0.9.4/wafer/schedule/migrations/0007_venue_add_video.py
+-rw-r-----   0 neil      (1000) neil      (1000)     2344 2019-10-16 08:40:41.000000 wafer-0.9.4/wafer/schedule/migrations/0008_add_schedule_block_and_datetimes.py
+-rw-r-----   0 neil      (1000) neil      (1000)     4486 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/schedule/migrations/0009_migrate_to_datetimes.py
+-rw-r-----   0 neil      (1000) neil      (1000)      881 2019-10-16 08:40:41.000000 wafer-0.9.4/wafer/schedule/migrations/0010_cleanup_old_data.py
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.4/wafer/schedule/migrations/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)    15163 2020-09-17 06:23:19.000000 wafer-0.9.4/wafer/schedule/models.py
+-rw-r-----   0 neil      (1000) neil      (1000)     2085 2018-05-28 20:25:08.000000 wafer-0.9.4/wafer/schedule/serializers.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/schedule/templates/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/schedule/templates/admin/
+-rw-r-----   0 neil      (1000) neil      (1000)     2122 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/schedule/templates/admin/scheduleitem_list.html
+-rw-r-----   0 neil      (1000) neil      (1000)      643 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/schedule/templates/admin/slot_list.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/schedule/templates/wafer.schedule/
+-rw-r-----   0 neil      (1000) neil      (1000)     4043 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/schedule/templates/wafer.schedule/current.html
+-rw-r-----   0 neil      (1000) neil      (1000)     6713 2020-08-13 07:18:53.000000 wafer-0.9.4/wafer/schedule/templates/wafer.schedule/edit_schedule.html
+-rw-r-----   0 neil      (1000) neil      (1000)     3474 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/schedule/templates/wafer.schedule/full_schedule.html
+-rw-r-----   0 neil      (1000) neil      (1000)     7290 2019-10-16 08:40:41.000000 wafer-0.9.4/wafer/schedule/templates/wafer.schedule/penta_schedule.xml
+-rw-r-----   0 neil      (1000) neil      (1000)      535 2018-10-14 08:22:43.000000 wafer-0.9.4/wafer/schedule/templates/wafer.schedule/schedule_item.html
+-rw-r-----   0 neil      (1000) neil      (1000)      291 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/schedule/templates/wafer.schedule/venue.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/schedule/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-06-11 12:55:14.000000 wafer-0.9.4/wafer/schedule/tests/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)    36434 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/schedule/tests/test_admin.py
+-rw-r-----   0 neil      (1000) neil      (1000)    22658 2020-09-17 06:23:19.000000 wafer-0.9.4/wafer/schedule/tests/test_models.py
+-rw-r-----   0 neil      (1000) neil      (1000)    72170 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/schedule/tests/test_views.py
+-rw-r-----   0 neil      (1000) neil      (1000)      732 2018-11-04 13:39:20.000000 wafer-0.9.4/wafer/schedule/urls.py
+-rw-r-----   0 neil      (1000) neil      (1000)    15945 2020-02-23 17:35:31.000000 wafer-0.9.4/wafer/schedule/views.py
+-rw-r-----   0 neil      (1000) neil      (1000)    10183 2020-07-27 09:12:38.000000 wafer-0.9.4/wafer/settings.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/snippets/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2013-07-29 09:20:38.000000 wafer-0.9.4/wafer/snippets/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     2486 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/snippets/markdown_field.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/sponsors/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2013-07-29 09:20:38.000000 wafer-0.9.4/wafer/sponsors/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      539 2018-10-14 08:22:43.000000 wafer-0.9.4/wafer/sponsors/admin.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/sponsors/migrations/
+-rw-r-----   0 neil      (1000) neil      (1000)     3152 2014-10-25 18:38:10.000000 wafer-0.9.4/wafer/sponsors/migrations/0001_initial.py
+-rw-r-----   0 neil      (1000) neil      (1000)      810 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/sponsors/migrations/0002_non-null_files.py
+-rw-r-----   0 neil      (1000) neil      (1000)      405 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/sponsors/migrations/0003_add_ordering_option.py
+-rw-r-----   0 neil      (1000) neil      (1000)      752 2016-10-09 11:19:28.000000 wafer-0.9.4/wafer/sponsors/migrations/0004_auto_20160813_1328.py
+-rw-r-----   0 neil      (1000) neil      (1000)      552 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/sponsors/migrations/0005_sponsorshippackage_symbol.py
+-rw-r-----   0 neil      (1000) neil      (1000)      410 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/sponsors/migrations/0006_allow_blank_files_description.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1179 2018-10-14 08:22:43.000000 wafer-0.9.4/wafer/sponsors/migrations/0007_tagged_file_support.py
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.4/wafer/sponsors/migrations/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     5177 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/sponsors/models.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1585 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/sponsors/serializers.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/sponsors/templates/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/
+-rw-r-----   0 neil      (1000) neil      (1000)     1192 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/packages.html
+-rw-r-----   0 neil      (1000) neil      (1000)      702 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/sponsor.html
+-rw-r-----   0 neil      (1000) neil      (1000)     1526 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/sponsors.html
+-rw-r-----   0 neil      (1000) neil      (1000)      833 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/sponsors_block.html
+-rw-r-----   0 neil      (1000) neil      (1000)      690 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/sponsors_footer.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/sponsors/templatetags/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/sponsors/templatetags/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1275 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/sponsors/templatetags/sponsors.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/sponsors/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)     8632 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/sponsors/tests/test_models.py
+-rw-r-----   0 neil      (1000) neil      (1000)      611 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/sponsors/urls.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1312 2018-10-14 08:22:43.000000 wafer-0.9.4/wafer/sponsors/views.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/static/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/static/css/
+-rw-r-----   0 neil      (1000) neil      (1000)      291 2019-10-15 10:30:54.000000 wafer-0.9.4/wafer/static/css/markitup_styling.css
+-rw-r-----   0 neil      (1000) neil      (1000)     1638 2020-08-02 09:05:35.000000 wafer-0.9.4/wafer/static/css/wafer.css
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/static/img/
+-rw-r-----   0 neil      (1000) neil      (1000)     8777 2018-03-02 08:47:41.000000 wafer-0.9.4/wafer/static/img/glyphicons-halflings-white.png
+-rw-r-----   0 neil      (1000) neil      (1000)    12799 2018-03-02 08:47:41.000000 wafer-0.9.4/wafer/static/img/glyphicons-halflings.png
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/static/js/
+-rw-r-----   0 neil      (1000) neil      (1000)     9149 2020-08-02 09:05:35.000000 wafer-0.9.4/wafer/static/js/edit_schedule.js
+-rw-r-----   0 neil      (1000) neil      (1000)     1322 2020-04-22 11:34:09.000000 wafer-0.9.4/wafer/static/js/scheduledatetime.js
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2018-08-13 19:35:00.000000 wafer-0.9.4/wafer/talks/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     5631 2020-07-12 12:40:38.000000 wafer-0.9.4/wafer/talks/admin.py
+-rw-r-----   0 neil      (1000) neil      (1000)     7087 2020-04-18 11:22:39.000000 wafer-0.9.4/wafer/talks/forms.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/migrations/
+-rw-r-----   0 neil      (1000) neil      (1000)     3207 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/talks/migrations/0001_initial.py
+-rw-r-----   0 neil      (1000) neil      (1000)      383 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/talks/migrations/0002_auto_20150813_2327.py
+-rw-r-----   0 neil      (1000) neil      (1000)      527 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/talks/migrations/0003_talk_private_notes.py
+-rw-r-----   0 neil      (1000) neil      (1000)      454 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/talks/migrations/0004_edit_private_notes_permission.py
+-rw-r-----   0 neil      (1000) neil      (1000)      441 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/talks/migrations/0005_add_kv.py
+-rw-r-----   0 neil      (1000) neil      (1000)      963 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/talks/migrations/0006_author_helptext.py
+-rw-r-----   0 neil      (1000) neil      (1000)      404 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/talks/migrations/0007_add_ordering_option.py
+-rw-r-----   0 neil      (1000) neil      (1000)      527 2016-10-09 11:19:28.000000 wafer-0.9.4/wafer/talks/migrations/0008_auto_20160629_1404.py
+-rw-r-----   0 neil      (1000) neil      (1000)      757 2016-10-09 11:19:28.000000 wafer-0.9.4/wafer/talks/migrations/0009_auto_20160813_1819.py
+-rw-r-----   0 neil      (1000) neil      (1000)      583 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/talks/migrations/0010_auto_20161121_2134.py
+-rw-r-----   0 neil      (1000) neil      (1000)      632 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/talks/migrations/0011_talk_status_data_migration.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1108 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/talks/migrations/0012_add_tracks.py
+-rw-r-----   0 neil      (1000) neil      (1000)      599 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/talks/migrations/0013_talk_types_optional.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1033 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/talks/migrations/0014_video.py
+-rw-r-----   0 neil      (1000) neil      (1000)      644 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/talks/migrations/0015_add_withdrawn_status.py
+-rw-r-----   0 neil      (1000) neil      (1000)     4151 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/talks/migrations/0016_add_reviews.py
+-rw-r-----   0 neil      (1000) neil      (1000)      701 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/talks/migrations/0017_talk_submission_time.py
+-rw-r-----   0 neil      (1000) neil      (1000)      809 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/talks/migrations/0018_talk_type_submission_details.py
+-rw-r-----   0 neil      (1000) neil      (1000)      539 2020-08-28 06:57:41.000000 wafer-0.9.4/wafer/talks/migrations/0019_talkurl_length.py
+-rw-r-----   0 neil      (1000) neil      (1000)      382 2020-09-19 18:58:40.000000 wafer-0.9.4/wafer/talks/migrations/0020_talk_url_public.py
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.4/wafer/talks/migrations/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)    14749 2020-09-19 17:28:03.000000 wafer-0.9.4/wafer/talks/models.py
+-rw-r-----   0 neil      (1000) neil      (1000)     2173 2020-09-19 17:28:03.000000 wafer-0.9.4/wafer/talks/serializers.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/static/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/static/wafer/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/static/wafer/talks/
+-rw-r-----   0 neil      (1000) neil      (1000)      736 2020-04-18 11:22:39.000000 wafer-0.9.4/wafer/talks/static/wafer/talks/talk-categorization.js
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/templates/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/
+-rw-r-----   0 neil      (1000) neil      (1000)      245 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/review_talk.html
+-rw-r-----   0 neil      (1000) neil      (1000)      463 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/reviewed-badge.html
+-rw-r-----   0 neil      (1000) neil      (1000)      967 2018-05-03 14:13:35.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/speakers.html
+-rw-r-----   0 neil      (1000) neil      (1000)     5872 2020-09-19 17:28:03.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/talk.html
+-rw-r-----   0 neil      (1000) neil      (1000)     1561 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/talk_form.html
+-rw-r-----   0 neil      (1000) neil      (1000)      574 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/talk_tracks.html
+-rw-r-----   0 neil      (1000) neil      (1000)      608 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/talk_types.html
+-rw-r-----   0 neil      (1000) neil      (1000)      667 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/talk_withdraw.html
+-rw-r-----   0 neil      (1000) neil      (1000)     2960 2020-07-02 10:28:47.000000 wafer-0.9.4/wafer/talks/templates/wafer.talks/talks.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/templatetags/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/talks/templatetags/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      510 2020-02-10 16:46:01.000000 wafer-0.9.4/wafer/talks/templatetags/review.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/talks/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2013-03-09 14:18:26.000000 wafer-0.9.4/wafer/talks/tests/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1278 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/talks/tests/test_talk_type.py
+-rw-r-----   0 neil      (1000) neil      (1000)    32996 2020-09-19 17:28:03.000000 wafer-0.9.4/wafer/talks/tests/test_views.py
+-rw-r-----   0 neil      (1000) neil      (1000)     4342 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/talks/tests/test_wafer_basic_talks.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1357 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/talks/urls.py
+-rw-r-----   0 neil      (1000) neil      (1000)    11367 2020-08-17 06:55:38.000000 wafer-0.9.4/wafer/talks/views.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/templates/
+-rw-r-----   0 neil      (1000) neil      (1000)      206 2020-02-04 13:01:55.000000 wafer-0.9.4/wafer/templates/403.html
+-rw-r-----   0 neil      (1000) neil      (1000)      206 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/templates/404.html
+-rw-r-----   0 neil      (1000) neil      (1000)      239 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/templates/500.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/templates/markitup/
+-rw-r-----   0 neil      (1000) neil      (1000)      290 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/templates/markitup/preview.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/templates/wafer/
+-rw-r-----   0 neil      (1000) neil      (1000)     1714 2020-09-10 09:16:06.000000 wafer-0.9.4/wafer/templates/wafer/base.html
+-rw-r-----   0 neil      (1000) neil      (1000)      271 2020-04-18 11:25:23.000000 wafer-0.9.4/wafer/templates/wafer/base_form.html
+-rw-r-----   0 neil      (1000) neil      (1000)      222 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/templates/wafer/index.html
+-rw-r-----   0 neil      (1000) neil      (1000)     3460 2020-09-10 09:16:06.000000 wafer-0.9.4/wafer/templates/wafer/nav.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2013-07-29 09:48:59.000000 wafer-0.9.4/wafer/tests/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      746 2017-12-16 14:33:09.000000 wafer-0.9.4/wafer/tests/api_utils.py
+-rw-r-----   0 neil      (1000) neil      (1000)     3984 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/tests/test_menu.py
+-rw-r-----   0 neil      (1000) neil      (1000)      679 2020-09-10 09:16:06.000000 wafer-0.9.4/wafer/tests/utils.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/tickets/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-07-02 13:08:39.000000 wafer-0.9.4/wafer/tickets/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      147 2014-07-02 13:08:39.000000 wafer-0.9.4/wafer/tickets/admin.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1131 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/tickets/forms.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/tickets/management/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-07-02 13:08:39.000000 wafer-0.9.4/wafer/tickets/management/__init__.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/tickets/management/commands/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-07-02 13:08:39.000000 wafer-0.9.4/wafer/tickets/management/commands/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1196 2014-07-02 13:08:39.000000 wafer-0.9.4/wafer/tickets/management/commands/import_quicket_guest_list.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/tickets/migrations/
+-rw-r-----   0 neil      (1000) neil      (1000)     1555 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/tickets/migrations/0001_initial.py
+-rw-r-----   0 neil      (1000) neil      (1000)      394 2015-08-14 13:57:48.000000 wafer-0.9.4/wafer/tickets/migrations/0002_auto_20150813_1926.py
+-rw-r-----   0 neil      (1000) neil      (1000)      415 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/tickets/migrations/0003_longer_email_field.py
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.4/wafer/tickets/migrations/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)      729 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/tickets/models.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1961 2020-09-10 09:16:06.000000 wafer-0.9.4/wafer/tickets/serializers.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/tickets/templates/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/tickets/templates/wafer.tickets/
+-rw-r-----   0 neil      (1000) neil      (1000)      766 2019-12-04 11:38:56.000000 wafer-0.9.4/wafer/tickets/templates/wafer.tickets/claim.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/tickets/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2015-08-14 13:57:48.000000 wafer-0.9.4/wafer/tickets/tests/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)    14217 2020-09-10 09:16:06.000000 wafer-0.9.4/wafer/tickets/tests/test_views.py
+-rw-r-----   0 neil      (1000) neil      (1000)      589 2020-09-10 09:16:06.000000 wafer-0.9.4/wafer/tickets/urls.py
+-rw-r-----   0 neil      (1000) neil      (1000)     5392 2020-09-10 09:16:06.000000 wafer-0.9.4/wafer/tickets/views.py
+-rw-r-----   0 neil      (1000) neil      (1000)      939 2019-04-09 12:39:28.000000 wafer-0.9.4/wafer/urls.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/users/
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2013-03-09 15:46:47.000000 wafer-0.9.4/wafer/users/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1867 2020-04-18 11:22:55.000000 wafer-0.9.4/wafer/users/admin.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1820 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/users/forms.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/users/migrations/
+-rw-r-----   0 neil      (1000) neil      (1000)     1547 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/users/migrations/0001_initial.py
+-rw-r-----   0 neil      (1000) neil      (1000)      426 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/users/migrations/0002_userprofile_kv.py
+-rw-r-----   0 neil      (1000) neil      (1000)      366 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/users/migrations/0003_auto_20160329_2003.py
+-rw-r-----   0 neil      (1000) neil      (1000)        0 2014-09-08 11:26:08.000000 wafer-0.9.4/wafer/users/migrations/__init__.py
+-rw-r-----   0 neil      (1000) neil      (1000)     4238 2020-07-27 09:12:38.000000 wafer-0.9.4/wafer/users/models.py
+-rw-r-----   0 neil      (1000) neil      (1000)      394 2016-08-17 12:10:47.000000 wafer-0.9.4/wafer/users/serializers.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/users/templates/
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/users/templates/wafer.users/
+-rw-r-----   0 neil      (1000) neil      (1000)      172 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/users/templates/wafer.users/edit_profile.html
+-rw-r-----   0 neil      (1000) neil      (1000)      431 2020-01-30 07:30:18.000000 wafer-0.9.4/wafer/users/templates/wafer.users/edit_user.html
+-rw-r-----   0 neil      (1000) neil      (1000)     7658 2020-01-30 07:30:18.000000 wafer-0.9.4/wafer/users/templates/wafer.users/profile.html
+-rw-r-----   0 neil      (1000) neil      (1000)     1313 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/users/templates/wafer.users/users.html
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer/users/tests/
+-rw-r-----   0 neil      (1000) neil      (1000)      610 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/users/tests/test_models.py
+-rw-r-----   0 neil      (1000) neil      (1000)     5893 2020-04-13 10:03:36.000000 wafer-0.9.4/wafer/users/tests/test_views.py
+-rw-r-----   0 neil      (1000) neil      (1000)      823 2018-05-03 14:13:58.000000 wafer-0.9.4/wafer/users/urls.py
+-rw-r-----   0 neil      (1000) neil      (1000)     5349 2020-04-18 11:20:50.000000 wafer-0.9.4/wafer/users/views.py
+-rw-r-----   0 neil      (1000) neil      (1000)     3158 2018-10-14 08:22:44.000000 wafer-0.9.4/wafer/utils.py
+-rw-r-----   0 neil      (1000) neil      (1000)     1416 2013-03-09 09:13:17.000000 wafer-0.9.4/wafer/wsgi.py
+drwxr-x---   0 neil      (1000) neil      (1000)        0 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer.egg-info/
+-rw-r-----   0 neil      (1000) neil      (1000)     4986 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer.egg-info/PKG-INFO
+-rw-r-----   0 neil      (1000) neil      (1000)     9414 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer.egg-info/SOURCES.txt
+-rw-r-----   0 neil      (1000) neil      (1000)        1 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer.egg-info/dependency_links.txt
+-rw-r-----   0 neil      (1000) neil      (1000)      287 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer.egg-info/requires.txt
+-rw-r-----   0 neil      (1000) neil      (1000)        6 2020-09-19 19:00:16.000000 wafer-0.9.4/wafer.egg-info/top_level.txt
```

### Comparing `wafer-0.9.3/.travis.yml` & `wafer-0.9.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/LICENSE` & `wafer-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/PKG-INFO` & `wafer-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wafer
-Version: 0.9.3
+Version: 0.9.4
 Summary: A wafer-thin Django library for running small conferences.
 Home-page: http://github.com/CTPUG/wafer
 Author: CTPUG
 Author-email: ctpug@googlegroups.com
 License: ISC
 Description: wafer
         =====
```

### Comparing `wafer-0.9.3/README.rst` & `wafer-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/Makefile` & `wafer-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/conf.py` & `wafer-0.9.4/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '0.9'
 # The full version, including alpha/beta/rc tags.
-release = '0.9.3'
+release = '0.9.4'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `wafer-0.9.3/docs/install.rst` & `wafer-0.9.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/make.bat` & `wafer-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/menus.rst` & `wafer-0.9.4/docs/menus.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/pages.rst` & `wafer-0.9.4/docs/pages.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/schedule.rst` & `wafer-0.9.4/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/settings.rst` & `wafer-0.9.4/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/sponsors.rst` & `wafer-0.9.4/docs/sponsors.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/static.rst` & `wafer-0.9.4/docs/static.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/docs/talks.rst` & `wafer-0.9.4/docs/talks.rst`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/setup.py` & `wafer-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         print("WARNING: cannot compile translations.")
         pass
     return glob('wafer/locale/*/LC_MESSAGES/django.mo')
 
 
 setup(
     name="wafer",
-    version="0.9.3",
+    version="0.9.4",
     url='http://github.com/CTPUG/wafer',
     license='ISC',
     description="A wafer-thin Django library for running small conferences.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author='CTPUG',
     author_email='ctpug@googlegroups.com',
```

### Comparing `wafer-0.9.3/utils/bump-version.sh` & `wafer-0.9.4/utils/bump-version.sh`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/compare/admin.py` & `wafer-0.9.4/wafer/compare/admin.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/compare/templates/admin/wafer.compare/change_form.html` & `wafer-0.9.4/wafer/compare/templates/admin/wafer.compare/change_form.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/compare/templates/admin/wafer.compare/compare.html` & `wafer-0.9.4/wafer/compare/templates/admin/wafer.compare/compare.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/compare/templates/admin/wafer.compare/compare_list.html` & `wafer-0.9.4/wafer/compare/templates/admin/wafer.compare/compare_list.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/context_processors.py` & `wafer-0.9.4/wafer/context_processors.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/kv/migrations/0001_initial.py` & `wafer-0.9.4/wafer/kv/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/kv/permissions.py` & `wafer-0.9.4/wafer/kv/permissions.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/kv/serializers.py` & `wafer-0.9.4/wafer/kv/serializers.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/kv/tests/test_kv_api.py` & `wafer-0.9.4/wafer/kv/tests/test_kv_api.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/kv/utils.py` & `wafer-0.9.4/wafer/kv/utils.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/kv/views.py` & `wafer-0.9.4/wafer/kv/views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/locale/pt_BR/LC_MESSAGES/django.mo` & `wafer-0.9.4/wafer/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/locale/pt_BR/LC_MESSAGES/django.po` & `wafer-0.9.4/wafer/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/locale/ru/LC_MESSAGES/django.mo` & `wafer-0.9.4/wafer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/locale/ru/LC_MESSAGES/django.po` & `wafer-0.9.4/wafer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/management/commands/wafer_add_default_groups.py` & `wafer-0.9.4/wafer/management/commands/wafer_add_default_groups.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/management/commands/wafer_emails.py` & `wafer-0.9.4/wafer/management/commands/wafer_emails.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/management/commands/wafer_registered_attendees.py` & `wafer-0.9.4/wafer/management/commands/wafer_registered_attendees.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/management/commands/wafer_speaker_contact_details.py` & `wafer-0.9.4/wafer/management/commands/wafer_speaker_contact_details.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/management/commands/wafer_speaker_tickets.py` & `wafer-0.9.4/wafer/management/commands/wafer_speaker_tickets.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/menu.py` & `wafer-0.9.4/wafer/menu.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/admin.py` & `wafer-0.9.4/wafer/pages/admin.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/forms.py` & `wafer-0.9.4/wafer/pages/forms.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/management/commands/load_pages.py` & `wafer-0.9.4/wafer/pages/management/commands/load_pages.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/management/tests/test_load_pages.py` & `wafer-0.9.4/wafer/pages/management/tests/test_load_pages.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/migrations/0001_initial.py` & `wafer-0.9.4/wafer/pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/migrations/0002_page_people.py` & `wafer-0.9.4/wafer/pages/migrations/0002_page_people.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/migrations/0003_non-null_people+files.py` & `wafer-0.9.4/wafer/pages/migrations/0003_non-null_people+files.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/migrations/0005_page_cache_time.py` & `wafer-0.9.4/wafer/pages/migrations/0005_page_cache_time.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/migrations/0006_menu_order.py` & `wafer-0.9.4/wafer/pages/migrations/0006_menu_order.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/models.py` & `wafer-0.9.4/wafer/pages/models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/serializers.py` & `wafer-0.9.4/wafer/pages/serializers.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/templates/wafer.pages/page.html` & `wafer-0.9.4/wafer/pages/templates/wafer.pages/page.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/templates/wafer.pages/page_compare.html` & `wafer-0.9.4/wafer/pages/templates/wafer.pages/page_compare.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/tests/test_menu.py` & `wafer-0.9.4/wafer/pages/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/tests/test_pages.py` & `wafer-0.9.4/wafer/pages/tests/test_pages.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/tests/test_views.py` & `wafer-0.9.4/wafer/pages/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/urls.py` & `wafer-0.9.4/wafer/pages/urls.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/pages/views.py` & `wafer-0.9.4/wafer/pages/views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/forms.py` & `wafer-0.9.4/wafer/registration/forms.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/sso.py` & `wafer-0.9.4/wafer/registration/sso.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/templates/registration/activation_complete.html` & `wafer-0.9.4/wafer/registration/templates/registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/templates/registration/activation_email.txt` & `wafer-0.9.4/wafer/registration/templates/registration/activation_email.txt`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/templates/registration/login.html` & `wafer-0.9.4/wafer/registration/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/templates/registration/registration_complete.html` & `wafer-0.9.4/wafer/registration/templates/registration/registration_complete.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/templatetags/wafer_crispy.py` & `wafer-0.9.4/wafer/registration/templatetags/wafer_crispy.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/templatetags/wafer_sso.py` & `wafer-0.9.4/wafer/registration/templatetags/wafer_sso.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/registration/views.py` & `wafer-0.9.4/wafer/registration/views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/admin.py` & `wafer-0.9.4/wafer/schedule/admin.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/migrations/0001_initial.py` & `wafer-0.9.4/wafer/schedule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/migrations/0003_protect_scheduleitems_from_deletion.py` & `wafer-0.9.4/wafer/schedule/migrations/0003_protect_scheduleitems_from_deletion.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/migrations/0006_schedule_item_update_timestamp.py` & `wafer-0.9.4/wafer/schedule/migrations/0006_schedule_item_update_timestamp.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/migrations/0007_venue_add_video.py` & `wafer-0.9.4/wafer/schedule/migrations/0007_venue_add_video.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/migrations/0008_add_schedule_block_and_datetimes.py` & `wafer-0.9.4/wafer/schedule/migrations/0008_add_schedule_block_and_datetimes.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/migrations/0009_migrate_to_datetimes.py` & `wafer-0.9.4/wafer/schedule/migrations/0009_migrate_to_datetimes.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/migrations/0010_cleanup_old_data.py` & `wafer-0.9.4/wafer/schedule/migrations/0010_cleanup_old_data.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/models.py` & `wafer-0.9.4/wafer/schedule/models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/serializers.py` & `wafer-0.9.4/wafer/schedule/serializers.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/templates/admin/scheduleitem_list.html` & `wafer-0.9.4/wafer/schedule/templates/admin/scheduleitem_list.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/templates/admin/slot_list.html` & `wafer-0.9.4/wafer/schedule/templates/admin/slot_list.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/templates/wafer.schedule/current.html` & `wafer-0.9.4/wafer/schedule/templates/wafer.schedule/current.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/templates/wafer.schedule/edit_schedule.html` & `wafer-0.9.4/wafer/schedule/templates/wafer.schedule/edit_schedule.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/templates/wafer.schedule/full_schedule.html` & `wafer-0.9.4/wafer/schedule/templates/wafer.schedule/full_schedule.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/templates/wafer.schedule/penta_schedule.xml` & `wafer-0.9.4/wafer/schedule/templates/wafer.schedule/penta_schedule.xml`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/templates/wafer.schedule/schedule_item.html` & `wafer-0.9.4/wafer/schedule/templates/wafer.schedule/schedule_item.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/tests/test_admin.py` & `wafer-0.9.4/wafer/schedule/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/tests/test_models.py` & `wafer-0.9.4/wafer/schedule/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/tests/test_views.py` & `wafer-0.9.4/wafer/schedule/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/urls.py` & `wafer-0.9.4/wafer/schedule/urls.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/schedule/views.py` & `wafer-0.9.4/wafer/schedule/views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/settings.py` & `wafer-0.9.4/wafer/settings.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/snippets/markdown_field.py` & `wafer-0.9.4/wafer/snippets/markdown_field.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/admin.py` & `wafer-0.9.4/wafer/sponsors/admin.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/migrations/0001_initial.py` & `wafer-0.9.4/wafer/sponsors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/migrations/0002_non-null_files.py` & `wafer-0.9.4/wafer/sponsors/migrations/0002_non-null_files.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/migrations/0004_auto_20160813_1328.py` & `wafer-0.9.4/wafer/sponsors/migrations/0004_auto_20160813_1328.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/migrations/0005_sponsorshippackage_symbol.py` & `wafer-0.9.4/wafer/sponsors/migrations/0005_sponsorshippackage_symbol.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/migrations/0007_tagged_file_support.py` & `wafer-0.9.4/wafer/sponsors/migrations/0007_tagged_file_support.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/models.py` & `wafer-0.9.4/wafer/sponsors/models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/serializers.py` & `wafer-0.9.4/wafer/sponsors/serializers.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/packages.html` & `wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/packages.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/sponsor.html` & `wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/sponsor.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/sponsors.html` & `wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/sponsors.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/sponsors_block.html` & `wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/sponsors_block.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/templates/wafer.sponsors/sponsors_footer.html` & `wafer-0.9.4/wafer/sponsors/templates/wafer.sponsors/sponsors_footer.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/templatetags/sponsors.py` & `wafer-0.9.4/wafer/sponsors/templatetags/sponsors.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/tests/test_models.py` & `wafer-0.9.4/wafer/sponsors/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/urls.py` & `wafer-0.9.4/wafer/sponsors/urls.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/sponsors/views.py` & `wafer-0.9.4/wafer/sponsors/views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/static/css/wafer.css` & `wafer-0.9.4/wafer/static/css/wafer.css`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/static/img/glyphicons-halflings-white.png` & `wafer-0.9.4/wafer/static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/static/img/glyphicons-halflings.png` & `wafer-0.9.4/wafer/static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/static/js/edit_schedule.js` & `wafer-0.9.4/wafer/static/js/edit_schedule.js`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/static/js/scheduledatetime.js` & `wafer-0.9.4/wafer/static/js/scheduledatetime.js`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/admin.py` & `wafer-0.9.4/wafer/talks/admin.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/forms.py` & `wafer-0.9.4/wafer/talks/forms.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0001_initial.py` & `wafer-0.9.4/wafer/talks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0003_talk_private_notes.py` & `wafer-0.9.4/wafer/talks/migrations/0003_talk_private_notes.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0006_author_helptext.py` & `wafer-0.9.4/wafer/talks/migrations/0006_author_helptext.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0008_auto_20160629_1404.py` & `wafer-0.9.4/wafer/talks/migrations/0008_auto_20160629_1404.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0009_auto_20160813_1819.py` & `wafer-0.9.4/wafer/talks/migrations/0009_auto_20160813_1819.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0010_auto_20161121_2134.py` & `wafer-0.9.4/wafer/talks/migrations/0010_auto_20161121_2134.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0011_talk_status_data_migration.py` & `wafer-0.9.4/wafer/talks/migrations/0011_talk_status_data_migration.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0012_add_tracks.py` & `wafer-0.9.4/wafer/talks/migrations/0012_add_tracks.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0013_talk_types_optional.py` & `wafer-0.9.4/wafer/talks/migrations/0013_talk_types_optional.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0014_video.py` & `wafer-0.9.4/wafer/talks/migrations/0014_video.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0015_add_withdrawn_status.py` & `wafer-0.9.4/wafer/talks/migrations/0015_add_withdrawn_status.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0016_add_reviews.py` & `wafer-0.9.4/wafer/talks/migrations/0016_add_reviews.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0017_talk_submission_time.py` & `wafer-0.9.4/wafer/talks/migrations/0017_talk_submission_time.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0018_talk_type_submission_details.py` & `wafer-0.9.4/wafer/talks/migrations/0018_talk_type_submission_details.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/migrations/0019_talkurl_length.py` & `wafer-0.9.4/wafer/talks/migrations/0019_talkurl_length.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/models.py` & `wafer-0.9.4/wafer/talks/models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/serializers.py` & `wafer-0.9.4/wafer/talks/serializers.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/static/wafer/talks/talk-categorization.js` & `wafer-0.9.4/wafer/talks/static/wafer/talks/talk-categorization.js`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/templates/wafer.talks/speakers.html` & `wafer-0.9.4/wafer/talks/templates/wafer.talks/speakers.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/templates/wafer.talks/talk.html` & `wafer-0.9.4/wafer/talks/templates/wafer.talks/talk.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/templates/wafer.talks/talk_form.html` & `wafer-0.9.4/wafer/talks/templates/wafer.talks/talk_form.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/templates/wafer.talks/talk_tracks.html` & `wafer-0.9.4/wafer/talks/templates/wafer.talks/talk_tracks.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/templates/wafer.talks/talk_types.html` & `wafer-0.9.4/wafer/talks/templates/wafer.talks/talk_types.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/templates/wafer.talks/talk_withdraw.html` & `wafer-0.9.4/wafer/talks/templates/wafer.talks/talk_withdraw.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/templates/wafer.talks/talks.html` & `wafer-0.9.4/wafer/talks/templates/wafer.talks/talks.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/tests/test_talk_type.py` & `wafer-0.9.4/wafer/talks/tests/test_talk_type.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/tests/test_views.py` & `wafer-0.9.4/wafer/talks/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/tests/test_wafer_basic_talks.py` & `wafer-0.9.4/wafer/talks/tests/test_wafer_basic_talks.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/urls.py` & `wafer-0.9.4/wafer/talks/urls.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/talks/views.py` & `wafer-0.9.4/wafer/talks/views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/templates/wafer/base.html` & `wafer-0.9.4/wafer/templates/wafer/base.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/templates/wafer/nav.html` & `wafer-0.9.4/wafer/templates/wafer/nav.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tests/api_utils.py` & `wafer-0.9.4/wafer/tests/api_utils.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tests/test_menu.py` & `wafer-0.9.4/wafer/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tests/utils.py` & `wafer-0.9.4/wafer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/forms.py` & `wafer-0.9.4/wafer/tickets/forms.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/management/commands/import_quicket_guest_list.py` & `wafer-0.9.4/wafer/tickets/management/commands/import_quicket_guest_list.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/migrations/0001_initial.py` & `wafer-0.9.4/wafer/tickets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/models.py` & `wafer-0.9.4/wafer/tickets/models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/serializers.py` & `wafer-0.9.4/wafer/tickets/serializers.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/templates/wafer.tickets/claim.html` & `wafer-0.9.4/wafer/tickets/templates/wafer.tickets/claim.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/tests/test_views.py` & `wafer-0.9.4/wafer/tickets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/urls.py` & `wafer-0.9.4/wafer/tickets/urls.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/tickets/views.py` & `wafer-0.9.4/wafer/tickets/views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/urls.py` & `wafer-0.9.4/wafer/urls.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/admin.py` & `wafer-0.9.4/wafer/users/admin.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/forms.py` & `wafer-0.9.4/wafer/users/forms.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/migrations/0001_initial.py` & `wafer-0.9.4/wafer/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/models.py` & `wafer-0.9.4/wafer/users/models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/templates/wafer.users/profile.html` & `wafer-0.9.4/wafer/users/templates/wafer.users/profile.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/templates/wafer.users/users.html` & `wafer-0.9.4/wafer/users/templates/wafer.users/users.html`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/tests/test_models.py` & `wafer-0.9.4/wafer/users/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/tests/test_views.py` & `wafer-0.9.4/wafer/users/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/urls.py` & `wafer-0.9.4/wafer/users/urls.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/users/views.py` & `wafer-0.9.4/wafer/users/views.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/utils.py` & `wafer-0.9.4/wafer/utils.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer/wsgi.py` & `wafer-0.9.4/wafer/wsgi.py`

 * *Files identical despite different names*

### Comparing `wafer-0.9.3/wafer.egg-info/PKG-INFO` & `wafer-0.9.4/wafer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wafer
-Version: 0.9.3
+Version: 0.9.4
 Summary: A wafer-thin Django library for running small conferences.
 Home-page: http://github.com/CTPUG/wafer
 Author: CTPUG
 Author-email: ctpug@googlegroups.com
 License: ISC
 Description: wafer
         =====
```

### Comparing `wafer-0.9.3/wafer.egg-info/SOURCES.txt` & `wafer-0.9.4/wafer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -184,16 +184,16 @@
 wafer/talks/migrations/0012_add_tracks.py
 wafer/talks/migrations/0013_talk_types_optional.py
 wafer/talks/migrations/0014_video.py
 wafer/talks/migrations/0015_add_withdrawn_status.py
 wafer/talks/migrations/0016_add_reviews.py
 wafer/talks/migrations/0017_talk_submission_time.py
 wafer/talks/migrations/0018_talk_type_submission_details.py
-wafer/talks/migrations/0019_talk_url_public.py
 wafer/talks/migrations/0019_talkurl_length.py
+wafer/talks/migrations/0020_talk_url_public.py
 wafer/talks/migrations/__init__.py
 wafer/talks/static/wafer/talks/talk-categorization.js
 wafer/talks/templates/wafer.talks/review_talk.html
 wafer/talks/templates/wafer.talks/reviewed-badge.html
 wafer/talks/templates/wafer.talks/speakers.html
 wafer/talks/templates/wafer.talks/talk.html
 wafer/talks/templates/wafer.talks/talk_form.html
```

