# Comparing `tmp/yaetos-0.9.8-py2.py3-none-any.whl.zip` & `tmp/yaetos-0.9.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 73316 bytes, number of entries: 57
+Zip file size: 73375 bytes, number of entries: 57
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 15:07 yaetos/__init__.py
 -rw-r--r--  2.0 unx     1181 b- defN 22-Mar-23 15:07 yaetos/clickhouse.py
 -rw-r--r--  2.0 unx     2846 b- defN 22-Mar-23 15:07 yaetos/daily_incremental_job.py
 -rw-r--r--  2.0 unx     5420 b- defN 22-Mar-23 15:07 yaetos/db_utils.py
 -rw-r--r--  2.0 unx    37664 b- defN 22-Mar-23 15:07 yaetos/deploy.py
 -rw-r--r--  2.0 unx    65917 b- defN 22-Apr-13 17:42 yaetos/etl_utils.py
 -rw-r--r--  2.0 unx      744 b- defN 22-Apr-27 08:39 yaetos/excel_utils.py
@@ -18,42 +18,42 @@
 -rw-r--r--  2.0 unx     1230 b- defN 22-Apr-13 21:50 yaetos/sql_job.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 15:07 yaetos/libs/analysis_toolkit/__init__.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-23 15:07 yaetos/libs/analysis_toolkit/api_helper.py
 -rw-r--r--  2.0 unx     8521 b- defN 22-Mar-23 15:07 yaetos/libs/analysis_toolkit/query_helper.py
 -rw-r--r--  2.0 unx      283 b- defN 22-Mar-23 15:07 yaetos/libs/analysis_toolkit/query_pandasql.py
 -rw-r--r--  2.0 unx     1599 b- defN 22-Mar-23 15:07 yaetos/libs/analysis_toolkit/query_sparksql_local.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 15:07 yaetos/libs/generic_jobs/__init__.py
--rw-r--r--  2.0 unx      390 b- defN 22-Apr-27 10:54 yaetos/libs/generic_jobs/copy_job.py
--rw-r--r--  2.0 unx      174 b- defN 22-Apr-27 10:54 yaetos/libs/generic_jobs/deployer.py
--rw-r--r--  2.0 unx      318 b- defN 22-Apr-27 10:54 yaetos/libs/generic_jobs/dummy_job.py
--rw-r--r--  2.0 unx      110 b- defN 22-Apr-27 10:54 yaetos/libs/generic_jobs/launcher.py
+-rw-r--r--  2.0 unx      390 b- defN 22-Apr-27 12:39 yaetos/libs/generic_jobs/copy_job.py
+-rw-r--r--  2.0 unx      174 b- defN 22-Apr-27 12:39 yaetos/libs/generic_jobs/deployer.py
+-rw-r--r--  2.0 unx      318 b- defN 22-Apr-27 12:39 yaetos/libs/generic_jobs/dummy_job.py
+-rw-r--r--  2.0 unx      110 b- defN 22-Apr-27 12:39 yaetos/libs/generic_jobs/launcher.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 15:07 yaetos/libs/pytest_utils/__init__.py
 -rw-r--r--  2.0 unx     1245 b- defN 22-Mar-23 15:07 yaetos/libs/pytest_utils/conftest.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 15:07 yaetos/libs/python_db_connectors/__init__.py
 -rw-r--r--  2.0 unx     1137 b- defN 22-Mar-23 15:07 yaetos/libs/python_db_connectors/query_hive.py
 -rw-r--r--  2.0 unx     1096 b- defN 22-Mar-23 15:07 yaetos/libs/python_db_connectors/query_mysql.py
 -rw-r--r--  2.0 unx     2669 b- defN 22-Mar-23 15:07 yaetos/libs/python_db_connectors/query_oracle.py
 -rw-r--r--  2.0 unx     1076 b- defN 22-Mar-23 15:07 yaetos/libs/python_db_connectors/query_redshift.py
 -rw-r--r--  2.0 unx     1104 b- defN 22-Mar-23 15:07 yaetos/libs/python_db_connectors/query_salesforce.py
 -rw-r--r--  2.0 unx     1491 b- defN 22-Mar-21 23:16 yaetos/scripts/Dockerfile_external_testing
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 15:07 yaetos/scripts/__init__.py
--rw-r--r--  2.0 unx     4407 b- defN 22-Apr-27 10:34 yaetos/scripts/install_env.py
+-rw-r--r--  2.0 unx     4856 b- defN 22-Apr-27 12:28 yaetos/scripts/install_env.py
 -rw-r--r--  2.0 unx     1083 b- defN 22-Apr-27 08:45 yaetos/scripts/requirements.txt
 -rw-r--r--  2.0 unx      790 b- defN 22-Mar-23 15:07 yaetos/scripts/requirements_alt.txt
 -rw-r--r--  2.0 unx     2764 b- defN 22-Mar-23 15:07 yaetos/scripts/setup_master.sh
 -rw-r--r--  2.0 unx     2816 b- defN 22-Mar-23 15:07 yaetos/scripts/setup_master_alt.sh
 -rw-r--r--  2.0 unx      926 b- defN 22-Mar-23 15:07 yaetos/scripts/setup_nodes.sh
 -rw-r--r--  2.0 unx      912 b- defN 22-Mar-23 15:07 yaetos/scripts/setup_nodes_alt.sh
 -rw-r--r--  2.0 unx     1806 b- defN 22-Mar-23 15:07 yaetos/scripts/setup_oracle.sh
 -rw-r--r--  2.0 unx     3198 b- defN 22-Mar-23 15:07 yaetos/scripts/terminate_idle_cluster.sh
 -rw-r--r--  2.0 unx      124 b- defN 22-Mar-23 15:07 yaetos/scripts/copy/conftest.py
