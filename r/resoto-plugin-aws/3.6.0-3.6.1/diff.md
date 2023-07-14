# Comparing `tmp/resoto-plugin-aws-3.6.0.tar.gz` & `tmp/resoto-plugin-aws-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-3.6.0.tar", last modified: Fri Jun 30 19:23:29 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-3.6.1.tar", last modified: Fri Jul 14 17:00:21 2023, max compression
```

## Comparing `resoto-plugin-aws-3.6.0.tar` & `resoto-plugin-aws-3.6.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.767750 resoto-plugin-aws-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-30 19:23:29.767750 resoto-plugin-aws-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.755750 resoto-plugin-aws-3.6.0/resoto_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (123)    29006 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.755750 resoto-plugin-aws-3.6.0/resoto_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.763750 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    24384 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)    18931 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)   116766 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.755750 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:18:02.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 19:23:29.000000 resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 19:23:29.767750 resoto-plugin-aws-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.763750 resoto-plugin-aws-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:29.767750 resoto-plugin-aws-3.6.0/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-30 19:17:21.000000 resoto-plugin-aws-3.6.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.454192 resoto-plugin-aws-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-14 17:00:21.454192 resoto-plugin-aws-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.434192 resoto-plugin-aws-3.6.1/resoto_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.438192 resoto-plugin-aws-3.6.1/resoto_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.446192 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18938 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117358 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.438192 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:54:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 17:00:21.454192 resoto-plugin-aws-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.446192 resoto-plugin-aws-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.454192 resoto-plugin-aws-3.6.1/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/test_utils.py
```

### Comparing `resoto-plugin-aws-3.6.0/PKG-INFO` & `resoto-plugin-aws-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.6.0
+Version: 3.6.1
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.6.0/README.md` & `resoto-plugin-aws-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/pyproject.toml` & `resoto-plugin-aws-3.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-aws"
-version = "3.6.0"
+version = "3.6.1"
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
-    "resotolib==3.6.0",
+    "resotolib==3.6.1",
     "retrying",
     "boto3",
     "botocore",
 ]
 
 [project.entry-points."resoto.plugins"]
 aws = "resoto_plugin_aws:AWSCollectorPlugin"
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/__init__.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import multiprocessing
 import os
 from concurrent import futures
 from pathlib import Path
-from typing import List, Optional, Tuple, Union, Sequence
+from typing import List, Optional, Tuple, Union, Sequence, Any
 import subprocess
 import json
 
 import boto3
 import botocore.exceptions
 from prometheus_client import Counter, Summary
 
@@ -25,15 +25,15 @@
 )
 from resotolib.config import Config, RunningConfig
 from resotolib.core.actions import CoreFeedback
 from resotolib.core.custom_command import execute_command_on_resource
 from resotolib.core.progress import ProgressDone, ProgressTree
 from resotolib.graph import Graph
 from resotolib.logger import log, setup_logger
-from resotolib.types import JsonElement
+from resotolib.types import JsonElement, Json
 from resotolib.utils import log_runtime
 from .collector import AwsAccountCollector
 from .configuration import AwsConfig
 from .resource.base import AwsAccount, AwsResource, get_client
 from .utils import arn_partition_by_region, aws_session, global_region_by_partition, get_aws_profiles_from_file
 
 logging.getLogger("boto").setLevel(logging.CRITICAL)
@@ -47,16 +47,16 @@
 
 GLOBAL_REGIONS = ("us-east-1", "us-gov-west-1", "cn-north-1")
 
 
 class AWSCollectorPlugin(BaseCollectorPlugin):
     cloud = "aws"
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
         self.__regions: List[str] = []
         self.core_feedback: Optional[CoreFeedback] = None
 
     @staticmethod
     def add_config(cfg: Config) -> None:
         cfg.add_config(AwsConfig)
 
@@ -121,23 +121,25 @@
                     collect_method,
                     account,
                     self.regions(profile=account.profile, partition=account.partition),
                     ArgumentParser.args,
                     Config.running_config,
                     self.core_feedback.with_context(cloud.id, account.dname),
                     cloud,
