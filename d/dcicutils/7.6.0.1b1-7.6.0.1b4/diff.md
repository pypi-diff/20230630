# Comparing `tmp/dcicutils-7.6.0.1b1.tar.gz` & `tmp/dcicutils-7.6.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.6.0.1b1.tar", max compression
+gzip compressed data, was "dcicutils-7.6.0.1b4.tar", max compression
```

## Comparing `dcicutils-7.6.0.1b1.tar` & `dcicutils-7.6.0.1b4.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0     1098 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/README.rst
--rw-r--r--   0        0        0        0 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/base.py
--rwxr-xr-x   0        0        0    51478 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0     1283 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/boto_s3.py
--rw-r--r--   0        0        0     1305 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/boto_sqs.py
--rw-r--r--   0        0        0    13786 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68919 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-06-29 11:54:12.285338 dcicutils-7.6.0.1b1/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6379 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/env_base.py
--rw-r--r--   0        0        0     9465 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3927 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46760 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66487 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33725 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27661 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-06-29 11:54:12.289338 dcicutils-7.6.0.1b1/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28887 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    13576 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3973 2023-06-29 11:54:12.293338 dcicutils-7.6.0.1b1/pyproject.toml
--rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 dcicutils-7.6.0.1b1/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/README.rst
+-rw-r--r--   0        0        0       43 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0     2225 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/boto_monkey_patching.py
+-rw-r--r--   0        0        0    13786 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68885 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-06-29 20:51:20.041054 dcicutils-7.6.0.1b4/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27661 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-06-29 20:51:20.045054 dcicutils-7.6.0.1b4/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3973 2023-06-29 20:51:20.049054 dcicutils-7.6.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 dcicutils-7.6.0.1b4/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.1b4/PKG-INFO
```

### Comparing `dcicutils-7.6.0.1b1/LICENSE.txt` & `dcicutils-7.6.0.1b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/README.rst` & `dcicutils-7.6.0.1b4/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/base.py` & `dcicutils-7.6.0.1b4/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/beanstalk_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/beanstalk_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from . import ff_utils
 from botocore.exceptions import ClientError
 from .base import (
     FOURSIGHT_URL,  # _FF_MAGIC_CNAME, _CGAP_MAGIC_CNAME, _FF_GOLDEN_DB, _CGAP_GOLDEN_DB,
     beanstalk_info, describe_beanstalk_environments, get_beanstalk_real_url,
     compute_ff_prd_env, compute_ff_stg_env, compute_cgap_prd_env, compute_cgap_stg_env, compute_prd_env_for_env,
 )
