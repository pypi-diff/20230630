# Comparing `tmp/resoto-plugin-aws-3.5.3.tar.gz` & `tmp/resoto-plugin-aws-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-3.5.3.tar", last modified: Wed Jun 21 14:22:50 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-3.6.0.tar", last modified: Fri Jun 30 19:23:29 2023, max compression
```

## Comparing `resoto-plugin-aws-3.5.3.tar` & `resoto-plugin-aws-3.6.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.285735 resoto-plugin-aws-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-21 14:22:50.285735 resoto-plugin-aws-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.273735 resoto-plugin-aws-3.5.3/resoto_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (123)    32234 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.273735 resoto-plugin-aws-3.5.3/resoto_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.277735 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    24038 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)   115330 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.273735 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:19:06.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 14:22:50.285735 resoto-plugin-aws-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.281735 resoto-plugin-aws-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.285735 resoto-plugin-aws-3.5.3/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.767750 resoto-plugin-aws-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-30 19:23:29.767750 resoto-plugin-aws-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.755750 resoto-plugin-aws-3.6.0/resoto_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    29006 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.755750 resoto-plugin-aws-3.6.0/resoto_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.763750 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24384 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18931 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116766 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.755750 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:18:02.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 19:23:29.767750 resoto-plugin-aws-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.763750 resoto-plugin-aws-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.767750 resoto-plugin-aws-3.6.0/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/test_utils.py
```

### Comparing `resoto-plugin-aws-3.5.3/PKG-INFO` & `resoto-plugin-aws-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.5.3
+Version: 3.6.0
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.5.3/README.md` & `resoto-plugin-aws-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/pyproject.toml` & `resoto-plugin-aws-3.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-aws"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3",
+    "resotolib==3.6.0",
     "retrying",
     "boto3",
     "botocore",
 ]
 
 [project.entry-points."resoto.plugins"]
 aws = "resoto_plugin_aws:AWSCollectorPlugin"
```

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/__init__.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import logging
 import multiprocessing
 import os
 from concurrent import futures
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, Sequence
+from typing import List, Optional, Tuple, Union, Sequence
+import subprocess
+import json
 
 import boto3
 import botocore.exceptions
-from botocore.model import ListShape, OperationModel, Shape, StringShape, StructureShape
-from jsons import pascalcase
 from prometheus_client import Counter, Summary
 
 import resotolib.logger
 import resotolib.proc
-from resoto_plugin_aws.aws_client import AwsClient
 from resotolib.args import ArgumentParser, Namespace
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.baseresources import (
     BaseAccount,
     BaseRegion,
     BaseResource,
     Cloud,
     metrics_resource_cleanup_exceptions,
     metrics_resource_pre_cleanup_exceptions,
 )
-from resotolib.config import Config, RunningConfig, current_config
+from resotolib.config import Config, RunningConfig
 from resotolib.core.actions import CoreFeedback
 from resotolib.core.custom_command import execute_command_on_resource
 from resotolib.core.progress import ProgressDone, ProgressTree
 from resotolib.graph import Graph
 from resotolib.logger import log, setup_logger
 from resotolib.types import JsonElement
-from resotolib.utils import NoExitArgumentParser, log_runtime
+from resotolib.utils import log_runtime
 from .collector import AwsAccountCollector
 from .configuration import AwsConfig
 from .resource.base import AwsAccount, AwsResource, get_client
 from .utils import arn_partition_by_region, aws_session, global_region_by_partition, get_aws_profiles_from_file
 
 logging.getLogger("boto").setLevel(logging.CRITICAL)
 
@@ -194,108 +193,47 @@
         "Arn: arn:aws:iam::882374444444:user/matthias\n"
         "```\n\n",
         allowed_on_kind="aws_resource",
     )
     def call_aws_function(
         self, config: Config, resource: Optional[BaseResource], args: List[str]
     ) -> Union[JsonElement, BaseResource]:
-        parser = NoExitArgumentParser()
-        parser.add_argument("--account")
-        parser.add_argument("--role")
-        parser.add_argument("--profile")
-        parser.add_argument("--region")
-        parser.add_argument("service")
-        parser.add_argument("operation")
-        p, remaining = parser.parse_known_args(args)
-        cfg = config.aws
-
-        def adjust_shape(o: str, shape: Optional[Shape]) -> Any:
-            if shape is None or isinstance(shape, StringShape):
-                return o
-            elif isinstance(shape, ListShape):
-                return o.split(",")
-            else:
-                # map and structure types are currently not supported
-                raise ValueError(f"Cannot convert {o} to {shape}")
+        if resource:
+            ac = resource.account()
+            session = aws_session(ac.id, ac.role, ac.profile, ac.partition)  # type: ignore
+        else:
+            session = aws_session()
 
