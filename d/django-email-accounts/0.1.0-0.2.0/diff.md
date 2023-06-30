# Comparing `tmp/django-email-accounts-0.1.0.tar.gz` & `tmp/django-email-accounts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-email-accounts-0.1.0.tar", last modified: Sat Jun 17 00:12:32 2023, max compression
+gzip compressed data, was "django-email-accounts-0.2.0.tar", last modified: Fri Jun 30 01:06:29 2023, max compression
```

## Comparing `django-email-accounts-0.1.0.tar` & `django-email-accounts-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-17 00:12:32.851386 django-email-accounts-0.1.0/
--rw-r--r--   0 fathi     (1000) fathi     (1000)    35149 2023-06-16 23:14:41.000000 django-email-accounts-0.1.0/LICENSE
--rw-r--r--   0 fathi     (1000) fathi     (1000)     2875 2023-06-17 00:12:32.850386 django-email-accounts-0.1.0/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)     2115 2023-06-17 00:08:48.000000 django-email-accounts-0.1.0/README.md
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-17 00:12:32.848386 django-email-accounts-0.1.0/django_email_accounts.egg-info/
--rw-r--r--   0 fathi     (1000) fathi     (1000)     2875 2023-06-17 00:12:32.000000 django-email-accounts-0.1.0/django_email_accounts.egg-info/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)      500 2023-06-17 00:12:32.000000 django-email-accounts-0.1.0/django_email_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2023-06-17 00:12:32.000000 django-email-accounts-0.1.0/django_email_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       88 2023-06-17 00:12:32.000000 django-email-accounts-0.1.0/django_email_accounts.egg-info/requires.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2023-06-17 00:12:32.000000 django-email-accounts-0.1.0/django_email_accounts.egg-info/top_level.txt
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-17 00:12:32.850386 django-email-accounts-0.1.0/email_accounts/
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 22:57:01.000000 django-email-accounts-0.1.0/email_accounts/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      851 2023-06-16 23:36:24.000000 django-email-accounts-0.1.0/email_accounts/admin.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      159 2023-06-16 23:39:48.000000 django-email-accounts-0.1.0/email_accounts/apps.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      252 2023-06-16 23:44:36.000000 django-email-accounts-0.1.0/email_accounts/filters.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      227 2023-06-16 23:38:04.000000 django-email-accounts-0.1.0/email_accounts/forms.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1773 2023-06-16 23:29:23.000000 django-email-accounts-0.1.0/email_accounts/models.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      281 2023-06-16 23:45:27.000000 django-email-accounts-0.1.0/email_accounts/serializers.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 23:47:44.000000 django-email-accounts-0.1.0/email_accounts/urls.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 22:58:48.000000 django-email-accounts-0.1.0/email_accounts/utils.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      441 2023-06-16 23:42:17.000000 django-email-accounts-0.1.0/email_accounts/views.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2023-06-17 00:12:32.851386 django-email-accounts-0.1.0/setup.cfg
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1125 2023-06-16 23:54:00.000000 django-email-accounts-0.1.0/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-30 01:06:29.972272 django-email-accounts-0.2.0/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)    35149 2023-06-16 23:14:41.000000 django-email-accounts-0.2.0/LICENSE
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     3562 2023-06-30 01:06:29.972272 django-email-accounts-0.2.0/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     2802 2023-06-30 01:03:04.000000 django-email-accounts-0.2.0/README.md
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-30 01:06:29.970272 django-email-accounts-0.2.0/django_email_accounts.egg-info/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     3562 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      500 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       88 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/requires.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-30 01:06:29.972272 django-email-accounts-0.2.0/email_accounts/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 22:57:01.000000 django-email-accounts-0.2.0/email_accounts/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      851 2023-06-16 23:36:24.000000 django-email-accounts-0.2.0/email_accounts/admin.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      159 2023-06-16 23:39:48.000000 django-email-accounts-0.2.0/email_accounts/apps.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      252 2023-06-16 23:44:36.000000 django-email-accounts-0.2.0/email_accounts/filters.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      227 2023-06-16 23:38:04.000000 django-email-accounts-0.2.0/email_accounts/forms.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1773 2023-06-16 23:29:23.000000 django-email-accounts-0.2.0/email_accounts/models.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      281 2023-06-16 23:45:27.000000 django-email-accounts-0.2.0/email_accounts/serializers.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1621 2023-06-30 00:43:38.000000 django-email-accounts-0.2.0/email_accounts/urls.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 22:58:48.000000 django-email-accounts-0.2.0/email_accounts/utils.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      441 2023-06-16 23:42:17.000000 django-email-accounts-0.2.0/email_accounts/views.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2023-06-30 01:06:29.972272 django-email-accounts-0.2.0/setup.cfg
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1125 2023-06-30 01:03:52.000000 django-email-accounts-0.2.0/setup.py
```

### Comparing `django-email-accounts-0.1.0/LICENSE` & `django-email-accounts-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-email-accounts-0.1.0/README.md` & `django-email-accounts-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -39,18 +39,37 @@
     ...
 ]
 ```
 
 4. Run migrations to create the necessary database tables:
 
 ```shell
+python manage.py makemigrations email_accounts
 python manage.py migrate
 ```
 
-5. You can now use the email-accounts functionality in your Django project.
+6. You can now use the email-accounts functionality in your Django project.
+
+If you want custom authentication templates, then, in your templates folder, create a `email_accounts` subdirectory in `templates` directory and create all authentication templates on it like this.
+
+```bash
+├── templates
+│   └── email_accounts
+│       ├── login.html
+│       ├── register.html
+│       └── password
+│           ├── change
+│           ├── ├── 1.html
+│           ├── └── 2.html
+│           └── reset
+│               ├── 1.html
+│               ├── 2.html
+│               ├── 3.html
+│               └── 4.html
+```
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/fathiabdelmalek/django-email-accounts).
 
 To contribute to the project, follow these steps:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-email-accounts-0.1.0/email_accounts/admin.py` & `django-email-accounts-0.2.0/email_accounts/admin.py`

 * *Files identical despite different names*

### Comparing `django-email-accounts-0.1.0/email_accounts/models.py` & `django-email-accounts-0.2.0/email_accounts/models.py`

 * *Files identical despite different names*

### Comparing `django-email-accounts-0.1.0/setup.py` & `django-email-accounts-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 extras_require = {
     "rest_framework": ["djangorestframework>=3.12"],
     "filters": ["django-filter>=2.4"],
 }
 
 setup(
     name='django-email-accounts',
-    version='0.1.0',
+    version='0.2.0',
     author='Fathi Abdelmalek',
     author_email='abdelmalek.fathi.2001@gmail.com',
     description='A Django app for user management with email-based authentication.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/fathiabdelmalek/django-email-accounts',
     packages=find_packages(),
```