+                    self.task_data or {},
                 )
                 for account in accounts
             ]
             for future in futures.as_completed(wait_for):
                 account_graph = future.result()
                 if not isinstance(account_graph, Graph):
                     log.debug(f"Skipping account graph of invalid type {type(account_graph)}")
                     continue
-                self.graph.merge(account_graph, skip_deferred_edges=True)
+                self.send_account_graph(account_graph)
+                del account_graph
 
         # collect done, purge all session caches
         aws_config.sessions().purge_caches()
 
     def regions(self, profile: Optional[str] = None, partition: str = "aws") -> List[str]:
         if len(self.__regions) == 0:
             if not Config.aws.region or (isinstance(Config.aws.region, list) and len(Config.aws.region) == 0):
@@ -602,14 +604,15 @@
 def collect_account(
     account: AwsAccount,
     regions: List[str],
     args: Namespace,
     running_config: RunningConfig,
     feedback: CoreFeedback,
     cloud: Cloud,
+    task_data: Json,
 ) -> Optional[Graph]:
     collector_name = f"aws_{account.id}"
     resotolib.proc.set_thread_name(collector_name)
 
     if args is not None:
         ArgumentParser.args = args
         setup_logger("resotoworker-aws", force=True, level=getattr(args, "log_level", None))
@@ -619,15 +622,15 @@
 
     if not authenticated(account, feedback):
         feedback.error(f"Skipping account {account.rtdname}. Reason: authentication failure.", log)
         return None
 
     log.debug(f"Starting new collect process for account {account.dname}")
 
-    aac = AwsAccountCollector(Config.aws, cloud, account, regions, feedback)
+    aac = AwsAccountCollector(Config.aws, cloud, account, regions, feedback, task_data)
     try:
         aac.collect()
     except botocore.exceptions.ClientError as e:
         feedback.error(
             f"Ignore account {account.dname}. Reason: An AWS {e.response['Error']['Code']} error occurred.", log
         )
         metrics_unhandled_account_exceptions.labels(account=account.dname).inc()
@@ -637,15 +640,15 @@
         metrics_unhandled_account_exceptions.labels(account=account.dname).inc()
         return None
 
     return aac.graph
 
 
 def collect_account_proxy(*args, queue: multiprocessing.Queue, **kwargs) -> None:  # type: ignore
-    resotolib.proc.initializer()
+    resotolib.proc.collector_initializer()
     queue.put(collect_account(*args, **kwargs))
 
 
 def collect_in_process(*args, **kwargs) -> Optional[Graph]:  # type: ignore
     ctx = multiprocessing.get_context("spawn")
     queue = ctx.Queue()
     kwargs["queue"] = queue
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/aws_client.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/collector.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from concurrent.futures import Future, ThreadPoolExecutor
-from typing import List, Type
+from typing import List, Type, Optional
+from datetime import datetime, timezone
 
 from resoto_plugin_aws.aws_client import AwsClient, ErrorAccumulator
 from resoto_plugin_aws.configuration import AwsConfig
 from resoto_plugin_aws.resource import (
     apigateway,
     athena,
     autoscaling,
@@ -48,14 +49,16 @@
 )
 
 from resotolib.baseresources import Cloud, EdgeType
 from resotolib.core.actions import CoreFeedback
 from resotolib.core.progress import ProgressDone, ProgressTree
 from resotolib.graph import Graph
 from resotolib.proc import set_thread_name