-        # it is not always possible to translate the operation or parameter name directly
-        # Example: modify-db-cluster --> ModifyDBCluster
-        #          --db-cluster-identifier --> --DBClusterIdentifier
-        # Use a lookup list for possible candidates
-        def get_name(is_name: str, possible_names: Iterable[str]) -> Optional[str]:
-            if is_name in possible_names:
-                return is_name
-            else:
-                for name in possible_names:
-                    if name.lower() == is_name.lower():
-                        return name
-                return None
-
-        def coerce_args(fn_args: List[str], om: OperationModel) -> Dict[str, Any]:
-            members: Dict[str, Shape] = om.input_shape.members if isinstance(om.input_shape, StructureShape) else {}
-            param_name: Optional[str] = None
-            param_shape: Optional[Shape] = None
-            arg_val: Dict[str, Any] = {}
-            for arg in fn_args:
-                if arg.startswith("--"):
-                    name = pascalcase(arg.removeprefix("--"))
-                    param_name = get_name(name, members)
-                    if param_name is not None:
-                        param_shape = members.get(param_name)
-                    bool_value = True
-                    if param_shape is None and arg.startswith("--no-"):
-                        name = name[2:]
-                        param_name = get_name(name, members)
-                        param_shape = members.get(name)
-                        bool_value = False
-                    if param_shape is None:
-                        raise ValueError(f"AWS: Unknown parameter {arg}")
-                    if param_shape.name == "Boolean" or param_shape.type_name == "Boolean":
-                        arg_val[name] = bool_value
-                        param_shape = None
-                        param_name = None
-                elif param_name is not None:
-                    arg_val[param_name] = adjust_shape(arg, param_shape)
-                    param_name = None
-                    param_shape = None
-                else:
-                    raise ValueError(f"AWS: Unexpected argument {arg}")
-            return arg_val
-
-        def create_client() -> AwsClient:
-            role = p.role or cfg.role
-            region = p.region or (cfg.region[0] if cfg.region else None)
-            profile = p.profile or (cfg.profiles[0] if cfg.profiles else None)
-            # possibly expensive call: account id is looked up if not provided
-            account = p.account or (cfg.account[0] if cfg.account else current_account_id(profile))
-            return AwsClient(cfg, account, role=role, profile=profile, region=region)
-
-        client = get_client(current_config(), resource) if resource else create_client()
-
-        # try to get the output shape of the operation
-        service_model = client.service_model(p.service)
-        op_name = get_name(pascalcase(p.operation), service_model.operation_names)
-        op: OperationModel = service_model.operation_model(op_name)
-        output_shape = op.output_shape.type_name
-        func_args = coerce_args(remaining, op)
-
-        # call single and treat result as list
-        response = client.call_single(p.service, p.operation, None, **func_args)
-        if response is None:
+        credentials = session.get_credentials()
+        env = os.environ.copy()
+
+        env["AWS_ACCESS_KEY_ID"] = credentials.access_key
+        env["AWS_SECRET_ACCESS_KEY"] = credentials.secret_key
+        env["AWS_SESSION_TOKEN"] = credentials.token
+        if resource:
+            env["AWS_DEFAULT_REGION"] = resource.region().id
+        else:
+            env["AWS_DEFAULT_REGION"] = session.region_name
+
+        cli_result = subprocess.run(["aws"] + args, timeout=10, capture_output=True, check=False, env=env)
+        if cli_result.returncode != 0:
+            raise RuntimeError(f"AWS {cli_result.stderr.decode('utf-8')}")
+        response_str = cli_result.stdout.decode("utf-8")
+        try:
+            response = json.loads(response_str)
+        except Exception:
+            response = response_str.splitlines()
+        if not response:
             result = []
         elif isinstance(response, list):
             result = response
         else:
             result = [response]
 
-        # Remove the "ResponseMetadata" from the result
-        for elem in result:
-            if isinstance(elem, dict):
-                elem.pop("ResponseMetadata", None)
-        return (result[0] if len(result) == 1 else None) if output_shape == "structure" else result
+        return result[0] if len(result) == 1 else result
 
     @staticmethod
     def update_tag(config: Config, resource: BaseResource, key: str, value: str) -> bool:
         """Update the tag of a resource"""
         if isinstance(resource, AwsResource):
             client = get_client(config, resource)
             return resource.update_resource_tag(client, key, value)
