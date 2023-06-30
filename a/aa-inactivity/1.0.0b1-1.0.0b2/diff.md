# Comparing `tmp/aa_inactivity-1.0.0b1.tar.gz` & `tmp/aa_inactivity-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_inactivity-1.0.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_inactivity-1.0.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_inactivity-1.0.0b1.tar` & `aa_inactivity-1.0.0b2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    35149 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     2931 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/README.md
--rw-r--r--   0        0        0      107 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/__init__.py
--rw-r--r--   0        0        0     2329 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/admin.py
--rw-r--r--   0        0        0      173 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/app_settings.py
--rw-r--r--   0        0        0      195 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/apps.py
--rw-r--r--   0        0        0     1052 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/auth_hooks.py
--rw-r--r--   0        0        0     2262 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/forms.py
--rw-r--r--   0        0        0     1552 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/helpers.py
--rw-r--r--   0        0        0     2313 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/managers.py
--rw-r--r--   0        0        0     5731 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0001_initial.py
--rw-r--r--   0        0        0      598 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0002_add_manage_leave_perm.py
--rw-r--r--   0        0        0     4250 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0003_add_webhooks.py
--rw-r--r--   0        0        0     1102 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0004_django4_update.py
--rw-r--r--   0        0        0     2183 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0005_various_improvements.py
--rw-r--r--   0        0        0        0 2023-06-12 13:23:21.256775 aa_inactivity-1.0.0b1/inactivity/migrations/__init__.py
--rw-r--r--   0        0        0     9119 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/models.py
--rw-r--r--   0        0        0      291 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/aa-bootstrap-fix.css
--rw-r--r--   0        0        0      107 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/aa-bootstrap-fix.min.css
--rw-r--r--   0        0        0     1445 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/inactivity.css
--rw-r--r--   0        0        0      383 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/manage_requests.css
--rw-r--r--   0        0        0      232 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/my_requests.css
--rw-r--r--   0        0        0    43262 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     5726 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tasks.py
--rw-r--r--   0        0        0      311 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/base.html
--rw-r--r--   0        0        0     1685 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/create_loa.html
--rw-r--r--   0        0        0     3436 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/inactive_users.html
--rw-r--r--   0        0        0     5778 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/manage_requests.html
--rw-r--r--   0        0        0     1069 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/modals/modal_dialog.html
--rw-r--r--   0        0        0     1275 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/modals/view_request_content.html
--rw-r--r--   0        0        0     5532 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/my_requests.html
--rw-r--r--   0        0        0     1862 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/partials/menu.html
--rw-r--r--   0        0        0      936 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/reject_request.html
--rw-r--r--   0        0        0        0 2023-06-12 13:23:21.257775 aa_inactivity-1.0.0b1/inactivity/tests/__init__.py
--rw-r--r--   0        0        0     6152 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/factories.py
--rw-r--r--   0        0        0     4671 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/test_forms.py
--rw-r--r--   0        0        0     5173 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/test_integration.py
--rw-r--r--   0        0        0     2474 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/test_managers.py
--rw-r--r--   0        0        0     3775 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/test_models.py
--rw-r--r--   0        0        0     8207 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/inactivity/tests/test_tasks.py
--rw-r--r--   0        0        0     5390 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/inactivity/tests/test_views.py
--rw-r--r--   0        0        0     1445 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/inactivity/urls.py
--rw-r--r--   0        0        0     8737 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/inactivity/views.py
--rw-r--r--   0        0        0     1634 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     4144 1970-01-01 00:00:00.000000 aa_inactivity-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-30 14:21:02.250709 aa_inactivity-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     2931 2023-06-30 14:21:02.250709 aa_inactivity-1.0.0b2/README.md
+-rw-r--r--   0        0        0      158 2023-06-30 14:21:02.250709 aa_inactivity-1.0.0b2/inactivity/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-30 14:21:02.250709 aa_inactivity-1.0.0b2/inactivity/admin.py
+-rw-r--r--   0        0        0      173 2023-06-30 14:21:02.250709 aa_inactivity-1.0.0b2/inactivity/app_settings.py
+-rw-r--r--   0        0        0      195 2023-06-30 14:21:02.250709 aa_inactivity-1.0.0b2/inactivity/apps.py
+-rw-r--r--   0        0        0     1052 2023-06-30 14:21:02.250709 aa_inactivity-1.0.0b2/inactivity/auth_hooks.py
+-rw-r--r--   0        0        0     2262 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/forms.py
+-rw-r--r--   0        0        0     1552 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/helpers.py
+-rw-r--r--   0        0        0     2313 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/managers.py
+-rw-r--r--   0        0        0     5731 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/migrations/0001_initial.py
+-rw-r--r--   0        0        0      598 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/migrations/0002_add_manage_leave_perm.py
+-rw-r--r--   0        0        0     4250 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/migrations/0003_add_webhooks.py
+-rw-r--r--   0        0        0     1102 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/migrations/0004_django4_update.py
+-rw-r--r--   0        0        0     2183 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/migrations/0005_various_improvements.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:21:02.277709 aa_inactivity-1.0.0b2/inactivity/migrations/__init__.py
+-rw-r--r--   0        0        0     9083 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/models.py
+-rw-r--r--   0        0        0      291 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/static/inactivity/css/aa-bootstrap-fix.css
+-rw-r--r--   0        0        0      107 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/static/inactivity/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0        0        0     1445 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/static/inactivity/css/inactivity.css
+-rw-r--r--   0        0        0      383 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/static/inactivity/css/manage_requests.css
+-rw-r--r--   0        0        0      232 2023-06-30 14:21:02.251709 aa_inactivity-1.0.0b2/inactivity/static/inactivity/css/my_requests.css
+-rw-r--r--   0        0        0    43262 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     5726 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/tasks.py
+-rw-r--r--   0        0        0      311 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/base.html
+-rw-r--r--   0        0        0     1685 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/create_loa.html
+-rw-r--r--   0        0        0     3436 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/inactive_users.html
+-rw-r--r--   0        0        0     5778 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/manage_requests.html
+-rw-r--r--   0        0        0     1069 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/modals/modal_dialog.html
+-rw-r--r--   0        0        0     1275 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/modals/view_request_content.html
+-rw-r--r--   0        0        0     5532 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/my_requests.html
+-rw-r--r--   0        0        0     1862 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/partials/menu.html
+-rw-r--r--   0        0        0      936 2023-06-30 14:21:02.252709 aa_inactivity-1.0.0b2/inactivity/templates/inactivity/reject_request.html
+-rw-r--r--   0        0        0        0 2023-06-30 14:21:02.278709 aa_inactivity-1.0.0b2/inactivity/tests/__init__.py
+-rw-r--r--   0        0        0     6152 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/tests/factories.py
+-rw-r--r--   0        0        0     4671 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/tests/test_forms.py
+-rw-r--r--   0        0        0     5173 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/tests/test_integration.py
+-rw-r--r--   0        0        0     2474 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/tests/test_managers.py
+-rw-r--r--   0        0        0     3775 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/tests/test_models.py
+-rw-r--r--   0        0        0     8207 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/tests/test_tasks.py
+-rw-r--r--   0        0        0     5390 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/tests/test_views.py
+-rw-r--r--   0        0        0     1445 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/urls.py
+-rw-r--r--   0        0        0     8675 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/inactivity/views.py
+-rw-r--r--   0        0        0     1822 2023-06-30 14:21:02.253709 aa_inactivity-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     4408 1970-01-01 00:00:00.000000 aa_inactivity-1.0.0b2/PKG-INFO
```

### Comparing `aa_inactivity-1.0.0b1/LICENSE` & `aa_inactivity-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/README.md` & `aa_inactivity-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/admin.py` & `aa_inactivity-1.0.0b2/inactivity/admin.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/auth_hooks.py` & `aa_inactivity-1.0.0b2/inactivity/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/forms.py` & `aa_inactivity-1.0.0b2/inactivity/forms.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/helpers.py` & `aa_inactivity-1.0.0b2/inactivity/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/managers.py` & `aa_inactivity-1.0.0b2/inactivity/managers.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/migrations/0001_initial.py` & `aa_inactivity-1.0.0b2/inactivity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/migrations/0002_add_manage_leave_perm.py` & `aa_inactivity-1.0.0b2/inactivity/migrations/0002_add_manage_leave_perm.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/migrations/0003_add_webhooks.py` & `aa_inactivity-1.0.0b2/inactivity/migrations/0003_add_webhooks.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/migrations/0004_django4_update.py` & `aa_inactivity-1.0.0b2/inactivity/migrations/0004_django4_update.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/migrations/0005_various_improvements.py` & `aa_inactivity-1.0.0b2/inactivity/migrations/0005_various_improvements.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/models.py` & `aa_inactivity-1.0.0b2/inactivity/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,17 +180,15 @@
     def to_output_dict(self) -> dict:
         requestor_display = user_for_display(self.user)
         approver_display = user_for_display(self.approver) if self.approver else None
         duration = (
             humanize.naturaldelta(self.end - self.start) if self.end else _("open end")
         )
         created_at_display = (
-            humanize.naturaltime(self.created_at, when=now())
-            if self.created_at
-            else "?"
+            humanize.naturaltime(self.created_at) if self.created_at else "?"
         )
         try:
             status = self.status
         except AttributeError:
             status_html = ""
         else:
             if status == self.Status.DENIED:
