# Comparing `tmp/aa_fleetfinder-1.2.0.tar.gz` & `tmp/aa_fleetfinder-1.3.0.tar.gz`

## Comparing `aa_fleetfinder-1.2.0.tar` & `aa_fleetfinder-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/apps.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/auth_hooks.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/constants.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/models.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/providers.py
--rw-r--r--   0        0        0    10216 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tasks.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/urls.py
--rw-r--r--   0        0        0     9365 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/views.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/django.pot
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/migrations/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/fleetfinder.css
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css
--rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css
--rw-r--r--   0        0        0    35554 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/base.html
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/create-fleet.html
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/dashboard.html
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/edit-fleet.html
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/fleet-details.html
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/join-fleet.html
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/css/multi-select-css.html
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/js/datetime-js.html
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templatetags/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templatetags/fleetfinder_versioned_static.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/__init__.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/test_access.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/test_auth_hooks.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/test_templatetags.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/LICENSE
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/README.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/apps.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/auth_hooks.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/constants.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/models.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/providers.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tasks.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/urls.py
+-rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/views.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/django.pot
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/migrations/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/fleetfinder.css
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css
+-rw-r--r--   0        0        0    35554 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/base.html
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/create-fleet.html
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/dashboard.html
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/edit-fleet.html
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/fleet-details.html
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/join-fleet.html
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/css/multi-select-css.html
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/js/datetime-js.html
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templatetags/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templatetags/fleetfinder_versioned_static.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/test_access.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/README.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/PKG-INFO
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/auth_hooks.py` & `aa_fleetfinder-1.3.0/fleetfinder/auth_hooks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """
 Auth hooks
 """
 
-# Django
-from django.utils.translation import gettext_lazy as _
-
 # Alliance Auth
 from allianceauth import hooks
 from allianceauth.services.hooks import MenuItemHook, UrlHook
 
 # AA Fleet Finder
-from fleetfinder import urls
+from fleetfinder import __title__, urls
 
 
 class FleetFinderMenuItem(MenuItemHook):  # pylint: disable=too-few-public-methods
     """
     This class ensures only authorized users will see the menu entry
     """
 
     def __init__(self):
         # Setup menu entry for sidebar
         MenuItemHook.__init__(
             self,
-            _("Fleet Finder"),
+            __title__,
             "fas fa-users fa-fw",
             "fleetfinder:dashboard",
             navactive=["fleetfinder:"],
         )
 
     def render(self, request):
         """
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/models.py` & `aa_fleetfinder-1.3.0/fleetfinder/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Models
 """
 
 # Django
 from django.db import models
+from django.utils.translation import gettext_lazy as _
 
 # Alliance Auth
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.groupmanagement.models import AuthGroup
 
 
 class General(models.Model):
@@ -30,33 +31,61 @@
 
 
 class Fleet(models.Model):
     """
     Fleet Model
     """
 
+    class EsiError(models.TextChoices):
+        """
+        Choices for SRP Status
+        """
+
+        NOT_IN_FLEET = "NOT_IN_FLEET", _(
+            "FC is not in the registered fleet anymore or fleet is no longer available."
+        )
+        NO_FLEET = "NO_FLEET", _("Registered fleet seems to be no longer available.")
+        NOT_FLEETBOSS = "NOT_FLEETBOSS", _("FC is no longer the fleet boss.")
+        FC_CHANGED_FLEET = "FC_CHANGED_FLEET", _("FC switched to another fleet.")
+
     fleet_id = models.BigIntegerField(primary_key=True)
-    name = models.CharField(max_length=50, default="")
+    name = models.CharField(max_length=50, default="", verbose_name=_("Fleet Name"))
     fleet_commander = models.ForeignKey(
         EveCharacter,
         on_delete=models.SET_NULL,
         related_name="fleetfinder_fleet_commander",
         default=None,
         null=True,
         blank=True,
+        verbose_name=_("Fleet Commander"),
     )
-    created_at = models.DateTimeField()
-    motd = models.TextField(blank=True, default="")
-    is_free_move = models.BooleanField()
+    created_at = models.DateTimeField(verbose_name=_("Creation date and time"))
+    motd = models.TextField(blank=True, default="", verbose_name=_("Fleet MOTD"))
+    is_free_move = models.BooleanField(verbose_name=_("Free move"))
 
     groups = models.ManyToManyField(
         AuthGroup,
         related_name="fleetfinder_restricted_groups",
         help_text="Groups listed here will be able to join the fleet",
+        verbose_name=_("Group restrictions"),
     )
 
+    last_esi_error = models.CharField(
+        max_length=16,
+        blank=True,
+        default="",
+        choices=EsiError.choices,
+        verbose_name=_("Last ESI error"),
+    )
+
+    last_esi_error_time = models.DateTimeField(
+        null=True, blank=True, default=None, verbose_name=_("Last ESI error time")
+    )
+
+    esi_error_count = models.IntegerField(default=0, verbose_name=_("ESI error count"))
+
     class Meta:  # pylint: disable=too-few-public-methods
         """
         Meta Definitions
         """
 
         default_permissions = ()
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/tasks.py` & `aa_fleetfinder-1.3.0/fleetfinder/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,233 @@
 """
 Tasks
 """
 
 # Standard Library
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from datetime import timedelta
 
 # Third Party
 from bravado.exception import HTTPNotFound
 from celery import shared_task
 
 # Django
-from django.core.cache import cache
 from django.utils import timezone
 
 # Alliance Auth
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.services.hooks import get_extension_logger
 from allianceauth.services.tasks import QueueOnce
 from esi.models import Token
 
 # Alliance Auth (External Libs)
+from app_utils.esi import fetch_esi_status
 from app_utils.logging import LoggerAddTag
 
 # AA Fleet Finder
 from fleetfinder import __title__