@@ -624,15 +562,18 @@
     set_account_names(accounts)
     return accounts
 
 
 def get_org_accounts(
     filter_current_account: bool, profile: Optional[str], core_feedback: CoreFeedback, partition: Optional[str] = None
 ) -> List[str]:
-    session = aws_session(profile=profile, partition=partition)
+    scrape_org_role_arn = Config.aws.scrape_org_role_arn
+    if scrape_org_role_arn is not None and len(str(scrape_org_role_arn).strip()) == 0:
+        scrape_org_role_arn = None
+    session = aws_session(profile=profile, partition=partition, role_arn=scrape_org_role_arn)
     client = session.client("organizations")
     accounts = []
     try:
         response = client.list_accounts()
         accounts = response.get("Accounts", [])
         while response.get("NextToken") is not None:
             response = client.list_accounts(NextToken=response["NextToken"])
```

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/aws_client.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/collector.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/configuration.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,21 @@
         metadata={"description": "List of AWS Account ID(s) to collect (null for all if scrape_org is true)"},
     )
     region: Optional[List[str]] = field(
         default=None,
         metadata={"description": "List of AWS Regions to collect (null for all)"},
     )
     scrape_org: bool = field(default=False, metadata={"description": "Scrape the entire AWS organization"})
+    scrape_org_role_arn: Optional[str] = field(
+        default=None,
+        metadata={
+            "description": "Role ARN to assume when listing AWS org accounts. If set to null Resoto will use the"
+            " default credentials it was started with to call organizations:ListAccounts"
+        },
+    )
     fork_process: bool = field(
         default=True,
         metadata={
             "description": "Fork collector process instead of using threads. "
             "Recommended if you want to scrape many accounts in parallel."
         },
     )
@@ -236,14 +243,18 @@
     discard_account_on_resource_error: bool = field(
         default=False,
         metadata={
             "description": "Fail the whole account if collecting a resource fails. "
             "If false, the error is logged and the resource is skipped."
         },
     )
+    collect_usage_metrics: Optional[bool] = field(
+        default=True,
+        metadata={"description": "Collect resource usage metrics via CloudWatch, enabled by default"},
+    )
 
     @staticmethod
     def from_json(json: Json) -> "AwsConfig":
         valid_fields = fields_dict(AwsConfig).keys()
         for field_name in json.copy().keys():
             if field_name not in valid_fields:
                 del json[field_name]
```

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/apigateway.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/apigateway.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/athena.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/autoscaling.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/base.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,14 +176,16 @@
                     aws_service=spec.service,
                     action=spec.api_action,
                     result_name=spec.result_property,
                     expected_errors=spec.expected_errors,
                     **kwargs,
                 )
                 cls.collect(items, builder)
+                if builder.config.collect_usage_metrics:
+                    cls.collect_usage_metrics(builder)
             except Boto3Error as e:
                 msg = f"Error while collecting {cls.__name__} in region {builder.region.name}: {e}"
                 builder.core_feedback.error(msg, log)
                 raise
             except Exception as e:
                 msg = f"Error while collecting {cls.__name__} in region {builder.region.name}: {e}"
                 builder.core_feedback.info(msg, log)
@@ -197,14 +199,19 @@
         # - add the resource to the graph
         # In case additional work needs to be done, override this method.
         for js in json:
             if instance := cls.from_api(js, builder):
                 builder.add_node(instance, js)
 
     @classmethod
+    def collect_usage_metrics(cls: Type[AwsResource], builder: GraphBuilder) -> None:
+        # Default behavior: do nothing
+        pass
+
+    @classmethod
     def called_collect_apis(cls) -> List[AwsApiSpec]:
         # The default implementation will return the defined api_spec if defined, otherwise an empty list.
         # In case your resource needs more than this api call, please override this method and return the proper list.
         if spec := cls.api_spec:
             return [spec]
         else:
             return []
@@ -469,26 +476,28 @@
         region: AwsRegion,
         client: AwsClient,
         executor: ExecutorQueue,
         core_feedback: CoreFeedback,
         global_instance_types: Optional[Dict[str, Any]] = None,
         graph_nodes_access: Optional[RWLock] = None,
         graph_edges_access: Optional[RWLock] = None,
+        last_run: Optional[datetime] = None,
     ) -> None:
         self.graph = graph
         self.cloud = cloud
         self.account = account
         self.region = region
         self.client = client
         self.executor = executor
         self.name = f"AWS:{account.name}:{region.name}"
         self.global_instance_types: Dict[str, Any] = global_instance_types if global_instance_types is not None else {}
         self.core_feedback = core_feedback
         self.graph_nodes_access = graph_nodes_access or RWLock()
         self.graph_edges_access = graph_edges_access or RWLock()