--rw-r--r--  2.0 unx     1018 b- defN 22-Apr-27 10:54 yaetos/scripts/copy/ex0_extraction_job.py
--rw-r--r--  2.0 unx      726 b- defN 22-Apr-27 10:54 yaetos/scripts/copy/ex1_frameworked_job.py
+-rw-r--r--  2.0 unx     1018 b- defN 22-Apr-27 12:39 yaetos/scripts/copy/ex0_extraction_job.py
+-rw-r--r--  2.0 unx      726 b- defN 22-Apr-27 12:39 yaetos/scripts/copy/ex1_frameworked_job.py
 -rw-r--r--  2.0 unx     1163 b- defN 22-Mar-23 15:07 yaetos/scripts/copy/ex1_frameworked_job_test.py
--rw-r--r--  2.0 unx     1284 b- defN 22-Apr-27 10:54 yaetos/scripts/copy/ex1_full_sql_job_test.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Apr-27 10:54 yaetos-0.9.8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     6405 b- defN 22-Apr-27 10:54 yaetos-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Apr-27 10:54 yaetos-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 22-Apr-27 10:54 yaetos-0.9.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 22-Apr-27 10:54 yaetos-0.9.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5025 b- defN 22-Apr-27 10:54 yaetos-0.9.8.dist-info/RECORD
-57 files, 196831 bytes uncompressed, 65230 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx     1284 b- defN 22-Apr-27 12:39 yaetos/scripts/copy/ex1_full_sql_job_test.py
+-rw-r--r--  2.0 unx    11357 b- defN 22-Apr-27 12:39 yaetos-0.9.9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     6405 b- defN 22-Apr-27 12:39 yaetos-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-Apr-27 12:39 yaetos-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 22-Apr-27 12:39 yaetos-0.9.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 22-Apr-27 12:39 yaetos-0.9.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5025 b- defN 22-Apr-27 12:39 yaetos-0.9.9.dist-info/RECORD
+57 files, 197280 bytes uncompressed, 65289 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -147,26 +147,26 @@
 
 Filename: yaetos/scripts/copy/ex1_frameworked_job_test.py
 Comment: 
 
 Filename: yaetos/scripts/copy/ex1_full_sql_job_test.py
 Comment: 
 
-Filename: yaetos-0.9.8.dist-info/LICENSE.md
+Filename: yaetos-0.9.9.dist-info/LICENSE.md
 Comment: 
 