-from fleetfinder.constants import (
-    CACHE_KEY_FLEET_CHANGED_ERROR,
-    CACHE_KEY_NO_FLEET_ERROR,
-    CACHE_KEY_NO_FLEETBOSS_ERROR,
-    CACHE_KEY_NOT_IN_FLEET_ERROR,
-    CACHE_MAX_ERROR_COUNT,
-    TASK_DEFAULT_KWARGS,
-)
 from fleetfinder.models import Fleet
 from fleetfinder.providers import esi
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
+ESI_ERROR_LIMIT = 50
+ESI_TIMEOUT_ONCE_ERROR_LIMIT_REACHED = 60
+ESI_MAX_RETRIES = 3
+ESI_MAX_ERROR_COUNT = 3
+ESI_ERROR_GRACE_TIME = 75
+
+TASK_TIME_LIMIT = 120  # Stop after 2 minutes
+
+# Params for all tasks
+TASK_DEFAULT_KWARGS = {"time_limit": TASK_TIME_LIMIT, "max_retries": ESI_MAX_RETRIES}
+
+
+class FleetViewAggregate:  # pylint: disable=too-few-public-methods
+    """
+    Helper class
+    """
+
+    def __init__(self, fleet, aggregate):
+        self.fleet = fleet
+        self.aggregate = aggregate
+
+
+@shared_task
+def _send_invitation(character_id, fleet_commander_token, fleet_id):
+    """
+    Open the fleet invite window in the eve client
+    :param character_id:
+    :param fleet_commander_token:
+    :param fleet_id:
+    """
+
+    invitation = {"character_id": character_id, "role": "squad_member"}
+
+    esi.client.Fleets.post_fleets_fleet_id_members(
+        fleet_id=fleet_id,
+        token=fleet_commander_token.valid_access_token(),
+        invitation=invitation,
+    ).result()
+
+
+def _close_esi_fleet(fleet: Fleet, reason: str) -> None:
+    """
+    Closing registered fleet
+    :param fleet:
+    :param reason:
+    """
+
+    logger.info(
+        f'Fleet "{fleet.name}" of {fleet.fleet_commander} (ESI ID: {fleet.fleet_id}) » '
+        f"Closing: {reason}"
+    )
+
+    fleet.delete()
+
+
+def _esi_fleet_error_handling(fleet: Fleet, error_key: str) -> None:
+    """
+    ESI error handling
+    :param fleet:
+    :type fleet:
+    :param error_key:
+    :type error_key:
+    :return:
+    :rtype:
+    """
+
+    time_now = timezone.now()
+
+    # Close ESI fleet if the consecutive error count is too high
+    if (
+        fleet.last_esi_error == error_key
+        and fleet.last_esi_error_time
+        >= (time_now - timedelta(seconds=ESI_ERROR_GRACE_TIME))
+        and fleet.esi_error_count >= ESI_MAX_ERROR_COUNT
+    ):
+        _close_esi_fleet(fleet=fleet, reason=error_key.label)
+
+        return
+
+    error_count = (
+        fleet.esi_error_count + 1
+        if fleet.last_esi_error == error_key
+        and fleet.last_esi_error_time
+        >= (time_now - timedelta(seconds=ESI_ERROR_GRACE_TIME))
+        else 1
+    )
+
+    logger.info(
+        f'Fleet "{fleet.name}" of {fleet.fleet_commander} (ESI ID: {fleet.fleet_id}) » '
+        f'Error: "{error_key.label}" ({error_count} of {ESI_MAX_ERROR_COUNT}).'
+    )
+
+    fleet.esi_error_count = error_count
+    fleet.last_esi_error = error_key
+    fleet.last_esi_error_time = time_now
+    fleet.save()
+
+
+@shared_task
+def _get_fleet_aggregate(fleet_infos):
+    """
+    Getting numbers for fleet composition
+    :param fleet_infos:
+    :return:
+    """
+
+    counts = {}
+
+    for member in fleet_infos:
+        type_ = member.get("ship_type_name")
+
+        if type_ in counts:
+            counts[type_] += 1
+        else:
+            counts[type_] = 1
+
+    return counts
+
+
+def _check_for_esi_fleet(fleet: Fleet):
+    required_scopes = ["esi-fleets.read_fleet.v1"]
+
+    # Check if there is a fleet
+    try:
+        fleet_commander_id = fleet.fleet_commander.character_id
+        esi_token = Token.get_token(fleet_commander_id, required_scopes)
+
+        fleet_from_esi = esi.client.Fleets.get_characters_character_id_fleet(
+            character_id=fleet_commander_id,
+            token=esi_token.valid_access_token(),
+        ).result()
+
+        return {"fleet": fleet_from_esi, "token": esi_token}
+    except HTTPNotFound:
+        _esi_fleet_error_handling(error_key=Fleet.EsiError.NOT_IN_FLEET, fleet=fleet)
+    except Exception:
+        _esi_fleet_error_handling(error_key=Fleet.EsiError.NO_FLEET, fleet=fleet)
+
+    return False
+
+
+def _process_fleet(fleet: Fleet):
+    """
+    Processing a fleet
+    :param fleet:
+    :type fleet:
+    :return:
+    :rtype:
+    """
+
+    fleet_id = fleet.fleet_id
+    fleet_name = fleet.name
+    fleet_commander = fleet.fleet_commander
+
+    logger.info(
+        f'Processing information for fleet "{fleet_name}" '
+        f"of {fleet_commander} (ESI ID: {fleet_id})"
+    )
+
+    # Check if there is a fleet
+    esi_fleet = _check_for_esi_fleet(fleet=fleet)
+    if esi_fleet and fleet.fleet_id == esi_fleet["fleet"]["fleet_id"]:
+        try:
+            fleet_from_esi = esi.client.Fleets.get_characters_character_id_fleet(
+                character_id=fleet.fleet_commander.character_id,
+                token=esi_fleet["token"].valid_access_token(),
+            ).result()
+        except HTTPNotFound:
+            _esi_fleet_error_handling(
+                fleet=fleet, error_key=Fleet.EsiError.NOT_IN_FLEET
+            )
+        except Exception:
+            _esi_fleet_error_handling(fleet=fleet, error_key=Fleet.EsiError.NO_FLEET)
+
+        # We have a valid fleet result from ESI
+        else:
+            if fleet_id == fleet_from_esi["fleet_id"]:
+                # Check if we deal with the fleet boss here
+                try:
+                    _ = esi.client.Fleets.get_fleets_fleet_id_members(
+                        fleet_id=fleet_from_esi["fleet_id"],
+                        token=esi_fleet["token"].valid_access_token(),
+                    ).result()
+                except Exception:
+                    _esi_fleet_error_handling(
+                        fleet=fleet, error_key=Fleet.EsiError.NOT_FLEETBOSS
+                    )
+            else:
+                _esi_fleet_error_handling(
+                    fleet=fleet, error_key=Fleet.EsiError.FC_CHANGED_FLEET
+                )
+
+
 @shared_task
 def open_fleet(character_id, motd, free_move, name, groups):
     """
     Open a fleet
     :param character_id:
     :param motd:
     :param free_move:
@@ -96,169 +282,47 @@
     )
     _processes = []
 
     with ThreadPoolExecutor(max_workers=50) as ex:
         for _character_id in character_ids:
             _processes.append(
                 ex.submit(
-                    send_invitation,
+                    _send_invitation,
                     character_id=_character_id,
                     fleet_commander_token=fleet_commander_token,
                     fleet_id=fleet_id,
                 )
             )
 
     for item in as_completed(_processes):
         _ = item.result()
 
 
-@shared_task
-def send_invitation(character_id, fleet_commander_token, fleet_id):
-    """
-    Open the fleet invite window in the eve client
-    :param character_id:
-    :param fleet_commander_token:
-    :param fleet_id:
-    """
-
-    invitation = {"character_id": character_id, "role": "squad_member"}
-
-    esi.client.Fleets.post_fleets_fleet_id_members(
-        fleet_id=fleet_id,
-        token=fleet_commander_token.valid_access_token(),
-        invitation=invitation,
-    ).result()
-
-
-def close_esi_fleet(fleet: Fleet, reason: str) -> None:
-    """
-    Closing registered fleet
-    :param fleet:
-    :param reason:
-    """
-
-    fleet_id = fleet.fleet_id
-
-    logger.info(f"Closing fleet with ID {fleet_id}. Reason: {reason}")
-
-    fleet.delete()
-
-
-def esi_fleetadvert_error_handling(
-    cache_key: str, fleet: Fleet, logger_message: str
-) -> None:
-    """
-    ESI error handling
-    :param cache_key:
-    :param fleet:
-    :param logger_message:
-    """
-
-    if int(cache.get(cache_key + str(fleet.fleet_id))) < CACHE_MAX_ERROR_COUNT:
-        error_count = int(cache.get(cache_key + str(fleet.fleet_id)))
-
-        error_count += 1
-
-        logger.info(f'"{logger_message}" Error Count: {error_count}.')
-
-        cache.set(cache_key + str(fleet.fleet_id), str(error_count), 75)
-    else:
-        close_esi_fleet(fleet=fleet, reason=logger_message)
-
-
-def init_error_caches(fleet: Fleet) -> None:
-    """
-    Initialize error caches
-    :param fleet:
-    """
-
-    if cache.get(CACHE_KEY_FLEET_CHANGED_ERROR + str(fleet.fleet_id)) is None:
-        cache.set(CACHE_KEY_FLEET_CHANGED_ERROR + str(fleet.fleet_id), "0", 75)
-
-    if cache.get(CACHE_KEY_NO_FLEET_ERROR + str(fleet.fleet_id)) is None:
-        cache.set(CACHE_KEY_NO_FLEET_ERROR + str(fleet.fleet_id), "0", 75)
-
-    if cache.get(CACHE_KEY_NOT_IN_FLEET_ERROR + str(fleet.fleet_id)) is None:
-        cache.set(CACHE_KEY_NOT_IN_FLEET_ERROR + str(fleet.fleet_id), "0", 75)
-
-    if cache.get(CACHE_KEY_NO_FLEETBOSS_ERROR + str(fleet.fleet_id)) is None:
-        cache.set(CACHE_KEY_NO_FLEETBOSS_ERROR + str(fleet.fleet_id), "0", 75)
-
-
-@shared_task(**{**TASK_DEFAULT_KWARGS, **{"base": QueueOnce}})
+@shared_task(**{**TASK_DEFAULT_KWARGS}, **{"base": QueueOnce})
 def check_fleet_adverts():
     """
     Scheduled task :: Check for fleets adverts
     """
 
-    required_scopes = ["esi-fleets.read_fleet.v1", "esi-fleets.write_fleet.v1"]
     fleets = Fleet.objects.all()
     fleet_count = fleets.count()
 
     processing_text = "Processing..." if fleet_count > 0 else "Nothing to do..."
 
     logger.info(f"{fleet_count} registered fleets found. {processing_text}")
 
     if fleet_count > 0:
-        for fleet in fleets:
-            fleet_id = fleet.fleet_id
-            fleet_name = fleet.name
-            fleet_commander = fleet.fleet_commander
-            init_error_caches(fleet=fleet)
-
-            logger.info(
-                f'Processing information for fleet "{fleet_name}" '
-                f"of {fleet_commander} (ESI ID: {fleet_id})"
-            )
+        # Abort if ESI seems to be offline or above the error limit
+        if not fetch_esi_status().is_ok:
+            logger.warning("ESI doesn't seem to be available at this time. Aborting.")
 
-            try:
-                esi_token = Token.get_token(
-                    fleet.fleet_commander.character_id, required_scopes
-                )
-                fleet_from_esi = esi.client.Fleets.get_characters_character_id_fleet(
-                    character_id=esi_token.character_id,
-                    token=esi_token.valid_access_token(),
-                ).result()
-            except HTTPNotFound:
-                esi_fleetadvert_error_handling(
-                    cache_key=CACHE_KEY_NOT_IN_FLEET_ERROR,
-                    fleet=fleet,
-                    logger_message=(
-                        "FC is not in the registered fleet anymore or fleet is no "
-                        "longer available."
-                    ),
-                )
-            except Exception:
-                esi_fleetadvert_error_handling(
-                    cache_key=CACHE_KEY_NO_FLEET_ERROR,
-                    fleet=fleet,
-                    logger_message="Registered fleet is no longer available.",
-                )
+            return
 
-            # We have a valid fleet result from ESI
-            else:
-                if fleet_id == fleet_from_esi["fleet_id"]:
-                    # Check if we deal with the fleet boss here
-                    try:
-                        _ = esi.client.Fleets.get_fleets_fleet_id_members(
-                            fleet_id=fleet_from_esi["fleet_id"],
-                            token=esi_token.valid_access_token(),
-                        ).result()
-                    except Exception:
-                        esi_fleetadvert_error_handling(
-                            cache_key=CACHE_KEY_NO_FLEETBOSS_ERROR,
-                            fleet=fleet,
-                            logger_message="FC is no longer the fleet boss.",
-                        )
-                else:
-                    esi_fleetadvert_error_handling(
-                        cache_key=CACHE_KEY_FLEET_CHANGED_ERROR,
-                        fleet=fleet,
-                        logger_message="FC switched to another fleet",
-                    )
+        for fleet in fleets:
+            _process_fleet(fleet=fleet)
 
 
 @shared_task
 def get_fleet_composition(fleet_id):
     """
     Getting the fleet composition
     :param fleet_id:
@@ -296,41 +360,10 @@
             member["solar_system_id"]
         )
         member["solar_system_name"] = ids_to_name[index_solar_system]["name"]
 
         index_ship_type = [x["id"] for x in ids_to_name].index(member["ship_type_id"])
         member["ship_type_name"] = ids_to_name[index_ship_type]["name"]
 
-    aggregate = get_fleet_aggregate(fleet_infos)
+    aggregate = _get_fleet_aggregate(fleet_infos)
 
     return FleetViewAggregate(fleet_infos, aggregate)
-
-
-@shared_task
-def get_fleet_aggregate(fleet_infos):
-    """
-    Getting numbers for fleet composition
-    :param fleet_infos:
-    :return:
-    """
-
-    counts = {}
-
-    for member in fleet_infos:
-        type_ = member.get("ship_type_name")
-
-        if type_ in counts:
-            counts[type_] += 1
-        else:
-            counts[type_] = 1
-
-    return counts
-
-
-class FleetViewAggregate:  # pylint: disable=too-few-public-methods
-    """
-    Helper class
-    """
-
-    def __init__(self, fleet, aggregate):
-        self.fleet = fleet
-        self.aggregate = aggregate
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/urls.py` & `aa_fleetfinder-1.3.0/fleetfinder/urls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/views.py` & `aa_fleetfinder-1.3.0/fleetfinder/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 
     if request.method == "POST":
         auth_groups = AuthGroup.objects.filter(internal=False).all()
 
         context = {}
 
         if "modified_fleet_data" in request.session:
-            context["error"] = request.session["modified_fleet_data"].get("error", "")
             context["motd"] = request.session["modified_fleet_data"].get("motd", "")
             context["name"] = request.session["modified_fleet_data"].get("name", "")
             context["groups"] = request.session["modified_fleet_data"].get("groups", "")
             context["is_free_move"] = request.session["modified_fleet_data"].get(
                 "free_move", ""
             )
             context["character_id"] = token.character_id
@@ -235,29 +234,26 @@
         motd = request.POST.get("motd", "")
         name = request.POST.get("name", "")
         groups = request.POST.getlist("groups", [])
 
         try:
             open_fleet(request.POST["character_id"], motd, free_move, name, groups)
         except HTTPNotFound as ex:
