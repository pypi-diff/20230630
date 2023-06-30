# Comparing `tmp/veerum-sdk-5.1.12.tar.gz` & `tmp/veerum-sdk-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veerum-sdk-5.1.12.tar", last modified: Thu Jun 29 20:46:48 2023, max compression
+gzip compressed data, was "veerum-sdk-5.2.0.tar", last modified: Fri Jun 30 17:51:58 2023, max compression
```

## Comparing `veerum-sdk-5.1.12.tar` & `veerum-sdk-5.2.0.tar`

### file list

```diff
@@ -1,220 +1,225 @@
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.544002 veerum-sdk-5.1.12/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)       76 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/MANIFEST.in
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6502 2023-06-29 20:46:48.543763 veerum-sdk-5.1.12/PKG-INFO
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6037 2023-06-26 19:27:33.000000 veerum-sdk-5.1.12/README.md
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)       38 2023-06-29 20:46:48.544057 veerum-sdk-5.1.12/setup.cfg
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1230 2023-06-29 20:46:42.000000 veerum-sdk-5.1.12/setup.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.501028 veerum-sdk-5.1.12/veerum/
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.503367 veerum-sdk-5.1.12/veerum/cli/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     5074 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/__init__.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.504627 veerum-sdk-5.1.12/veerum/cli/annotations/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      637 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/annotations/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      323 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/annotations/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1510 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/annotations/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      327 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/annotations/inspect.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.505274 veerum-sdk-5.1.12/veerum/cli/automations/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      634 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/automations/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      523 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/automations/relationship.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      674 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/automations/sync.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      780 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/common.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      338 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/debug.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.506917 veerum-sdk-5.1.12/veerum/cli/files/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      709 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/files/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      298 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/files/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1046 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/files/download.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1721 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/files/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      317 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/files/inspect.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      883 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/files/update.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2082 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/files/upload.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.507854 veerum-sdk-5.1.12/veerum/cli/jobs/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      654 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/jobs/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      262 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/jobs/misplaced_objects.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      298 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/jobs/populate_keys.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      274 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/jobs/warn_inactive_users.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.508660 veerum-sdk-5.1.12/veerum/cli/metadata/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      640 2023-06-26 19:27:33.000000 veerum-sdk-5.1.12/veerum/cli/metadata/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1047 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/metadata/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      342 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/metadata/inspect.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.509913 veerum-sdk-5.1.12/veerum/cli/metadata/keys/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      526 2023-06-26 19:27:33.000000 veerum-sdk-5.1.12/veerum/cli/metadata/keys/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      450 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/metadata/keys/add.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      340 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/metadata/keys/clear.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      566 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/metadata/keys/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      468 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/metadata/keys/set.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.510403 veerum-sdk-5.1.12/veerum/cli/metadata/upload/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3054 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/metadata/upload/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      505 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/metadata/upload/csvparser.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.511790 veerum-sdk-5.1.12/veerum/cli/milestones/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      694 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/milestones/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1595 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/milestones/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      318 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/milestones/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1004 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/milestones/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      342 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/milestones/inspect.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1725 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/milestones/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.512980 veerum-sdk-5.1.12/veerum/cli/models/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      747 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      302 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/delete.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.513228 veerum-sdk-5.1.12/veerum/cli/models/download/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      434 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/download/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1458 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      322 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/inspect.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.514001 veerum-sdk-5.1.12/veerum/cli/models/metadata/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      492 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/metadata/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      376 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/metadata/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      637 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/metadata/set.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1368 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.515549 veerum-sdk-5.1.12/veerum/cli/models/upload/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      112 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/upload/__helpers.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     7122 2023-06-20 21:00:34.000000 veerum-sdk-5.1.12/veerum/cli/models/upload/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3066 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/upload/potree.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      749 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/upload/potree2.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1373 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/upload/tiles.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1506 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/models/upload/unity.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.517306 veerum-sdk-5.1.12/veerum/cli/objects/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      857 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      574 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      378 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/deleteone.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2509 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/fileparser.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      714 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6109 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/ingest.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      389 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/inspect.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2642 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.517743 veerum-sdk-5.1.12/veerum/cli/objects/upload/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      112 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/upload/__helpers.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3073 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/objects/upload/__init__.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.519185 veerum-sdk-5.1.12/veerum/cli/organizations/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      746 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2712 2023-06-20 21:00:34.000000 veerum-sdk-5.1.12/veerum/cli/organizations/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      336 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      537 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      358 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/inspect.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.520092 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      637 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      379 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      370 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      528 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/integrations_shared.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.520774 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/iol_sap/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      466 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/iol_sap/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      389 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/iol_sap/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      449 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/iol_sap/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.521679 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/maximo/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      464 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/maximo/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      479 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/maximo/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      278 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/maximo/maximo_shared.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      546 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/maximo/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.522615 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/pi_system/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      470 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/pi_system/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      563 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/pi_system/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      766 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/pi_system/pi_shared.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      621 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/pi_system/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.523331 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/watson_ir/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      470 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/watson_ir/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      408 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/watson_ir/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      451 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/watson_ir/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.524281 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/wms/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      459 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/wms/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      411 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/wms/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      479 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/wms/update.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      311 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/organizations/integrations/wms/wms_shared.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2812 2023-06-20 21:00:34.000000 veerum-sdk-5.1.12/veerum/cli/organizations/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.526391 veerum-sdk-5.1.12/veerum/cli/paper_objects/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      809 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1552 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      411 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      542 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/delete_many.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      623 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/fileparser.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      781 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6858 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/ingest.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      383 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/inspect.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1172 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/paper_objects/update.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      350 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/retcode.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.527798 veerum-sdk-5.1.12/veerum/cli/tags/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      629 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/tags/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      714 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/tags/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      328 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/tags/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      365 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/tags/deleteone.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      337 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/tags/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      615 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/tags/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.529376 veerum-sdk-5.1.12/veerum/cli/timeseries/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      722 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1984 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/create.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.530805 veerum-sdk-5.1.12/veerum/cli/timeseries/data/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      557 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/data/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      634 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/data/add.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      364 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/data/clear.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      472 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/data/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      353 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/data/get.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      249 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/data/set.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      322 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/delete.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1604 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      347 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/inspect.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2168 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/timeseries/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.531962 veerum-sdk-5.1.12/veerum/cli/users/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      726 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      917 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      928 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      317 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/inspect.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.532879 veerum-sdk-5.1.12/veerum/cli/users/organizations/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      549 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/organizations/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      364 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/organizations/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      497 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/organizations/join.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      505 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/organizations/leave.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1114 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.533821 veerum-sdk-5.1.12/veerum/cli/users/workscopes/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      543 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/workscopes/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      358 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/workscopes/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      479 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/workscopes/join.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      487 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/users/workscopes/leave.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      510 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/version.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.534052 veerum-sdk-5.1.12/veerum/cli/workbreakdowns/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      147 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workbreakdowns/__init__.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.535414 veerum-sdk-5.1.12/veerum/cli/workscopes/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      756 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3497 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/create.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2209 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/delete.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.536093 veerum-sdk-5.1.12/veerum/cli/workscopes/features/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      484 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/features/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      498 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/features/add.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      482 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/features/remove.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2924 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      342 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/inspect.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.537443 veerum-sdk-5.1.12/veerum/cli/workscopes/tags/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      557 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/tags/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      441 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/tags/add.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      344 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/tags/clear.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      569 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/tags/find.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      458 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/tags/remove.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      461 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/tags/set.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     4049 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/cli/workscopes/update.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.537672 veerum-sdk-5.1.12/veerum/fme/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1081 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/fme/installcli.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.541272 veerum-sdk-5.1.12/veerum/sdk/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      583 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/sdk/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      856 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/sdk/annotations.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      529 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/sdk/automations.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     7667 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/sdk/base.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2276 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/sdk/files.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      515 2023-04-28 18:51:52.000000 veerum-sdk-5.1.12/veerum/sdk/jobs.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3583 2023-06-26 19:27:33.000000 veerum-sdk-5.1.12/veerum/sdk/metadata.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1506 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/sdk/milestones.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2688 2023-06-20 21:00:34.000000 veerum-sdk-5.1.12/veerum/sdk/models.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2488 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/sdk/objects.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6479 2023-06-20 21:00:34.000000 veerum-sdk-5.1.12/veerum/sdk/organizations.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1696 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/sdk/paper_objects.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      966 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/sdk/tags.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2764 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/sdk/timeseries.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2964 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/sdk/users.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6361 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/sdk/workscopes.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.541504 veerum-sdk-5.1.12/veerum/tests/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)        0 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/tests/__init__.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.541869 veerum-sdk-5.1.12/veerum/utils/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)        0 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/utils/__init__.py
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)      120 2023-04-28 18:51:53.000000 veerum-sdk-5.1.12/veerum/utils/helpers.py
-drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-29 20:46:48.543378 veerum-sdk-5.1.12/veerum_sdk.egg-info/
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6502 2023-06-29 20:46:48.000000 veerum-sdk-5.1.12/veerum_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6121 2023-06-29 20:46:48.000000 veerum-sdk-5.1.12/veerum_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)        1 2023-06-29 20:46:48.000000 veerum-sdk-5.1.12/veerum_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)       43 2023-06-29 20:46:48.000000 veerum-sdk-5.1.12/veerum_sdk.egg-info/entry_points.txt
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)        7 2023-06-29 20:46:48.000000 veerum-sdk-5.1.12/veerum_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)       81 2023-06-29 20:46:48.000000 veerum-sdk-5.1.12/veerum_sdk.egg-info/requires.txt
--rw-r--r--   0 Jason Schweiller   (505) staff       (20)        7 2023-06-29 20:46:48.000000 veerum-sdk-5.1.12/veerum_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:58.002783 veerum-sdk-5.2.0/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)       76 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/MANIFEST.in
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6796 2023-06-30 17:51:58.002554 veerum-sdk-5.2.0/PKG-INFO
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6332 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/README.md
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)       38 2023-06-30 17:51:58.002840 veerum-sdk-5.2.0/setup.cfg
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1230 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/setup.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.948347 veerum-sdk-5.2.0/veerum/
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.950808 veerum-sdk-5.2.0/veerum/cli/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     5133 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/cli/__init__.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.951837 veerum-sdk-5.2.0/veerum/cli/annotations/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      637 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/annotations/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      323 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/annotations/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1510 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/annotations/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      327 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/annotations/inspect.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.952744 veerum-sdk-5.2.0/veerum/cli/automations/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      634 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/automations/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      523 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/automations/relationship.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      674 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/automations/sync.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      780 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/common.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      338 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/debug.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.954479 veerum-sdk-5.2.0/veerum/cli/files/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      709 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/files/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      298 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/files/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1046 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/files/download.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1721 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/files/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      317 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/files/inspect.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      883 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/files/update.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2082 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/files/upload.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.955982 veerum-sdk-5.2.0/veerum/cli/jobs/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      654 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/jobs/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      262 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/jobs/misplaced_objects.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      298 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/jobs/populate_keys.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      274 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/jobs/warn_inactive_users.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.957510 veerum-sdk-5.2.0/veerum/cli/metadata/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      640 2023-06-26 19:27:33.000000 veerum-sdk-5.2.0/veerum/cli/metadata/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1047 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/metadata/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      342 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/metadata/inspect.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.959202 veerum-sdk-5.2.0/veerum/cli/metadata/keys/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      526 2023-06-26 19:27:33.000000 veerum-sdk-5.2.0/veerum/cli/metadata/keys/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      450 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/metadata/keys/add.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      340 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/metadata/keys/clear.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      566 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/metadata/keys/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      468 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/metadata/keys/set.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.959788 veerum-sdk-5.2.0/veerum/cli/metadata/upload/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3054 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/metadata/upload/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      505 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/metadata/upload/csvparser.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.961585 veerum-sdk-5.2.0/veerum/cli/milestones/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      694 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/milestones/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1595 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/milestones/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      318 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/milestones/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1004 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/milestones/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      342 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/milestones/inspect.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1725 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/milestones/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.962867 veerum-sdk-5.2.0/veerum/cli/models/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      747 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      302 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/delete.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.963135 veerum-sdk-5.2.0/veerum/cli/models/download/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      434 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/download/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1458 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      322 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/inspect.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.963962 veerum-sdk-5.2.0/veerum/cli/models/metadata/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      492 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/metadata/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      376 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/metadata/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      637 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/metadata/set.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1368 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.965828 veerum-sdk-5.2.0/veerum/cli/models/upload/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      112 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/upload/__helpers.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     7122 2023-06-20 21:00:34.000000 veerum-sdk-5.2.0/veerum/cli/models/upload/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3066 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/upload/potree.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      749 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/upload/potree2.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1373 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/upload/tiles.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1506 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/models/upload/unity.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.967824 veerum-sdk-5.2.0/veerum/cli/objects/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      857 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      574 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      378 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/deleteone.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2509 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/fileparser.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      714 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6109 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/ingest.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      389 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/inspect.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2642 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.968327 veerum-sdk-5.2.0/veerum/cli/objects/upload/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      112 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/upload/__helpers.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3073 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/objects/upload/__init__.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.969272 veerum-sdk-5.2.0/veerum/cli/organization_configs/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      641 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/cli/organization_configs/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      372 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/cli/organization_configs/inspect.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1902 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/cli/organization_configs/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.970797 veerum-sdk-5.2.0/veerum/cli/organizations/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      746 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1803 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/cli/organizations/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      336 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      537 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      358 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/inspect.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.971837 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      637 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      379 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      370 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      528 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/integrations_shared.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.973477 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/iol_sap/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      466 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/iol_sap/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      389 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/iol_sap/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      449 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/iol_sap/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.975063 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/maximo/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      464 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/maximo/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      479 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/maximo/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      278 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/maximo/maximo_shared.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      546 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/maximo/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.976306 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/pi_system/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      470 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/pi_system/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      563 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/pi_system/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      766 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/pi_system/pi_shared.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      621 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/pi_system/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.977323 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/watson_ir/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      470 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/watson_ir/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      408 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/watson_ir/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      451 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/watson_ir/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.978691 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/wms/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      459 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/wms/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      411 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/wms/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      479 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/wms/update.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      311 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/organizations/integrations/wms/wms_shared.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1774 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/cli/organizations/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.981556 veerum-sdk-5.2.0/veerum/cli/paper_objects/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      809 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1552 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      411 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      542 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/delete_many.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      623 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/fileparser.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      781 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6858 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/ingest.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      383 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/inspect.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1172 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/paper_objects/update.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      350 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/retcode.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.983147 veerum-sdk-5.2.0/veerum/cli/tags/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      629 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/tags/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      714 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/tags/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      328 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/tags/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      365 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/tags/deleteone.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      337 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/tags/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      615 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/tags/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.984560 veerum-sdk-5.2.0/veerum/cli/timeseries/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      722 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1984 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/create.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.986038 veerum-sdk-5.2.0/veerum/cli/timeseries/data/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      557 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/data/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      634 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/data/add.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      364 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/data/clear.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      472 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/data/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      353 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/data/get.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      249 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/data/set.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      322 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/delete.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1604 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      347 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/inspect.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2168 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/timeseries/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.987271 veerum-sdk-5.2.0/veerum/cli/users/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      726 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      917 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      928 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      317 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/inspect.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.988469 veerum-sdk-5.2.0/veerum/cli/users/organizations/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      549 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/organizations/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      364 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/organizations/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      497 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/organizations/join.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      505 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/organizations/leave.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1114 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.989714 veerum-sdk-5.2.0/veerum/cli/users/workscopes/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      543 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/workscopes/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      358 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/workscopes/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      479 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/workscopes/join.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      487 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/users/workscopes/leave.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      510 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/version.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.990039 veerum-sdk-5.2.0/veerum/cli/workbreakdowns/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      147 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workbreakdowns/__init__.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.991783 veerum-sdk-5.2.0/veerum/cli/workscopes/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      756 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3497 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/create.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2209 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/delete.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.992606 veerum-sdk-5.2.0/veerum/cli/workscopes/features/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      484 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/features/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      498 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/features/add.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      482 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/features/remove.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2924 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      342 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/inspect.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.994445 veerum-sdk-5.2.0/veerum/cli/workscopes/tags/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      557 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/tags/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      441 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/tags/add.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      344 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/tags/clear.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      569 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/tags/find.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      458 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/tags/remove.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      461 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/tags/set.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     4049 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/cli/workscopes/update.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.994749 veerum-sdk-5.2.0/veerum/fme/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1081 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/fme/installcli.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:57.999923 veerum-sdk-5.2.0/veerum/sdk/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      647 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/sdk/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      856 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/sdk/annotations.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      529 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/sdk/automations.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     7667 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/sdk/base.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2276 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/sdk/files.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      515 2023-04-28 18:51:52.000000 veerum-sdk-5.2.0/veerum/sdk/jobs.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     3583 2023-06-26 19:27:33.000000 veerum-sdk-5.2.0/veerum/sdk/metadata.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1506 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/sdk/milestones.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2688 2023-06-20 21:00:34.000000 veerum-sdk-5.2.0/veerum/sdk/models.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2488 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/sdk/objects.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1168 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/sdk/organization_configs.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     5646 2023-06-30 17:51:39.000000 veerum-sdk-5.2.0/veerum/sdk/organizations.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     1696 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/sdk/paper_objects.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      966 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/sdk/tags.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2764 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/sdk/timeseries.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     2964 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/sdk/users.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6361 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/sdk/workscopes.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:58.000182 veerum-sdk-5.2.0/veerum/tests/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)        0 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/tests/__init__.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:58.000700 veerum-sdk-5.2.0/veerum/utils/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)        0 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/utils/__init__.py
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)      120 2023-04-28 18:51:53.000000 veerum-sdk-5.2.0/veerum/utils/helpers.py
+drwxr-xr-x   0 Jason Schweiller   (505) staff       (20)        0 2023-06-30 17:51:58.002256 veerum-sdk-5.2.0/veerum_sdk.egg-info/
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6796 2023-06-30 17:51:57.000000 veerum-sdk-5.2.0/veerum_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)     6285 2023-06-30 17:51:57.000000 veerum-sdk-5.2.0/veerum_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)        1 2023-06-30 17:51:57.000000 veerum-sdk-5.2.0/veerum_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)       43 2023-06-30 17:51:57.000000 veerum-sdk-5.2.0/veerum_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)        7 2023-06-30 17:51:57.000000 veerum-sdk-5.2.0/veerum_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)       81 2023-06-30 17:51:57.000000 veerum-sdk-5.2.0/veerum_sdk.egg-info/requires.txt
+-rw-r--r--   0 Jason Schweiller   (505) staff       (20)        7 2023-06-30 17:51:57.000000 veerum-sdk-5.2.0/veerum_sdk.egg-info/top_level.txt
```

### Comparing `veerum-sdk-5.1.12/PKG-INFO` & `veerum-sdk-5.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: veerum-sdk
-Version: 5.1.12
-Summary: SDK & CLI for interacting with the Veerum API
-Home-page: https://github.com/Veerum/veerum-sdk
-Author: Veerum Inc.
-Author-email: info@veerum.com
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 
 #  veerum-sdk (1.0)
 
 SDK &amp; CLI tools for interacting with the Veerum API
 
 ### Table of Contents
 1. [Updating](#update)
@@ -71,15 +57,15 @@
 
 #### Prereqs
  * Python 3.7 - https://www.python.org/downloads/release/python-371/
    * FME server/engine = 64 bit AMD
  * Git
  * Visual studio c++ build tools - https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools
  * Once these are installed, in terminal...
-   * `python3 -m pip3 install --upgrade pip3`
+   * `python3 -m pip install --upgrade pip` **(note: if pip is not upgraded, the veerum command will not be installed correctly)**
    * `pip3 install --upgrade setuptools`
  
 #### Install Process
  * Generating new ssh key
    * On local machine run the following command in terminal `ssh-keygen -t rsa -b 4096 -C "your-email@veerum.com"`
    * It will prompt you for a name for the ssh files, you can leave it as default or give it a new name (defaults to id_rsa)
    * Open the file create that ends with extension `.pub`. Default location should be `~/.ssh` (UserFolder/.ssh). Copy the contents of the .pub file you created it should start with something like `ssh-rsa`.
@@ -103,14 +89,16 @@
 
 In 'veerum-sdk' root folder run.
 
 `make dev`
 
 Subsiquent changes will be applied to local machine without having to run again.
 
+Make sure you have upgraded pip as instructed in Prereqs above, and ensure that /Library/Frameworks/Python.framework/Versions/3.7/bin (or whatever python version you are using), is added to the PATH variable.
+
 note about tuspy library: Our backend is using a forked version of the tus-node-server, so I am locking the tuspy client in setup.py to the latest version at the time of the forked version in the backend.
 
 <a name = "deployment"></a>
 ###  Deployment
 1) Increment version of CLI in `setup.py`
 2) Put everything into the `dev` branch while testing is happening in both the `dev` and `staging` environments
 3) Once release is ready for `prod`, merge `dev` -> `prod` in the CLI repo
