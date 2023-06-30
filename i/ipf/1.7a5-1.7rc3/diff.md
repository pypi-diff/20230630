# Comparing `tmp/ipf-1.7a5.tar.gz` & `tmp/ipf-1.7rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ipf-1.7a5.tar", last modified: Fri Jun 17 15:57:36 2022, max compression
+gzip compressed data, was "ipf-1.7rc3.tar", last modified: Fri Jun 23 19:24:11 2023, max compression
```

## Comparing `ipf-1.7a5.tar` & `ipf-1.7rc3.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/
--rw-r--r--   0 blau       (501) staff       (20)     3653 2022-06-17 15:57:36.000000 ipf-1.7a5/PKG-INFO
--rw-r--r--   0 blau       (501) staff       (20)    11358 2022-04-26 00:48:11.000000 ipf-1.7a5/LICENSE-2.0.txt
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/
--rw-r--r--   0 blau       (501) staff       (20)     6103 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/catalog.py
--rw-r--r--   0 blau       (501) staff       (20)     1480 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/error.py
--rw-r--r--   0 blau       (501) staff       (20)     2086 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/paths.py
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/bin/
--rwxr-xr-x   0 blau       (501) staff       (20)      585 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/bin/ipf_workflow
--rwxr-xr-x   0 blau       (501) staff       (20)      353 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/bin/ipf_configure_xsede
--rw-r--r--   0 blau       (501) staff       (20)     9913 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/log.py
--rw-r--r--   0 blau       (501) staff       (20)     3323 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/dt.py
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/etc/
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/etc/ipf/
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/etc/ipf/init.d/
--rwxr-xr-x   0 blau       (501) staff       (20)     2344 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/etc/ipf/init.d/ipf-WORKFLOW
--rw-r--r--   0 blau       (501) staff       (20)      502 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/etc/ipf/logging.conf
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/etc/ipf/xsede/
--rw-r--r--   0 blau       (501) staff       (20)    38688 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/xsede/ca_certs.pem
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/
--rw-r--r--   0 blau       (501) staff       (20)     1223 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/etc/ipf/workflow/sysinfo_publish.json
--rw-r--r--   0 blau       (501) staff       (20)      460 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/ipfinfo.json
--rw-r--r--   0 blau       (501) staff       (20)      468 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/etc/ipf/workflow/sysinfo.json
--rw-r--r--   0 blau       (501) staff       (20)      276 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/etc/ipf/workflow/ipfinfo_publish_periodic.json
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/
--rw-r--r--   0 blau       (501) staff       (20)      315 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/lmod.json
--rw-r--r--   0 blau       (501) staff       (20)     1326 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/serviceremotepublish.json
--rw-r--r--   0 blau       (501) staff       (20)     1662 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/moab_pbs_compute.json
--rw-r--r--   0 blau       (501) staff       (20)      350 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/extmodules.json
--rw-r--r--   0 blau       (501) staff       (20)     1064 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/extmodulesremote.json
--rw-r--r--   0 blau       (501) staff       (20)     1535 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/condor_compute.json
--rw-r--r--   0 blau       (501) staff       (20)      333 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/abstractservice.json
--rw-r--r--   0 blau       (501) staff       (20)      627 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/pbs_activity.json
--rw-r--r--   0 blau       (501) staff       (20)      634 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/sge_activity.json
--rw-r--r--   0 blau       (501) staff       (20)      582 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/ipfinfo_publish.json
--rw-r--r--   0 blau       (501) staff       (20)     1512 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/sge_compute.json
--rw-r--r--   0 blau       (501) staff       (20)     1508 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/pbs_compute.json
--rw-r--r--   0 blau       (501) staff       (20)      640 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/slurm_activity.json
--rw-r--r--   0 blau       (501) staff       (20)      321 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/modules.json
--rw-r--r--   0 blau       (501) staff       (20)     1526 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/slurm_compute.json
--rw-r--r--   0 blau       (501) staff       (20)     1513 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/openstack_compute.json
--rw-r--r--   0 blau       (501) staff       (20)     1735 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/catalina_pbs_compute.json
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/etc/ipf/workflow/glue2/
--rw-r--r--   0 blau       (501) staff       (20)      114 2022-04-26 01:11:35.000000 ipf-1.7a5/ipf/etc/ipf/workflow/glue2/empty.txt
--rw-r--r--   0 blau       (501) staff       (20)      277 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/etc/ipf/workflow/sysinfo_publish_periodic.json
--rw-r--r--   0 blau       (501) staff       (20)        0 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/__init__.py
--rw-r--r--   0 blau       (501) staff       (20)     3030 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/step_info.py
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/var/
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/var/ipf/
--rw-r--r--   0 blau       (501) staff       (20)      114 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/var/ipf/README.txt
--rw-r--r--   0 blau       (501) staff       (20)    14411 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/step.py
--rw-r--r--   0 blau       (501) staff       (20)     5025 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/engine.py
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/xsede/
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/xsede/test/
--rwxr-xr-x   0 blau       (501) staff       (20)      875 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/xsede/test/validate_activities.py
--rwxr-xr-x   0 blau       (501) staff       (20)      657 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/xsede/test/validate_compute.py
--rwxr-xr-x   0 blau       (501) staff       (20)      573 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/xsede/test/validate_modules.py
--rw-r--r--   0 blau       (501) staff       (20)     6628 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/xsede/test/subscribe_amqp.py
--rwxr-xr-x   0 blau       (501) staff       (20)     2222 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/xsede/test/validate.py
--rw-r--r--   0 blau       (501) staff       (20)        0 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/xsede/__init__.py
--rw-r--r--   0 blau       (501) staff       (20)     3228 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/xsede/sysinfo.py
--rw-r--r--   0 blau       (501) staff       (20)    40003 2022-06-01 16:12:07.000000 ipf-1.7a5/ipf/xsede/configure_workflows.py
--rw-r--r--   0 blau       (501) staff       (20)     8445 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/sysinfo.py
--rw-r--r--   0 blau       (501) staff       (20)     6351 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/workflow.py
--rw-r--r--   0 blau       (501) staff       (20)    13773 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/ipfinfo.py
--rw-r--r--   0 blau       (501) staff       (20)     4022 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/fileread.py
--rw-r--r--   0 blau       (501) staff       (20)      439 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/pre_populate_position.py
--rw-r--r--   0 blau       (501) staff       (20)     2919 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/data.py
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf/glue2/
--rw-r--r--   0 blau       (501) staff       (20)     6575 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/installedservices.py
--rw-r--r--   0 blau       (501) staff       (20)     3013 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/sge_tacc.py
--rw-r--r--   0 blau       (501) staff       (20)     6745 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/service.py
--rw-r--r--   0 blau       (501) staff       (20)     8566 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/computing_service.py
--rw-r--r--   0 blau       (501) staff       (20)     2610 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/benchmark.py
--rw-r--r--   0 blau       (501) staff       (20)    22021 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/nimbus.py
--rw-r--r--   0 blau       (501) staff       (20)     2481 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/unicore.py
--rw-r--r--   0 blau       (501) staff       (20)     7732 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/computing_share_accel_info.py
--rw-r--r--   0 blau       (501) staff       (20)     5458 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/domain.py
--rw-r--r--   0 blau       (501) staff       (20)    53511 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/slurm.py
--rw-r--r--   0 blau       (501) staff       (20)    20800 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/loadleveler.py
--rw-r--r--   0 blau       (501) staff       (20)     8483 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/moab.py
--rw-r--r--   0 blau       (501) staff       (20)     5234 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/valet.py
--rw-r--r--   0 blau       (501) staff       (20)    24825 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/execution_environment.py
--rw-r--r--   0 blau       (501) staff       (20)    27314 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/computing_activity.py
--rw-r--r--   0 blau       (501) staff       (20)     4716 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/activity.py
--rw-r--r--   0 blau       (501) staff       (20)    19674 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/openstack.py
--rw-r--r--   0 blau       (501) staff       (20)     3988 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/resource.py
--rw-r--r--   0 blau       (501) staff       (20)        0 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/__init__.py
--rw-r--r--   0 blau       (501) staff       (20)    26862 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/sge.py
--rw-r--r--   0 blau       (501) staff       (20)     2448 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/genesisII.py
--rw-r--r--   0 blau       (501) staff       (20)     8085 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/types.py
--rw-r--r--   0 blau       (501) staff       (20)    14807 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/condor.py
--rw-r--r--   0 blau       (501) staff       (20)     4369 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/gram.py
--rw-r--r--   0 blau       (501) staff       (20)    10362 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/application.py
--rw-r--r--   0 blau       (501) staff       (20)    10576 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/storageservice.py
--rw-r--r--   0 blau       (501) staff       (20)     2004 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/step.py
--rw-r--r--   0 blau       (501) staff       (20)     6532 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/location.py
--rw-r--r--   0 blau       (501) staff       (20)    12319 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/endpoint.py
--rw-r--r--   0 blau       (501) staff       (20)     3936 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/catalina.py
--rw-r--r--   0 blau       (501) staff       (20)    27065 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/computing_share.py
--rw-r--r--   0 blau       (501) staff       (20)     5371 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/share.py
--rw-r--r--   0 blau       (501) staff       (20)     6613 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/computing_manager_accel_info.py
--rw-r--r--   0 blau       (501) staff       (20)    10579 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/computing_endpoint.py
--rw-r--r--   0 blau       (501) staff       (20)     4830 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/entity.py
--rw-r--r--   0 blau       (501) staff       (20)    17046 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/modules.py
--rw-r--r--   0 blau       (501) staff       (20)    26935 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/accelerator_environment.py
--rw-r--r--   0 blau       (501) staff       (20)    25886 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/lsf.py
--rw-r--r--   0 blau       (501) staff       (20)     2944 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/pbs_psc.py
--rw-r--r--   0 blau       (501) staff       (20)     4249 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/manager.py
--rw-r--r--   0 blau       (501) staff       (20)    17423 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/computing_manager.py
--rw-r--r--   0 blau       (501) staff       (20)    11032 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/glue2/abstractservice.py
--rw-r--r--   0 blau       (501) staff       (20)    19496 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/cobalt.py
--rw-r--r--   0 blau       (501) staff       (20)     2621 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/contact.py
--rw-r--r--   0 blau       (501) staff       (20)    32391 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/pbs.py
--rw-r--r--   0 blau       (501) staff       (20)    14586 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/glue2/compute.py
--rw-r--r--   0 blau       (501) staff       (20)     4459 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/run_workflow.py
--rw-r--r--   0 blau       (501) staff       (20)     6367 2022-04-26 00:48:11.000000 ipf-1.7a5/ipf/daemon.py
--rw-r--r--   0 blau       (501) staff       (20)    14215 2022-04-26 00:48:36.000000 ipf-1.7a5/ipf/publish.py
-drwxr-xr-x   0 blau       (501) staff       (20)        0 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf.egg-info/
--rw-r--r--   0 blau       (501) staff       (20)     3653 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf.egg-info/PKG-INFO
--rw-r--r--   0 blau       (501) staff       (20)        1 2022-04-26 01:15:11.000000 ipf-1.7a5/ipf.egg-info/not-zip-safe
--rw-r--r--   0 blau       (501) staff       (20)     3228 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf.egg-info/SOURCES.txt
--rw-r--r--   0 blau       (501) staff       (20)      118 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf.egg-info/entry_points.txt
--rw-r--r--   0 blau       (501) staff       (20)       26 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf.egg-info/requires.txt
--rw-r--r--   0 blau       (501) staff       (20)        4 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf.egg-info/top_level.txt
--rw-r--r--   0 blau       (501) staff       (20)        1 2022-06-17 15:57:36.000000 ipf-1.7a5/ipf.egg-info/dependency_links.txt
--rw-r--r--   0 blau       (501) staff       (20)      388 2022-06-17 15:57:36.000000 ipf-1.7a5/MANIFEST.in
--rw-r--r--   0 blau       (501) staff       (20)     2752 2022-04-26 00:48:11.000000 ipf-1.7a5/README.md
--rw-r--r--   0 blau       (501) staff       (20)     3806 2022-06-16 18:52:31.000000 ipf-1.7a5/setup.py
--rw-r--r--   0 blau       (501) staff       (20)       98 2022-06-17 15:57:36.000000 ipf-1.7a5/setup.cfg
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.875905 ipf-1.7rc3/
+-rw-r--r--   0 blau       (501) staff       (20)    11357 2023-02-09 15:30:03.000000 ipf-1.7rc3/LICENSE
+-rw-r--r--   0 blau       (501) staff       (20)      392 2023-06-23 19:24:11.000000 ipf-1.7rc3/MANIFEST.in
+-rw-r--r--   0 blau       (501) staff       (20)     3386 2023-06-23 19:24:11.875986 ipf-1.7rc3/PKG-INFO
+-rw-r--r--   0 blau       (501) staff       (20)     2877 2023-02-09 15:30:03.000000 ipf-1.7rc3/README.md
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.852439 ipf-1.7rc3/ipf/
+-rw-r--r--   0 blau       (501) staff       (20)        0 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/__init__.py
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.856266 ipf-1.7rc3/ipf/bin/
+-rwxr-xr-x   0 blau       (501) staff       (20)      351 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/bin/ipf_configure
+-rwxr-xr-x   0 blau       (501) staff       (20)      585 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/bin/ipf_workflow
+-rw-r--r--   0 blau       (501) staff       (20)     6103 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/catalog.py
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.857096 ipf-1.7rc3/ipf/configure/
+-rw-r--r--   0 blau       (501) staff       (20)        0 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/configure/__init__.py
+-rw-r--r--   0 blau       (501) staff       (20)    39970 2023-06-09 22:06:56.000000 ipf-1.7rc3/ipf/configure/configure_workflows.py
+-rw-r--r--   0 blau       (501) staff       (20)     3228 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/configure/sysinfo.py
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.858186 ipf-1.7rc3/ipf/configure/test/
+-rw-r--r--   0 blau       (501) staff       (20)     6668 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/configure/test/subscribe_amqp.py
+-rwxr-xr-x   0 blau       (501) staff       (20)     2222 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/configure/test/validate.py
+-rwxr-xr-x   0 blau       (501) staff       (20)      875 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/configure/test/validate_activities.py
+-rwxr-xr-x   0 blau       (501) staff       (20)      657 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/configure/test/validate_compute.py
+-rwxr-xr-x   0 blau       (501) staff       (20)      573 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/configure/test/validate_modules.py
+-rw-r--r--   0 blau       (501) staff       (20)     6367 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/daemon.py
+-rw-r--r--   0 blau       (501) staff       (20)     2919 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/data.py
+-rw-r--r--   0 blau       (501) staff       (20)     3323 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/dt.py
+-rw-r--r--   0 blau       (501) staff       (20)     5025 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/engine.py
+-rw-r--r--   0 blau       (501) staff       (20)     1480 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/error.py
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.845936 ipf-1.7rc3/ipf/etc/
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.858524 ipf-1.7rc3/ipf/etc/ipf/
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.858660 ipf-1.7rc3/ipf/etc/ipf/ca-certificates/
+-rw-r--r--   0 blau       (501) staff       (20)    38688 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/etc/ipf/ca-certificates/ca_certs.pem
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.858893 ipf-1.7rc3/ipf/etc/ipf/init.d/
+-rwxr-xr-x   0 blau       (501) staff       (20)     2344 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/init.d/ipf-WORKFLOW
+-rw-r--r--   0 blau       (501) staff       (20)      502 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/logging.conf
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.859819 ipf-1.7rc3/ipf/etc/ipf/workflow/
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.859952 ipf-1.7rc3/ipf/etc/ipf/workflow/glue2/
+-rw-r--r--   0 blau       (501) staff       (20)      114 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/glue2/empty.txt
+-rw-r--r--   0 blau       (501) staff       (20)      460 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/ipfinfo.json
+-rw-r--r--   0 blau       (501) staff       (20)      276 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/ipfinfo_publish_periodic.json
+-rw-r--r--   0 blau       (501) staff       (20)      468 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/sysinfo.json
+-rw-r--r--   0 blau       (501) staff       (20)     1223 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/sysinfo_publish.json
+-rw-r--r--   0 blau       (501) staff       (20)      277 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/sysinfo_publish_periodic.json
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.846458 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.862701 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/
+-rw-r--r--   0 blau       (501) staff       (20)      336 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/abstractservice.json
+-rw-r--r--   0 blau       (501) staff       (20)     1735 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/catalina_pbs_compute.json
+-rw-r--r--   0 blau       (501) staff       (20)     1535 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/condor_compute.json
+-rw-r--r--   0 blau       (501) staff       (20)      350 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/extmodules.json
+-rw-r--r--   0 blau       (501) staff       (20)     1085 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/extmodulesremote.json
+-rw-r--r--   0 blau       (501) staff       (20)      582 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/ipfinfo_publish.json
+-rw-r--r--   0 blau       (501) staff       (20)      315 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/lmod.json
+-rw-r--r--   0 blau       (501) staff       (20)     1662 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/moab_pbs_compute.json
+-rw-r--r--   0 blau       (501) staff       (20)      321 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/modules.json
+-rw-r--r--   0 blau       (501) staff       (20)     1513 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/openstack_compute.json
+-rw-r--r--   0 blau       (501) staff       (20)      627 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/pbs_activity.json
+-rw-r--r--   0 blau       (501) staff       (20)     1508 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/pbs_compute.json
+-rw-r--r--   0 blau       (501) staff       (20)     1349 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/serviceremotepublish.json
+-rw-r--r--   0 blau       (501) staff       (20)      634 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/sge_activity.json
+-rw-r--r--   0 blau       (501) staff       (20)     1512 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/sge_compute.json
+-rw-r--r--   0 blau       (501) staff       (20)      640 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/slurm_activity.json
+-rw-r--r--   0 blau       (501) staff       (20)     1526 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/slurm_compute.json
+-rw-r--r--   0 blau       (501) staff       (20)     4022 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/fileread.py
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.875315 ipf-1.7rc3/ipf/glue2/
+-rw-r--r--   0 blau       (501) staff       (20)        0 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/__init__.py
+-rw-r--r--   0 blau       (501) staff       (20)    11051 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/abstractservice.py
+-rw-r--r--   0 blau       (501) staff       (20)    26949 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/accelerator_environment.py
+-rw-r--r--   0 blau       (501) staff       (20)     4716 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/activity.py
+-rw-r--r--   0 blau       (501) staff       (20)    10367 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/application.py
+-rw-r--r--   0 blau       (501) staff       (20)     2610 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/benchmark.py
+-rw-r--r--   0 blau       (501) staff       (20)     3936 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/catalina.py
+-rw-r--r--   0 blau       (501) staff       (20)    19496 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/cobalt.py
+-rw-r--r--   0 blau       (501) staff       (20)    14586 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/compute.py
+-rw-r--r--   0 blau       (501) staff       (20)    27319 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/computing_activity.py
+-rw-r--r--   0 blau       (501) staff       (20)    10602 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/computing_endpoint.py
+-rw-r--r--   0 blau       (501) staff       (20)    17446 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/computing_manager.py
+-rw-r--r--   0 blau       (501) staff       (20)     6636 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/computing_manager_accel_info.py
+-rw-r--r--   0 blau       (501) staff       (20)     8589 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/computing_service.py
+-rw-r--r--   0 blau       (501) staff       (20)    27079 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/computing_share.py
+-rw-r--r--   0 blau       (501) staff       (20)     7746 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/computing_share_accel_info.py
+-rw-r--r--   0 blau       (501) staff       (20)    14807 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/condor.py
+-rw-r--r--   0 blau       (501) staff       (20)     2621 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/contact.py
+-rw-r--r--   0 blau       (501) staff       (20)     5458 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/domain.py
+-rw-r--r--   0 blau       (501) staff       (20)    12319 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/endpoint.py
+-rw-r--r--   0 blau       (501) staff       (20)     4862 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/entity.py
+-rw-r--r--   0 blau       (501) staff       (20)    24821 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/execution_environment.py
+-rw-r--r--   0 blau       (501) staff       (20)     2448 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/genesisII.py
+-rw-r--r--   0 blau       (501) staff       (20)     4369 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/gram.py
+-rw-r--r--   0 blau       (501) staff       (20)     6579 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/installedservices.py
+-rw-r--r--   0 blau       (501) staff       (20)    20800 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/loadleveler.py
+-rw-r--r--   0 blau       (501) staff       (20)     6564 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/location.py
+-rw-r--r--   0 blau       (501) staff       (20)    25886 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/lsf.py
+-rw-r--r--   0 blau       (501) staff       (20)     4281 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/manager.py
+-rw-r--r--   0 blau       (501) staff       (20)     8483 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/moab.py
+-rw-r--r--   0 blau       (501) staff       (20)    17078 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/modules.py
+-rw-r--r--   0 blau       (501) staff       (20)    22021 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/nimbus.py
+-rw-r--r--   0 blau       (501) staff       (20)    19674 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/openstack.py
+-rw-r--r--   0 blau       (501) staff       (20)    32391 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/pbs.py
+-rw-r--r--   0 blau       (501) staff       (20)     2944 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/pbs_psc.py
+-rw-r--r--   0 blau       (501) staff       (20)     4020 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/resource.py
+-rw-r--r--   0 blau       (501) staff       (20)     6779 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/service.py
+-rw-r--r--   0 blau       (501) staff       (20)    26894 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/sge.py
+-rw-r--r--   0 blau       (501) staff       (20)     3013 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/sge_tacc.py
+-rw-r--r--   0 blau       (501) staff       (20)     5403 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/share.py
+-rw-r--r--   0 blau       (501) staff       (20)    53498 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/slurm.py
+-rw-r--r--   0 blau       (501) staff       (20)     2004 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/step.py
+-rw-r--r--   0 blau       (501) staff       (20)    10595 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/storageservice.py
+-rw-r--r--   0 blau       (501) staff       (20)     8085 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/types.py
+-rw-r--r--   0 blau       (501) staff       (20)     2481 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/glue2/unicore.py
+-rw-r--r--   0 blau       (501) staff       (20)     5266 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/glue2/valet.py
+-rw-r--r--   0 blau       (501) staff       (20)    13807 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/ipfinfo.py
+-rw-r--r--   0 blau       (501) staff       (20)     9913 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/log.py
+-rw-r--r--   0 blau       (501) staff       (20)     2086 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/paths.py
+-rw-r--r--   0 blau       (501) staff       (20)      439 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/pre_populate_position.py
+-rw-r--r--   0 blau       (501) staff       (20)    14215 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/publish.py
+-rw-r--r--   0 blau       (501) staff       (20)     4459 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/run_workflow.py
+-rw-r--r--   0 blau       (501) staff       (20)    14411 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/step.py
+-rw-r--r--   0 blau       (501) staff       (20)     3030 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/step_info.py
+-rw-r--r--   0 blau       (501) staff       (20)     8445 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/sysinfo.py
+-rw-r--r--   0 blau       (501) staff       (20)      284 2023-02-09 15:30:03.000000 ipf-1.7rc3/ipf/urnprefix.py
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.846685 ipf-1.7rc3/ipf/var/
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.875457 ipf-1.7rc3/ipf/var/ipf/
+-rw-r--r--   0 blau       (501) staff       (20)      114 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/var/ipf/README.txt
+-rw-r--r--   0 blau       (501) staff       (20)     6351 2022-12-22 20:34:43.000000 ipf-1.7rc3/ipf/workflow.py
+drwxr-xr-x   0 blau       (501) staff       (20)        0 2023-06-23 19:24:11.855918 ipf-1.7rc3/ipf.egg-info/
+-rw-r--r--   0 blau       (501) staff       (20)     3386 2023-06-23 19:24:11.000000 ipf-1.7rc3/ipf.egg-info/PKG-INFO
+-rw-r--r--   0 blau       (501) staff       (20)     3273 2023-06-23 19:24:11.000000 ipf-1.7rc3/ipf.egg-info/SOURCES.txt
+-rw-r--r--   0 blau       (501) staff       (20)        1 2023-06-23 19:24:11.000000 ipf-1.7rc3/ipf.egg-info/dependency_links.txt
+-rw-r--r--   0 blau       (501) staff       (20)      115 2023-06-23 19:24:11.000000 ipf-1.7rc3/ipf.egg-info/entry_points.txt
+-rw-r--r--   0 blau       (501) staff       (20)        1 2022-12-22 20:44:40.000000 ipf-1.7rc3/ipf.egg-info/not-zip-safe
+-rw-r--r--   0 blau       (501) staff       (20)       26 2023-06-23 19:24:11.000000 ipf-1.7rc3/ipf.egg-info/requires.txt
+-rw-r--r--   0 blau       (501) staff       (20)        4 2023-06-23 19:24:11.000000 ipf-1.7rc3/ipf.egg-info/top_level.txt
+-rw-r--r--   0 blau       (501) staff       (20)       98 2023-06-23 19:24:11.876280 ipf-1.7rc3/setup.cfg
+-rw-r--r--   0 blau       (501) staff       (20)     3845 2023-06-23 19:01:52.000000 ipf-1.7rc3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ipf-1.7a5/PKG-INFO` & `ipf-1.7rc3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ipf
-Version: 1.7a5
+Version: 1.7rc3
 Summary: The Information Publishing Framework