-            if request.POST.get("origin", "") == "edit":
-                # Here ccp returns "character not in fleet".
-                # Instead, push our own message to be clearer
-                messages.error(
-                    request,
-                    mark_safe(
-                        _("<h4>Error!</h4><p>Fleet advert is no longer valid</p>")
-                    ),
-                )
+            esi_error_message = ex.swagger_result["error"]
+            error_message = _(
+                f"<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
+            )
 
+            messages.error(request, mark_safe(error_message))
+
+            if request.POST.get("origin", "") == "edit":
                 return redirect("fleetfinder:dashboard")
 
             if request.POST.get("origin", "") == "create":
                 request.session["modified_fleet_data"] = {
-                    "error": ex.swagger_result["error"],
                     "motd": motd,
                     "name": name,
                     "free_move": free_move,
                     "groups": groups,
                 }
 
                 return redirect("fleetfinder:create_fleet")
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/locale/django.pot` & `aa_fleetfinder-1.3.0/fleetfinder/locale/es/LC_MESSAGES/django.po`

 * *Files 25% similar despite different names*

```diff
@@ -4,74 +4,122 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 01:20+0200\n"
+"POT-Creation-Date: 2023-06-28 15:41+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: auth_hooks.py:25 templates/fleetfinder/base.html:5
+#: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:18
-msgid "Create Fleet"
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Fleet Finder v{__version__}"
+msgstr ""
+
+#: models.py:44
+msgid ""
+"FC is not in the registered fleet anymore or fleet is no longer available."
+msgstr ""
+
+#: models.py:46
+msgid "Registered fleet seems to be no longer available."
+msgstr ""
+
+#: models.py:47
+msgid "FC is no longer the fleet boss."
+msgstr ""
+
+#: models.py:48
+msgid "FC switched to another fleet."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:29
+#: models.py:51 templates/fleetfinder/create-fleet.html:25
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:38
+#: models.py:59 templates/fleetfinder/dashboard.html:17
+msgid "Fleet Commander"
+msgstr ""
+
+#: models.py:61
+msgid "Creation date and time"
+msgstr ""
+
+#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: templates/fleetfinder/edit-fleet.html:58
+msgid "Fleet MOTD"
+msgstr ""
+
+#: models.py:63
+msgid "Free move"
+msgstr ""
+
+#: models.py:69
+msgid "Group restrictions"
+msgstr ""
+
+#: models.py:77
+msgid "Last ESI error"
+msgstr ""
+
+#: models.py:81
+msgid "Last ESI error time"
+msgstr ""
+
+#: models.py:84
+msgid "ESI error count"
+msgstr ""
+
+#: templates/fleetfinder/create-fleet.html:5
+#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/partials/header/header-navigation.html:18
+msgid "Create Fleet"
+msgstr ""
+
+#: templates/fleetfinder/create-fleet.html:34
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:40
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all of the authed groups."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:63
-#: templates/fleetfinder/edit-fleet.html:58
-msgid "Fleet MOTD"
-msgstr ""
-
-#: templates/fleetfinder/create-fleet.html:73
+#: templates/fleetfinder/create-fleet.html:69
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:75
+#: templates/fleetfinder/create-fleet.html:71
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
 msgstr ""
 
-#: templates/fleetfinder/dashboard.html:17
-msgid "Fleet Commander"
-msgstr ""
-
 #: templates/fleetfinder/dashboard.html:18
 #: templates/fleetfinder/fleet-details.html:44
 msgid "Name"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:19
 msgid "Created At"
@@ -146,10 +194,12 @@
 msgid "View Fleet Details"
 msgstr ""
 
 #: views.py:99
 msgid "Edit Fleet Advert"
 msgstr ""
 
-#: views.py:248
-msgid "<h4>Error!</h4><p>Fleet advert is no longer valid</p>"
+#: views.py:243
+#, python-brace-format
+msgid ""
+"<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/locale/de/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.0/fleetfinder/locale/ja/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,158 +1,205 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-12 08:35+0200\n"
-"PO-Revision-Date: 2023-04-12 09:55+0000\n"
-"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetfinder/de/>\n"
-"Language: de\n"
+"POT-Creation-Date: 2023-06-28 15:41+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.4\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: auth_hooks.py:25 templates/fleetfinder/base.html:5
+#: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
-msgstr "Flottenfinder"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:18
-#: templates/fleetfinder/create-fleet.html:5
-msgid "Create Fleet"
-msgstr "Flotte erstellen"
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Fleet Finder v{__version__}"
+msgstr ""
+
+#: models.py:44
+msgid ""
+"FC is not in the registered fleet anymore or fleet is no longer available."
+msgstr ""
+
+#: models.py:46
+msgid "Registered fleet seems to be no longer available."
+msgstr ""
+
+#: models.py:47
+msgid "FC is no longer the fleet boss."
+msgstr ""
+
+#: models.py:48
+msgid "FC switched to another fleet."
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:29
+#: models.py:51 templates/fleetfinder/create-fleet.html:25
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
-msgstr "Flottenname"
+msgstr ""
+
+#: models.py:59 templates/fleetfinder/dashboard.html:17
+msgid "Fleet Commander"
+msgstr ""
+
+#: models.py:61
+msgid "Creation date and time"
+msgstr ""
+
+#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: templates/fleetfinder/edit-fleet.html:58
+msgid "Fleet MOTD"
+msgstr ""
+
+#: models.py:63
+msgid "Free move"
+msgstr ""
+
+#: models.py:69
+msgid "Group restrictions"
+msgstr ""
+
+#: models.py:77
+msgid "Last ESI error"
+msgstr ""
+
+#: models.py:81
+msgid "Last ESI error time"
+msgstr ""
+
+#: models.py:84
+msgid "ESI error count"
+msgstr ""
+
+#: templates/fleetfinder/create-fleet.html:5
+#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/partials/header/header-navigation.html:18
+msgid "Create Fleet"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:38
+#: templates/fleetfinder/create-fleet.html:34
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
-msgstr "Gruppenauswahl"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:40
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all of the authed groups."
 msgstr ""
-"Nur die ausgewählten Gruppen haben Zugriff zu dieser Flotte, Wenn keine "
-"Gruppen ausgewählt sind ist die Flotte für alle verfügbar."
 
-#: templates/fleetfinder/create-fleet.html:63
-#: templates/fleetfinder/edit-fleet.html:58
-msgid "Fleet MOTD"
-msgstr "Flotten MOTD"
-
-#: templates/fleetfinder/create-fleet.html:73
+#: templates/fleetfinder/create-fleet.html:69
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
-msgstr "Freie Bewegung aktiv"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:75
+#: templates/fleetfinder/create-fleet.html:71
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
-msgstr "Absenden"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
-msgstr "Verfügbare Flotten"
-
-#: templates/fleetfinder/dashboard.html:17
-msgid "Fleet Commander"
-msgstr "Flottenkommandant"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:18
 #: templates/fleetfinder/fleet-details.html:44
 msgid "Name"
-msgstr "Name"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:19
 msgid "Created At"
-msgstr "Erstellt um"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:20
 msgid "Join"
-msgstr "Beitreten"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:23
 msgid "Details"
-msgstr "Details"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr "Bearbeiten"
+msgstr ""
 
 #: templates/fleetfinder/edit-fleet.html:5
 #: templates/fleetfinder/edit-fleet.html:11
 msgid "Edit Fleet"
-msgstr "Flotte bearbeiten"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:5
 msgid "Fleet Details"