+from resotolib.types import Json
+from resotolib.json import value_in_path
 
 from .utils import global_region_by_partition
 
 log = logging.getLogger("resoto.plugins.aws")
 
 global_resources: List[Type[AwsResource]] = (
     cloudfront.resources
@@ -123,15 +126,21 @@
     additional_calls = [AwsApiSpec("ec2", "start-instances"), AwsApiSpec("ec2", "stop-instances")]
     specs = [spec for r in all_resources for spec in r.called_mutator_apis()] + additional_calls
     return sorted(specs, key=lambda s: s.service + "::" + s.api_action)
 
 
 class AwsAccountCollector:
     def __init__(
-        self, config: AwsConfig, cloud: Cloud, account: AwsAccount, regions: List[str], core_feedback: CoreFeedback
+        self,
+        config: AwsConfig,
+        cloud: Cloud,
+        account: AwsAccount,
+        regions: List[str],
+        core_feedback: CoreFeedback,
+        task_data: Json,
     ) -> None:
         self.config = config
         self.cloud = cloud
         self.account = account
         self.core_feedback = core_feedback
         self.global_region = AwsRegion(
             id=global_region_by_partition(account.partition), tags={}, name="global", account=account
@@ -144,25 +153,47 @@
             account.id,
             role=account.role,
             profile=account.profile,
             region=self.global_region.id,
             partition=account.partition,
             error_accumulator=self.error_accumulator,
         )
+        self.task_data = task_data
 
     def collect(self) -> None:
         with ThreadPoolExecutor(
             thread_name_prefix=f"aws_{self.account.id}", max_workers=self.config.resource_pool_size
         ) as executor:
             # The shared executor is used to spread work for the whole account.
             # Note: only tasks_per_key threads are running max for each region.
             tpk = self.config.shared_tasks_per_key([r.id for r in self.regions])
             shared_queue = ExecutorQueue(executor, tasks_per_key=tpk, name=self.account.safe_name)
+
+            def get_last_run() -> Optional[datetime]:
+                td = self.task_data
+                if not td:
+                    return None
+                timestamp = value_in_path(td, ["timing", td.get("step", ""), "started_at"])
+
+                if timestamp is None:
+                    return None
+
+                return datetime.fromtimestamp(timestamp, timezone.utc)
+
+            last_run = get_last_run()
+
             global_builder = GraphBuilder(
-                self.graph, self.cloud, self.account, self.global_region, self.client, shared_queue, self.core_feedback
+                self.graph,
+                self.cloud,
+                self.account,
+                self.global_region,
+                self.client,
+                shared_queue,
+                self.core_feedback,
+                last_run=last_run,
             )
             global_builder.submit_work("iam", self.update_account)
 
             # mark open progress for all regions
             progress = ProgressTree(self.account.dname, path=[self.cloud.id])
             progress.add_progress(ProgressDone(self.global_region.safe_name, 0, 1))
             for region in self.regions:
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/configuration.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
         d["_holder"] = None
         self.__dict__.update(d)
 
     def sessions(self) -> AwsSessionHolder:
         if self._holder is None:
             with self._lock:
                 if self._holder is None:
-                    log.info("Create a new AWS session holder")
+                    log.debug("Creating a new AWS session holder")
                     self._holder = AwsSessionHolder(
                         access_key_id=self.access_key_id,
                         secret_access_key=self.secret_access_key,
                         role=self.role,
                         role_override=self.role_override,
                     )
         return self._holder
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/apigateway.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/apigateway.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/athena.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/autoscaling.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/base.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import concurrent
 import logging
 from abc import ABC
 from collections import defaultdict, deque
 from concurrent.futures import Executor, Future
-from datetime import datetime, timezone
+from datetime import datetime, timezone, timedelta
 from functools import lru_cache, reduce
 from threading import Event, Lock
 from typing import Any, Callable, ClassVar, Deque, Dict, Iterator, List, Optional, Tuple, Type, TypeVar
+from math import ceil
 
 from attr import evolve, field
 from attrs import define
 from boto3.exceptions import Boto3Error
+from resotolib.utils import utc
 
 from resoto_plugin_aws.aws_client import AwsClient
 from resoto_plugin_aws.configuration import AwsConfig
 from resoto_plugin_aws.resource.pricing import AwsPricingPrice
 from resoto_plugin_aws.utils import arn_partition
 from resotolib.baseresources import (
     BaseAccount,
@@ -489,15 +491,36 @@
         self.client = client
         self.executor = executor
         self.name = f"AWS:{account.name}:{region.name}"
         self.global_instance_types: Dict[str, Any] = global_instance_types if global_instance_types is not None else {}
         self.core_feedback = core_feedback
         self.graph_nodes_access = graph_nodes_access or RWLock()
         self.graph_edges_access = graph_edges_access or RWLock()
-        self.last_run = last_run
+        self.last_run_started_at = last_run
+        self.created_at = utc()
+
+        if self.last_run_started_at:
+            now = utc()
+            start = self.last_run_started_at
+            delta = now - start
+            # AWS requires period to be a muliple of 60, ceil because we want to overlap when in doubt
+            delta = timedelta(seconds=ceil(delta.seconds / 60) * 60)
+            min_delta = max(delta, timedelta(seconds=600))
+            # in case the last collection happened too quickly, raise the metrics timedelta to 600s,
+            # otherwise we get no results from AWS
+            if min_delta != delta:
+                start = now - min_delta
+                delta = min_delta
+        else:
+            now = utc()
+            delta = timedelta(hours=1)
+            start = now - delta
+
+        self.metrics_start = start
+        self.metrics_delta = delta
 
     def submit_work(self, service: str, fn: Callable[..., T], *args: Any, **kwargs: Any) -> Future[T]:
         """
         Use this method for work that can be done in parallel.
         Note: the executor pool is shared between all regions and only allows the configured number of tasks per key.
               Key: RegionId:Service in the same region and the same service start only the configured number of tasks
         """
@@ -625,8 +648,9 @@
             region,
             self.client.for_region(region.safe_name),
             self.executor,
             self.core_feedback,
             self.global_instance_types,
             self.graph_nodes_access,
             self.graph_edges_access,
+            self.last_run_started_at,
         )
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudformation.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudformation.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudfront.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudtrail.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cloudwatch.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudwatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         ref_id: str,
         metric_id: Optional[str] = None,
         stat: str = "Sum",
         unit: str = "Count",
         **dimensions: str,
     ) -> "AwsCloudwatchQuery":
         dims = "_".join(f"{k}+{v}" for k, v in dimensions.items())
