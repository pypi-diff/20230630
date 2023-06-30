# Comparing `tmp/inmanta_module_postgresql-0.4.2-py3-none-any.whl.zip` & `tmp/inmanta_module_postgresql-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 26409 bytes, number of entries: 14
--rw-rw-r--  2.0 unx      623 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/__init__.py
--rw-rw-r--  2.0 unx     6551 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/resources.py
--rw-rw-r--  2.0 unx      849 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/setup.cfg
--rw-rw-r--  2.0 unx     5418 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/model/_init.cf
--rw-rw-r--  2.0 unx     4259 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/model/ha.cf
--rw-rw-r--  2.0 unx     4712 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/templates/pg_hba.conf.j2
--rw-rw-r--  2.0 unx     4870 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/templates/pg_hba_master.conf.j2
--rw-rw-r--  2.0 unx    23038 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/templates/postgresql.conf.j2
--rw-rw-r--  2.0 unx    22906 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/templates/postgresql_master.conf.j2
--rw-rw-r--  2.0 unx      340 b- defN 23-May-03 05:50 inmanta_plugins/postgresql/templates/recovery.conf.j2
--rw-rw-r--  2.0 unx      260 b- defN 23-May-03 05:50 inmanta_module_postgresql-0.4.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-03 05:50 inmanta_module_postgresql-0.4.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-May-03 05:50 inmanta_module_postgresql-0.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1409 b- defN 23-May-03 05:50 inmanta_module_postgresql-0.4.2.dist-info/RECORD
-14 files, 75343 bytes uncompressed, 23981 bytes compressed:  68.2%
+Zip file size: 26410 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx      623 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/__init__.py
+-rw-rw-r--  2.0 unx     6551 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/resources.py
+-rw-rw-r--  2.0 unx      849 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/setup.cfg
+-rw-rw-r--  2.0 unx     5418 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/model/_init.cf
+-rw-rw-r--  2.0 unx     4259 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/model/ha.cf
+-rw-rw-r--  2.0 unx     4712 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/templates/pg_hba.conf.j2
+-rw-rw-r--  2.0 unx     4870 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/templates/pg_hba_master.conf.j2
+-rw-rw-r--  2.0 unx    23038 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/templates/postgresql.conf.j2
+-rw-rw-r--  2.0 unx    22906 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/templates/postgresql_master.conf.j2
+-rw-rw-r--  2.0 unx      340 b- defN 23-Jun-30 09:07 inmanta_plugins/postgresql/templates/recovery.conf.j2
+-rw-rw-r--  2.0 unx      260 b- defN 23-Jun-30 09:07 inmanta_module_postgresql-0.4.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-30 09:07 inmanta_module_postgresql-0.4.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jun-30 09:07 inmanta_module_postgresql-0.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Jun-30 09:07 inmanta_module_postgresql-0.4.3.dist-info/RECORD
+14 files, 75343 bytes uncompressed, 23982 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: inmanta_plugins/postgresql/templates/postgresql_master.conf.j2
 Comment: 
 
 Filename: inmanta_plugins/postgresql/templates/recovery.conf.j2
 Comment: 
 
-Filename: inmanta_module_postgresql-0.4.2.dist-info/METADATA
+Filename: inmanta_module_postgresql-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_postgresql-0.4.2.dist-info/WHEEL
+Filename: inmanta_module_postgresql-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_postgresql-0.4.2.dist-info/top_level.txt
+Filename: inmanta_module_postgresql-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_postgresql-0.4.2.dist-info/RECORD
+Filename: inmanta_module_postgresql-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/postgresql/setup.cfg

```diff
@@ -19,15 +19,15 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-postgresql
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.4.2
+version = 0.4.3
 license = Apache 2.0
 version_tag = 
 
 [options]
 install_requires = inmanta-module-exec
 	inmanta-module-ip
 	inmanta-module-ssh
```

## Comparing `inmanta_module_postgresql-0.4.2.dist-info/RECORD` & `inmanta_module_postgresql-0.4.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 inmanta_plugins/postgresql/__init__.py,sha256=YoYA_JM47oSvILkupBV5bTcabcPpPr-4T_Go2e_ohVI,623
 inmanta_plugins/postgresql/resources.py,sha256=6864Sk50rqWjgylTVfE2t9NRAj6eeu6CqC1Cfsu2jMQ,6551
-inmanta_plugins/postgresql/setup.cfg,sha256=ZqNrtEE1CS2s5stPumFk-HARzhFdnJoZs3vcnq0xFck,849
+inmanta_plugins/postgresql/setup.cfg,sha256=HrRPToeySD_AGYWlk8HS72UMVD2Hv_ow9wFZDkFF97U,849
 inmanta_plugins/postgresql/model/_init.cf,sha256=jF-VXw3ybXjXciSQ8hOpr6IT5kJ2oCxz2Ge2T_Xpqp0,5418
 inmanta_plugins/postgresql/model/ha.cf,sha256=zt5IdcXyRyGZahPXLJXRlU6V6-06MLAB8nC-RI04yE8,4259
 inmanta_plugins/postgresql/templates/pg_hba.conf.j2,sha256=Ln_eRTiO1MGBjyvp_XD6Ta2l5Jf_irVtsYjzirIUtmg,4712
 inmanta_plugins/postgresql/templates/pg_hba_master.conf.j2,sha256=uVesRjWzUYIV10k6TcraT9e6QYzQaXxlclRitLxNMe8,4870
 inmanta_plugins/postgresql/templates/postgresql.conf.j2,sha256=5EbUebOxp6KlXTeVxqxGV20WchDZ-G_OnkUtcqdtbsw,23038
 inmanta_plugins/postgresql/templates/postgresql_master.conf.j2,sha256=IUdY8a1F301_qRirE2LR0WjGQgosqLqbeDRYjDWy2Hs,22906
 inmanta_plugins/postgresql/templates/recovery.conf.j2,sha256=XsbCT7XkMyvs8Dq2o8jhIBmIfC4S816lITPydwzTi_E,340
-inmanta_module_postgresql-0.4.2.dist-info/METADATA,sha256=fBvYY5s8ndF2iHPcMxb8WmDxWg6wG6iwTzsgIAUjIPw,260
-inmanta_module_postgresql-0.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-inmanta_module_postgresql-0.4.2.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_postgresql-0.4.2.dist-info/RECORD,,
+inmanta_module_postgresql-0.4.3.dist-info/METADATA,sha256=qkTy7Mn3_bo_6h3lFZfbGvnAoelMsgGBCkfq3j9TRzU,260
+inmanta_module_postgresql-0.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+inmanta_module_postgresql-0.4.3.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_postgresql-0.4.3.dist-info/RECORD,,
```