```

### Comparing `veerum-sdk-5.1.12/README.md` & `veerum-sdk-5.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: veerum-sdk
+Version: 5.2.0
+Summary: SDK & CLI for interacting with the Veerum API
+Home-page: https://github.com/Veerum/veerum-sdk
+Author: Veerum Inc.
+Author-email: info@veerum.com
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 
 #  veerum-sdk (1.0)
 
 SDK &amp; CLI tools for interacting with the Veerum API
 
 ### Table of Contents
 1. [Updating](#update)
@@ -57,15 +71,15 @@
 
 #### Prereqs
  * Python 3.7 - https://www.python.org/downloads/release/python-371/
    * FME server/engine = 64 bit AMD
  * Git
  * Visual studio c++ build tools - https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools
  * Once these are installed, in terminal...
-   * `python3 -m pip3 install --upgrade pip3`
+   * `python3 -m pip install --upgrade pip` **(note: if pip is not upgraded, the veerum command will not be installed correctly)**
    * `pip3 install --upgrade setuptools`
  
 #### Install Process
  * Generating new ssh key
    * On local machine run the following command in terminal `ssh-keygen -t rsa -b 4096 -C "your-email@veerum.com"`
    * It will prompt you for a name for the ssh files, you can leave it as default or give it a new name (defaults to id_rsa)
    * Open the file create that ends with extension `.pub`. Default location should be `~/.ssh` (UserFolder/.ssh). Copy the contents of the .pub file you created it should start with something like `ssh-rsa`.
@@ -89,14 +103,16 @@
 
 In 'veerum-sdk' root folder run.
 
 `make dev`
 
 Subsiquent changes will be applied to local machine without having to run again.
 
+Make sure you have upgraded pip as instructed in Prereqs above, and ensure that /Library/Frameworks/Python.framework/Versions/3.7/bin (or whatever python version you are using), is added to the PATH variable.
+
 note about tuspy library: Our backend is using a forked version of the tus-node-server, so I am locking the tuspy client in setup.py to the latest version at the time of the forked version in the backend.
 
 <a name = "deployment"></a>
 ###  Deployment
 1) Increment version of CLI in `setup.py`
 2) Put everything into the `dev` branch while testing is happening in both the `dev` and `staging` environments
 3) Once release is ready for `prod`, merge `dev` -> `prod` in the CLI repo