+        self.last_run = last_run
 
     def submit_work(self, service: str, fn: Callable[..., T], *args: Any, **kwargs: Any) -> Future[T]:
         """
         Use this method for work that can be done in parallel.
         Note: the executor pool is shared between all regions and only allows the configured number of tasks per key.
               Key: RegionId:Service in the same region and the same service start only the configured number of tasks
         """
```

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudformation.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudformation.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudfront.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudtrail.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudwatch.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudwatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,50 +337,56 @@
 class AwsCloudwatchQuery:
     metric_name: str
     namespace: str
     dimensions: Tuple[Tuple[str, str], ...]
     period: timedelta
     ref_id: str
     metric_id: str
+    stat: str = "Sum"
+    unit: str = "Count"
 
     def to_json(self) -> Json:
         return {
             "Id": self.metric_id,
             "MetricStat": {
                 "Metric": {
                     "Namespace": self.namespace,
                     "MetricName": self.metric_name,
                     "Dimensions": [{"Name": k, "Value": v} for k, v in self.dimensions],
                 },
                 "Period": int((self.period.total_seconds() / 60) * 60),  # round to the next 60 seconds
-                "Stat": "Sum",
-                "Unit": "Count",
+                "Stat": self.stat,
+                "Unit": self.unit,
             },
             "ReturnData": True,
         }
 
     @staticmethod
     def create(
         metric_name: str,
         namespace: str,
         period: timedelta,
         ref_id: str,
         metric_id: Optional[str] = None,
+        stat: str = "Sum",
+        unit: str = "Count",
         **dimensions: str,
     ) -> "AwsCloudwatchQuery":
         dims = "_".join(f"{k}+{v}" for k, v in dimensions.items())
         rid = metric_id or re.sub("\\W", "_", f"{metric_name}-{namespace}-{dims}".lower())
         # noinspection PyTypeChecker
         return AwsCloudwatchQuery(
             metric_name=metric_name,
             namespace=namespace,
             period=period,
             dimensions=tuple(dimensions.items()),
             ref_id=ref_id,
             metric_id=rid,
+            stat=stat,
+            unit=unit,
         )
 
 
 @define(eq=False, slots=False)
 class AwsCloudwatchMessageData:
     mapping: ClassVar[Dict[str, Bender]] = {"code": S("Code"), "value": S("Value")}
     code: Optional[str] = field(default=None)
```

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cognito.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cognito.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/config.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/dynamodb.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/ec2.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import ClassVar, Dict, Optional, List, Type, Any
 import copy
 
 from attrs import define, field
 from resoto_plugin_aws.aws_client import AwsClient
 
 from resoto_plugin_aws.resource.base import AwsResource, GraphBuilder, AwsApiSpec, get_client
@@ -1039,14 +1039,55 @@
     def collect(cls: Type[AwsResource], json: List[Json], builder: GraphBuilder) -> None:
         for reservation in json:
             for instance_in in reservation["Instances"]:
                 mapped = bend(cls.mapping, instance_in)
                 instance = AwsEc2Instance.from_json(mapped)
                 builder.add_node(instance, instance_in)
 
+    @classmethod
+    def collect_usage_metrics(cls: Type[AwsResource], builder: GraphBuilder) -> None:
+        instances = {
+            instance.id: instance
+            for instance in builder.nodes(clazz=AwsEc2Instance)
+            if instance.region().id == builder.region.id
+        }
+        queries = []
+        now = utc()
+        if builder.last_run:
+            start = builder.last_run
+            delta = now - start
+        else:
+            delta = timedelta(hours=1)
+            start = now - delta
+        for instance_id in instances:
+            queries.append(
+                AwsCloudwatchQuery.create(
+                    metric_name="CPUUtilization",
+                    namespace="AWS/EC2",
+                    period=delta,
+                    ref_id=instance_id,
+                    stat="Average",
+                    unit="Percent",
+                    InstanceId=instance_id,
+                )
+            )
+
+        metric_name = {"CPUUtilization": "cpu"}
+
+        stat_name = {
+            "Average": "avg",
+        }
+
+        for query, metric in AwsCloudwatchMetricData.query_for(builder.client, queries, start, now).items():
+            instance = instances.get(query.ref_id)
+            metric_value = next(iter(metric.metric_values), None)
+
+            if instance and metric_value:
+                instance._metrics[metric_name[query.metric_name]] = {stat_name[query.stat]: metric_value}
+
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         super().connect_in_graph(builder, source)
         # connect instance type and copy values
         # noinspection PyTypeChecker
         if instance_type := builder.instance_type(self.region(), self.instance_type):
             self.instance_cores = instance_type.instance_cores
             self.instance_memory = instance_type.instance_memory