```

### Comparing `aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/inactivity.css` & `aa_inactivity-1.0.0b2/inactivity/static/inactivity/css/inactivity.css`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif` & `aa_inactivity-1.0.0b2/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif` & `aa_inactivity-1.0.0b2/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/tasks.py` & `aa_inactivity-1.0.0b2/inactivity/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/create_loa.html` & `aa_inactivity-1.0.0b2/inactivity/templates/inactivity/create_loa.html`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/inactive_users.html` & `aa_inactivity-1.0.0b2/inactivity/templates/inactivity/inactive_users.html`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/manage_requests.html` & `aa_inactivity-1.0.0b2/inactivity/templates/inactivity/manage_requests.html`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/modals/modal_dialog.html` & `aa_inactivity-1.0.0b2/inactivity/templates/inactivity/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/modals/view_request_content.html` & `aa_inactivity-1.0.0b2/inactivity/templates/inactivity/modals/view_request_content.html`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/my_requests.html` & `aa_inactivity-1.0.0b2/inactivity/templates/inactivity/my_requests.html`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/partials/menu.html` & `aa_inactivity-1.0.0b2/inactivity/templates/inactivity/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/reject_request.html` & `aa_inactivity-1.0.0b2/inactivity/templates/inactivity/reject_request.html`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/tests/factories.py` & `aa_inactivity-1.0.0b2/inactivity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/tests/test_forms.py` & `aa_inactivity-1.0.0b2/inactivity/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/tests/test_integration.py` & `aa_inactivity-1.0.0b2/inactivity/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/tests/test_managers.py` & `aa_inactivity-1.0.0b2/inactivity/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/tests/test_models.py` & `aa_inactivity-1.0.0b2/inactivity/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/tests/test_tasks.py` & `aa_inactivity-1.0.0b2/inactivity/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/tests/test_views.py` & `aa_inactivity-1.0.0b2/inactivity/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/urls.py` & `aa_inactivity-1.0.0b2/inactivity/urls.py`

 * *Files identical despite different names*