-        rid = metric_id or re.sub("\\W", "_", f"{metric_name}-{namespace}-{dims}".lower())
+        rid = metric_id or re.sub("\\W", "_", f"{metric_name}-{namespace}-{dims}-{stat}".lower())
         # noinspection PyTypeChecker
         return AwsCloudwatchQuery(
             metric_name=metric_name,
             namespace=namespace,
             period=period,
             dimensions=tuple(dimensions.items()),
             ref_id=ref_id,
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/cognito.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cognito.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/config.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/dynamodb.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/ec2.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/ec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
-from datetime import datetime, timedelta
-from typing import ClassVar, Dict, Optional, List, Type, Any
+from datetime import datetime
+from typing import ClassVar, Dict, Optional, List, Type, Any, Callable, NamedTuple
 import copy
 
 from attrs import define, field
 from resoto_plugin_aws.aws_client import AwsClient
 
 from resoto_plugin_aws.resource.base import AwsResource, GraphBuilder, AwsApiSpec, get_client
 from resoto_plugin_aws.resource.cloudwatch import AwsCloudwatchQuery, AwsCloudwatchMetricData
 from resoto_plugin_aws.resource.kms import AwsKmsKey
 from resoto_plugin_aws.resource.s3 import AwsS3Bucket
-from resoto_plugin_aws.utils import ToDict, TagsValue
+from resoto_plugin_aws.utils import ToDict, TagsValue, identity
 from resotolib.baseresources import (
     BaseInstance,
     EdgeType,
     BaseVolume,
     BaseInstanceType,
     VolumeStatus,
     InstanceStatus,
@@ -898,14 +898,19 @@
     "shutting-down": InstanceStatus.STOPPED,
     "terminated": InstanceStatus.TERMINATED,
     "stopping": InstanceStatus.STOPPED,
     "stopped": InstanceStatus.STOPPED,
 }
 
 
+class MetricNormalization(NamedTuple):
+    name: str
+    normalize_value: Callable[[float], float] = identity
+
+
 @define(eq=False, slots=False)
 class AwsEc2Instance(EC2Taggable, AwsResource, BaseInstance):
     kind: ClassVar[str] = "aws_ec2_instance"
     api_spec: ClassVar[AwsApiSpec] = AwsApiSpec(service_name, "describe-instances", "Reservations")
     reference_kinds: ClassVar[ModelReference] = {
         "predecessors": {"default": ["aws_vpc"], "delete": ["aws_ec2_keypair", "aws_vpc"]},
         "successors": {"default": ["aws_ec2_keypair"]},
@@ -1044,49 +1049,60 @@
                 builder.add_node(instance, instance_in)
 
     @classmethod
     def collect_usage_metrics(cls: Type[AwsResource], builder: GraphBuilder) -> None:
         instances = {
             instance.id: instance
             for instance in builder.nodes(clazz=AwsEc2Instance)
-            if instance.region().id == builder.region.id
+            if instance.region().id == builder.region.id and instance.instance_status == InstanceStatus.RUNNING
         }
         queries = []
-        now = utc()
-        if builder.last_run:
-            start = builder.last_run
-            delta = now - start
-        else:
-            delta = timedelta(hours=1)
-            start = now - delta
+
+        delta = builder.metrics_delta
+        start = builder.metrics_start
+        now = builder.created_at
+
         for instance_id in instances:
-            queries.append(
-                AwsCloudwatchQuery.create(
-                    metric_name="CPUUtilization",
-                    namespace="AWS/EC2",
-                    period=delta,
-                    ref_id=instance_id,
-                    stat="Average",
-                    unit="Percent",
-                    InstanceId=instance_id,
-                )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name="CPUUtilization",
+                        namespace="AWS/EC2",
+                        period=delta,
+                        ref_id=instance_id,
+                        stat=stat,
+                        unit="Percent",
+                        InstanceId=instance_id,
+                    )
+                    for stat in ["Minimum", "Average", "Maximum"]
+                ]
             )
 