-Home-page: https://github.com/xsede/ipf
+Home-page: https://github.com/access-ci-org/ipf
 Author: Eric Blau, Warren Smith
 Author-email: blau@anl.gov
 License: Apache
-Description: 
-        # ipf-xsede %VER%-%REL%
-        # README
-        ## Overview
-        
-        The Information Publishing Framework (IPF) is a generic framework for gathering and publishing information. IPF
-        focuses narrowly on gatethering and publishing, and not on analyzing or visualizing information. IPF grew out of
-        work to publish information about TeraGrid compute resources using the
-        [GLUE 2 specification](http://www.ogf.org/documents/GFD.147.pdf). IPF continues to support data gathering and
-        publishing in the XSEDE program which succeeded TeraGrid.
-        
-        IPF gathers and publishes information using simple workflows. These workflows are defined using JSON (see the
-        etc/workflows directory) and steps in the workflows are implemented as Python classes. Each step in the
-        workflow can require input Data, can produce output Data, and can publish Representations of Data. A typical
-        workflow consists of a number of information gathering steps and a few steps that publish Representations to
-        files or to remote services (e.g. REST, messaging).
-        
-        Workflow steps specify what Data they require and what Data they produce. This allows IPF to construct
-        workflows based on partial information - in the case where there are not steps that produce the same Data, an
-        entire workflow can be constructed from a single publish step and its required input Data. At the other
-        extreme, workflows can be exactly specified with specific steps identified and the outputs of steps bound to
-        the inputs of other steps. A typical workflow (e.g. GLUE 2) specifies what steps to include but lets IPF
-        automatically link outputs to inputs of these steps.
-        
-        Workflows can run to completion relatively quickly or they can continuously run. The first type of workflow
-        can be used to run a few commands or look at status files and publish that information. The second type of
-        workflow can be used to monitor log files and publish entries written to those files. Workflows are typically
-        run periodically as cron jobs. The program libexec/run_workflow.py is for executing workflows that complete
-        quickly and the program libexec/run_workflow_daemon.py is used to manage long-running workflows. The daemon
-        
-        ## License
-        
-        This software is licensed under Version 2.0 of the Apache License.
-        
-        ## Installation
-        
-        Installation instructions are in [docs/INSTALL.md](docs/INSTALL.md).
-        
-        ## Contact Information
-        
-        This software is maintained by [XSEDE](https://www.github.com/XSEDE).  and you can contact the XSEDE helpdesk
-        if you need help using it.
-        
-        If you have problems with this software you are welcome to submit an [issue](https://github.com/XSEDE/ipf/issues).
-        
-        ## Acknowledgements
-        
-        This work was supported by the TeraGrid, XSEDE, FutureGrid, and XSEDE 2 projects under National Science Foundation
-        grants 0503697, 1053575, 0910812, and 1548562.
-        
 Keywords: monitoring information gathering publishing glue2
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Topic :: System :: Monitoring
+License-File: LICENSE
+
+
+# access-ci-org/ipf %VER%-%REL%
+# README
+
+## Overview
+
+The Information Publishing Framework (IPF) is a generic framework used by resource operators to gather and publish
+dynamic resource information in [GLUE 2 serialized format](http://www.ogf.org/documents/GFD.147.pdf). IPF was used
+by the TeraGrid, XSEDE, and XSEDE 2 programs, and is currently being used by the ACCESS-CI program to publish
+high-performance compute cluster information.
+
+IPF gathers and publishes information using simple workflows. These workflows are defined using JSON (see the
+etc/workflows directory) and steps in the workflows are implemented as Python classes. Each step in the
+workflow can require input Data, can produce output Data, and can publish Representations of Data. A typical
+workflow consists of a number of information gathering steps and a few steps that publish representations to
+files or to remote services (e.g. REST, messaging).
+
+Workflow steps specify what Data they require and what Data they produce. This allows IPF to construct
+workflows based on partial information - in the case where there are not steps that produce the same Data, an
+entire workflow can be constructed from a single publish step and its required input Data. At the other
+extreme, workflows can be exactly specified with specific steps identified and the outputs of steps bound to
+the inputs of other steps. A typical workflow (e.g. GLUE 2) specifies what steps to include but lets IPF
+automatically link outputs to inputs of these steps.
+
+Workflows can run to completion relatively quickly or they can continuously run. The first type of workflow
+can be used to run a few commands or look at status files and publish that information. The second type of
+workflow can be used to monitor log files and publish entries written to those files. Workflows are typically
+run periodically as cron jobs. The program libexec/run_workflow.py is for executing workflows that complete
+quickly and the program libexec/run_workflow_daemon.py is used to manage long-running workflows. The daemon
+
+## License
+
+This software is licensed the Apache License Version 2.0.
+
+## Installation
+
+Installation instructions are in [docs/INSTALL.md](docs/INSTALL.md).
+
+## Support Information
+
+This software is currently maintained by the ACCESS CONECT project.
+
+The source is maintained in the [ACCESS-CI GitHub](https://github.com/access-ci-org/ipf).  ACCESS-CI resource
+providers and other members of the ACCESS-CI community are encourage to contribute bug fixes and improvements.
+
+Software bugs may be reported as GitHub issues.  ACCESS-CI related support requests should be submitted through
+the ACCESS-CI ticket system.
+
+## Acknowledgements
+
+This work was supported by the TeraGrid, XSEDE, FutureGrid, XSEDE 2, and ACCESS CONECT projects under
+National Science Foundation grants 0503697, 1053575, 0910812, 1548562, and 2138307.
```

### Comparing `ipf-1.7a5/LICENSE-2.0.txt` & `ipf-1.7rc3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `ipf-1.7a5/ipf/catalog.py` & `ipf-1.7rc3/ipf/catalog.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/error.py` & `ipf-1.7rc3/ipf/error.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/paths.py` & `ipf-1.7rc3/ipf/paths.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/bin/ipf_workflow` & `ipf-1.7rc3/ipf/bin/ipf_workflow`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/log.py` & `ipf-1.7rc3/ipf/log.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/dt.py` & `ipf-1.7rc3/ipf/dt.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/init.d/ipf-WORKFLOW` & `ipf-1.7rc3/ipf/etc/ipf/init.d/ipf-WORKFLOW`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/xsede/ca_certs.pem` & `ipf-1.7rc3/ipf/etc/ipf/ca-certificates/ca_certs.pem`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/sysinfo_publish.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/sysinfo_publish.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/serviceremotepublish.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/serviceremotepublish.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7336111111111111%*

 * *Differences: {"'name'": "'Publishservices'",*

 * * "'steps'": "{1: {'params': {'resource_name': 'testing.access-ci.org'}}, 4: {'description': "*

 * *            "'Publish service and endpoint information to ACCESS', 'params': {'services': "*

 * *            "['opspub1.access-ci.org', 'opspub2.access-ci.org'], 'ssl_options': {'ca_certs': "*

 * *            "'ca-certificates/ca_certs.pem'}, 'vhost': 'infopub'}}}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "name": "XSEDEservices",
+    "name": "Publishservices",
     "steps": [
         {
             "name": "ipf.glue2.location.LocationStep",
             "params": {
                 "location": {
                     "Country": "US",
                     "Latitude": 38.0,
@@ -12,15 +12,15 @@
                     "Place": "City"
                 }
             }
         },
         {
             "name": "ipf.sysinfo.ResourceNameStep",
             "params": {
-                "resource_name": "testing.xsede.org"
+                "resource_name": "testing.access-ci.org"
             }
         },
         {
             "name": "ipf.glue2.abstractservice.AbstractServiceStep"
         },
         {
             "name": "ipf.publish.FileStep",
@@ -28,28 +28,28 @@
                 "path": "extserv.json",
                 "publish": [
                     "ipf.glue2.abstractservice.ASOgfJson"
                 ]
             }
         },
         {
-            "description": "Publish service and endpoint information to XSEDE",
+            "description": "Publish service and endpoint information to ACCESS",
             "name": "ipf.publish.AmqpStep",
             "params": {
                 "exchange": "glue2.compute",
                 "publish": [
                     "ipf.glue2.abstractservice.ASOgfJson"
                 ],
                 "services": [
-                    "info1.dyn.xsede.org",
-                    "info2.dyn.xsede.org"
+                    "opspub1.access-ci.org",
+                    "opspub2.access-ci.org"
                 ],
                 "ssl_options": {
-                    "ca_certs": "xsede/ca_certs.pem",
+                    "ca_certs": "ca-certificates/ca_certs.pem",
                     "certfile": "/tmp/x509up_u501",
                     "keyfile": "/tmp/x509up_u501"
                 },
-                "vhost": "xsede"
+                "vhost": "infopub"
             }
         }
     ]
 }
```

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/moab_pbs_compute.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/moab_pbs_compute.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/extmodulesremote.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/sge_compute.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2701655982905983%*

 * *Differences: {"'description'": "'This workflow gathers GLUE2 compute information by interacting with SGE'",*

 * * "'name'": "'sge_compute'",*

 * * "'steps'": "{2: {'name': 'ipf.glue2.location.LocationStep', 'params': {replace: "*

 * *            "OrderedDict([('location', OrderedDict([('Name', 'Name of Center'), ('Place', 'City'), "*

 * *            "('Country', 'US'), ('Latitude', 38.0), ('Longitude', -90.0)]))])}}, 10: {'name': "*

 * *            "'ipf.glue2.sge.ComputingManagerAcceleratorInfoStep'}, 11: {'params': {'publish': "*

 * *            " […]*

```diff
@@ -1,43 +1,69 @@
 {
-    "name": "modules",
+    "description": "This workflow gathers GLUE2 compute information by interacting with SGE",
+    "name": "sge_compute",
     "steps": [
         {
-            "name": "ipf.sysinfo.ResourceNameStep",
+            "name": "ipf.sysinfo.ResourceNameStep"
+        },
+        {
+            "name": "ipf.sysinfo.PlatformStep"
+        },
+        {
+            "name": "ipf.glue2.location.LocationStep",
             "params": {
-                "resource_name": "testing.xsede.org"
+                "location": {
+                    "Country": "US",
+                    "Latitude": 38.0,
+                    "Longitude": -90.0,
+                    "Name": "Name of Center",
+                    "Place": "City"
+                }
             }
         },
         {
-            "name": "ipf.glue2.modules.ExtendedModApplicationsStep"
+            "name": "ipf.glue2.sge.ComputingActivitiesStep"
+        },
+        {
+            "name": "ipf.glue2.sge.ComputingSharesStep"
+        },
+        {
+            "name": "ipf.glue2.sge.ComputingShareAcceleratorInfoStep"
+        },
+        {
+            "name": "ipf.glue2.sge.ComputingServiceStep"
         },
         {
+            "name": "ipf.glue2.sge.ExecutionEnvironmentsStep"
+        },
+        {
+            "name": "ipf.glue2.sge.AcceleratorEnvironmentsStep"
+        },
+        {
+            "name": "ipf.glue2.sge.ComputingManagerStep"
+        },
+        {
+            "name": "ipf.glue2.sge.ComputingManagerAcceleratorInfoStep"
+        },
+        {
+            "description": "Publish JSON version of compute resource description to a file for debugging",
             "name": "ipf.publish.FileStep",
             "params": {
-                "path": "extended_modules.json",
+                "path": "compute.json",
                 "publish": [
-                    "ipf.glue2.application.ApplicationsOgfJson"
+                    "ipf.glue2.compute.PublicOgfJson"
                 ]
             }
         },
         {
-            "description": "Publish extended modules to XSEDE",
-            "name": "ipf.publish.AmqpStep",
+            "description": "Publish a description of current jobs in JSON to a file for debugging",
+            "name": "ipf.publish.FileStep",
             "params": {
-                "exchange": "glue2.applications",
+                "path": "activities.json",
                 "publish": [
-                    "ipf.glue2.application.ApplicationsOgfJson"
-                ],
-                "services": [
-                    "info1.dyn.xsede.org",
-                    "info2.dyn.xsede.org"
-                ],
-                "ssl_options": {
-                    "ca_certs": "xsede/ca_certs.pem",
-                    "certfile": "/tmp/x509up_u501",
-                    "keyfile": "/tmp/x509up_u501"
-                },
-                "vhost": "xsede"
+                    "ipf.glue2.compute.PrivateOgfJson"
+                ]
             }
         }
-    ]
+    ],
+    "timeout": 55
 }
```

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/condor_compute.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/condor_compute.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/pbs_activity.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/pbs_activity.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/sge_activity.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/sge_activity.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/ipfinfo_publish.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/ipfinfo_publish.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/sge_compute.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/pbs_compute.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7115384615384616%*

 * *Differences: {"'description'": "'This workflow gathers GLUE2 compute information by interacting with PBS'",*

 * * "'name'": "'compute'",*

 * * "'steps'": "{3: {'name': 'ipf.glue2.pbs.ComputingActivitiesStep'}, 4: {'name': "*

 * *            "'ipf.glue2.pbs.ComputingSharesStep'}, 5: {'name': "*

 * *            "'ipf.glue2.pbs.ComputingShareAcceleratorInfoStep'}, 6: {'name': "*

 * *            "'ipf.glue2.pbs.ComputingServiceStep'}, 7: {'name': "*

 * *            "'ipf.glue2.pbs.ExecutionEnvironmentsStep'}, 8: {'name': "*

 * *            "'ipf.glue2.pbs.Ac […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "description": "This workflow gathers GLUE2 compute information by interacting with SGE",
-    "name": "sge_compute",
+    "description": "This workflow gathers GLUE2 compute information by interacting with PBS",
+    "name": "compute",
     "steps": [
         {
             "name": "ipf.sysinfo.ResourceNameStep"
         },
         {
             "name": "ipf.sysinfo.PlatformStep"
         },
@@ -17,36 +17,36 @@
                     "Longitude": -90.0,
                     "Name": "Name of Center",
                     "Place": "City"
                 }
             }
         },
         {
-            "name": "ipf.glue2.sge.ComputingActivitiesStep"
+            "name": "ipf.glue2.pbs.ComputingActivitiesStep"
         },
         {
-            "name": "ipf.glue2.sge.ComputingSharesStep"
+            "name": "ipf.glue2.pbs.ComputingSharesStep"
         },
         {
-            "name": "ipf.glue2.sge.ComputingShareAcceleratorInfoStep"
+            "name": "ipf.glue2.pbs.ComputingShareAcceleratorInfoStep"
         },
         {
-            "name": "ipf.glue2.sge.ComputingServiceStep"
+            "name": "ipf.glue2.pbs.ComputingServiceStep"
         },
         {
-            "name": "ipf.glue2.sge.ExecutionEnvironmentsStep"
+            "name": "ipf.glue2.pbs.ExecutionEnvironmentsStep"
         },
         {
-            "name": "ipf.glue2.sge.AcceleratorEnvironmentsStep"
+            "name": "ipf.glue2.pbs.AcceleratorEnvironmentsStep"
         },
         {
-            "name": "ipf.glue2.sge.ComputingManagerStep"
+            "name": "ipf.glue2.pbs.ComputingManagerStep"
         },
         {
-            "name": "ipf.glue2.sge.ComputingManagerAcceleratorInfoStep"
+            "name": "ipf.glue2.pbs.ComputingManagerAcceleratorInfoStep"
         },
         {
             "description": "Publish JSON version of compute resource description to a file for debugging",
             "name": "ipf.publish.FileStep",
             "params": {
                 "path": "compute.json",
                 "publish": [
```

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/pbs_compute.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/catalina_pbs_compute.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8583333333333334%*

 * *Differences: {"'description'": "'This workflow gathers GLUE2 compute information by interacting with Catalina "*

 * *                  "and PBS'",*

 * * "'steps'": "{insert: [(3, OrderedDict([('name', 'ipf.glue2.pbs.ComputingActivitiesStep'), "*

 * *            "('outputs', ['step-catalina-activities'])])), (4, OrderedDict([('name', "*

 * *            "'ipf.glue2.catalina.ComputingActivitiesStep'), ('id', "*

 * *            "'step-catalina-activities')]))]}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "description": "This workflow gathers GLUE2 compute information by interacting with PBS",
+    "description": "This workflow gathers GLUE2 compute information by interacting with Catalina and PBS",
     "name": "compute",
     "steps": [
         {
             "name": "ipf.sysinfo.ResourceNameStep"
         },
         {
             "name": "ipf.sysinfo.PlatformStep"
@@ -17,14 +17,24 @@
                     "Longitude": -90.0,
                     "Name": "Name of Center",
                     "Place": "City"
                 }
             }
         },
         {
+            "name": "ipf.glue2.pbs.ComputingActivitiesStep",
+            "outputs": [
+                "step-catalina-activities"
+            ]
+        },
+        {
+            "id": "step-catalina-activities",
+            "name": "ipf.glue2.catalina.ComputingActivitiesStep"
+        },
+        {
             "name": "ipf.glue2.pbs.ComputingActivitiesStep"
         },
         {
             "name": "ipf.glue2.pbs.ComputingSharesStep"
         },
         {
             "name": "ipf.glue2.pbs.ComputingShareAcceleratorInfoStep"
```

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/slurm_activity.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/slurm_activity.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/slurm_compute.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/slurm_compute.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/etc/ipf/workflow/templates/glue2/openstack_compute.json` & `ipf-1.7rc3/ipf/etc/ipf/workflow/templates/glue2/openstack_compute.json`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/step_info.py` & `ipf-1.7rc3/ipf/step_info.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/step.py` & `ipf-1.7rc3/ipf/step.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/engine.py` & `ipf-1.7rc3/ipf/engine.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/xsede/test/validate_activities.py` & `ipf-1.7rc3/ipf/configure/test/validate_activities.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/xsede/test/validate_compute.py` & `ipf-1.7rc3/ipf/configure/test/validate_compute.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/xsede/test/validate_modules.py` & `ipf-1.7rc3/ipf/configure/test/validate_modules.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/xsede/test/subscribe_amqp.py` & `ipf-1.7rc3/ipf/configure/test/subscribe_amqp.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,18 @@
                       help="the virtual host in the messaging service to connect to")
     parser.add_option("-e","--exchange",default="amq.topic",dest="exchange",
                       help="an exchange in the virtual host to publish or subscribe to")
     return parser
 
 #######################################################################################################################
 
-if os.path.exists(os.path.join("etc","ipf","xsede","ca_certs.pem")):
-    ca_cert_file = (os.path.join("etc","ipf","xsede","ca_certs.pem"))
-elif os.path.exists(os.path.join(os.path.dirname(os.path.abspath(__file__)),"etc","ipf","xsede","ca_certs.pem")):
-    ca_cert_file = os.path.join(os.path.dirname(os.path.abspath(__file__)),"etc","ipf","xsede","ca_certs.pem")
+if os.path.exists(os.path.join("etc","ipf","ca-certificates","ca_certs.pem")):
+    ca_cert_file = (os.path.join("etc","ipf","ca-certificates","ca_certs.pem"))
+elif os.path.exists(os.path.join(os.path.dirname(os.path.abspath(__file__)),"etc","ipf","ca-certificates","ca_certs.pem")):
+    ca_cert_file = os.path.join(os.path.dirname(os.path.abspath(__file__)),"etc","ipf","ca-certificates","ca_certs.pem")
 
 def connect(options):
     # port 5671 is for SSL, port 5672 is for TCP
     if options.keyfile is not None or options.certfile is not None:
         if options.keyfile is None:
             print("you must specify a key file for user with your cert file")
             sys.exit(1)
```

### Comparing `ipf-1.7a5/ipf/xsede/test/validate.py` & `ipf-1.7rc3/ipf/configure/test/validate.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/xsede/sysinfo.py` & `ipf-1.7rc3/ipf/configure/sysinfo.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/xsede/configure_workflows.py` & `ipf-1.7rc3/ipf/configure/configure_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,32 +54,32 @@
                         help='Set the base directory')
     parser.add_argument('--scheduler', \
                         help='set the scheduler name')
     parser.add_argument('-scheduler_params', action='store', \
                         help='comma delimited key:value pairs for parameters for your scheduler')
     parser.add_argument('--amqp_username', \
                         #action='store_const',const='username', dest='mode',\
-                        help='Username for publishing to XSEDE AMQP. Not needed if using certificate')
+                        help='Username for publishing to AMQP. Not needed if using certificate')
     parser.add_argument('--amqp_certificate', \
                         #action='store_const',const='certificate', dest='mode',\
-                        help='Location of certificate for publishing to XSEDE AMQP. Not needed if using username')
+                        help='Location of certificate for publishing to AMQP. Not needed if using username')
     parser.add_argument('--amqp_password', \
-                        help='Password for publishing to XSEDE AMQP. Not needed if using certificate')
+                        help='Password for publishing to AMQP. Not needed if using certificate')
     parser.add_argument('--amqp_certificate_key', \
-                        help='Location of certificate key for publishing to XSEDE AMQP. Not needed if using username')
+                        help='Location of certificate key for publishing to AMQP. Not needed if using username')
     parser.add_argument('--modulepath', \
                         help='MODULEPATH for software publishing workflow')
     parser.add_argument('--servicepath', \
                         help='SERVICEPATH for service publishing workflow')
     parser.add_argument('--workflows', \
                         help='Comma delimited list of workflows to configure')
     parser.add_argument('--workflowtemplate', \
                         help='Path to configured workflow to use as template for new workflow')