### Comparing `aa_inactivity-1.0.0b1/inactivity/views.py` & `aa_inactivity-1.0.0b2/inactivity/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required, permission_required
 from django.http import JsonResponse
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils.html import format_html
-from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 
 from allianceauth.notifications import notify
 
 from .forms import CreateRequestForm, RejectRequestForm
 from .helpers import user_for_display
 from .models import InactivityPing, InactivityPingConfig, LeaveOfAbsence, Webhook
@@ -253,20 +252,20 @@
     for obj in InactivityPing.objects.all():
         obj: InactivityPing
         user_obj = user_for_display(obj.user)
         row = {
             "pk": obj.pk,
             "user_html": {"display": user_obj.html, "sort": user_obj.name},
             "last_login_at": {
-                "display": humanize.naturaltime(obj.last_login_at, when=now())
+                "display": humanize.naturaltime(obj.last_login_at)
                 if obj.last_login_at
                 else "?",
                 "sort": obj.last_login_at.isoformat() if obj.last_login_at else None,
             },
             "policy": obj.config.name,
             "notified_at": {
-                "display": humanize.naturaltime(obj.timestamp, when=now()),
+                "display": humanize.naturaltime(obj.timestamp),
                 "sort": obj.timestamp.isoformat(),
             },
         }
         data.append(row)
     return JsonResponse({"data": data})
```

### Comparing `aa_inactivity-1.0.0b1/PKG-INFO` & `aa_inactivity-1.0.0b2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aa-inactivity
-Version: 1.0.0b1
-Summary: Activity monitoring app for Alliance Auth
+Version: 1.0.0b2
+Summary: "Activity monitoring app for Alliance Auth.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>, Rebecca Murphy <rebecca@rcmurphy.me>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,19 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: aa-memberaudit>=2.8.1
 Requires-Dist: allianceauth-app-utils>=1.18
 Requires-Dist: allianceauth>=3.4,<4
 Requires-Dist: django-multiselectfield
 Requires-Dist: py-cord>=2.4.1
 Requires-Dist: pytz>=2023.3
-Requires-Dist: humanize>=4.6
+Requires-Dist: humanize>=4.7
+Project-URL: Changelog, https://gitlab.com/eclipse-expeditions/aa-inactivity/-/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://gitlab.com/eclipse-expeditions/aa-inactivity
+Project-URL: Source, https://gitlab.com/eclipse-expeditions/aa-inactivity
+Project-URL: Tracker, https://gitlab.com/eclipse-expeditions/aa-inactivity/-/issues
 
 # AA Inactivity
 
 This is a player activity monitoring plugin app for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth) (AA).
 
 ![release](https://img.shields.io/pypi/v/aa-inactivity?label=release)
 ![License](https://img.shields.io/badge/license-GPL-green)
```