-        metric_name = {"CPUUtilization": "cpu"}
+        metric_normalizers = {"CPUUtilization": MetricNormalization("cpu", lambda x: round(x, ndigits=3))}
 
         stat_name = {
+            "Minimum": "min",
             "Average": "avg",
+            "Maximum": "max",
         }
 
-        for query, metric in AwsCloudwatchMetricData.query_for(builder.client, queries, start, now).items():
+        cloudwatch_result = AwsCloudwatchMetricData.query_for(builder.client, queries, start, now)
+
+        for query, metric in cloudwatch_result.items():
             instance = instances.get(query.ref_id)
+            if instance is None:
+                continue
             metric_value = next(iter(metric.metric_values), None)
+            if metric_value is None:
+                continue
+
+            name = metric_normalizers[query.metric_name].name
+            value = metric_normalizers[query.metric_name].normalize_value(metric_value)
 
-            if instance and metric_value:
-                instance._metrics[metric_name[query.metric_name]] = {stat_name[query.stat]: metric_value}
+            instance._resource_usage[name][stat_name[query.stat]] = value
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         super().connect_in_graph(builder, source)
         # connect instance type and copy values
         # noinspection PyTypeChecker
         if instance_type := builder.instance_type(self.region(), self.instance_type):
             self.instance_cores = instance_type.instance_cores
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/ecs.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/ecs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/efs.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/eks.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/eks.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elasticache.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elasticbeanstalk.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elb.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/elbv2.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elbv2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/glacier.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/glacier.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/iam.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/iam.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/kinesis.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/kms.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/lambda_.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/lambda_.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/pricing.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/pricing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/rds.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/redshift.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/route53.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/route53.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/s3.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sagemaker.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sagemaker.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/service_quotas.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/service_quotas.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sns.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sns.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/resource/sqs.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws/utils.py` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 from configparser import ConfigParser
 from pathlib import Path
-from typing import Any, Callable, Dict, Iterable, List, Optional
+from typing import Any, Callable, Dict, Iterable, List, Optional, TypeVar
 
 from boto3.session import Session as BotoSession
 from botocore.exceptions import ConnectionClosedError, CredentialRetrievalError
 from prometheus_client import Counter
 from retrying import retry
 
 from resotolib.baseresources import BaseRegion, BaseResource
@@ -180,7 +180,14 @@
         self.name = name
 
     def execute(self, source: List[Json]) -> Optional[str]:
         for k in source:
             if k.get("Key") == self.name:
                 return k.get("Value", "")
         return None
+
+
+T = TypeVar("T")
+
+
+def identity(x: T) -> T:
+    return x
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/PKG-INFO` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.6.0
+Version: 3.6.1
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.6.0/resoto_plugin_aws.egg-info/SOURCES.txt` & `resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/__init__.py` & `resoto-plugin-aws-3.6.1/test/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 def no_feedback() -> CoreFeedback:
     return CoreFeedback("123", "step1", "collect", Queue())
 
 
 @fixture
 def account_collector(aws_config: AwsConfig, no_feedback: CoreFeedback) -> AwsAccountCollector:
     account = AwsAccount(id="test")