-    parser.add_argument('--publish_to_xsede', action='store_true', \
-                        help='Configure the services to publish to XSEDE')
+    parser.add_argument('--publish', action='store_true', \
+                        help='Configure the services to publish to ACCESS-CI')
     parser.add_argument('--compute_interval', \
                         help='Interval in seconds for the compute workflow to wait before rerunning')
     parser.add_argument('--modules', \
                         help='Any modules that need to be loaded in the init scripts for workflows')
     parser.add_argument('--environment', \
                         help='Any environment variables that needs to be loaded in the init scripts for workflows, such as \n * batch scheduler commands that need to be in PATH \n * scheduler-related environment variables may need to be set')
     parser.add_argument('--pbs_log_dir', \
@@ -144,16 +144,16 @@
     else:
         sched_name = getSchedulerName()
     #if template_json is a compute workflow, then compute_json should be template_json
     compute_json = getComputeJsonForScheduler(sched_name,template_json)
     setResourceName(resource_name, compute_json)
     setLocation(compute_json,args,template_json)
     updateFilePublishPaths(resource_name, compute_json)
-    if (args.publish_to_xsede):
-        addXsedeAmqpToWorkflow("compute",compute_json, template_json, args)
+    if (args.publish):
+        addAccessAmqpToWorkflow("compute",compute_json, template_json, args)
     writeComputeWorkflow(resource_name, compute_json)
     writePeriodicComputeWorkflow(resource_name,args)
 
     module_names = getModules(args)
     env_vars = getEnvironmentVariables(args)
     writeComputeInit(resource_name, module_names, env_vars)
 
@@ -163,56 +163,56 @@
     else:
         sched_name = getSchedulerName()
 
     activity_json = getActivityJsonForScheduler(sched_name,template_json)
     setResourceName(resource_name, activity_json)
     updateActivityLogFile(resource_name, activity_json, args)
     updateFilePublishPaths(resource_name, activity_json)
-    if (args.publish_to_xsede):
-        addXsedeAmqpToWorkflow("activity",activity_json, template_json, args)
+    if (args.publish):
+        addAccessAmqpToWorkflow("activity",activity_json, template_json, args)
     writeActivityWorkflow(resource_name, activity_json)
 
     module_names = getModules(args)
     env_vars = getEnvironmentVariables(args)
     writeActivityInit(resource_name, module_names, env_vars)
 
 
 def configure_extmodules_workflow(resource_name,args,template_json):
     extmodules_json = getExtModulesJson(template_json)
     setSupportContact(extmodules_json,args)
     setResourceName(resource_name, extmodules_json)
     updateFilePublishPaths(resource_name, extmodules_json)
-    if (args.publish_to_xsede):
-        addXsedeAmqpToWorkflow("extmodules",extmodules_json, template_json, args)
+    if (args.publish):
+        addAccessAmqpToWorkflow("extmodules",extmodules_json, template_json, args)
     writeExtModulesWorkflow(resource_name, extmodules_json)
     writePeriodicExtModulesWorkflow(resource_name,args)
 
     module_names = getModules(args)
     env_vars = getEnvironmentVariables(args)
     writeExtModulesInit(resource_name, module_names, env_vars)
 
 def configure_services_workflow(resource_name,args,template_json):
     services_json = getAbstractServicesJson(template_json)
     setResourceName(resource_name, services_json)
     updateFilePublishPaths(resource_name, services_json)
-    if (args.publish_to_xsede):
-        addXsedeAmqpToWorkflow("services",services_json, template_json, args)
+    if (args.publish):
+        addAccessAmqpToWorkflow("services",services_json, template_json, args)
     writeAbstractServicesWorkflow(resource_name, services_json)
     writePeriodicAbstractServicesWorkflow(resource_name,args)
 
 
     module_names = getModules(args)
     env_vars = getEnvironmentVariables(args)
     writeAbstractServicesInit(resource_name, module_names, env_vars)
 
 
 def configure_ipfinfo_workflow(resource_name,args,template_json):
     ipfinfo_json = getIPFInfoJson(template_json)
-    if (args.publish_to_xsede):
-        addXsedeAmqpToWorkflow("ipfinfo",ipfinfo_json, template_json, args)
+    if (args.publish):
+        addAccessAmqpToWorkflow("ipfinfo",ipfinfo_json, template_json, args)
     writeIPFInfoWorkflow(ipfinfo_json)
 
     module_names = getModules(args)
     env_vars = getEnvironmentVariables(args)
     writeIPFInfoInit(resource_name, module_names, env_vars)
 
 #######################################################################################################################
@@ -220,15 +220,15 @@
     if template_json is not None:
         for step_json in template_json["steps"]:
             if step_json["name"] == "ipf.sysinfo.ResourceNameStep":
                 if "params" in step_json:
                     resource_name = step_json["params"]["resource_name"]
             return resource_name
     else:
-        print('\nNo XSEDE resource name specified.  You must do one of:\n     * make sure xdresourceid is in your path\n     *use the command line option "--resource_name <name>"\n     *specify a template file that defines the resource name, using --workflowtemplate <file.json>')
+        print('\nNo resource name specified.  You must do one of:\n     * make sure xdresourceid is in your path\n     *use the command line option "--resource_name <name>"\n     *specify a template file that defines the resource name, using --workflowtemplate <file.json>')
         raise SystemExit
     return
 
 
 def getTemplateJson(template_name):
     if template_name:
         if not testReadFile(template_name):
@@ -385,37 +385,37 @@
 def updateFilePublishPaths(resource_name, workflow_json):
     res_name = resource_name.split(".")[0]
     for step_json in workflow_json["steps"]:
         if step_json["name"] == "ipf.publish.FileStep":
             step_json["params"]["path"] = res_name + \
                 "_" + step_json["params"]["path"]
 
-def addXsedeAmqpToWorkflow(workflow_name,workflow_json, template_json, args):
-    if not args.publish_to_xsede:
+def addAccessAmqpToWorkflow(workflow_name,workflow_json, template_json, args):
+    if not args.publish:
         return False
     if workflow_name == "compute":
         publish_step = "ipf.glue2.compute.PublicOgfJson"
         exchange = "glue2.compute"
-        description = "Publish compute resource description to XSEDE"
+        description = "Publish compute resource description to ACCESS-CI"
     elif workflow_name == "activity":
         publish_step = "ipf.glue2.computing_activity.ComputingActivityOgfJson"
         exchange = "glue2.computing_activity"
-        description = "Publish job updates to XSEDE"
+        description = "Publish job updates to ACCESS-CI"
     elif workflow_name == "extmodules":
         publish_step = "ipf.glue2.application.ApplicationsOgfJson"
         exchange = "glue2.applications"
-        description = "Publish modules to XSEDE"
+        description = "Publish modules to ACCESS-CI"
     elif workflow_name == "services":
         publish_step = "ipf.glue2.abstractservice.ASOgfJson"
         exchange = "glue2.compute"
-        description = "Publish Services to XSEDE"
+        description = "Publish Services to ACCESS-CI"
     elif workflow_name == "ipfinfo":
         publish_step = "ipf.ipfinfo.IPFInformationJson"
         exchange = "glue2.compute"
-        description = "Publish IPFInfo to XSEDE"
+        description = "Publish IPFInfo to ACCESS-CI"
     if args.amqp_certificate:
         cert_path = args.amqp_certificate
         if not testReadFile(cert_path):
             raise Exception("No certificate found at %s" % cert_path)
         
         if args.amqp_certificate_key:
             key_path = args.amqp_certificate_key
@@ -431,16 +431,16 @@
     elif template_json is not None:
         try:
             template_json["name"].index("_"+workflow_name)
         except ValueError:
             #Template is not for workflow--copy section in
             for step in template_json["steps"]:
                 #compute workflow has two publish steps, copy both
-                if step["name"] == "ipf.publish.AmqpStep" and "xsede.org" in step["params"]["services"][0]:
-                    if workflow_name == "compute" and step["description"] == "Publish description of current jobs to XSEDE":
+                if step["name"] == "ipf.publish.AmqpStep" and "access-ci.org" in step["params"]["services"][0]:
+                    if workflow_name == "compute" and step["description"] == "Publish description of current jobs to ACCESS-CI":
                         publish_description = step["description"]
                     else:
                         publish_description = description
                     amqp_step = copy.deepcopy(step)
                     amqp_step["description"] = publish_description
                     amqp_step["params"]["publish"] = [publish_step]
                     amqp_step["params"]["exchange"] = exchange
@@ -454,30 +454,30 @@
     #No template json to copy
     amqp_step = {}
     amqp_step["name"] = "ipf.publish.AmqpStep"
     amqp_step["description"] = description 
     amqp_step["params"] = {}
     amqp_step["params"]["publish"] = [publish_step]
     amqp_step["params"]["services"] = [
-        "infopub.xsede.org", "infopub-alt.xsede.org"]
-    amqp_step["params"]["vhost"] = "xsede"
+        "opspub.access-ci.org", "opspub-alt.access-ci.org"]
+    amqp_step["params"]["vhost"] = "infopub"
     amqp_step["params"]["exchange"] = exchange
     amqp_step["params"]["ssl_options"] = {}