-msgstr "Flottendetails"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:13
 msgid "Fleet Composition"
-msgstr "Flottenzusammansetzung"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:21
 msgid "Ship Name"
-msgstr "Schiffsname"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:22
 msgid "Quantity"
-msgstr "Anzahl"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:36
 msgid "Fleet Members"
-msgstr "Flottenmitglieder"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:45
 msgid "Ship type"
-msgstr "Schiffstyp"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:46
 msgid "System"
-msgstr "System"
+msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:5 views.py:79
 msgid "Join Fleet"
-msgstr "Flotte beitreten"
+msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:11
 msgid "Fleet Invitation"
-msgstr "Flotteneinladung"
+msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
-msgstr "Wähle einzuladende Charaktere"
+msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
 msgid "Send fleet invite(s)"
-msgstr "Flotteneinladung(en) senden"
+msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
-msgstr "Navigation umschalten"
+msgstr ""
 
 #: views.py:92
 msgid "View Fleet Details"
-msgstr "Flottendetails anzeigen"
+msgstr ""
 
 #: views.py:99
 msgid "Edit Fleet Advert"
-msgstr "Flottenanzeige bearbeiten"
+msgstr ""
 
-#: views.py:248
-msgid "<h4>Error!</h4><p>Fleet advert is no longer valid</p>"
-msgstr "<h4>Fehler!</h4><p>Flottenanzeige ist nicht mehr gültig</p>"
+#: views.py:243
+#, python-brace-format
+msgid ""
+"<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo` & `aa_fleetfinder-1.3.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,86 +8,122 @@
 "apps/aa-fleetfinder/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.16.4\n"
+"X-Generator: Weblate 4.18.1\n"
 
-msgid "<h4>Error!</h4><p>Fleet advert is no longer valid</p>"
-msgstr "<h4>Ошибка!</h4><p>Оповещение некорректно</p>"
+msgid ""
+"<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
+msgstr ""
+"<h4>Ошибка!</h4><p>ESI вернул следующую ошибку: {esi_error_message}</p>"
 
 msgid "Available Fleets"
 msgstr "Доступные флота"
 
 msgid "Create Fleet"
 msgstr "Создание флота"
 
 msgid "Created At"
 msgstr "Создан"
 
+msgid "Creation date and time"
+msgstr "Дата и время создания"
+
 msgid "Details"
 msgstr "Подробности"
 
+msgid "ESI error count"
+msgstr "Счетчик ESI ошибок"
+
 msgid "Edit"
 msgstr "Редактировать"
 
 msgid "Edit Fleet"
 msgstr "Редактировать флот"
 
 msgid "Edit Fleet Advert"
 msgstr "Редактировать оповещение"
 
 msgid "Enable Free Move"
 msgstr "Разрешить Free Move"
 
+msgid "FC is no longer the fleet boss."
+msgstr "ФК больше не руководитель флота."
+
+msgid ""
+"FC is not in the registered fleet anymore or fleet is no longer available."
+msgstr "ФК больше не состоит в зарегистрированном флоте или флот недоступен."
+
+msgid "FC switched to another fleet."
+msgstr "ФК перешел в другой флот."
+
 msgid "Fleet Commander"
 msgstr "Командир флота"
 
 msgid "Fleet Composition"
 msgstr "Состав флота"
 
 msgid "Fleet Details"
 msgstr "Детальная информация"
 
 msgid "Fleet Finder"
 msgstr "Поиск флота"
 
+msgid "Fleet Finder v{__version__}"
+msgstr "Поиск флота v{__version__}"
+
 msgid "Fleet Invitation"
-msgstr "Приглашение"
+msgstr "Приглашение во флот"
 
 msgid "Fleet MOTD"
 msgstr "MOTD флота"
 
 msgid "Fleet Members"
 msgstr "Пилоты флота"
 
 msgid "Fleet Name"
 msgstr "Название флота"
 
+msgid "Free move"
+msgstr "Свободное перемещение"
+
+msgid "Group restrictions"
+msgstr "Ограничения групп"
+
 msgid "Join"
 msgstr "Присоединиться"
 
 msgid "Join Fleet"
-msgstr "Присоединиться"
+msgstr "Присоединиться к флоту"
+
+msgid "Last ESI error"
+msgstr "Последняя ESI ошибка"
+
+msgid "Last ESI error time"
+msgstr "Время последней ESI ошибки"
 
 msgid "Name"
 msgstr "Название"
 
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all of the authed groups."
 msgstr ""
 "Только выбранные группы будут иметь доступ к флоту. Если группы не выбраны, "
 "флот будет доступен всем авторизованным группам."
 
 msgid "Quantity"
 msgstr "Количество"
 
+msgid "Registered fleet seems to be no longer available."
+msgstr "Похоже, зарегистрированный флот больше недоступен."
+
 msgid "Select Groups"
 msgstr "Выбор групп"
 
 msgid "Select the characters to invite"
 msgstr "Выберите пилота для приглашения"
 
 msgid "Send fleet invite(s)"
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/locale/ru/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.0/fleetfinder/locale/uk/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,160 +1,209 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-12 08:35+0200\n"
-"PO-Revision-Date: 2023-04-21 14:50+0000\n"
-"Last-Translator: Nikolay <nick.postnikov@gmail.com>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetfinder/ru/>\n"
-"Language: ru\n"
+"POT-Creation-Date: 2023-06-28 15:41+0200\n"
+"PO-Revision-Date: 2023-06-29 14:19+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetfinder/uk/>\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.16.4\n"
+"X-Generator: Weblate 4.18.1\n"
 
-#: auth_hooks.py:25 templates/fleetfinder/base.html:5
+#: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
-msgstr "Поиск флота"
+msgstr "Пошук флоту"
 
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:18
-#: templates/fleetfinder/create-fleet.html:5
-msgid "Create Fleet"
-msgstr "Создание флота"
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Fleet Finder v{__version__}"
+msgstr "Пошук флоту v{__version__}"
+
+#: models.py:44
+msgid ""
+"FC is not in the registered fleet anymore or fleet is no longer available."
+msgstr ""
+
+#: models.py:46
+msgid "Registered fleet seems to be no longer available."
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:29
+#: models.py:47
+msgid "FC is no longer the fleet boss."
+msgstr ""
+
+#: models.py:48
+msgid "FC switched to another fleet."
+msgstr ""
+
+#: models.py:51 templates/fleetfinder/create-fleet.html:25
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
-msgstr "Название флота"
+msgstr "Назва флоту"
 
-#: templates/fleetfinder/create-fleet.html:38
+#: models.py:59 templates/fleetfinder/dashboard.html:17
+msgid "Fleet Commander"
+msgstr "Командувач флотом"
+
+#: models.py:61
+msgid "Creation date and time"
+msgstr ""
+
+#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: templates/fleetfinder/edit-fleet.html:58
+msgid "Fleet MOTD"
+msgstr "\"Шапка\" флоту"
+
+#: models.py:63
+#, fuzzy
+#| msgid "Enable Free Move"
+msgid "Free move"
+msgstr "Дозволити вільне переміщення"
+
+#: models.py:69
+msgid "Group restrictions"
+msgstr ""
+
+#: models.py:77
+msgid "Last ESI error"
+msgstr ""
+
+#: models.py:81
+msgid "Last ESI error time"
+msgstr ""
+
+#: models.py:84
+msgid "ESI error count"
+msgstr ""
+
+#: templates/fleetfinder/create-fleet.html:5
+#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/partials/header/header-navigation.html:18
+msgid "Create Fleet"
+msgstr "Створити флот"
+
+#: templates/fleetfinder/create-fleet.html:34
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
-msgstr "Выбор групп"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:40
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all of the authed groups."
 msgstr ""
