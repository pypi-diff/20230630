# Comparing `tmp/django_simple_accounting-0.1.3.tar.gz` & `tmp/django_simple_accounting-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_accounting-0.1.3.tar", max compression
+gzip compressed data, was "django_simple_accounting-0.1.4.tar", max compression
```

## Comparing `django_simple_accounting-0.1.3.tar` & `django_simple_accounting-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/LICENSE
--rw-r--r--   0        0        0      738 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/README.md
--rw-r--r--   0        0        0      510 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/simple_accounting/__init__.py
--rw-r--r--   0        0        0      606 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/simple_accounting/admin.py
--rw-r--r--   0        0        0     3407 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/simple_accounting/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/simple_accounting/migrations/__init__.py
--rw-r--r--   0        0        0     3352 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/simple_accounting/models.py
--rw-r--r--   0        0        0      603 2023-06-30 08:08:48.827607 django_simple_accounting-0.1.3/simple_accounting/utils.py
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 django_simple_accounting-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-30 11:13:14.042378 django_simple_accounting-0.1.4/LICENSE
+-rw-r--r--   0        0        0      738 2023-06-30 11:13:14.042378 django_simple_accounting-0.1.4/README.md
+-rw-r--r--   0        0        0      534 2023-06-30 11:13:14.046378 django_simple_accounting-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 11:13:14.046378 django_simple_accounting-0.1.4/simple_accounting/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-30 11:13:14.046378 django_simple_accounting-0.1.4/simple_accounting/admin.py
+-rw-r--r--   0        0        0     3407 2023-06-30 11:13:14.046378 django_simple_accounting-0.1.4/simple_accounting/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-30 11:13:14.046378 django_simple_accounting-0.1.4/simple_accounting/migrations/__init__.py
+-rw-r--r--   0        0        0     3494 2023-06-30 11:13:14.046378 django_simple_accounting-0.1.4/simple_accounting/models.py
+-rw-r--r--   0        0        0      603 2023-06-30 11:13:14.046378 django_simple_accounting-0.1.4/simple_accounting/utils.py
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 django_simple_accounting-0.1.4/PKG-INFO
```

### Comparing `django_simple_accounting-0.1.3/LICENSE` & `django_simple_accounting-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.3/README.md` & `django_simple_accounting-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.3/simple_accounting/migrations/0001_initial.py` & `django_simple_accounting-0.1.4/simple_accounting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.3/simple_accounting/models.py` & `django_simple_accounting-0.1.4/simple_accounting/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     owner = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         on_delete=models.deletion.CASCADE
     )
 
     posted_timestamp = models.DateTimeField(
-        help_text=_("Time the transaction was posted. Change this field to model retroactive ledger entries."),
+        help_text=_("Time the transaction was posted."),
         db_index=True
     )
 
     created_at = models.DateTimeField(
         auto_now_add=True
     )
     updated_at = models.DateTimeField(auto_now=True, blank=True, null=True)
@@ -86,27 +86,51 @@
 class TransactionEvidence(models.Model):
     OBJECT_TYPE_ORDER = 0
 
     OBJECT_TYPES = [
         (OBJECT_TYPE_ORDER, _("Order"))
     ]
 
-    transaction = models.ForeignKey(Transaction, on_delete=models.CASCADE, related_name="evidences")
+    transaction = models.ForeignKey(
+        Transaction,
+        on_delete=models.CASCADE,
+        related_name="evidences"
+    )
     object_type = models.IntegerField(choices=OBJECT_TYPES)
     object_id = models.IntegerField()
 
     def __str__(self):
-        return f"Type: {self.object_type}, Object ID: {self.object_id} to Transaction: {self.transaction}"
+        return f"Type: {self.object_type}, "\
+            "Object ID: {self.object_id} to Transaction: {self.transaction}"
 
 
 class LedgerEntry(models.Model):
-    ledger = models.ForeignKey(Ledger, on_delete=models.CASCADE, related_name="entries")
-    transaction = models.ForeignKey(Transaction, on_delete=models.CASCADE, related_name="entries")
+    ledger = models.ForeignKey(
+        Ledger,
+        on_delete=models.CASCADE,
+        related_name="entries"
+    )
+    transaction = models.ForeignKey(
+        Transaction,
+        on_delete=models.CASCADE,
+        related_name="entries"
+    )
 
-    debit = models.DecimalField(max_digits=15, decimal_places=2, null=True, blank=True)
-    credit = models.DecimalField(max_digits=15, decimal_places=2, null=True, blank=True)
+    debit = models.DecimalField(
+        max_digits=15,
+        decimal_places=2,
+        null=True,
+        blank=True
+    )
+    credit = models.DecimalField(
+        max_digits=15,
+        decimal_places=2,
+        null=True,
+        blank=True
+    )
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True, blank=True, null=True)
 
     def __str__(self):
-        return f"Entry: DEBIT: {self.debit} CREDIT: {self.credit} Ledger: {self.ledger}"
+        return f"Entry: DEBIT: {self.debit}"\
+            "CREDIT: {self.credit} Ledger: {self.ledger}"
```

### Comparing `django_simple_accounting-0.1.3/simple_accounting/utils.py` & `django_simple_accounting-0.1.4/simple_accounting/utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.3/PKG-INFO` & `django_simple_accounting-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: django-simple-accounting
-Version: 0.1.3
+Version: 0.1.4
 Summary: Plain and simple accounting module for Django
 License: MIT
 Author: Šarūnas Navickas
 Author-email: sarunas@griaustinis.lt
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # django-simple-accounting
 Plain and Simple Accounting module for Django
```