-Filename: yaetos-0.9.8.dist-info/METADATA
+Filename: yaetos-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: yaetos-0.9.8.dist-info/WHEEL
+Filename: yaetos-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: yaetos-0.9.8.dist-info/entry_points.txt
+Filename: yaetos-0.9.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: yaetos-0.9.8.dist-info/top_level.txt
+Filename: yaetos-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: yaetos-0.9.8.dist-info/RECORD
+Filename: yaetos-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yaetos/scripts/install_env.py

```diff
@@ -82,14 +82,21 @@
     os.system("mkdir -p conf/")
     copyfile(f'{package_path}/scripts/copy/aws_config.cfg.example', f'{cwd}/conf/aws_config.cfg')
     copyfile(f'{package_path}/scripts/copy/jobs_metadata_external.yml', f'{cwd}/conf/jobs_metadata.yml')
     copyfile(f'{package_path}/scripts/copy/connections.cfg.example', f'{cwd}/conf/connections.cfg')
     copyfile(f'{package_path}/scripts/copy/requirements_extra.txt', f'{cwd}/conf/requirements_extra.txt')
 
     # Sample jobs
+    os.system("mkdir -p jobs/generic/")
+    copyfile(f'{package_path}/libs/generic_jobs/copy_job.py', f'{cwd}/jobs/generic/copy_job.py')
+    copyfile(f'{package_path}/libs/generic_jobs/deployer.py', f'{cwd}/jobs/generic/deployer.py')
+    copyfile(f'{package_path}/libs/generic_jobs/dummy_job.py', f'{cwd}/jobs/generic/dummy_job.py')
+    copyfile(f'{package_path}/libs/generic_jobs/launcher.py', f'{cwd}/jobs/generic/launcher.py')
+
+    # Sample jobs
     os.system("mkdir -p jobs/examples/")
     copyfile(f'{package_path}/scripts/copy/ex0_extraction_job.py', f'{cwd}/jobs/examples/ex0_extraction_job.py')
     copyfile(f'{package_path}/scripts/copy/ex1_frameworked_job.py', f'{cwd}/jobs/examples/ex1_frameworked_job.py')
     copyfile(f'{package_path}/scripts/copy/ex1_full_sql_job.sql', f'{cwd}/jobs/examples/ex1_full_sql_job.sql')
 
     # Sample jobs tests
     os.system("mkdir -p tests/jobs/example/")
```

## Comparing `yaetos-0.9.8.dist-info/LICENSE.md` & `yaetos-0.9.9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `yaetos-0.9.8.dist-info/METADATA` & `yaetos-0.9.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaetos
-Version: 0.9.8
+Version: 0.9.9
 Summary: Data Pipelines with Spark on AWS
 Home-page: https://github.com/arthurprevot/yaetos
 Author: Arthur Prevot
 Author-email: prevota@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/arthurprevot/yaetos/issues
 Project-URL: Source, https://github.com/arthurprevot/yaetos/
```

## Comparing `yaetos-0.9.8.dist-info/RECORD` & `yaetos-0.9.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 yaetos/libs/python_db_connectors/query_hive.py,sha256=qg8c1tYW6l6imFjZAFlFpj-fjPpO7PDXUOxdNrKxE7M,1137
 yaetos/libs/python_db_connectors/query_mysql.py,sha256=Kh8_Czgv-y2r7sEU_CbqkOP8DoTYMX-Xi2DYnSSxmFQ,1096
 yaetos/libs/python_db_connectors/query_oracle.py,sha256=PG6XLhB5NJgKELXbeen-0AylpCuXFIth7-eGZN2g5YA,2669
 yaetos/libs/python_db_connectors/query_redshift.py,sha256=3kqHchFmPNZfHfBoN8LmaTaa4sGcwi8dwxWrvg55fME,1076
 yaetos/libs/python_db_connectors/query_salesforce.py,sha256=XoKB-Boqt1BfiNvCkbNbjv529XVjCWpWB8xEEmYGDGQ,1104
 yaetos/scripts/Dockerfile_external_testing,sha256=sCaG6FSJF7lyrmoTrMf0op8ln8jXhYFGSpYE6uOoi-8,1491
 yaetos/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-yaetos/scripts/install_env.py,sha256=PaNoHz9M26_X5XjXuO7-zwVny7x3E2nQqOuMrflv7-s,4407