-"Только выбранные группы будут иметь доступ к флоту. Если группы не выбраны, "
-"флот будет доступен всем авторизованным группам."
-
-#: templates/fleetfinder/create-fleet.html:63
-#: templates/fleetfinder/edit-fleet.html:58
-msgid "Fleet MOTD"
-msgstr "MOTD флота"
 
-#: templates/fleetfinder/create-fleet.html:73
+#: templates/fleetfinder/create-fleet.html:69
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
-msgstr "Разрешить Free Move"
+msgstr "Дозволити вільне переміщення"
 
-#: templates/fleetfinder/create-fleet.html:75
+#: templates/fleetfinder/create-fleet.html:71
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
-msgstr "Отправить"
+msgstr "Відправити"
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
-msgstr "Доступные флота"
-
-#: templates/fleetfinder/dashboard.html:17
-msgid "Fleet Commander"
-msgstr "Командир флота"
+msgstr "Доступні флоти"
 
 #: templates/fleetfinder/dashboard.html:18
 #: templates/fleetfinder/fleet-details.html:44
 msgid "Name"
-msgstr "Название"
+msgstr "Назва"
 
 #: templates/fleetfinder/dashboard.html:19
 msgid "Created At"
-msgstr "Создан"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:20
 msgid "Join"
-msgstr "Присоединиться"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:23
 msgid "Details"
-msgstr "Подробности"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr "Редактировать"
+msgstr "Редагувати"
 
 #: templates/fleetfinder/edit-fleet.html:5
 #: templates/fleetfinder/edit-fleet.html:11
 msgid "Edit Fleet"
-msgstr "Редактировать флот"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:5
 msgid "Fleet Details"
-msgstr "Детальная информация"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:13
 msgid "Fleet Composition"
-msgstr "Состав флота"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:21
 msgid "Ship Name"
-msgstr "Название корабля"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:22
 msgid "Quantity"
-msgstr "Количество"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:36
 msgid "Fleet Members"
-msgstr "Пилоты флота"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:45
 msgid "Ship type"
-msgstr "Тип корабля"
+msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:46
 msgid "System"
 msgstr "Система"
 
 #: templates/fleetfinder/join-fleet.html:5 views.py:79
 msgid "Join Fleet"
-msgstr "Присоединиться"
+msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:11
 msgid "Fleet Invitation"
-msgstr "Приглашение"
+msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
-msgstr "Выберите пилота для приглашения"
+msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
 msgid "Send fleet invite(s)"
-msgstr "Отправить приглашение(я)"
+msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
-msgstr "Переключить навигацию"
+msgstr ""
 
 #: views.py:92
 msgid "View Fleet Details"
-msgstr "Показать подробности"
+msgstr ""
 
 #: views.py:99
 msgid "Edit Fleet Advert"
-msgstr "Редактировать оповещение"
+msgstr ""
 
-#: views.py:248
-msgid "<h4>Error!</h4><p>Fleet advert is no longer valid</p>"
-msgstr "<h4>Ошибка!</h4><p>Оповещение некорректно</p>"
+#: views.py:243
+#, python-brace-format
+msgid ""
+"<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
+msgstr ""
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/locale/uk/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -4,76 +4,122 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 01:20+0200\n"
+"POT-Creation-Date: 2023-06-28 15:41+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural= n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : n"
-"%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: auth_hooks.py:25 templates/fleetfinder/base.html:5
+#: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:18
-msgid "Create Fleet"
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Fleet Finder v{__version__}"
+msgstr ""
+
+#: models.py:44
+msgid ""
+"FC is not in the registered fleet anymore or fleet is no longer available."
+msgstr ""
+
+#: models.py:46
+msgid "Registered fleet seems to be no longer available."
+msgstr ""
+
+#: models.py:47
+msgid "FC is no longer the fleet boss."
+msgstr ""
+
+#: models.py:48
+msgid "FC switched to another fleet."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:29
+#: models.py:51 templates/fleetfinder/create-fleet.html:25
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
-msgstr "Назва флоту"
+msgstr ""
+
+#: models.py:59 templates/fleetfinder/dashboard.html:17
+msgid "Fleet Commander"
+msgstr ""
+
+#: models.py:61
+msgid "Creation date and time"
+msgstr ""
+
+#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: templates/fleetfinder/edit-fleet.html:58
+msgid "Fleet MOTD"
+msgstr ""
+
+#: models.py:63
+msgid "Free move"
+msgstr ""
+
+#: models.py:69
+msgid "Group restrictions"
+msgstr ""
+
+#: models.py:77
+msgid "Last ESI error"
+msgstr ""
+
+#: models.py:81
+msgid "Last ESI error time"
+msgstr ""
+
+#: models.py:84
+msgid "ESI error count"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:38
+#: templates/fleetfinder/create-fleet.html:5
+#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/partials/header/header-navigation.html:18
+msgid "Create Fleet"
+msgstr ""
+
+#: templates/fleetfinder/create-fleet.html:34
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:40
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all of the authed groups."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:63
-#: templates/fleetfinder/edit-fleet.html:58
-msgid "Fleet MOTD"
-msgstr ""
-
-#: templates/fleetfinder/create-fleet.html:73
+#: templates/fleetfinder/create-fleet.html:69
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:75
+#: templates/fleetfinder/create-fleet.html:71
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
 msgstr ""
 
-#: templates/fleetfinder/dashboard.html:17
-msgid "Fleet Commander"
-msgstr ""
-
 #: templates/fleetfinder/dashboard.html:18
 #: templates/fleetfinder/fleet-details.html:44
 msgid "Name"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:19
 msgid "Created At"
@@ -85,15 +131,15 @@
 
 #: templates/fleetfinder/dashboard.html:23
 msgid "Details"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr "Редагувати"
+msgstr ""
 
 #: templates/fleetfinder/edit-fleet.html:5
 #: templates/fleetfinder/edit-fleet.html:11
 msgid "Edit Fleet"
 msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:5
@@ -148,10 +194,12 @@
 msgid "View Fleet Details"
 msgstr ""
 
 #: views.py:99
 msgid "Edit Fleet Advert"
 msgstr ""
 
-#: views.py:248
-msgid "<h4>Error!</h4><p>Fleet advert is no longer valid</p>"
+#: views.py:243
+#, python-brace-format
+msgid ""
+"<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/migrations/0001_initial.py` & `aa_fleetfinder-1.3.0/fleetfinder/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # Django
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("eveonline", "0017_alliance_and_corp_names_are_not_unique"),
         ("groupmanagement", "0019_adding_restricted_to_groups"),
     ]
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/fleetfinder.css` & `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/fleetfinder.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js` & `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js` & `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css` & `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css` & `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js` & `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/create-fleet.html` & `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/edit-fleet.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 {% extends "fleetfinder/base.html" %}
 
 {% load i18n %}
 