-from .boto_s3 import boto_s3_client, boto_s3_resource
 from .common import REGION
 from .env_utils import is_stg_or_prd_env, is_orchestrated
 from .misc_utils import PRINT, exported, obsolete, remove_suffix, prompt_for_input
 
 
 exported(
     # These used to be defined here, and there may be other files or even repos that import these,
@@ -1053,15 +1052,15 @@
     """
     new_buckets = [
         'elasticbeanstalk-%s-blobs' % new,
         'elasticbeanstalk-%s-files' % new,
         'elasticbeanstalk-%s-wfoutput' % new,
         'elasticbeanstalk-%s-system' % new,
     ]
-    s3 = boto_s3_client(region_name=REGION)
+    s3 = boto3.client('s3', region_name=REGION)
     for bucket in new_buckets:
         s3.create_bucket(Bucket=bucket)
     PRINT('=== CREATED NEW S3 BUCKETS ===' % new)
     PRINT('MAKE SURE TO UPDATE CORS POLICY FOR -files AND -wfoutput BUCKETS!')
 
 
 def delete_s3_buckets(env_name):
@@ -1080,15 +1079,15 @@
         'elasticbeanstalk-%s-files' % env_name,
         'elasticbeanstalk-%s-wfoutput' % env_name,
         'elasticbeanstalk-%s-system' % env_name,
         'elasticbeanstalk-%s-metadata-bundles' % env_name,
         # note that tibanna logs are shared so are not so easy to delete
     ]
 
-    s3 = boto_s3_resource()
+    s3 = boto3.resource('s3')
     for bucket in buckets:
         PRINT("deleting content for " + bucket)
         try:
             s3.Bucket(bucket).objects.delete()
             s3.Bucket(bucket).delete()
         except Exception:  # noqa: E722
             PRINT(bucket + " not found skipping...")
@@ -1278,15 +1277,15 @@
         'elasticbeanstalk-%s-system' % new,
     ]
     old_buckets = [
         'elasticbeanstalk-%s-blobs' % old,
         'elasticbeanstalk-%s-files' % old,
         'elasticbeanstalk-%s-wfoutput' % old,
     ]
-    s3 = boto_s3_client(region_name=REGION)
+    s3 = boto3.client('s3', region_name=REGION)
     for bucket in new_buckets:
         try:
             s3.create_bucket(Bucket=bucket)
         except:  # noqa: E722
             PRINT("bucket %s already created..." % bucket)
 
     # now copy them
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/cloudformation_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/codebuild_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/command_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/common.py` & `dcicutils-7.6.0.1b4/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/creds_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/data_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/deployment_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/deployment_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import sys
 import toml
 import time
 import boto3
 from git import Repo
 
 from .base import compute_ff_prd_env, compute_cgap_prd_env
-from .boto_s3 import boto_s3_client
 from .common import LEGACY_GLOBAL_ENV_BUCKET, LEGACY_CGAP_GLOBAL_ENV_BUCKET, DEFAULT_ECOSYSTEM
 from .env_utils import (
     get_standard_mirror_env, data_set_for_env, get_bucket_env,
     is_fourfront_env, is_cgap_env, is_stg_or_prd_env, is_test_env, is_hotseat_env,
     is_indexer_env, indexer_env_for_env, full_env_name,
 )
 from .misc_utils import PRINT, Retry, apply_dict_overrides, override_environ, file_contents
@@ -110,15 +109,15 @@
     @classmethod
     def upload_application_to_s3(cls, zip_location):
         """ Uploads the zip file at zip_location to the specified S3 bucket
 
         :param zip_location: where to find zip file to upload
         :return: True in success, False otherwise
         """
-        s3_client = boto_s3_client()
+        s3_client = boto3.client('s3')
         return s3_client.put_object(
             ACL='public-read',
             Body=open(zip_location, 'rb'),
             Bucket=cls.S3_BUCKET,
             Key=os.path.basename(zip_location)  # application_version_name.zip
         )
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/diff_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/docker_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/ecr_scripts.py` & `dcicutils-7.6.0.1b4/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/ecr_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/ecs_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/env_base.py` & `dcicutils-7.6.0.1b4/dcicutils/env_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import boto3
 import contextlib
 import os
 
 from typing import Optional
-from .boto_s3 import boto_s3_resource
 from .common import LEGACY_GLOBAL_ENV_BUCKET, S3BucketName
 from .exceptions import (
     # CannotInferEnvFromManyGlobalEnvs,
     # MissingGlobalEnv,
     SynonymousEnvironmentVariablesMismatched, LegacyDispatchDisabled,
 )
 from .misc_utils import (
@@ -68,15 +68,15 @@
         env_bucket_name = (
             # prefer a given bucket
             env_bucket
             # or GLOBAL_ENV_BUCKET
             or cls.global_env_bucket_name()
             # but failing that, for legacy system, just use legacy name
             or cls._legacy_global_env_bucket_for_testing())
-        s3_resource = boto_s3_resource()
+        s3_resource = boto3.resource('s3')
         env_bucket_model = s3_resource.Bucket(env_bucket_name)
         key_names = [key_obj.key for key_obj in env_bucket_model.objects.all()]
         configs = cls.filter_config_names(key_names, kind=kind)
         return sorted(configs)
 
     @classmethod
     def filter_config_names(cls, configs, kind):
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/env_manager.py` & `dcicutils-7.6.0.1b4/dcicutils/env_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import boto3
 import botocore.client
 import json
 import logging
 import urllib.request
 
 from typing import Optional
-from .boto_s3 import boto_s3_client
 from .env_base import EnvBase
 from .env_utils import full_env_name
 from .exceptions import CannotInferEnvFromManyGlobalEnvs, MissingGlobalEnv
 from .misc_utils import ignored
 
 
 logger = logging.getLogger(__name__)
@@ -63,15 +63,15 @@
         :param env_description: a dictionary (optional, not preferred, a substitute for a name in testing or debugging)
         :param s3: an s3 client such as from boto3.client('s3') or from the .s3 attribute of an s3Utils instance
 
         Although the s3 client can be created for you, but if you already have acess to an s3 client via some existing
         object, you should pass that.
         """
 
-        self.s3 = s3 or boto_s3_client()
+        self.s3 = s3 or boto3.client('s3')
         if env_name and env_description:
             raise ValueError("You may only specify an env_name or an env_description")
         if env_description:
             self.env_description = env_description
         else:  # env_name is given or is None and must be inferred
             env_description = self.verify_and_get_env_config(s3_client=self.s3,
                                                              global_bucket=self.global_env_bucket_name(),
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/env_scripts.py` & `dcicutils-7.6.0.1b4/dcicutils/env_scripts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import argparse
+import boto3
 import json
 import yaml
-from .boto_s3 import boto_s3_client
+
 from .lang_utils import disjoined_list
 from .misc_utils import PRINT, print_error_message
 
 
 EPILOG = __doc__
 
 
 def get_envs_buckets(client=None):
-    client = client or boto_s3_client()
+    client = client or boto3.client('s3')
     all_buckets = [bucket['Name'] for bucket in client.list_buckets()['Buckets']]
     envs_buckets = [bucket for bucket in all_buckets if bucket.endswith("-envs")]
     return envs_buckets
 
 
 LEGACY_FF_ENVS_BUCKET = 'foursight-prod-envs'
 
@@ -38,15 +39,15 @@
 
 
 def show_global_env_bucket(bucket, mode='json', key=None):
 
     single_key = key
     # print(f"bucket={bucket} mode={mode} single_key={single_key}")
 
-    client = boto_s3_client()
+    client = boto3.client('s3')
 
     if bucket is None:
         envs_buckets = get_envs_buckets(client=client)
         if envs_buckets:
             PRINT("There are no obvious envs buckets.")
         else:
             PRINT(f"There is no default bucket. Please use a '--bucket' argument"
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/env_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/env_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import boto3
 import contextlib
 import copy
 import functools
 import json
 import os
 import re
 
 from botocore.exceptions import HTTPClientError, ClientError
 from typing import Optional
 from urllib.parse import urlparse
 from . import env_utils_legacy as legacy
-from .boto_s3 import boto_s3_client
 from .common import (
     EnvName, OrchestratedApp, APP_FOURFRONT, APP_CGAP, ChaliceStage, CHALICE_STAGE_DEV, CHALICE_STAGE_PROD, UrlString,
 )
 from .env_base import EnvBase, LegacyController
 from .env_utils_legacy import ALLOW_ENVIRON_BY_DEFAULT
 from .exceptions import (
     EnvUtilsLoadError, BeanstalkOperationNotImplemented, MissingFoursightBucketTable, IncompleteFoursightBucketTable,
@@ -451,15 +451,15 @@
         """
          Returns the contents of an environmental configuration file.
 
         :param env_bucket: the name of a bucket (the global_env_bucket)
         :param config_key: the name of a key (the name of a configuration - an ff_env or ecosystem)
         """
         try:
-            s3 = boto_s3_client()
+            s3 = boto3.client('s3')
             metadata = s3.get_object(Bucket=env_bucket, Key=config_key)
             data = json.load(metadata['Body'])
             return data
         except HTTPClientError as err_obj:
             if cls._CREDENTIALS_ERROR_PATTERN.match(str(err_obj)):  # Some sort of plausibility test
                 raise EnvUtilsLoadError("Credentials problem, perhaps expired or wrong account.",
                                         env_bucket=env_bucket, config_key=config_key, encapsulated_error=err_obj)
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/env_utils_legacy.py` & `dcicutils-7.6.0.1b4/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/es_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/exceptions.py` & `dcicutils-7.6.0.1b4/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/ff_mocks.py` & `dcicutils-7.6.0.1b4/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/ff_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/ff_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from collections import namedtuple
 from dcicutils.lang_utils import disjoined_list
 from elasticsearch.exceptions import AuthorizationException
 from typing import Optional, Dict, List
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 from . import s3_utils, es_utils
-from .boto_sqs import boto_sqs_client
 from .common import (
     # KeyValuestringDictList, KeyValuestringDict,
     AnyAuthDict, AuthDict, SimpleAuthPair, AuthData, AnyAuthData, PortalEnvName,
     # S3BucketName, S3KeyName,
 )
 from .misc_utils import PRINT
 
@@ -1338,15 +1337,15 @@
 
 
 def internal_compute_stuff_in_queues(ff_env_index_namespace, check_secondary) -> bool:
     if not ff_env_index_namespace:
         raise ValueError(f"Must provide a full fourfront environment name to this function"
                          f" (such as 'fourfront-webdev'). You gave: {ff_env_index_namespace!r}")
     stuff_in_queue = False
-    client = boto_sqs_client(region_name='us-east-1')
+    client = boto3.client('sqs', region_name='us-east-1')
     queue_names = ['-indexer-queue']
     if check_secondary:
         queue_names.append('-secondary-indexer-queue')
     for queue_name in queue_names:
         try:
             queue_url = client.get_queue_url(
                 QueueName=ff_env_index_namespace + queue_name
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/function_cache_decorator.py` & `dcicutils-7.6.0.1b4/dcicutils/function_cache_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def function_cache(*decorator_args, **decorator_kwargs):
     """
     Exactly analogous to the functools.lru_cache decorator, but also allows specifying
     that if the return value of the function is None then no caching is to be done;
     use the nocache_none decorator kwarg set to True to do this. And more generally, use
-    the nocache decorator kwarg set to anything to not cache any value which equals that.
+    the nocache decorator kwart set to anything to not cache any value which equals that.
 
     Also like @lru_cache, this supports the maxsize decorator argument, as well
     as the cache_info and cache_clear functions on the decorated function.
     The maxsize can be specified either as the first argument to the
     decorator or as a maxsize kwarg to the decorator.
 
     In addition we support a ttl (time to live) decorator kwarg which can be specified,
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/glacier_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/glacier_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import boto3
 from typing import Union, List, Tuple
 from concurrent.futures import ThreadPoolExecutor
 from tqdm import tqdm
-from .boto_s3 import boto_s3_client
 from .common import (
     S3_GLACIER_CLASSES, S3StorageClass, MAX_MULTIPART_CHUNKS, MAX_STANDARD_COPY_SIZE,
     ENCODED_LIFECYCLE_TAG_KEY
 )
 from .command_utils import require_confirmation
 from .misc_utils import PRINT
 from .ff_utils import get_metadata, search_metadata, get_health_page, patch_metadata
@@ -48,15 +48,15 @@
                    one item, or you can use the phase methods above with the single item list (recommended).
                    If you want to use the internal methods, see:
                        * get_portal_file_and_restore_from_glacier
                        * copy_object_back_to_original_location
                        * patch_file_lifecycle_status
                        * delete_glaciered_object_versions
         """
-        self.s3 = boto_s3_client()
+        self.s3 = boto3.client('s3')
         self.env_name = env_name
         self.key_manager = CGAPKeyManager()
         self.env_key = self.key_manager.get_keydict_for_env(env_name)
         self.health_page = get_health_page(key=self.env_key, ff_env=env_name)
 
     @classmethod
     def is_glacier_storage_class(cls, storage_class: S3StorageClass):
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/jh_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/kibana/dashboards.json` & `dcicutils-7.6.0.1b4/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/kibana/readme.md` & `dcicutils-7.6.0.1b4/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/lang_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/log_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/misc_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/obfuscation_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/opensearch_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/project_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/qa_checkers.py` & `dcicutils-7.6.0.1b4/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/qa_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/redis_tools.py` & `dcicutils-7.6.0.1b4/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/redis_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/s3_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/s3_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+import boto3
 import json
 import logging
 import mimetypes
 import os
 
 from io import BytesIO
 from typing import Optional, Any, Union
 from typing_extensions import Literal
 from zipfile import ZipFile
 from .base import get_beanstalk_real_url
-from .boto_s3 import boto_s3_client, boto_s3_resource
 from .common import (
     EnvName,
     # LegacyAuthDict, AnyAuthDict, AuthDict,
     AnyJsonData, KeyValuestringDictList,
     # KeyValuestringDict, PortalEnvName,
     S3KeyName, S3BucketName, ServerAuthDict
 )
@@ -96,15 +96,15 @@
         3) With no GLOBAL_ENV_BUCKET or env kwarg,
            we expect bucket kwargs to be set, and use those as bucket names directly.
         """
         EnvUtils.init(env_name=env)
         self.url = ''
         self._health_json_url = None
         self._health_json = None
-        self.s3 = boto_s3_client(region_name='us-east-1')
+        self.s3 = boto3.client('s3', region_name='us-east-1')
         global_bucket = EnvManager.global_env_bucket_name()
         self.env_manager = None  # In a legacy environment, this will continue to be None
         if sys_bucket is None:
             # The choice to discriminate first on sys_bucket being None is part of the resolution of
             # https://hms-dbmi.atlassian.net/browse/C4-674
             if global_bucket:
                 # env_config = self.verify_and_get_env_config(s3_client=self.s3, global_bucket=global_bucket, env=env)
@@ -442,15 +442,15 @@
         if not bucket:
             bucket = self.outfile_bucket
         self.s3.delete_object(Bucket=bucket, Key=key)
 
     @classmethod
     def size(cls, bucket: str) -> int:
         """Slowly and expensively (if there are a lot of them), count the number of items in a bucket."""
-        sbuck = boto_s3_resource().Bucket(bucket)  # get only head of objects so we can count them
+        sbuck = boto3.resource('s3').Bucket(bucket)  # get only head of objects so we can count them
         # There is apparently no sbuck.objects.count(), so one has to enumerate them all.
         # Although one avenue we didn't try that is mentioned in StackOverflow is to go to the billing department
         # in the AWS console, whch knows how many objects there are.
         # TODO: It is recommended that if there are expected to be a lot of objects, we should paginate through
         #       them in chunks of 1000, rather than just pulling .all().
         # Ref: https://stackoverflow.com/questions/2862617/how-can-i-tell-how-many-objects-ive-stored-in-an-s3-bucket
         return sum(1 for _ in sbuck.objects.all())
```

### Comparing `dcicutils-7.6.0.1b1/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.6.0.1b4/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/secrets_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/snapshot_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/task_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/dcicutils/trace_utils.py` & `dcicutils-7.6.0.1b4/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.1b1/pyproject.toml` & `dcicutils-7.6.0.1b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.6.0.1b1"  # TODO: To become 7.6.0
+version = "7.6.0.1b4"  # TODO: To become 7.6.0
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.6.0.1b1/setup.py` & `dcicutils-7.6.0.1b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.6.0.1b1',
+    'version': '7.6.0.1b4',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.6.0.1b1/PKG-INFO` & `dcicutils-7.6.0.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.6.0.1b1
+Version: 7.6.0.1b4
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