-    amqp_step["params"]["ssl_options"]["ca_certs"] = "xsede/ca_certs.pem"
+    amqp_step["params"]["ssl_options"]["ca_certs"] = "ca-certificates/ca_certs.pem"
     if cert_path is not None:
         amqp_step["params"]["ssl_options"]["certfile"] = cert_path
         amqp_step["params"]["ssl_options"]["keyfile"] = key_path
     else:
         amqp_step["params"]["username"] = username
         amqp_step["params"]["password"] = password
     workflow_json["steps"].append(amqp_step)
     
     if workflow_name == "compute":
         amqp_step = copy.deepcopy(amqp_step)
-        amqp_step["description"] = "Publish description of current jobs to XSEDE"
+        amqp_step["description"] = "Publish description of current jobs to ACCESS-CI"
         amqp_step["params"]["publish"] = ["ipf.glue2.compute.PrivateOgfJson"]
         amqp_step["params"]["exchange"] = "glue2.computing_activities"
         workflow_json["steps"].append(amqp_step)
     return True
 
 
 def updateActivityLogFile(resource_name, activity_json, args):
```

### Comparing `ipf-1.7a5/ipf/sysinfo.py` & `ipf-1.7rc3/ipf/sysinfo.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/workflow.py` & `ipf-1.7rc3/ipf/workflow.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/ipfinfo.py` & `ipf-1.7rc3/ipf/ipfinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import os
 import json
 
 from ipf.data import Data, Representation
 from ipf.error import StepError
 from ipf.step import Step
 from ipf.paths import IPF_PARENT_PATH, IPF_ETC_PATH, IPF_WORKFLOW_PATHS, IPF_VAR_PATH
+from ipf.urnprefix import IPF_URN_PREFIX
 from ipf.sysinfo import ResourceName
 
 from .glue2.entity import *
 
 #######################################################################################################################
 
 
@@ -258,15 +259,15 @@
 
     def run(self):
         ipfinfo = IPFInformation()
         ipfinfo.ipf_version = self._getInput(IPFVersion)
         ipfinfo.workflows = self._getInput(IPFWorkflows)
         ipfinfo.resource_name = self._getInput(SiteName)
         ipfinfo.type = "IPF"