-{% block page_title %}{% translate "Create Fleet" %}{% endblock %}
+{% block page_title %}{% translate "Edit Fleet" %}{% endblock %}
 
 {% block fleetfinder_block %}
-    {% if error %}
-        <div class="alert alert-danger" role="alert">{{ error }}</div>
-    {%endif%}
-
     <div class="panel panel-primary">
         <div class="panel-heading">
-            <div class="panel-title">{% translate "Create Fleet" %}</div>
+            <div class="panel-title">
+                {% translate "Edit Fleet" %}
+            </div>
         </div>
 
         <div class="panel-body">
             <div class="row">
                 <div class="col-md-10 col-md-offset-1">
                     <form class="form-signin" role="form" action="{% url 'fleetfinder:save_fleet' %}" method="POST">
                         {% csrf_token %}
 
                         <input type="hidden" name="character_id" id="character_id" value="{{ character_id }}">
-                        <input type="hidden" name="origin" id="origin" value="create">
+                        <input type="hidden" name="origin" id="origin" value="edit">
 
                         <div class="row">
                             <div class="col-sm-12">
                                 <div class="form-group">
                                     <label for="name" class="control-label">{% translate "Fleet Name" %}</label>
-                                    <input type="text" class="form-control" name="name" id="name" {% if name %}value="{{ name }}"{% endif %}>
+                                    <input type="text" class="form-control" name="name" id="name" value="{{ fleet.name }}">
                                 </div>
                             </div>
                         </div>
 
                         <div class="row">
                             <div class="col-sm-12">
                                 <div class="form-group">
                                     <label for="groups" style="margin-bottom: 0;">{% translate "Select Groups" %}</label>
+
                                     <span class="help-block text-small">
                                         {% translate "Only selected groups will have access to the fleet. If no groups are selected the fleet will be available to all of the authed groups." %}
                                     </span>
 
                                     <select name="groups" id="groups" multiple>
                                         {% for group in auth_groups %}
-                                            {% if groups %}
-                                                {% if group in groups %}
-                                                    <option value="{{ group.group_id }}" selected>{{ group }}</option>
-                                                {% else %}
-                                                    <option value="{{ group.group_id }}" selected>{{ group }}</option>
-                                                {% endif %}
+                                            {% if group in fleet.groups.all %}
+                                                <option value="{{ group.group_id }}" selected>{{ group }}</option>
                                             {% else %}
                                                 <option value="{{ group.group_id }}">{{ group }}</option>
                                             {% endif %}
                                         {% endfor %}
                                     </select>
                                 </div>
                             </div>
@@ -59,21 +54,21 @@
 
                         <div class="row">
                             <div class="col-sm-12">
                                 <div class="form-group" >
                                     <label for="motd" class="control-label">{% translate "Fleet MOTD" %}</label>
 
                                     <div>
-                                        <textarea class="form-control" name="motd" id="motd" rows="10">{% if motd %}{{ motd }}{% endif %}</textarea>
+                                        <textarea class="form-control" name="motd" id="motd" rows="10">{{ fleet.motd }}</textarea>
                                     </div>
                                 </div>
                             </div>
                         </div>
 
-                        <input type="checkbox" style="margin-right: 5px;" class="form-check-input" name="free_move" id="free_move" {% if is_free_move %}checked{% endif %}>
+                        <input type="checkbox" style="margin-right: 5px;" class="form-check-input" name="free_move" id="free_move"{% if fleet.is_free_move %} checked{% endif %}>
                         <label for="free_move" class="form-check-label">{% translate "Enable Free Move" %}</label>
 
                         <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                     </form>
                 </div>
             </div>
         </div>
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/dashboard.html` & `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/edit-fleet.html` & `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/create-fleet.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 {% extends "fleetfinder/base.html" %}
 
 {% load i18n %}
 
-{% block page_title %}{% translate "Edit Fleet" %}{% endblock %}
+{% block page_title %}{% translate "Create Fleet" %}{% endblock %}
 
 {% block fleetfinder_block %}
     <div class="panel panel-primary">
         <div class="panel-heading">
-            <div class="panel-title">
-                {% translate "Edit Fleet" %}
-            </div>
+            <div class="panel-title">{% translate "Create Fleet" %}</div>
         </div>
 
         <div class="panel-body">
             <div class="row">
                 <div class="col-md-10 col-md-offset-1">
                     <form class="form-signin" role="form" action="{% url 'fleetfinder:save_fleet' %}" method="POST">
                         {% csrf_token %}
 
                         <input type="hidden" name="character_id" id="character_id" value="{{ character_id }}">
-                        <input type="hidden" name="origin" id="origin" value="edit">
+                        <input type="hidden" name="origin" id="origin" value="create">
 
                         <div class="row">
                             <div class="col-sm-12">
                                 <div class="form-group">
                                     <label for="name" class="control-label">{% translate "Fleet Name" %}</label>
-                                    <input type="text" class="form-control" name="name" id="name" value="{{ fleet.name }}">
+                                    <input type="text" class="form-control" name="name" id="name" {% if name %}value="{{ name }}"{% endif %}>
                                 </div>
                             </div>
                         </div>
 
                         <div class="row">
                             <div class="col-sm-12">
                                 <div class="form-group">
                                     <label for="groups" style="margin-bottom: 0;">{% translate "Select Groups" %}</label>
-
                                     <span class="help-block text-small">
                                         {% translate "Only selected groups will have access to the fleet. If no groups are selected the fleet will be available to all of the authed groups." %}
                                     </span>
 
                                     <select name="groups" id="groups" multiple>
                                         {% for group in auth_groups %}
-                                            {% if group in fleet.groups.all %}
-                                                <option value="{{ group.group_id }}" selected>{{ group }}</option>
+                                            {% if groups %}
+                                                {% if group in groups %}
+                                                    <option value="{{ group.group_id }}" selected>{{ group }}</option>
+                                                {% else %}
+                                                    <option value="{{ group.group_id }}" selected>{{ group }}</option>
+                                                {% endif %}
                                             {% else %}
                                                 <option value="{{ group.group_id }}">{{ group }}</option>
                                             {% endif %}
                                         {% endfor %}
                                     </select>
                                 </div>
                             </div>
@@ -54,21 +55,21 @@
 
                         <div class="row">
                             <div class="col-sm-12">
                                 <div class="form-group" >
                                     <label for="motd" class="control-label">{% translate "Fleet MOTD" %}</label>
 
                                     <div>
-                                        <textarea class="form-control" name="motd" id="motd" rows="10">{{ fleet.motd }}</textarea>
+                                        <textarea class="form-control" name="motd" id="motd" rows="10">{% if motd %}{{ motd }}{% endif %}</textarea>
                                     </div>
                                 </div>
                             </div>
                         </div>
 