```

### Comparing `veerum-sdk-5.1.12/setup.py` & `veerum-sdk-5.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import setuptools
 
-VERSION = '5.1.12'
+VERSION = '5.2.0'
+
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
```

### Comparing `veerum-sdk-5.1.12/veerum/cli/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from . import metadata
 from . import objects
 from . import version
 from . import debug
 from . import tags
 from . import paper_objects
 from . import automations
+from . import organization_configs
 
 from . import retcode
 from ..sdk import base
 
 from backports.datetime_fromisoformat import MonkeyPatch
 
 # Make sure datetime.fromisoformat is available in earlier python versions
@@ -116,15 +117,16 @@
 		metadata,
 		objects,
 		version,
 		debug,
 		jobs,
 		tags,
 		paper_objects,
-		automations
+		automations,
+		organization_configs
 	]
 
 	for utility in utilities:
 		if hasattr(utility, 'add_arguments'):
 			utility.add_arguments(subparser)
 
 	return parser.parse_args()
```

### Comparing `veerum-sdk-5.1.12/veerum/cli/annotations/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/annotations/find.py` & `veerum-sdk-5.2.0/veerum/cli/annotations/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/automations/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/automations/relationship.py` & `veerum-sdk-5.2.0/veerum/cli/automations/relationship.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/automations/sync.py` & `veerum-sdk-5.2.0/veerum/cli/automations/sync.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/common.py` & `veerum-sdk-5.2.0/veerum/cli/common.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/files/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/files/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/files/download.py` & `veerum-sdk-5.2.0/veerum/cli/files/download.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/files/find.py` & `veerum-sdk-5.2.0/veerum/cli/files/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/files/update.py` & `veerum-sdk-5.2.0/veerum/cli/files/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/files/upload.py` & `veerum-sdk-5.2.0/veerum/cli/files/upload.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/jobs/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/metadata/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/metadata/find.py` & `veerum-sdk-5.2.0/veerum/cli/metadata/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/metadata/keys/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/metadata/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/metadata/keys/find.py` & `veerum-sdk-5.2.0/veerum/cli/metadata/keys/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/metadata/upload/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/metadata/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/milestones/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/milestones/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/milestones/create.py` & `veerum-sdk-5.2.0/veerum/cli/milestones/create.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/milestones/find.py` & `veerum-sdk-5.2.0/veerum/cli/milestones/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/milestones/update.py` & `veerum-sdk-5.2.0/veerum/cli/milestones/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/find.py` & `veerum-sdk-5.2.0/veerum/cli/models/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/metadata/set.py` & `veerum-sdk-5.2.0/veerum/cli/models/metadata/set.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/update.py` & `veerum-sdk-5.2.0/veerum/cli/models/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/upload/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/models/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/upload/potree.py` & `veerum-sdk-5.2.0/veerum/cli/models/upload/potree.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/upload/potree2.py` & `veerum-sdk-5.2.0/veerum/cli/models/upload/potree2.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/upload/tiles.py` & `veerum-sdk-5.2.0/veerum/cli/models/upload/tiles.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/models/upload/unity.py` & `veerum-sdk-5.2.0/veerum/cli/models/upload/unity.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/objects/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/objects/delete.py` & `veerum-sdk-5.2.0/veerum/cli/objects/delete.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/objects/fileparser.py` & `veerum-sdk-5.2.0/veerum/cli/objects/fileparser.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/objects/find.py` & `veerum-sdk-5.2.0/veerum/cli/objects/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/objects/ingest.py` & `veerum-sdk-5.2.0/veerum/cli/objects/ingest.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/objects/update.py` & `veerum-sdk-5.2.0/veerum/cli/objects/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/objects/upload/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/objects/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/create.py` & `veerum-sdk-5.2.0/veerum/cli/organization_configs/update.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,19 @@
 def add_arguments(subparser):
 	parser = subparser.add_parser(
-		'create',
-		description='Create a new organization'
+		'update',
+		description='Specify an organization config'
 	)
 	parser.set_defaults(command=main)
 
 	parser.add_argument(
-		'-n',
-		'--name',
+		'-o',
+		'--organization',
 		required=True,
-		help=''
-	)
-	parser.add_argument(
-		'-s',
-		'--slug',
-		required=True,
-		help=''
-	)
-	parser.add_argument(
-		'--99',
-		dest='ninenine',
-		default=False,
-		action='store_true',
-		help=''
-	)
-	parser.add_argument(
-		'-l',
-		'--nonUseLockPeriodDays',
-		default=None,
-		help='A period of inactivity in days when the user account should be locked'
-	)
-	parser.add_argument(
-		'-e',
-		'--pwdExpiresInDays',
-		default=None,
-		help='Amount of the days that a user password should expire'
-	)
-	parser.add_argument(
-		'-a',
-		'--maxLockoutAttempts',
-		default=None,
-		help='Total amount attempts of incorrect password input before the user will be locked out on some period'
-	)
-	parser.add_argument(
-		'-ti',
-		'--timeOfInactivityInSecs',
-		default=None,
-		help='Amount of seconds before logging of the app automatically'
-	)
-	parser.add_argument(
-		'-acid',
-		'--auth0ConnId',
-		default=None,
-		help='Auth0 connection ID required for SSO'
-	)
-	parser.add_argument(
-		'-clientid',
-		'--auth0ClientId',
-		default=None,
-		help='Auth client ID required for SSO'
+		help='ID of organization to modify'
 	)
 	parser.add_argument(
 		'-rlu',
 		'--rateLimitUsers',
 		default=None,
 		help='To change the number of available API requests to list users per organization'
 	)