-        ipfinfo.id = "urn:glue2:PublisherInfo:%s" % '-'.join(
+        ipfinfo.id = IPF_URN_PREFIX + "PublisherInfo:%s" % '-'.join(
             [ipfinfo.type, IPFVersionTxt(ipfinfo.ipf_version).get()])
         # self._output(IPFInformation(self._getInput(IPFVersion).ipf_version,
         #                               self._getInput(IPFWorkflows).workflows,
         #                               self._getInput(ResourceName).resource_name))
         self._output(ipfinfo)
 
 
@@ -305,15 +306,15 @@
         if "CreationTime" in doc:
             self.CreationTime = textToDateTime(doc["CreationTime"])
         else:
             self.CreationTime = datetime.datetime.now(tzoffset(0))
         self.Validity = doc.get("Validity", Location.DEFAULT_VALIDITY)
         self.ipf_version = doc.get("ipf_version", "unknown")
         self.type = "IPF"
-        self.ID = "urn:ogf:glue2:xsede.org:PublisherInfo:%s" % str.join(
+        self.ID = IPF_URN_PREFIX + "PublisherInfo:%s" % str.join(
             '-', self.type, self.ipf_version)
         self.id = self.ID
         self.workflows = doc.get("workflows", "unknown")
         self.resource_name = doc.get("resource_name", "unknown")
 
 #######################################################################################################################
 
@@ -357,12 +358,12 @@
             doc["Version"] = IPFVersionTxt(self.data.ipf_version).get()
         if self.data.resource_name is not None:
             doc["Hostname"] = SiteNameTxt(self.data.resource_name).get()
         if self.data.workflows is not None:
             doc["Workflows"] = IPFWorkflowsTxt(self.data.workflows).get()
         doc["Type"] = "IPF"
         s = '-'
-        doc["ID"] = "urn:ogf:glue2:xsede.org:PublisherInfo:%s" % s.join(
+        doc["ID"] = IPF_URN_PREFIX + "PublisherInfo:%s" % s.join(
             (doc["Type"], doc["Version"]))
         return doc
 
 #######################################################################################################################
```

### Comparing `ipf-1.7a5/ipf/fileread.py` & `ipf-1.7rc3/ipf/fileread.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/data.py` & `ipf-1.7rc3/ipf/data.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/installedservices.py` & `ipf-1.7rc3/ipf/glue2/installedservices.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         handle.Value = name+"/"+version
 
         apps.add(env, [handle])
 
 #######################################################################################################################
 
 
-class ComputingServiceXsedeJson(ServiceOgfJson):
+class ComputingServiceInstalledJson(ServiceOgfJson):
     data_cls = ComputingService
 
     def __init__(self, data):
         ServiceOgfJson.__init__(self, data)
 
     def get(self):
         return json.dumps(self.toJson(), sort_keys=True, indent=4)
```

### Comparing `ipf-1.7a5/ipf/glue2/sge_tacc.py` & `ipf-1.7rc3/ipf/glue2/sge_tacc.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/service.py` & `ipf-1.7rc3/ipf/glue2/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #   limitations under the License.                                            #
 ###############################################################################
 
 import json
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .entity import *
 
 #######################################################################################################################
 
 class Service(Entity):
     def __init__(self):
@@ -33,15 +34,15 @@
         self.QualityLevel = None                        # string (QualityLevel)
         self.StatusInfo = []                            # list of string (uri)
         self.Complexity = None                          # string
         self.EndpointID = []                            # list of string (ID)
         self.ShareID = []                               # list of string (ID)
         self.ManagerID = []                             # list of string (ID)
         self.ContactID = []                             # list of string (ID)
-        self.LocationID = "urn:ogf:glue2:xsede.org:Location:unknown"  # string (ID)
+        self.LocationID = IPF_URN_PREFIX + "Location:unknown"  # string (ID)
         self.ServiceID = []                             # list of string (ID)
 
 #######################################################################################################################
 
 class ServiceTeraGridXml(EntityTeraGridXml):
     data_cls = Service
```

### Comparing `ipf-1.7a5/ipf/glue2/computing_service.py` & `ipf-1.7rc3/ipf/glue2/computing_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import time
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.error import NoMoreInputsError,StepError
 from ipf.sysinfo import ResourceName
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .computing_activity import ComputingActivity, ComputingActivities
 from .computing_share import ComputingShares
 from .location import Location
 from .service import *
 from .step import GlueStep
 
@@ -53,17 +54,17 @@
         self.location = self._getInput(Location).ID
         self.activities = self._getInput(ComputingActivities).activities
         self.shares = self._getInput(ComputingShares).shares
 
         service = self._run()
 
         service.id = self.resource_name
-        service.ID = "urn:ogf:glue2:xsede.org:ComputingService:%s" % (self.resource_name)
+        service.ID = IPF_URN_PREFIX+"ComputingService:%s" % (self.resource_name)
         service.LocationID = self.location
-        service.ManagerID = ["urn:ogf:glue2:xsede.org:ComputingManager:%s" % (self.resource_name)]
+        service.ManagerID = [IPF_URN_PREFIX+"ComputingManager:%s" % (self.resource_name)]
 
 
         service._addActivities(self.activities)
         service._addShares(self.shares)
 
         for share in self.shares:
             share.ServiceID = service.ID
```

### Comparing `ipf-1.7a5/ipf/glue2/benchmark.py` & `ipf-1.7rc3/ipf/glue2/benchmark.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/nimbus.py` & `ipf-1.7rc3/ipf/glue2/nimbus.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/unicore.py` & `ipf-1.7rc3/ipf/glue2/unicore.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/computing_share_accel_info.py` & `ipf-1.7rc3/ipf/glue2/computing_share_accel_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import json
 import time
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.sysinfo import ResourceName
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .computing_share import ComputingShares
 #from .computing_manager import ComputingManager
 from .accelerator_environment import AcceleratorEnvironments
 from .entity import *
 #from .manager import *
 from .step import GlueStep
@@ -50,24 +51,24 @@
         self.share_accel_info = None
 
     def run(self):
         self.resource_name = self._getInput(ResourceName).resource_name
         self.accel_envs = self._getInput(AcceleratorEnvironments).accel_envs
         #self.manager = self._getInput(ComputingManager).manager
         self.shares = self._getInput(ComputingShares).shares
-        self.ComputingManagerID = "urn:ogf:glue2:xsede.org:ComputingManager:%s" % (self.resource_name)
+        self.ComputingManagerID = IPF_URN_PREFIX+"ComputingManager:%s" % (self.resource_name)
         #self.UsedAcceleratorSlots = None         # integer
         accel_shares = []
 
         for computing_share in self.shares:
             share_accel_info = self._run()
             share_accel_info.id = "%s" % (self.resource_name)
-            share_accel_info.ID = "urn:ogf:glue2:xsede.org:ComputingShareAcceleratorInfo:%s.%s" % (computing_share.Name,self.resource_name)
+            share_accel_info.ID = IPF_URN_PREFIX+"ComputingShareAcceleratorInfo:%s.%s" % (computing_share.Name,self.resource_name)
             share_accel_info.Name = computing_share.Name
-            #share_accel_info.ID = "urn:ogf:glue2:xsede.org:ComputingShareAcceleratorInfo:%s" % (self.resource_name)
+            #share_accel_info.ID = IPF_URN_PREFIX+"ComputingShareAcceleratorInfo:%s" % (self.resource_name)
             share_accel_info.ComputingShareID.append(computing_share.ID)
             share_accel_info._addComputingShare(computing_share)
             computing_share.ComputingShareAccelInfoID=share_accel_info.ID
             if share_accel_info.UsedAcceleratorSlots is not None:
                 if share_accel_info.TotalAcceleratorSlots is not None:
                     if share_accel_info.FreeAcceleratorSlots == None:
                         share_accel_info.FreeAcceleratorSlots = 0
```

### Comparing `ipf-1.7a5/ipf/glue2/domain.py` & `ipf-1.7rc3/ipf/glue2/domain.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/slurm.py` & `ipf-1.7rc3/ipf/glue2/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import itertools
 import os
 import re
 
 import ipf.dt
 from ipf.error import StepError
 from ipf.log import LogFileWatcher
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from . import computing_activity
 from . import computing_manager
 from . import computing_manager_accel_info
 from . import computing_service
 from . import computing_share
 from . import computing_share_accel_info
@@ -170,19 +171,19 @@
         job.LocalOwner = m.group(1)
     m = re.search(Account,job_str)
     if m is not None:
         job.Extension["LocalAccount"] = m.group(1)
     m = re.search(Partition,job_str)
     if m is not None:
         job.Queue = m.group(1)
-        job.EnvironmentID = "urn:ogf:glue2:xsede.org:ExecutionEnvironment:%s.%s" % (m.group(1),step.resource_name)
+        job.EnvironmentID = IPF_URN_PREFIX+"ExecutionEnvironment:%s.%s" % (m.group(1),step.resource_name)
     m = re.search(Reservation,job_str)
     if m is not None and m.group(1) != "(null)":
         job.Extension["ReservationName"] = m.group(1)
-        job.EnvironmentID = "urn:ogf:glue2:xsede.org:ExecutionEnvironment:%s.%s" % (m.group(1),step.resource_name)
+        job.EnvironmentID = IPF_URN_PREFIX+"ExecutionEnvironment:%s.%s" % (m.group(1),step.resource_name)
     m = re.search(JobState,job_str)
     if m is not None:
         state = m.group(1)  # see squeue man page for state descriptions
         if state == "CANCELLED":
             job.State = [computing_activity.ComputingActivity.STATE_TERMINATED]
         elif state == "COMPLETED":
             job.State = [computing_activity.ComputingActivity.STATE_FINISHED]
@@ -487,26 +488,26 @@
         m = re.search(State,partition_str)
         if m is not None:
             if m.group(1) == "UP":
                 share.ServingState = "production"
             else:
                 share.ServingState = "closed"
 
-        share.EnvironmentID = ["urn:ogf:glue2:xsede.org:ExecutionEnvironment:%s.%s" % (share.Name,self.resource_name)]
+        share.EnvironmentID = [IPF_URN_PREFIX+"ExecutionEnvironment:%s.%s" % (share.Name,self.resource_name)]
         return share
 
     def _getReservation(self, rsrv_str):
         share = computing_share.ComputingShare()
         share.Extension["Reservation"] = True
 
         m = re.search(ReservationName,rsrv_str)
         if m is None:
             raise StepError("didn't find 'ReservationName'")
         share.Name = m.group(1)
-        share.EnvironmentID = ["urn:ogf:glue2:xsede.org:ExecutionEnvironment:%s.%s" % (share.Name,self.resource_name)]
+        share.EnvironmentID = [IPF_URN_PREFIX+"ExecutionEnvironment:%s.%s" % (share.Name,self.resource_name)]
         m = re.search(PartitionName,rsrv_str)
         if m is not None:                                                                                              
             share.MappingQueue = m.group(1)
         m = re.search(NodCnt,rsrv_str)
         if m is not None:
             share.MaxSlotsPerJob = int(m.group(1))
 
@@ -723,15 +724,15 @@
         rsrv.Extension["Reservation"] = True
 
         # ID set by ExecutionEnvironment
         m = re.search(ReservationName,rsrv_str)
         if m is None:
             raise StepError("didn't find 'ReservationName'")
         rsrv.Name = m.group(1)
-        rsrv.ShareID = ["urn:ogf:glue2:xsede.org:ComputingShare:%s.%s" % (rsrv.Name,self.resource_name)]
+        rsrv.ShareID = [IPF_URN_PREFIX+"ComputingShare:%s.%s" % (rsrv.Name,self.resource_name)]
 
         m = re.search(StartTime,rsrv_str)
         if m is not None:
             rsrv.Extension["StartTime"] = _getDateTime(m.group(1))
         m = re.search(EndTime,rsrv_str)
         if m is not None:
             rsrv.Extension["EndTime"] = _getDateTime(m.group(1))
@@ -1058,15 +1059,15 @@
         Nodes = self.params.get("Nodes","Nodes=(\S+)")
         State = self.params.get("State","State=(\S+)")
         # ID set by ExecutionEnvironment
         m = re.search(ReservationName,rsrv_str)
         if m is None:
             raise StepError("didn't find 'ReservationName'")
         rsrv.Name = m.group(1)
-        rsrv.ShareID = ["urn:ogf:glue2:xsede.org:ComputingShare:%s.%s" % (rsrv.Name,self.resource_name)]
+        rsrv.ShareID = [IPF_URN_PREFIX+"ComputingShare:%s.%s" % (rsrv.Name,self.resource_name)]
 
         m = re.search(StartTime,rsrv_str)
         if m is not None:
             rsrv.Extension["StartTime"] = _getDateTime(m.group(1))
         m = re.search(EndTime,rsrv_str)
         if m is not None:
             rsrv.Extension["EndTime"] = _getDateTime(m.group(1))
```

### Comparing `ipf-1.7a5/ipf/glue2/loadleveler.py` & `ipf-1.7rc3/ipf/glue2/loadleveler.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/moab.py` & `ipf-1.7rc3/ipf/glue2/moab.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/valet.py` & `ipf-1.7rc3/ipf/glue2/valet.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import subprocess
 import os
 import sys
 import re
 import hashlib
 
 from ipf.error import StepError
+from ipf.urnprefix import IPF_URN_PREFIX
 from . import application
 from .types import AppEnvState, ApplicationHandle
 
 #######################################################################################################################
 
 valetPrefix = os.getenv('VALET_PREFIX')
 if valetPrefix:
@@ -95,15 +96,15 @@
                                 pathhashobject = hashlib.md5(path.encode('utf-8'))
                                 env.path_hash = pathhashobject.hexdigest()
 
                                 handle = application.ApplicationHandle()
                                 handle.Type = ApplicationHandle.VALET
                                 handle.Value = str(versId)
 
-                                # env.ExecutionEnvironmentID = 'urn:ogf:glue2:xsede.org:ExecutionEnvironment:{:s}'.format(self.resource_name)
+                                # env.ExecutionEnvironmentID = IPF_URN_PREFIX+'ExecutionEnvironment:{:s}'.format(self.resource_name)
                                 apps.add(env, [handle])
 
         except Exception as e:
             self.warning(str(e))
             return None
 
         return apps
```

### Comparing `ipf-1.7a5/ipf/glue2/execution_environment.py` & `ipf-1.7rc3/ipf/glue2/execution_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.error import StepError
 from ipf.sysinfo import ResourceName
 from ipf.sysinfo import Platform
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .resource import *
 from .step import GlueStep
 
 #######################################################################################################################
 
 
@@ -57,23 +58,23 @@
 
     def run(self):
         self.resource_name = self._getInput(ResourceName).resource_name
 
         host_groups = self._run()
         for host_group in host_groups:
             host_group.id = "%s.%s" % (host_group.Name, self.resource_name)
-            host_group.ID = "urn:ogf:glue2:xsede.org:ExecutionEnvironment:%s.%s" % (
+            host_group.ID = IPF_URN_PREFIX+"ExecutionEnvironment:%s.%s" % (
                 host_group.Name, self.resource_name)
-            host_group.ManagerID = "urn:ogf:glue2:xsede.org:ComputingManager:%s" % (
+            host_group.ManagerID = IPF_URN_PREFIX+"ComputingManager:%s" % (
                 self.resource_name)
         #accel_groups = copy.deepcopy(host_groups)
         # for accel_group in accel_groups:
         #    accel_group.id = "%s.%s" % (host_group.Name,self.resource_name)
-        #    accel_group.ID = "urn:ogf:glue2:xsede.org:AcceleratorEnvironment:%s.%s" % (accel_group.Name,self.resource_name)
-        #    accel_group.ManagerID = "urn:ogf:glue2:xsede.org:ComputingManager:%s" % (self.resource_name)
+        #    accel_group.ID = IPF_URN_PREFIX+"AcceleratorEnvironment:%s.%s" % (accel_group.Name,self.resource_name)
+        #    accel_group.ManagerID = IPF_URN_PREFIX+"ComputingManager:%s" % (self.resource_name)
 
         self._output(ExecutionEnvironments(self.resource_name, host_groups))
         # self._output(AcceleratorEnvironments(self.resource_name,accel_groups))
 
     def _shouldUseName(self, hosts):
         names = set()
         for host in hosts:
@@ -138,15 +139,15 @@
         if host.PhysicalCPUs == None:
             return False
 
         # if the host is associated with a queue, check that it is a good one
         if len(host.ShareID) == 0:
             return True
         for share in host.ShareID:
-            m = re.search("urn:ogf:glue2:xsede.org:ComputingShare:(\S+).%s" %
+            m = re.search(IPF_URN_PREFIX+"ComputingShare:(\S+).%s" %
                           self.resource_name, share)
             if self._includeQueue(m.group(1)):
                 return True
 
         # if the host is associated with a partition, check that it is a good one
         if len(host.Partitions) == 0:
             return True
```

### Comparing `ipf-1.7a5/ipf/glue2/computing_activity.py` & `ipf-1.7rc3/ipf/glue2/computing_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.error import StepError
 from ipf.paths import IPF_VAR_PATH
 from ipf.sysinfo import ResourceName
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .activity import *
 from .step import GlueStep
 
 #######################################################################################################################
 
 class ComputingActivitiesStep(GlueStep):
@@ -53,17 +54,17 @@
 
         activities = self._run()
         for activity in activities:
             if activity.LocalOwner is None:
                 activity.id = "%s.unknown.%s" % (activity.LocalIDFromManager,self.resource_name)
             else:
                 activity.id = "%s.%s.%s" % (activity.LocalIDFromManager,activity.LocalOwner,self.resource_name)
-            activity.ID = "urn:ogf:glue2:xsede.org:ComputingActivity:%s.%s" % (activity.LocalIDFromManager,self.resource_name)
+            activity.ID = IPF_URN_PREFIX+"ComputingActivity:%s.%s" % (activity.LocalIDFromManager,self.resource_name)
             if activity.Queue is not None:
-                activity.ShareID = "urn:ogf:glue2:xsede.org:ComputingShare:%s.%s" % (activity.Queue,self.resource_name)
+                activity.ShareID = IPF_URN_PREFIX+"ComputingShare:%s.%s" % (activity.Queue,self.resource_name)
             activity.hide = self.params.get("hide_job_attribs",[])
 
         self._output(ComputingActivities(self.resource_name,activities))
 
     def _run(self):
         raise StepError("ComputingActivitiesStep._run not overriden")
 
@@ -127,17 +128,17 @@
         self._run()
 
     def output(self, activity):
         if activity.LocalOwner is None:
             activity.id = "%s.unknown.%s" % (activity.LocalIDFromManager,self.resource_name)
         else:
             activity.id = "%s.%s.%s" % (activity.LocalIDFromManager,activity.LocalOwner,self.resource_name)
-        activity.ID = "urn:ogf:glue2:xsede.org:ComputingActivity:%s.%s" % (activity.LocalIDFromManager,self.resource_name)
+        activity.ID = IPF_URN_PREFIX+"ComputingActivity:%s.%s" % (activity.LocalIDFromManager,self.resource_name)
         if activity.Queue is not None:
-            activity.ShareID = "urn:ogf:glue2:xsede.org:ComputingShare:%s.%s" % (activity.Queue,self.resource_name)
+            activity.ShareID = IPF_URN_PREFIX+"ComputingShare:%s.%s" % (activity.Queue,self.resource_name)
         activity.hide = self.params.get("hide_job_attribs",[])
         
         self._output(activity)
 
     def _run(self):
         raise StepError("ComputingActivityUpdateStep._run not overriden")
```

### Comparing `ipf-1.7a5/ipf/glue2/activity.py` & `ipf-1.7rc3/ipf/glue2/activity.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/openstack.py` & `ipf-1.7rc3/ipf/glue2/openstack.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/resource.py` & `ipf-1.7rc3/ipf/glue2/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 
 import json
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 
 from .entity import *
+from ipf.urnprefix import IPF_URN_PREFIX
 
 #######################################################################################################################
 
 class Resource(Entity):
     def __init__(self):
         Entity.__init__(self)
 
-        self.ManagerID = "urn:ogf:glue2:xsede.org:ComputingManager:unknown"  # string (uri)
+        self.ManagerID = IPF_URN_PREFIX+"ComputingManager:unknown"  # string (uri)
         self.ShareID = []                             # list of string (uri)
         self.ActivityID = []                          # list of string (uri)
 
 #######################################################################################################################
 
 class ResourceTeraGridXml(EntityTeraGridXml):
     data_cls = Resource
```

### Comparing `ipf-1.7a5/ipf/glue2/sge.py` & `ipf-1.7rc3/ipf/glue2/sge.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import time
 import xml.sax
 import xml.sax.handler
 
 from ipf.dt import *
 from ipf.error import StepError
 from ipf.log import LogFileWatcher
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from . import computing_activity
 from . import computing_manager
 from . import computing_service
 from . import computing_share
 from . import execution_environment
 from . import accelerator_environment
@@ -593,15 +594,15 @@
         if name == "host":
             self.cur_host = execution_environment.ExecutionEnvironment()
             self.cur_host.Name = attrs.getValue("name")
             self.cur_host.TotalInstances = 1
         elif name == "queue":
             queue = attrs.getValue("name")
             self.cur_host.ShareID.append(
-                "urn:ogf:glue2:xsede.org:ComputingShare:%s.%s" % (queue, self.step.resource_name))
+                IPF_URN_PREFIX+"ComputingShare:%s.%s" % (queue, self.step.resource_name))
         elif name == "hostvalue":
             self.hostvalue_name = attrs.getValue("name")
 
     def endElement(self, name):
         if name == "host":
             if self.cur_host.PhysicalCPUs is not None:
                 self.hosts.append(self.cur_host)
```

### Comparing `ipf-1.7a5/ipf/glue2/genesisII.py` & `ipf-1.7rc3/ipf/glue2/genesisII.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/types.py` & `ipf-1.7rc3/ipf/glue2/types.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/condor.py` & `ipf-1.7rc3/ipf/glue2/condor.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/gram.py` & `ipf-1.7rc3/ipf/glue2/gram.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/application.py` & `ipf-1.7rc3/ipf/glue2/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.error import StepError
 from ipf.step import Step
 from ipf.sysinfo import ResourceName
 from ipf.ipfinfo import IPFInformation, IPFInformationJson, IPFInformationTxt
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .entity import *
 
 #######################################################################################################################
 
 
 class ApplicationEnvironment(Entity):
@@ -134,15 +135,15 @@
         Entity.__init__(self)
 
         # string (ApplicationHandle_t)
         self.Type = "unknown"
         # string
         self.Value = "unknown"
         # string (ID)
-        self.ApplicationEnvironmentID = "urn:ogf:glue2:xsede.org:ApplicationEnvironment:unknown"
+        self.ApplicationEnvironmentID = IPF_URN_PREFIX+"ApplicationEnvironment:unknown"
 
 #######################################################################################################################
 
 
 class ApplicationHandleOgfJson(EntityOgfJson):
     data_cls = ApplicationHandle
 
@@ -179,26 +180,26 @@
     def add(self, env, handles):
         if env.AppVersion is None:
             app_version = "unknown"
         else:
             app_version = env.AppVersion
         env.Name = "%s-%s" % (env.AppName, app_version)
         env.id = "%s.%s.%s" % (app_version, env.AppName, self.resource_name)
-        env.ID = "urn:ogf:glue2:xsede.org:ApplicationEnvironment:%s.%s.%s.%s" % (
+        env.ID = IPF_URN_PREFIX+"ApplicationEnvironment:%s.%s.%s.%s" % (
             app_version, env.AppName, self.resource_name, env.path_hash)
-        env.ComputingManagerID = "urn:ogf:glue2:xsede.org:ComputingManager:%s" % (
+        env.ComputingManagerID = IPF_URN_PREFIX+"ComputingManager:%s" % (
             self.resource_name)
 
         env.ApplicationHandleID = []
         for handle in handles:
             handle.ApplicationEnvironmentID = env.ID
             handle.Name = "%s-%s" % (env.AppName, app_version)
             handle.id = "%s.%s.%s.%s" % (
                 handle.Type, app_version, env.AppName, self.resource_name)
-            handle.ID = "urn:ogf:glue2:xsede.org:ApplicationHandle:%s:%s.%s.%s.%s" % \
+            handle.ID = IPF_URN_PREFIX+"ApplicationHandle:%s:%s.%s.%s.%s" % \
                         (handle.Type, app_version, env.AppName,
                          self.resource_name, env.path_hash)
             env.ApplicationHandleID.append(handle.ID)
 
         self.environments.append(env)
         self.handles.extend(handles)
```

### Comparing `ipf-1.7a5/ipf/glue2/storageservice.py` & `ipf-1.7rc3/ipf/glue2/storageservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import os
 import re
 import pprint
 
 from ipf.dt import localtzoffset
 from ipf.error import StepError
 from ipf.log import LogDirectoryWatcher
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from . import computing_manager
 from . import service
 #from . import computing_share
 from . import execution_environment
 from ipf.step import Step
 import json
@@ -182,15 +183,15 @@
                     ServiceType = "ComputingService"
                 else:
                     if st[0] == "information":
                         ServiceType = "InformationService"
                     else:
                         ServiceType = "LoginService"
         serv.resource_name = self.resource_name 
-        serv.ID = "urn:ogf:ogf:glue2:xsede.org:%s:%s-%s" % (ServiceType,serv.Name,self.resource_name)
+        serv.ID = IPF_URN_PREFIX+"%s:%s-%s" % (ServiceType,serv.Name,self.resource_name)
         serv.ServiceType = ServiceType
         servlist.add(serv)
         
 #######################################################################################################################
 
 class StorageServiceOgfJson(EntityOgfJson):
     data_cls = Service
@@ -255,15 +256,15 @@
         for serv in self.data.services:
             if serv is not None:
                 endpoint = Endpoint()
                 endpoint.URL = serv.Endpoint
                 endpoint.InterfaceName = serv.Type
                 endpoint.InterfaceVersion = serv.Version
                 endpoint.Name = serv.Name
-                endpoint.ID = "urn:ogf:glue2:xsede.org:Endpoint:%s-%s-%s" % (serv.Version, serv.Name, serv.resource_name)
+                endpoint.ID = IPF_URN_PREFIX+"Endpoint:%s-%s-%s" % (serv.Version, serv.Name, serv.resource_name)
                 endpoint.ServiceID = serv.ID
                 endpoint.QualityLevel = serv.QualityLevel
                 serv.EndpointID = endpoint.ID
                 #if self.data.id is None:
                 #self.data.id = serv.resource_name
                 doc[serv.ServiceType].append(StorageServiceOgfJson(serv).toJson())
                 doc["Endpoint"].append(EndpointOgfJson(endpoint).toJson())
```

### Comparing `ipf-1.7a5/ipf/glue2/step.py` & `ipf-1.7rc3/ipf/glue2/step.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/location.py` & `ipf-1.7rc3/ipf/glue2/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import os
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.sysinfo import SiteName
 from ipf.step import Step
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .entity import *
 
 #######################################################################################################################
 
 class LocationStep(Step):
     def __init__(self):
@@ -69,15 +70,15 @@
         # Entity
         if "CreationTime" in doc:
             self.CreationTime = textToDateTime(doc["CreationTime"])
         else:
             self.CreationTime = datetime.datetime.now(tzoffset(0))
         self.Validity = doc.get("Validity",Location.DEFAULT_VALIDITY)
         self.Name = doc.get("Name","unknown")
-        self.ID = "urn:ogf:glue2:xsede.org:Location:%s" % self.Name.replace(" ","")
+        self.ID = IPF_URN_PREFIX+"Location:%s" % self.Name.replace(" ","")
         self.id = self.ID
         self.OtherInfo = doc.get("OtherInfo",[])
         self.Extension = doc.get("Extension",{})
 
         self.Address = doc.get("Address")
         self.Place = doc.get("Place")
         self.Country = doc.get("Country")
```

### Comparing `ipf-1.7a5/ipf/glue2/endpoint.py` & `ipf-1.7rc3/ipf/glue2/endpoint.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/catalina.py` & `ipf-1.7rc3/ipf/glue2/catalina.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/computing_share.py` & `ipf-1.7rc3/ipf/glue2/computing_share.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import time
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.error import StepError
 from ipf.sysinfo import ResourceName
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .computing_activity import ComputingActivity, ComputingActivities
 from .accelerator_environment import AcceleratorEnvironments
 #from .computing_share_accel_info import ComputingShareAcceleratorInfo
 from .step import GlueStep
 from .share import *
 
@@ -54,21 +55,21 @@
         self.resource_name = self._getInput(ResourceName).resource_name
         self.activities = self._getInput(ComputingActivities).activities
 
         shares = self._run()
 
         for share in shares:
             share.id = "%s.%s" % (share.Name,self.resource_name)
-            share.ID = "urn:ogf:glue2:xsede.org:ComputingShare:%s.%s" % (share.Name,self.resource_name)
-            share.ServiceID = "urn:ogf:glue2:xsede.org:ComputingService:%s" % (self.resource_name)
+            share.ID = IPF_URN_PREFIX+"ComputingShare:%s.%s" % (share.Name,self.resource_name)
+            share.ServiceID = IPF_URN_PREFIX+"ComputingService:%s" % (self.resource_name)
 
         self._addActivities(shares)
         for share in shares:
             if share.UsedAcceleratorSlots > 0:
-                share.ComputingShareAccelInfoID = "urn:ogf:glue2:xsede.org:ComputingShareAcceleratorInfo:%s.%s" % (share.Name,self.resource_name)
+                share.ComputingShareAccelInfoID = IPF_URN_PREFIX+"ComputingShareAcceleratorInfo:%s.%s" % (share.Name,self.resource_name)
 
         self._output(ComputingShares(self.resource_name,shares))
 
     def _run(self):
         raise StepError("ComputingSharesStep._run not overriden")
 
     def _addActivities(self, shares):
```

### Comparing `ipf-1.7a5/ipf/glue2/share.py` & `ipf-1.7rc3/ipf/glue2/share.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 #   limitations under the License.                                            #
 ###############################################################################
 
 import json
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .entity import *
 
 #######################################################################################################################
 
 class Share(Entity):
     def __init__(self):
         Entity.__init__(self)
 
         self.Description = None                       # string
         self.EndpointID = []                          # list of string (uri)
         self.ResourceID = []                          # list of string (uri)
         self.EnvironmentID = []                          # list of string (uri)
-        self.ServiceID = "urn:ogf:glue2:xsede.org:Service:unknown"  # string (uri)
+        self.ServiceID = IPF_URN_PREFIX+"Service:unknown"  # string (uri)
         self.ActivityID = []                          # list of string (uri)
         self.MappingPolicyID = []                     # list of string (uri)
 
 #######################################################################################################################
 
 class ShareTeraGridXml(EntityTeraGridXml):
     data_cls = Share
```

### Comparing `ipf-1.7a5/ipf/glue2/computing_manager_accel_info.py` & `ipf-1.7rc3/ipf/glue2/computing_manager_accel_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import json
 import time
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.sysinfo import ResourceName
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .computing_share import ComputingShares
 #from .computing_manager import ComputingManager
 from .accelerator_environment import AcceleratorEnvironments
 from .entity import *
 #from .manager import *
 from .step import GlueStep
@@ -54,19 +55,19 @@
     def run(self):
         self.resource_name = self._getInput(ResourceName).resource_name
         self.accel_envs = self._getInput(AcceleratorEnvironments).accel_envs
         #self.manager = self._getInput(ComputingManager).manager
         #self.shares = self._getInput(ComputingShares).shares
 
         manager_accel_info = self._run()
-        manager_accel_info.ComputingManagerID = "urn:ogf:glue2:xsede.org:ComputingManager:%s" % (
+        manager_accel_info.ComputingManagerID = IPF_URN_PREFIX+"ComputingManager:%s" % (
             self.resource_name)
 
         manager_accel_info.id = "%s" % (self.resource_name)
-        manager_accel_info.ID = "urn:ogf:glue2:xsede.org:ComputingManagerAcceleratorInfo:%s" % (
+        manager_accel_info.ID = IPF_URN_PREFIX+"ComputingManagerAcceleratorInfo:%s" % (
             self.resource_name)
 
         if self.accel_envs:
             for accel_env in self.accel_envs:
                 manager_accel_info._addAcceleratorEnvironment(accel_env)
         # for share in self.shares:
         #    manager_accel_info._addComputingShare(share)
```

### Comparing `ipf-1.7a5/ipf/glue2/computing_endpoint.py` & `ipf-1.7rc3/ipf/glue2/computing_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.error import StepError
 from ipf.sysinfo import ResourceName
 
 from ipf.glue2.endpoint import *
 from ipf.glue2.step import GlueStep
+from ipf.urnprefix import IPF_URN_PREFIX
 
 #######################################################################################################################
 
 class ComputingEndpointStep(GlueStep):
     def __init__(self):
         GlueStep.__init__(self)
 
@@ -48,16 +49,16 @@
         endpoints = self._run()
 
         for i in range(0,len(endpoints)):
             if endpoints[i].Name == None:
                 endpoints[i].Name = "endpoint-%d" % (i+1)
         for endpoint in endpoints:
             endpoint.id = "%s.%s" % (endpoint.Name,self.resource_name)
-            endpoint.ID = "urn:ogf:glue2:xsede.org:ComputingEndpoint:%s.%s" % (endpoint.Name,self.resource_name)
-            endpoint.ServiceID = "urn:ogf:glue2:xsede.org:ComputingService:%s" % (self.resource_name)
+            endpoint.ID = IPF_URN_PREFIX+"ComputingEndpoint:%s.%s" % (endpoint.Name,self.resource_name)
+            endpoint.ServiceID = IPF_URN_PREFIX+"ComputingService:%s" % (self.resource_name)
 
             self._output(endpoint)
 
     def _run(self):
         raise StepError("ComputingEndpointStep._run not overriden")
 
 #######################################################################################################################
```

### Comparing `ipf-1.7a5/ipf/glue2/entity.py` & `ipf-1.7rc3/ipf/glue2/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 
 import datetime
 import json
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
+from ipf.urnprefix import IPF_URN_PREFIX
 
 #######################################################################################################################
 
 class Entity(Data):
     def __init__(self):
         Data.__init__(self)
 
         self.CreationTime = datetime.datetime.now(tzoffset(0))
         self.Validity = None
-        self.ID = "urn:ogf:glue2:xsede.org:Unknown:unknown"   # string (uri)
+        self.ID = IPF_URN_PREFIX+"Unknown:unknown"   # string (uri)
         self.Name = None                        # string
         self.OtherInfo = []                     # list of string
         self.Extension = {}                     # (key,value) strings
 
 #######################################################################################################################
 
 class EntityTeraGridXml(Representation):
```

### Comparing `ipf-1.7a5/ipf/glue2/modules.py` & `ipf-1.7rc3/ipf/glue2/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import subprocess
 import os
 import re
 import hashlib
 
 from ipf.error import StepError
+from ipf.urnprefix import IPF_URN_PREFIX
 from . import application
 from . import service
 from .types import AppEnvState, ApplicationHandle
 
 #######################################################################################################################
 
 
@@ -393,15 +394,15 @@
             if "NOPUBLISH" in flagslist:
                 publishflag = False
                 self.debug("NOPUBLISH set for "+path)
 
         handle = application.ApplicationHandle()
         handle.Type = ApplicationHandle.MODULE
         handle.Value = env.AppName+"/"+env.AppVersion
-        env.ExecutionEnvironmentID = "urn:ogf:glue2:xsede.org:ExecutionEnvironment:%s" % (
+        env.ExecutionEnvironmentID = IPF_URN_PREFIX+"ExecutionEnvironment:%s" % (
             self.resource_name)
 
         if publishflag == True:
             apps.add(env, [handle])
 
     def _InferDescription(self, text, env):
         handle = application.ApplicationHandle()
```

### Comparing `ipf-1.7a5/ipf/glue2/accelerator_environment.py` & `ipf-1.7rc3/ipf/glue2/accelerator_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.error import StepError
 from ipf.sysinfo import ResourceName
 from ipf.sysinfo import Platform
+from ipf.urnprefix import IPF_URN_PREFIX
 
 
 from .resource import *
 from .step import GlueStep
 
 #######################################################################################################################
 
@@ -56,17 +57,17 @@
     def run(self):
         self.resource_name = self._getInput(ResourceName).resource_name
 
         host_groups = self._run()
         if host_groups:
             for host_group in host_groups:
                 host_group.id = "%s.%s" % (host_group.Name, self.resource_name)
-                host_group.ID = "urn:ogf:glue2:xsede.org:AcceleratorEnvironment:%s.%s" % (
+                host_group.ID = IPF_URN_PREFIX+"AcceleratorEnvironment:%s.%s" % (
                     host_group.Name, self.resource_name)
-                host_group.ManagerID = "urn:ogf:glue2:xsede.org:ComputingManager:%s" % (
+                host_group.ManagerID = IPF_URN_PREFIX+"ComputingManager:%s" % (
                     self.resource_name)
                 self.debug("host_group.id "+host_group.id)
                 self.debug("host_group.uas " +
                            str(host_group.UsedAcceleratorSlots))
 
         self._output(AcceleratorEnvironments(self.resource_name, host_groups))
 
@@ -142,15 +143,15 @@
         if host.PhysicalAccelerators == None:
             return False
 
         # if the host is associated with a queue, check that it is a good one
         if len(host.ShareID) == 0:
             return True
         for share in host.ShareID:
-            m = re.search("urn:ogf:glue2:xsede.org:ComputingShare:(\S+).%s" %
+            m = re.search(IPF_URN_PREFIX+"ComputingShare:(\S+).%s" %
                           self.resource_name, share)
             if self._includeQueue(m.group(1)):
                 return True
         # if the host is associated with a partition, check that it is a good one
         if len(host.Partitions) == 0:
             return True
         partition_list = host.Partitions.split(',')
```

### Comparing `ipf-1.7a5/ipf/glue2/lsf.py` & `ipf-1.7rc3/ipf/glue2/lsf.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/pbs_psc.py` & `ipf-1.7rc3/ipf/glue2/pbs_psc.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/manager.py` & `ipf-1.7rc3/ipf/glue2/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 #   limitations under the License.                                            #
 ###############################################################################
 
 import json
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .entity import *
 
 #######################################################################################################################
 
 class Manager(Entity):
     def __init__(self):
         Entity.__init__(self)
 
         self.ProductName = "unknown"                  # string
         self.ProductVersion = None                    # string
-        self.ServiceID = "urn:ogf:glue2:xsede.org:Service:unknown"  # string (ID)
+        self.ServiceID = IPF_URN_PREFIX+"Service:unknown"  # string (ID)
         self.ResourceID = []                          # list of string (ID)
 
 #######################################################################################################################
 
 class ManagerTeraGridXml(EntityTeraGridXml):
     data_cls = Manager
```

### Comparing `ipf-1.7a5/ipf/glue2/computing_manager.py` & `ipf-1.7rc3/ipf/glue2/computing_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import json
 import time
 from xml.dom.minidom import getDOMImplementation
 
 from ipf.data import Data, Representation
 from ipf.dt import *
 from ipf.sysinfo import ResourceName
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from .computing_share import ComputingShares
 from .execution_environment import ExecutionEnvironments
 from .accelerator_environment import AcceleratorEnvironments
 from .computing_manager_accel_info import ComputingManagerAcceleratorInfo
 from .manager import *
 from .step import GlueStep
@@ -55,16 +56,16 @@
         self.shares = self._getInput(ComputingShares).shares
         self.accel_envs = self._getInput(AcceleratorEnvironments).accel_envs
         self.CMAccelInfo = self._getInput(ComputingManagerAcceleratorInfo)
 
         manager = self._run()
 
         manager.id = "%s" % (self.resource_name)
-        manager.ID = "urn:ogf:glue2:xsede.org:ComputingManager:%s" % (self.resource_name)
-        manager.ServiceID = "urn:ogf:glue2:xsede.org:ComputingService:%s" % (self.resource_name)
+        manager.ID = IPF_URN_PREFIX+"ComputingManager:%s" % (self.resource_name)
+        manager.ServiceID = IPF_URN_PREFIX+"ComputingService:%s" % (self.resource_name)
         if self.CMAccelInfo.TotalPhysicalAccelerators is not None:
             manager.ComputingManagerAcceleratorInfoID=self.CMAccelInfo.ID
 
         for exec_env in self.exec_envs:
             manager._addExecutionEnvironment(exec_env)
         if self.accel_envs:
             for accel_env in self.accel_envs:
```

### Comparing `ipf-1.7a5/ipf/glue2/abstractservice.py` & `ipf-1.7rc3/ipf/glue2/abstractservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import re
 import pprint
 import hashlib
 
 from ipf.dt import localtzoffset
 from ipf.error import StepError
 from ipf.log import LogDirectoryWatcher
+from ipf.urnprefix import IPF_URN_PREFIX
 
 from . import computing_manager
 from . import service
 #from . import computing_share
 from . import execution_environment
 from ipf.step import Step
 import json
@@ -192,15 +193,15 @@
                         else:
                             ServiceType = "UntypedService"
         serv.resource_name = self.resource_name
         endpointhash = ''
         if (serv.Endpoint != ''):
             endpointhashobject = hashlib.md5(str(serv.Endpoint).encode('utf-8'))
             endpointhash = "-"+endpointhashobject.hexdigest()
-        serv.ID = "urn:ogf:ogf:glue2:xsede.org:%s:%s-%s%s" % (ServiceType,
+        serv.ID = IPF_URN_PREFIX+"%s:%s-%s%s" % (ServiceType,
                                             serv.Name, self.resource_name, endpointhash)
         serv.ServiceType = ServiceType
         servlist.add(serv)
 
 #######################################################################################################################
 
 
@@ -270,15 +271,15 @@
                 endpoint.InterfaceName = serv.Type
                 endpoint.InterfaceVersion = serv.Version
                 endpoint.Name = serv.Name
                 endpointhash = ''
                 if (serv.Endpoint != ''):
                     endpointhashobject = hashlib.md5(str(serv.Endpoint).encode('utf-8'))
                     endpointhash = "-"+endpointhashobject.hexdigest()
-                endpoint.ID = "urn:ogf:glue2:xsede.org:Endpoint:%s-%s-%s%s" % (
+                endpoint.ID = IPF_URN_PREFIX+"Endpoint:%s-%s-%s%s" % (
                     serv.Version, serv.Name, serv.resource_name, endpointhash)
                 endpoint.ServiceID = serv.ID
                 endpoint.QualityLevel = serv.QualityLevel
                 serv.EndpointID = endpoint.ID
                 if serv.ServiceType not in doc:
                     doc[serv.ServiceType] = []
                 doc[serv.ServiceType].append(
```

### Comparing `ipf-1.7a5/ipf/glue2/cobalt.py` & `ipf-1.7rc3/ipf/glue2/cobalt.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/contact.py` & `ipf-1.7rc3/ipf/glue2/contact.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/pbs.py` & `ipf-1.7rc3/ipf/glue2/pbs.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/glue2/compute.py` & `ipf-1.7rc3/ipf/glue2/compute.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/run_workflow.py` & `ipf-1.7rc3/ipf/run_workflow.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/daemon.py` & `ipf-1.7rc3/ipf/daemon.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf/publish.py` & `ipf-1.7rc3/ipf/publish.py`

 * *Files identical despite different names*

### Comparing `ipf-1.7a5/ipf.egg-info/PKG-INFO` & `ipf-1.7rc3/ipf.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ipf
-Version: 1.7a5
+Version: 1.7rc3
 Summary: The Information Publishing Framework
-Home-page: https://github.com/xsede/ipf
+Home-page: https://github.com/access-ci-org/ipf
 Author: Eric Blau, Warren Smith
 Author-email: blau@anl.gov
 License: Apache
-Description: 
-        # ipf-xsede %VER%-%REL%
-        # README
-        ## Overview
-        
-        The Information Publishing Framework (IPF) is a generic framework for gathering and publishing information. IPF
-        focuses narrowly on gatethering and publishing, and not on analyzing or visualizing information. IPF grew out of
-        work to publish information about TeraGrid compute resources using the
-        [GLUE 2 specification](http://www.ogf.org/documents/GFD.147.pdf). IPF continues to support data gathering and
-        publishing in the XSEDE program which succeeded TeraGrid.
-        
-        IPF gathers and publishes information using simple workflows. These workflows are defined using JSON (see the
-        etc/workflows directory) and steps in the workflows are implemented as Python classes. Each step in the
-        workflow can require input Data, can produce output Data, and can publish Representations of Data. A typical
-        workflow consists of a number of information gathering steps and a few steps that publish Representations to
-        files or to remote services (e.g. REST, messaging).
-        
-        Workflow steps specify what Data they require and what Data they produce. This allows IPF to construct
-        workflows based on partial information - in the case where there are not steps that produce the same Data, an
-        entire workflow can be constructed from a single publish step and its required input Data. At the other
-        extreme, workflows can be exactly specified with specific steps identified and the outputs of steps bound to
-        the inputs of other steps. A typical workflow (e.g. GLUE 2) specifies what steps to include but lets IPF
-        automatically link outputs to inputs of these steps.
-        
-        Workflows can run to completion relatively quickly or they can continuously run. The first type of workflow
-        can be used to run a few commands or look at status files and publish that information. The second type of
-        workflow can be used to monitor log files and publish entries written to those files. Workflows are typically
-        run periodically as cron jobs. The program libexec/run_workflow.py is for executing workflows that complete
-        quickly and the program libexec/run_workflow_daemon.py is used to manage long-running workflows. The daemon
-        
-        ## License
-        
-        This software is licensed under Version 2.0 of the Apache License.
-        
-        ## Installation
-        
-        Installation instructions are in [docs/INSTALL.md](docs/INSTALL.md).
-        
-        ## Contact Information
-        
-        This software is maintained by [XSEDE](https://www.github.com/XSEDE).  and you can contact the XSEDE helpdesk
-        if you need help using it.
-        
-        If you have problems with this software you are welcome to submit an [issue](https://github.com/XSEDE/ipf/issues).
-        
-        ## Acknowledgements
-        
-        This work was supported by the TeraGrid, XSEDE, FutureGrid, and XSEDE 2 projects under National Science Foundation
-        grants 0503697, 1053575, 0910812, and 1548562.
-        
 Keywords: monitoring information gathering publishing glue2
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Topic :: System :: Monitoring
+License-File: LICENSE
+
+
+# access-ci-org/ipf %VER%-%REL%
+# README
+
+## Overview
+
+The Information Publishing Framework (IPF) is a generic framework used by resource operators to gather and publish
+dynamic resource information in [GLUE 2 serialized format](http://www.ogf.org/documents/GFD.147.pdf). IPF was used
+by the TeraGrid, XSEDE, and XSEDE 2 programs, and is currently being used by the ACCESS-CI program to publish
+high-performance compute cluster information.
+
+IPF gathers and publishes information using simple workflows. These workflows are defined using JSON (see the
+etc/workflows directory) and steps in the workflows are implemented as Python classes. Each step in the
+workflow can require input Data, can produce output Data, and can publish Representations of Data. A typical
+workflow consists of a number of information gathering steps and a few steps that publish representations to
+files or to remote services (e.g. REST, messaging).
+
+Workflow steps specify what Data they require and what Data they produce. This allows IPF to construct
+workflows based on partial information - in the case where there are not steps that produce the same Data, an
+entire workflow can be constructed from a single publish step and its required input Data. At the other
+extreme, workflows can be exactly specified with specific steps identified and the outputs of steps bound to
+the inputs of other steps. A typical workflow (e.g. GLUE 2) specifies what steps to include but lets IPF
+automatically link outputs to inputs of these steps.
+
+Workflows can run to completion relatively quickly or they can continuously run. The first type of workflow
+can be used to run a few commands or look at status files and publish that information. The second type of
+workflow can be used to monitor log files and publish entries written to those files. Workflows are typically
+run periodically as cron jobs. The program libexec/run_workflow.py is for executing workflows that complete
+quickly and the program libexec/run_workflow_daemon.py is used to manage long-running workflows. The daemon
+
+## License
+
+This software is licensed the Apache License Version 2.0.
+
+## Installation
+
+Installation instructions are in [docs/INSTALL.md](docs/INSTALL.md).
+
+## Support Information
+
+This software is currently maintained by the ACCESS CONECT project.
+
+The source is maintained in the [ACCESS-CI GitHub](https://github.com/access-ci-org/ipf).  ACCESS-CI resource
+providers and other members of the ACCESS-CI community are encourage to contribute bug fixes and improvements.
+
+Software bugs may be reported as GitHub issues.  ACCESS-CI related support requests should be submitted through
+the ACCESS-CI ticket system.
+
+## Acknowledgements
+
+This work was supported by the TeraGrid, XSEDE, FutureGrid, XSEDE 2, and ACCESS CONECT projects under
+National Science Foundation grants 0503697, 1053575, 0910812, 1548562, and 2138307.
```

### Comparing `ipf-1.7a5/ipf.egg-info/SOURCES.txt` & `ipf-1.7rc3/ipf.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE-2.0.txt
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ipf/__init__.py
 ipf/catalog.py
 ipf/daemon.py
@@ -16,25 +16,35 @@
 ipf/paths.py
 ipf/pre_populate_position.py
 ipf/publish.py
 ipf/run_workflow.py
 ipf/step.py
 ipf/step_info.py
 ipf/sysinfo.py
+ipf/urnprefix.py
 ipf/workflow.py
 ipf.egg-info/PKG-INFO
 ipf.egg-info/SOURCES.txt
 ipf.egg-info/dependency_links.txt
 ipf.egg-info/entry_points.txt
 ipf.egg-info/not-zip-safe
 ipf.egg-info/requires.txt
 ipf.egg-info/top_level.txt
-ipf/bin/ipf_configure_xsede
+ipf/bin/ipf_configure
 ipf/bin/ipf_workflow
+ipf/configure/__init__.py
+ipf/configure/configure_workflows.py
+ipf/configure/sysinfo.py
+ipf/configure/test/subscribe_amqp.py
+ipf/configure/test/validate.py
+ipf/configure/test/validate_activities.py
+ipf/configure/test/validate_compute.py
+ipf/configure/test/validate_modules.py
 ipf/etc/ipf/logging.conf
+ipf/etc/ipf/ca-certificates/ca_certs.pem
 ipf/etc/ipf/init.d/ipf-WORKFLOW
 ipf/etc/ipf/workflow/ipfinfo.json
 ipf/etc/ipf/workflow/ipfinfo_publish_periodic.json
 ipf/etc/ipf/workflow/sysinfo.json
 ipf/etc/ipf/workflow/sysinfo_publish.json
 ipf/etc/ipf/workflow/sysinfo_publish_periodic.json
 ipf/etc/ipf/workflow/glue2/empty.txt
@@ -51,15 +61,14 @@
 ipf/etc/ipf/workflow/templates/glue2/pbs_activity.json
 ipf/etc/ipf/workflow/templates/glue2/pbs_compute.json
 ipf/etc/ipf/workflow/templates/glue2/serviceremotepublish.json
 ipf/etc/ipf/workflow/templates/glue2/sge_activity.json
 ipf/etc/ipf/workflow/templates/glue2/sge_compute.json
 ipf/etc/ipf/workflow/templates/glue2/slurm_activity.json
 ipf/etc/ipf/workflow/templates/glue2/slurm_compute.json
-ipf/etc/ipf/xsede/ca_certs.pem
 ipf/glue2/__init__.py
 ipf/glue2/abstractservice.py
 ipf/glue2/accelerator_environment.py
 ipf/glue2/activity.py
 ipf/glue2/application.py
 ipf/glue2/benchmark.py
 ipf/glue2/catalina.py
@@ -98,16 +107,8 @@
 ipf/glue2/share.py
 ipf/glue2/slurm.py
 ipf/glue2/step.py
 ipf/glue2/storageservice.py
 ipf/glue2/types.py
 ipf/glue2/unicore.py
 ipf/glue2/valet.py
-ipf/var/ipf/README.txt
-ipf/xsede/__init__.py
-ipf/xsede/configure_workflows.py
-ipf/xsede/sysinfo.py
-ipf/xsede/test/subscribe_amqp.py
-ipf/xsede/test/validate.py
-ipf/xsede/test/validate_activities.py
-ipf/xsede/test/validate_compute.py
-ipf/xsede/test/validate_modules.py
+ipf/var/ipf/README.txt
```

### Comparing `ipf-1.7a5/README.md` & `ipf-1.7rc3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
-# ipf-xsede %VER%-%REL%
+# access-ci-org/ipf %VER%-%REL%
 # README
+
 ## Overview
 
-The Information Publishing Framework (IPF) is a generic framework for gathering and publishing information. IPF
-focuses narrowly on gatethering and publishing, and not on analyzing or visualizing information. IPF grew out of
-work to publish information about TeraGrid compute resources using the
-[GLUE 2 specification](http://www.ogf.org/documents/GFD.147.pdf). IPF continues to support data gathering and
-publishing in the XSEDE program which succeeded TeraGrid.
+The Information Publishing Framework (IPF) is a generic framework used by resource operators to gather and publish
+dynamic resource information in [GLUE 2 serialized format](http://www.ogf.org/documents/GFD.147.pdf). IPF was used
+by the TeraGrid, XSEDE, and XSEDE 2 programs, and is currently being used by the ACCESS-CI program to publish
+high-performance compute cluster information.
 
 IPF gathers and publishes information using simple workflows. These workflows are defined using JSON (see the
 etc/workflows directory) and steps in the workflows are implemented as Python classes. Each step in the
 workflow can require input Data, can produce output Data, and can publish Representations of Data. A typical
-workflow consists of a number of information gathering steps and a few steps that publish Representations to
+workflow consists of a number of information gathering steps and a few steps that publish representations to
 files or to remote services (e.g. REST, messaging).
 
 Workflow steps specify what Data they require and what Data they produce. This allows IPF to construct
 workflows based on partial information - in the case where there are not steps that produce the same Data, an
 entire workflow can be constructed from a single publish step and its required input Data. At the other
 extreme, workflows can be exactly specified with specific steps identified and the outputs of steps bound to
 the inputs of other steps. A typical workflow (e.g. GLUE 2) specifies what steps to include but lets IPF
@@ -26,24 +26,27 @@
 can be used to run a few commands or look at status files and publish that information. The second type of
 workflow can be used to monitor log files and publish entries written to those files. Workflows are typically
 run periodically as cron jobs. The program libexec/run_workflow.py is for executing workflows that complete
 quickly and the program libexec/run_workflow_daemon.py is used to manage long-running workflows. The daemon
 
 ## License
 
-This software is licensed under Version 2.0 of the Apache License.
+This software is licensed the Apache License Version 2.0.
 
 ## Installation
 
 Installation instructions are in [docs/INSTALL.md](docs/INSTALL.md).
 
-## Contact Information
+## Support Information
+
+This software is currently maintained by the ACCESS CONECT project.
 
-This software is maintained by [XSEDE](https://www.github.com/XSEDE).  and you can contact the XSEDE helpdesk
-if you need help using it.
+The source is maintained in the [ACCESS-CI GitHub](https://github.com/access-ci-org/ipf).  ACCESS-CI resource
+providers and other members of the ACCESS-CI community are encourage to contribute bug fixes and improvements.
 
-If you have problems with this software you are welcome to submit an [issue](https://github.com/XSEDE/ipf/issues).
+Software bugs may be reported as GitHub issues.  ACCESS-CI related support requests should be submitted through
+the ACCESS-CI ticket system.
 
 ## Acknowledgements
 
-This work was supported by the TeraGrid, XSEDE, FutureGrid, and XSEDE 2 projects under National Science Foundation
-grants 0503697, 1053575, 0910812, and 1548562.
+This work was supported by the TeraGrid, XSEDE, FutureGrid, XSEDE 2, and ACCESS CONECT projects under
+National Science Foundation grants 0503697, 1053575, 0910812, 1548562, and 2138307.
```

### Comparing `ipf-1.7a5/setup.py` & `ipf-1.7rc3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 # manifest specifies files to include in the source distribution
 def _createManifest():
     f = open(_getManifestFileName(),"w")
     f.write("""
 include README.md
 include LICENSE-2.0.txt
 include ipf/bin/ipf_workflow
-include ipf/bin/ipf_configure_xsede
+include ipf/bin/ipf_configure
 include ipf/etc/ipf/logging.conf
 include ipf/etc/ipf/workflow/*.json
 include ipf/etc/ipf/workflow/glue2/empty.txt
 include ipf/etc/ipf/workflow/templates/glue2/*.json
 include ipf/etc/ipf/init.d/ipf-WORKFLOW
-include ipf/etc/ipf/xsede/ca_certs.pem
+include ipf/etc/ipf/ca-certificates/ca_certs.pem
 include ipf/var/ipf/README.txt
     """)
     f.close()
 
 def _deleteManifest():
     os.remove(_getManifestFileName())
 
@@ -67,40 +67,40 @@
 def workflow_paths(directory):
     return [path for path in [os.path.join(directory,file) for file in os.listdir(directory)] if os.path.isfile(path) and path.endswith(".json")]
 
 if __name__ == "__main__":
     _createManifest()
     _createSetupCfg()
     setup(name="ipf",
-          version="1.7a5",
+          version="1.7rc3",
           description="The Information Publishing Framework",
           long_description=readme(),
           classifiers=[
               "Development Status :: 5 - Production/Stable",
               "License :: OSI Approved :: Apache Software License",
               "Programming Language :: Python :: 2",
               "Topic :: System :: Monitoring",
           ],
           keywords="monitoring information gathering publishing glue2",
-          url="https://github.com/xsede/ipf",
+          url="https://github.com/access-ci-org/ipf",
           author="Eric Blau, Warren Smith",
           author_email="blau@anl.gov",
           license="Apache",
-          packages=["ipf","ipf.glue2","ipf.xsede","ipf.xsede.test"],
+          packages=["ipf","ipf.glue2","ipf.configure","ipf.configure.test"],
           install_requires=["amqp >=1.4","python-dateutil"],
           entry_points={
               "console_scripts": ["ipf_workflow=ipf.run_workflow:main",
-                                  "ipf_configure_xsede=ipf.xsede.configure_workflows:configure"],
+                                  "ipf_configure=ipf.configure.configure_workflows:configure"],
           },
           #include_package_data=True,
           include_package_data=False,
           # data files only applies to the rpm
           data_files = [
               ("/etc/ipf",["ipf/etc/ipf/logging.conf"]),
-              ("/etc/ipf/xsede",["ipf/etc/ipf/xsede/ca_certs.pem"]),
+              ("/etc/ipf/ca-certificates",["ipf/etc/ipf/ca-certificates/ca_certs.pem"]),
               ("/etc/ipf/workflow",workflow_paths("ipf/etc/ipf/workflow")),
               ("/etc/ipf/workflow/glue2",["ipf/etc/ipf/workflow/glue2/empty.txt"]),
               ("/etc/ipf/workflow/glue2",[]),
               ("/etc/ipf/workflow/templates/glue2",workflow_paths("ipf/etc/ipf/workflow/templates/glue2")),
               ("/etc/ipf/init.d",["ipf/etc/ipf/init.d/ipf-WORKFLOW"]),
               ("/var/ipf",[])
           ],
```