```

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/ecs.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/ecs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/efs.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/eks.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/eks.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elasticache.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elasticbeanstalk.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elb.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elbv2.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elbv2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/glacier.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/glacier.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/iam.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/iam.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/kinesis.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/kms.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/lambda_.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/lambda_.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/pricing.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/pricing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/rds.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/redshift.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/route53.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/route53.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/s3.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sagemaker.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sagemaker.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/service_quotas.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/service_quotas.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sns.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sns.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sqs.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws/utils.py` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,25 @@
     retry_on_exception=retry_on_session_error,
 )
 def aws_session(
     account: Optional[str] = None,
     role: Optional[str] = None,
     profile: Optional[str] = None,
     partition: Optional[str] = None,
+    role_arn: Optional[str] = None,
 ) -> BotoSession:
     if partition is None:
         partition = "aws"
     global_region = global_region_by_partition(partition)
 
     if Config.aws.role_override:
         role = Config.aws.role
-    if role and account:
-        role_arn = f"arn:{partition}:iam::{account}:role/{role}"
+    if (role and account) or role_arn:
+        if role_arn is None:
+            role_arn = f"arn:{partition}:iam::{account}:role/{role}"
         if profile:
             session = BotoSession(
                 profile_name=profile,
                 region_name=global_region,
             )
         else:
             session = BotoSession(
```

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/PKG-INFO` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.5.3
+Version: 3.6.0
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/SOURCES.txt` & `resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/__init__.py` & `resoto-plugin-aws-3.6.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/aws_client_test.py` & `resoto-plugin-aws-3.6.0/test/aws_client_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/collector_test.py` & `resoto-plugin-aws-3.6.0/test/collector_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/configuration_test.py` & `resoto-plugin-aws-3.6.0/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/graphbuilder_test.py` & `resoto-plugin-aws-3.6.0/test/graphbuilder_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/__init__.py` & `resoto-plugin-aws-3.6.0/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/apigateway_test.py` & `resoto-plugin-aws-3.6.0/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/athena_test.py` & `resoto-plugin-aws-3.6.0/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/autoscaling_test.py` & `resoto-plugin-aws-3.6.0/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/base_test.py` & `resoto-plugin-aws-3.6.0/test/resources/base_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/cloudformation_test.py` & `resoto-plugin-aws-3.6.0/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/cloudfront_test.py` & `resoto-plugin-aws-3.6.0/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/cloudtrail_test.py` & `resoto-plugin-aws-3.6.0/test/resources/cloudtrail_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/cloudwatch_test.py` & `resoto-plugin-aws-3.6.0/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/cognito_test.py` & `resoto-plugin-aws-3.6.0/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/dynamodb_test.py` & `resoto-plugin-aws-3.6.0/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/ec2_test.py` & `resoto-plugin-aws-3.6.0/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/ecs_test.py` & `resoto-plugin-aws-3.6.0/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/eks_test.py` & `resoto-plugin-aws-3.6.0/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/elasticache_test.py` & `resoto-plugin-aws-3.6.0/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/elasticbeanstalk_test.py` & `resoto-plugin-aws-3.6.0/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/elb_test.py` & `resoto-plugin-aws-3.6.0/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/elbv2_test.py` & `resoto-plugin-aws-3.6.0/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/glacier_test.py` & `resoto-plugin-aws-3.6.0/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/iam_test.py` & `resoto-plugin-aws-3.6.0/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/kinesis_test.py` & `resoto-plugin-aws-3.6.0/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/kms_test.py` & `resoto-plugin-aws-3.6.0/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/lambda_test.py` & `resoto-plugin-aws-3.6.0/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/pricing_test.py` & `resoto-plugin-aws-3.6.0/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/rds_test.py` & `resoto-plugin-aws-3.6.0/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/redshift_test.py` & `resoto-plugin-aws-3.6.0/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/route53_test.py` & `resoto-plugin-aws-3.6.0/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/s3_test.py` & `resoto-plugin-aws-3.6.0/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/sagemaker_test.py` & `resoto-plugin-aws-3.6.0/test/resources/sagemaker_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/service_quotas_test.py` & `resoto-plugin-aws-3.6.0/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/sns_test.py` & `resoto-plugin-aws-3.6.0/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/resources/sqs_test.py` & `resoto-plugin-aws-3.6.0/test/resources/sqs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.3/test/test_utils.py` & `resoto-plugin-aws-3.6.0/test/test_utils.py`

 * *Files identical despite different names*