+yaetos/scripts/install_env.py,sha256=hktZKec08zNZxRuuBWdW23zIWZ6UcgyCm4HI6Iny1sY,4856
 yaetos/scripts/requirements.txt,sha256=KftFjy-LKZzYaIHcLX4yIQe_pxLxQju7gzM9PvZuJmM,1083
 yaetos/scripts/requirements_alt.txt,sha256=VD0qiC2nDtQuQJyJlcfWBX7_uGJAMLFPY-2Hf_4nys0,790
 yaetos/scripts/setup_master.sh,sha256=4fngyF_NX40b375jAC08usooAnSmgUoDwHJ3GAZ2tck,2764
 yaetos/scripts/setup_master_alt.sh,sha256=8hI_n1g7C4vzlrQXmeZiIyRr829204MUYirnIAwxaJE,2816
 yaetos/scripts/setup_nodes.sh,sha256=gyW-L6uHKqQZaJIXDO9Q01g9EheKjH2oRe6PAIYZU5g,926
 yaetos/scripts/setup_nodes_alt.sh,sha256=ECnogjdLPGAVCXWHsJkPUzmgUVJQwJqGdh5YIkgB7aM,912
 yaetos/scripts/setup_oracle.sh,sha256=O5yYKMwN7sQktkSDGxficBtUXS8KVn0w4sv0u-yqXKM,1806
 yaetos/scripts/terminate_idle_cluster.sh,sha256=inm9WsM54TQzDhGeKcahTLcMEUwZ-3t-aqu1NA4l6ew,3198
 yaetos/scripts/copy/conftest.py,sha256=nfad95eE_L8krl2sAjJzUecHc5KnIPbtG8T1_yZElwk,124
 yaetos/scripts/copy/ex0_extraction_job.py,sha256=oVaRGrKfEOSnSOFlSWRnrEEnnu_m10Re3lc0iWGRjBA,1018
 yaetos/scripts/copy/ex1_frameworked_job.py,sha256=Tcw3Fa51Mhr7gd4XbvFP42W_NDSZcYsMSkV4o8C4ZGA,726
 yaetos/scripts/copy/ex1_frameworked_job_test.py,sha256=yQLgdYEvob5NKrDqMxXlqcZdzV4PeFVo6QIqroWJflo,1163
 yaetos/scripts/copy/ex1_full_sql_job_test.py,sha256=rTe3oNq7Rv3elt9O0Z79EwEA-w1g2sOfl3qRq1NIPag,1284
-yaetos-0.9.8.dist-info/LICENSE.md,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-yaetos-0.9.8.dist-info/METADATA,sha256=fYHvwSW69A6gicNLiHsuOXu7URBayb6CvkdZ09skkBE,6405
-yaetos-0.9.8.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-yaetos-0.9.8.dist-info/entry_points.txt,sha256=O17yD82azSBTWjB-NIVmfeL41F5T-4KPZZT5ydArJLE,65
-yaetos-0.9.8.dist-info/top_level.txt,sha256=4d8fcdZlsikTlWZWMvRpzyITZurOkH4KEBMFKkJW9Rs,7
-yaetos-0.9.8.dist-info/RECORD,,
+yaetos-0.9.9.dist-info/LICENSE.md,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+yaetos-0.9.9.dist-info/METADATA,sha256=x6trDmvWnEAlUT3DR3EY6Nk9D1m3vIOfy2e8uC_HCQg,6405
+yaetos-0.9.9.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+yaetos-0.9.9.dist-info/entry_points.txt,sha256=O17yD82azSBTWjB-NIVmfeL41F5T-4KPZZT5ydArJLE,65
+yaetos-0.9.9.dist-info/top_level.txt,sha256=4d8fcdZlsikTlWZWMvRpzyITZurOkH4KEBMFKkJW9Rs,7
+yaetos-0.9.9.dist-info/RECORD,,
```