@@ -86,26 +37,32 @@
 	)
 	parser.add_argument(
 		'-rlw',
 		'--rateLimitWorkscopes',
 		default=None,
 		help='To change the number of available API requests to list workscopes per organization'
 	)
+	parser.add_argument(
+		'-rlos',
+		'--rateLimitObjectsSearch',
+		default=None,
+		help='To change the number of available API requests to search objects per organization'
+	)
+	parser.add_argument(
+		'-rloss',
+		'--rateLimitObjectsSpatialSearch',
+		default=None,
+		help='To change the number of available API requests to spatial search objects per organization'
+	)
 
 async def main(args):
 	# TODO: {KL} sanitize the slug
-	return await args.client.create(
-		name=args.name,
-		slug=args.slug,
-		ninenine=args.ninenine,
-		nonUseLockPeriodDays=args.nonUseLockPeriodDays,
-		pwdExpiresInDays=args.pwdExpiresInDays,
-		maxLockoutAttempts=args.maxLockoutAttempts,
-		timeOfInactivityInSecs=args.timeOfInactivityInSecs,
-		auth0ConnId=args.auth0ConnId,
-		auth0ClientId=args.auth0ClientId,
+	return await args.client.update(
+		args.organization,
 		rateLimitUsers=args.rateLimitUsers,
 		rateLimitAnnotations=args.rateLimitAnnotations,
 		rateLimitFiles=args.rateLimitFiles,
 		rateLimitModels=args.rateLimitModels,
-		rateLimitWorkscopes=args.rateLimitWorkscopes
+		rateLimitWorkscopes=args.rateLimitWorkscopes,
+		rateLimitObjectsSearch=args.rateLimitObjectsSearch,
+		rateLimitObjectsSpatialSearch=args.rateLimitObjectsSpatialSearch
 	)
```

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/find.py` & `veerum-sdk-5.2.0/veerum/cli/organizations/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/integrations/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/organizations/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/integrations/integrations_shared.py` & `veerum-sdk-5.2.0/veerum/cli/organizations/integrations/integrations_shared.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/integrations/maximo/update.py` & `veerum-sdk-5.2.0/veerum/cli/organizations/integrations/maximo/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/integrations/pi_system/create.py` & `veerum-sdk-5.2.0/veerum/cli/organizations/integrations/pi_system/create.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/integrations/pi_system/pi_shared.py` & `veerum-sdk-5.2.0/veerum/cli/organizations/integrations/pi_system/pi_shared.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/integrations/pi_system/update.py` & `veerum-sdk-5.2.0/veerum/cli/organizations/integrations/pi_system/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/organizations/update.py` & `veerum-sdk-5.2.0/veerum/cli/timeseries/update.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,102 @@
 def add_arguments(subparser):
 	parser = subparser.add_parser(
 		'update',
-		description='Modify an organization'
+		description='Update a timeseries'
 	)
-	parser.set_defaults(command=main)
+	parser.set_defaults(command=main, current=None)
 
 	parser.add_argument(
-		'-o',
-		'--organization',
+		'-t',
+		'--timeseries',
+		dest='timeseries',
 		required=True,
-		help='ID of organization to modify'
-	)
-	parser.add_argument(
-		'-n',
-		'--name',
-		default=None,
-		help='Name of the organization'
-	)
-	parser.add_argument(
-		'-l',
-		'--nonUseLockPeriodDays',
-		default=None,
-		help='A period of inactivity in days when the user account should be locked'
+		help='ID of timeseries to modify'
 	)
+
 	parser.add_argument(
-		'-e',
-		'--pwdExpiresInDays',
+		'-w',
+		'--workscope',
 		default=None,
-		help='Amount of the days that a user password should expire'
+		help='ID of the workscope this timeseries should be attached to'
 	)
 	parser.add_argument(
-		'-a',
-		'--maxLockoutAttempts',
+		'--x-unit',
 		default=None,
-		help='Total attempts amount of incorrect password input before the user will be locked out on some period'
+		help='Units for the x-axis'
 	)
 	parser.add_argument(
-		'-ti',
-		'--timeOfInactivityInSecs',
+		'--y-unit',
 		default=None,
-		help='Amount of seconds before logging of the app automatically'
+		help='Units for the y-axis'
 	)
 	parser.add_argument(
-		'-acid',
-		'--auth0ConnId',
+		'--x-label',
 		default=None,
-		help='Auth0 connection ID required for SSO'
+		help='Label for the x-axis'
 	)
 	parser.add_argument(
-		'-clientid',
-		'--auth0ClientId',
+		'--y-label',
 		default=None,
-		help='Auth client ID required for SSO'
+		help='Label for the y-axis'
 	)
-	parser.add_argument(
-		'-dws',
-		'--defaultOrgWs',
-		help='Comma separated default workscope IDs. List of ws user has access to depending on his default ws rights',
+
+	group = parser.add_mutually_exclusive_group()
+	group.add_argument(
+		'--current',
+		dest='current',
+		action='store_true',
+		help='Indicates that this timeseries is the most recent and displays it from the UI'
+	)
+	group.add_argument(
+		'--not-current',
+		dest='current',
+		action='store_false',
+		help='Indicates that this timeseries is not the most recent and hides it from the UI'
 	)
+
 	parser.add_argument(
-		'-rlu',
-		'--rateLimitUsers',
+		'-n',
+		'--name',
 		default=None,
-		help='To change the number of available API requests to list users per organization'
 	)
 	parser.add_argument(
-		'-rla',
-		'--rateLimitAnnotations',
+		'--type',
 		default=None,
-		help='To change the number of available API requests to list annotations per organization'
 	)
+
 	parser.add_argument(
-		'-rlf',
-		'--rateLimitFiles',
+		'--point-style',
+		dest='point_style',
 		default=None,
-		help='To change the number of available API requests to list files per organization'
+		choices=['circle', 'cross', 'crossRot', 'dash', 'line', 'rect', 'rectRounded', 'rectRot', 'star', 'triangle'],
+		help='How to style the points in the rendered chart'
 	)
 	parser.add_argument(
-		'-rlm',
-		'--rateLimitModels',
+		'--point-color',
+		dest='point_color',
 		default=None,
-		help='To change the number of available API requests to list models per organization'
+		help='A hex color (e.g. #000000)',
 	)
 	parser.add_argument(
-		'-rlw',
-		'--rateLimitWorkscopes',
+		'--chart-radius',
+		dest='chart_radius',
+		type=float,
 		default=None,
-		help='To change the number of available API requests to list workscopes per organization'
+		help='The size of the graph points in the rendered chart. Must be >= 0.',
 	)
 
 async def main(args):
 	return await args.client.update(
-		args.organization,
+		args.timeseries,
+		workscope=args.workscope,
+		x_unit=args.x_unit,
+		y_unit=args.y_unit,
+		x_label=args.x_label,
+		y_label=args.y_label,
+		current=args.current,
 		name=args.name,
-		nonUseLockPeriodDays=args.nonUseLockPeriodDays,
-		pwdExpiresInDays=args.pwdExpiresInDays,
-		maxLockoutAttempts=args.maxLockoutAttempts,
-		timeOfInactivityInSecs=args.timeOfInactivityInSecs,
-		auth0ConnId=args.auth0ConnId,
-		auth0ClientId=args.auth0ClientId,
-		defaultOrgWs=args.defaultOrgWs,
-		rateLimitUsers=args.rateLimitUsers,
-		rateLimitAnnotations=args.rateLimitAnnotations,
-		rateLimitFiles=args.rateLimitFiles,
-		rateLimitModels=args.rateLimitModels,
-		rateLimitWorkscopes=args.rateLimitWorkscopes
+		type=args.type,
+		point_style=args.point_style,
+		point_color=args.point_color,
+		chart_radius=args.chart_radius,
 	)
```

### Comparing `veerum-sdk-5.1.12/veerum/cli/paper_objects/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/paper_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/paper_objects/create.py` & `veerum-sdk-5.2.0/veerum/cli/paper_objects/create.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/paper_objects/delete_many.py` & `veerum-sdk-5.2.0/veerum/cli/paper_objects/delete_many.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/paper_objects/fileparser.py` & `veerum-sdk-5.2.0/veerum/cli/paper_objects/fileparser.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/paper_objects/find.py` & `veerum-sdk-5.2.0/veerum/cli/paper_objects/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/paper_objects/ingest.py` & `veerum-sdk-5.2.0/veerum/cli/paper_objects/ingest.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/paper_objects/update.py` & `veerum-sdk-5.2.0/veerum/cli/paper_objects/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/tags/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/tags/create.py` & `veerum-sdk-5.2.0/veerum/cli/tags/create.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/tags/update.py` & `veerum-sdk-5.2.0/veerum/cli/tags/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/timeseries/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/timeseries/create.py` & `veerum-sdk-5.2.0/veerum/cli/timeseries/create.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/timeseries/data/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/timeseries/data/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/timeseries/data/add.py` & `veerum-sdk-5.2.0/veerum/cli/timeseries/data/add.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/timeseries/find.py` & `veerum-sdk-5.2.0/veerum/cli/timeseries/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/users/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/users/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/users/create.py` & `veerum-sdk-5.2.0/veerum/cli/users/create.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/users/find.py` & `veerum-sdk-5.2.0/veerum/cli/users/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/users/organizations/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/users/organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/users/update.py` & `veerum-sdk-5.2.0/veerum/cli/users/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/users/workscopes/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/users/workscopes/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/workscopes/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/workscopes/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/workscopes/create.py` & `veerum-sdk-5.2.0/veerum/cli/workscopes/create.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/workscopes/delete.py` & `veerum-sdk-5.2.0/veerum/cli/workscopes/delete.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/workscopes/find.py` & `veerum-sdk-5.2.0/veerum/cli/workscopes/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/workscopes/tags/__init__.py` & `veerum-sdk-5.2.0/veerum/cli/workscopes/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/workscopes/tags/find.py` & `veerum-sdk-5.2.0/veerum/cli/workscopes/tags/find.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/cli/workscopes/update.py` & `veerum-sdk-5.2.0/veerum/cli/workscopes/update.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/fme/installcli.py` & `veerum-sdk-5.2.0/veerum/fme/installcli.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/__init__.py` & `veerum-sdk-5.2.0/veerum/sdk/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 from .annotations import Client as Annotations
 from .metadata import Client as Metadata
 from .objects import Client as Objects
 from .jobs import Client as Jobs
 from .tags import Client as Tags
 from .paper_objects import Client as PaperObjects
 from .automations import Client as Automations
+from .organization_configs import Client as OrganizationConfigs
```

### Comparing `veerum-sdk-5.1.12/veerum/sdk/annotations.py` & `veerum-sdk-5.2.0/veerum/sdk/annotations.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/automations.py` & `veerum-sdk-5.2.0/veerum/sdk/automations.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/base.py` & `veerum-sdk-5.2.0/veerum/sdk/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # DOCKER = true, when running inside docker container
 if 'DOCKER' in os.environ:
 	VEERUM_CONFIG_PATH = os.path.join('/run', 'secrets', 'veerum_config')
 
 USER_CONFIG_PATH = os.path.expanduser(VEERUM_CONFIG_PATH)
 DEFAULT_PROFILE = 'default'
-DEFAULT_USER_AGENT = 'VeerumSDK/0.3.0'
+DEFAULT_USER_AGENT = 'VeerumSDK/5.2.0'
 DEFAULT_ENDPOINT = 'http://production.api.local'
 
 DEFAULT_CONFIG = {
 	DEFAULT_PROFILE: {
 		'user_agent': DEFAULT_USER_AGENT,
 	}
 }
```

### Comparing `veerum-sdk-5.1.12/veerum/sdk/files.py` & `veerum-sdk-5.2.0/veerum/sdk/files.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/jobs.py` & `veerum-sdk-5.2.0/veerum/sdk/jobs.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/metadata.py` & `veerum-sdk-5.2.0/veerum/sdk/metadata.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/milestones.py` & `veerum-sdk-5.2.0/veerum/sdk/milestones.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/models.py` & `veerum-sdk-5.2.0/veerum/sdk/models.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/objects.py` & `veerum-sdk-5.2.0/veerum/sdk/objects.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/organizations.py` & `veerum-sdk-5.2.0/veerum/sdk/organizations.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,38 +22,30 @@
                ninenine=False,
                nonUseLockPeriodDays=None,
                pwdExpiresInDays=None,
                maxLockoutAttempts=None,
                timeOfInactivityInSecs=None,
                auth0ConnId=None,
                auth0ClientId=None,
-               rateLimitUsers=None,
-               rateLimitAnnotations=None,
-               rateLimitFiles=None,
-               rateLimitModels=None,
-               rateLimitWorkscopes=None
+               hundred=False
                ):
         return self.send_request(
             method='POST',
             path='organizations',
             json=self.pack(
                 name=name,
                 slug=slug,
                 ninenine=ninenine,
                 nonUseLockPeriodDays=nonUseLockPeriodDays,
                 pwdExpiresInDays=pwdExpiresInDays,
                 maxLockoutAttempts=maxLockoutAttempts,
                 timeOfInactivityInSecs=timeOfInactivityInSecs,
                 auth0ConnId=auth0ConnId,
                 auth0ClientId=auth0ClientId,
-                rateLimit_users=rateLimitUsers,
-                rateLimit_annotations=rateLimitAnnotations,
-                rateLimit_files=rateLimitFiles,
-                rateLimit_models=rateLimitModels,
-                rateLimit_workscopes=rateLimitWorkscopes
+                hundred=hundred
             )
         )
 
     def get(self, organization):
         return self.send_request(
             method='GET',
             path=self.join('organizations', organization)
@@ -64,37 +56,28 @@
                name=None,
                nonUseLockPeriodDays=None,
                pwdExpiresInDays=None,
                maxLockoutAttempts=None,
                timeOfInactivityInSecs=None,
                auth0ConnId=None,
                auth0ClientId=None,
-               defaultOrgWs=None,
-               rateLimitUsers=None,
-               rateLimitAnnotations=None,
-               rateLimitFiles=None,
-               rateLimitModels=None,
-               rateLimitWorkscopes=None):
+               defaultOrgWs=None
+               ):
         return self.send_request(
             method='PATCH',
             path=self.join('organizations', organization),
             json=self.pack(
                 name=name,
                 nonUseLockPeriodDays=nonUseLockPeriodDays,
                 pwdExpiresInDays=pwdExpiresInDays,
                 maxLockoutAttempts=maxLockoutAttempts,
                 timeOfInactivityInSecs=timeOfInactivityInSecs,
                 auth0ConnId=auth0ConnId,
                 auth0ClientId=auth0ClientId,
-                defaultOrgWs=defaultOrgWs,
-                rateLimit_users=rateLimitUsers,
-                rateLimit_annotations=rateLimitAnnotations,
-                rateLimit_files=rateLimitFiles,
-                rateLimit_models=rateLimitModels,
-                rateLimit_workscopes=rateLimitWorkscopes
+                defaultOrgWs=defaultOrgWs
             )
         )
 
     def delete(self, organization):
         return self.send_request(
             method='DELETE',
             path=self.join('organizations', organization)
```

### Comparing `veerum-sdk-5.1.12/veerum/sdk/paper_objects.py` & `veerum-sdk-5.2.0/veerum/sdk/paper_objects.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/tags.py` & `veerum-sdk-5.2.0/veerum/sdk/tags.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/timeseries.py` & `veerum-sdk-5.2.0/veerum/sdk/timeseries.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/users.py` & `veerum-sdk-5.2.0/veerum/sdk/users.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum/sdk/workscopes.py` & `veerum-sdk-5.2.0/veerum/sdk/workscopes.py`

 * *Files identical despite different names*

### Comparing `veerum-sdk-5.1.12/veerum_sdk.egg-info/PKG-INFO` & `veerum-sdk-5.2.0/veerum_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veerum-sdk
-Version: 5.1.12
+Version: 5.2.0
 Summary: SDK & CLI for interacting with the Veerum API
 Home-page: https://github.com/Veerum/veerum-sdk
 Author: Veerum Inc.
 Author-email: info@veerum.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 
 #### Prereqs
  * Python 3.7 - https://www.python.org/downloads/release/python-371/
    * FME server/engine = 64 bit AMD
  * Git
  * Visual studio c++ build tools - https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools
  * Once these are installed, in terminal...
-   * `python3 -m pip3 install --upgrade pip3`
+   * `python3 -m pip install --upgrade pip` **(note: if pip is not upgraded, the veerum command will not be installed correctly)**
    * `pip3 install --upgrade setuptools`
  
 #### Install Process
  * Generating new ssh key
    * On local machine run the following command in terminal `ssh-keygen -t rsa -b 4096 -C "your-email@veerum.com"`
    * It will prompt you for a name for the ssh files, you can leave it as default or give it a new name (defaults to id_rsa)
    * Open the file create that ends with extension `.pub`. Default location should be `~/.ssh` (UserFolder/.ssh). Copy the contents of the .pub file you created it should start with something like `ssh-rsa`.
@@ -103,14 +103,16 @@
 
 In 'veerum-sdk' root folder run.
 
 `make dev`
 
 Subsiquent changes will be applied to local machine without having to run again.
 
+Make sure you have upgraded pip as instructed in Prereqs above, and ensure that /Library/Frameworks/Python.framework/Versions/3.7/bin (or whatever python version you are using), is added to the PATH variable.
+
 note about tuspy library: Our backend is using a forked version of the tus-node-server, so I am locking the tuspy client in setup.py to the latest version at the time of the forked version in the backend.
 
 <a name = "deployment"></a>
 ###  Deployment
 1) Increment version of CLI in `setup.py`
 2) Put everything into the `dev` branch while testing is happening in both the `dev` and `staging` environments
 3) Once release is ready for `prod`, merge `dev` -> `prod` in the CLI repo