-                        <input type="checkbox" style="margin-right: 5px;" class="form-check-input" name="free_move" id="free_move"{% if fleet.is_free_move %} checked{% endif %}>
+                        <input type="checkbox" style="margin-right: 5px;" class="form-check-input" name="free_move" id="free_move" {% if is_free_move %}checked{% endif %}>
                         <label for="free_move" class="form-check-label">{% translate "Enable Free Move" %}</label>
 
                         <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                     </form>
                 </div>
             </div>
         </div>
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/fleet-details.html` & `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/join-fleet.html` & `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/join-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html` & `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/templatetags/fleetfinder_versioned_static.py` & `aa_fleetfinder-1.3.0/fleetfinder/templatetags/fleetfinder_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/tests/test_access.py` & `aa_fleetfinder-1.3.0/fleetfinder/tests/test_access.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from django.urls import reverse
 
 # AA Fleet Finder
 from fleetfinder.tests.utils import create_fake_user
 
 
 class TestAccess(TestCase):
+    """
+    Testing module access
+    """
+
     @classmethod
     def setUpClass(cls) -> None:
         """
         Set up groups and users
         """
 
         super().setUpClass()
@@ -31,30 +35,30 @@
         # User can access fleetfinder
         cls.user_1002 = create_fake_user(
             1002, "Bruce Wayne", permissions=["fleetfinder.access_fleetfinder"]
         )
 
     def test_has_no_access(self):
         """
-        Test that a user without access get a 302
+        Test that a user without access gets a 302
         :return:
         """
 
         # given
         self.client.force_login(self.user_1001)
 
         # when
         res = self.client.get(reverse("fleetfinder:dashboard"))
 
         # then
         self.assertEqual(res.status_code, HTTPStatus.FOUND)
 
     def test_has_access(self):
         """
-        Test that a user with access get to see it
+        Test that a user with access gets to see it
         :return:
         """
 
         # given
         self.client.force_login(self.user_1002)
 
         # when
```

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/tests/test_auth_hooks.py` & `aa_fleetfinder-1.3.0/fleetfinder/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/tests/test_templatetags.py` & `aa_fleetfinder-1.3.0/fleetfinder/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/fleetfinder/tests/utils.py` & `aa_fleetfinder-1.3.0/fleetfinder/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     corporation_name: str = None,
     corporation_ticker: str = None,
     alliance_id: int = None,
     alliance_name: str = None,
     permissions: List[str] = None,
 ) -> User:
     """
-    Create a fake user incl. main character and (optional) permissions.
+    Create a fake user incl. Main character and (optional) permissions.
     """
 
     username = re.sub(r"[^\w\d@\.\+-]", "_", character_name)
     user = AuthUtils.create_user(username)
 
     if not corporation_id:
         corporation_id = 2001
```

### Comparing `aa_fleetfinder-1.2.0/LICENSE` & `aa_fleetfinder-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.2.0/README.md` & `aa_fleetfinder-1.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 [![Python](https://img.shields.io/pypi/pyversions/aa-fleetfinder)](https://pypi.org/project/aa-fleetfinder/)
 [![Django](https://img.shields.io/pypi/djversions/aa-fleetfinder?label=django)](https://pypi.org/project/aa-fleetfinder/)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](http://black.readthedocs.io/en/latest/)
 [![Discord](https://img.shields.io/discord/790364535294132234?label=discord)](https://discord.gg/zmh52wnfvM)
 [![Checks](https://github.com/ppfeufer/aa-fleetfinder/actions/workflows/automated-checks.yml/badge.svg)](https://github.com/ppfeufer/aa-fleetfinder/actions/workflows/automated-checks.yml)
 [![codecov](https://codecov.io/gh/ppfeufer/aa-fleetfinder/branch/master/graph/badge.svg?token=GFOR9GWRNQ)](https://codecov.io/gh/ppfeufer/aa-fleetfinder)
+[![Translation Status](https://weblate.ppfeufer.de/widgets/alliance-auth-apps/-/aa-fleetfinder/svg-badge.svg)](https://weblate.ppfeufer.de/engage/alliance-auth-apps/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-fleetfinder/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Control access to your fleets through Alliance Auth.
 
+---
 
 <!-- TOC -->
 * [AA Fleet Finder](#aa-fleet-finder)
   * [Installation](#installation)
     * [Step 1: Install the Package](#step-1-install-the-package)
     * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
     * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
     * [Step 4: Setup Permissions](#step-4-setup-permissions)
   * [Changelog](#changelog)
   * [Contributing](#contributing)
 <!-- TOC -->
 
+---
+
 
 ## Installation
 
 ### Step 1: Install the Package
 
 Make sure you're in the virtual environment (venv) of your Alliance Auth installation Then install the latest release directly from PyPi.
```

### Comparing `aa_fleetfinder-1.2.0/pyproject.toml` & `aa_fleetfinder-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aa-fleetfinder"
-version = "1.2.0"
+version = "1.3.0"
 description = "Fleet finder plugin for Alliance Auth"
 readme = "README.md"
 license = "GPL-3.0"
 requires-python = "~=3.8"
 authors = [
     { name = "Peter Pfeufer", email = "develop@ppfeufer.de" },
 ]
```

### Comparing `aa_fleetfinder-1.2.0/PKG-INFO` & `aa_fleetfinder-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-fleetfinder
-Version: 1.2.0
+Version: 1.3.0
 Summary: Fleet finder plugin for Alliance Auth
 Project-URL: Homepage, https://github.com/ppfeufer/aa-fleetfinder
 Project-URL: Documentation, https://github.com/ppfeufer/aa-fleetfinder/blob/master/README.md
 Project-URL: Source, https://github.com/ppfeufer/aa-fleetfinder.git
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetfinder/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/ppfeufer/aa-fleetfinder/issues
 Author-email: Peter Pfeufer <develop@ppfeufer.de>
@@ -37,32 +37,36 @@
 [![Python](https://img.shields.io/pypi/pyversions/aa-fleetfinder)](https://pypi.org/project/aa-fleetfinder/)
 [![Django](https://img.shields.io/pypi/djversions/aa-fleetfinder?label=django)](https://pypi.org/project/aa-fleetfinder/)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](http://black.readthedocs.io/en/latest/)
 [![Discord](https://img.shields.io/discord/790364535294132234?label=discord)](https://discord.gg/zmh52wnfvM)
 [![Checks](https://github.com/ppfeufer/aa-fleetfinder/actions/workflows/automated-checks.yml/badge.svg)](https://github.com/ppfeufer/aa-fleetfinder/actions/workflows/automated-checks.yml)
 [![codecov](https://codecov.io/gh/ppfeufer/aa-fleetfinder/branch/master/graph/badge.svg?token=GFOR9GWRNQ)](https://codecov.io/gh/ppfeufer/aa-fleetfinder)
+[![Translation Status](https://weblate.ppfeufer.de/widgets/alliance-auth-apps/-/aa-fleetfinder/svg-badge.svg)](https://weblate.ppfeufer.de/engage/alliance-auth-apps/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-fleetfinder/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Control access to your fleets through Alliance Auth.
 
+---
 
 <!-- TOC -->
 * [AA Fleet Finder](#aa-fleet-finder)
   * [Installation](#installation)
     * [Step 1: Install the Package](#step-1-install-the-package)
     * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
     * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
     * [Step 4: Setup Permissions](#step-4-setup-permissions)
   * [Changelog](#changelog)
   * [Contributing](#contributing)
 <!-- TOC -->
 
+---
+
 
 ## Installation
 
 ### Step 1: Install the Package
 
 Make sure you're in the virtual environment (venv) of your Alliance Auth installation Then install the latest release directly from PyPi.
```