-    return AwsAccountCollector(aws_config, Cloud(id="aws"), account, ["us-east-1"], no_feedback)
+    return AwsAccountCollector(aws_config, Cloud(id="aws"), account, ["us-east-1"], no_feedback, {})
```

### Comparing `resoto-plugin-aws-3.6.0/test/aws_client_test.py` & `resoto-plugin-aws-3.6.1/test/aws_client_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/collector_test.py` & `resoto-plugin-aws-3.6.1/test/collector_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/configuration_test.py` & `resoto-plugin-aws-3.6.1/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/graphbuilder_test.py` & `resoto-plugin-aws-3.6.1/test/graphbuilder_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/__init__.py` & `resoto-plugin-aws-3.6.1/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/apigateway_test.py` & `resoto-plugin-aws-3.6.1/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/athena_test.py` & `resoto-plugin-aws-3.6.1/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/autoscaling_test.py` & `resoto-plugin-aws-3.6.1/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/base_test.py` & `resoto-plugin-aws-3.6.1/test/resources/base_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/cloudformation_test.py` & `resoto-plugin-aws-3.6.1/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/cloudfront_test.py` & `resoto-plugin-aws-3.6.1/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/cloudtrail_test.py` & `resoto-plugin-aws-3.6.1/test/resources/cloudtrail_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/cloudwatch_test.py` & `resoto-plugin-aws-3.6.1/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/cognito_test.py` & `resoto-plugin-aws-3.6.1/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/dynamodb_test.py` & `resoto-plugin-aws-3.6.1/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/ec2_test.py` & `resoto-plugin-aws-3.6.1/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/ecs_test.py` & `resoto-plugin-aws-3.6.1/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/eks_test.py` & `resoto-plugin-aws-3.6.1/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/elasticache_test.py` & `resoto-plugin-aws-3.6.1/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/elasticbeanstalk_test.py` & `resoto-plugin-aws-3.6.1/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/elb_test.py` & `resoto-plugin-aws-3.6.1/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/elbv2_test.py` & `resoto-plugin-aws-3.6.1/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/glacier_test.py` & `resoto-plugin-aws-3.6.1/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/iam_test.py` & `resoto-plugin-aws-3.6.1/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/kinesis_test.py` & `resoto-plugin-aws-3.6.1/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/kms_test.py` & `resoto-plugin-aws-3.6.1/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/lambda_test.py` & `resoto-plugin-aws-3.6.1/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/pricing_test.py` & `resoto-plugin-aws-3.6.1/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/rds_test.py` & `resoto-plugin-aws-3.6.1/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/redshift_test.py` & `resoto-plugin-aws-3.6.1/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/route53_test.py` & `resoto-plugin-aws-3.6.1/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/s3_test.py` & `resoto-plugin-aws-3.6.1/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/sagemaker_test.py` & `resoto-plugin-aws-3.6.1/test/resources/sagemaker_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/service_quotas_test.py` & `resoto-plugin-aws-3.6.1/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/sns_test.py` & `resoto-plugin-aws-3.6.1/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/resources/sqs_test.py` & `resoto-plugin-aws-3.6.1/test/resources/sqs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.0/test/test_utils.py` & `resoto-plugin-aws-3.6.1/test/test_utils.py`

 * *Files identical despite different names*