```

### Comparing `veerum-sdk-5.1.12/veerum_sdk.egg-info/SOURCES.txt` & `veerum-sdk-5.2.0/veerum_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 veerum/cli/objects/fileparser.py
 veerum/cli/objects/find.py
 veerum/cli/objects/ingest.py
 veerum/cli/objects/inspect.py
 veerum/cli/objects/update.py
 veerum/cli/objects/upload/__helpers.py
 veerum/cli/objects/upload/__init__.py
+veerum/cli/organization_configs/__init__.py
+veerum/cli/organization_configs/inspect.py
+veerum/cli/organization_configs/update.py
 veerum/cli/organizations/__init__.py
 veerum/cli/organizations/create.py
 veerum/cli/organizations/delete.py
 veerum/cli/organizations/find.py
 veerum/cli/organizations/inspect.py
 veerum/cli/organizations/update.py
 veerum/cli/organizations/integrations/__init__.py
@@ -156,14 +159,15 @@
 veerum/sdk/base.py
 veerum/sdk/files.py
 veerum/sdk/jobs.py
 veerum/sdk/metadata.py
 veerum/sdk/milestones.py
 veerum/sdk/models.py
 veerum/sdk/objects.py
+veerum/sdk/organization_configs.py
 veerum/sdk/organizations.py
 veerum/sdk/paper_objects.py
 veerum/sdk/tags.py
 veerum/sdk/timeseries.py
 veerum/sdk/users.py
 veerum/sdk/workscopes.py
 veerum/tests/__init__.py
```

