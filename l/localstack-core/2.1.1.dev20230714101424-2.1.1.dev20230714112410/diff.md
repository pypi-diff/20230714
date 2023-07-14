# Comparing `tmp/localstack-core-2.1.1.dev20230714101424.tar.gz` & `tmp/localstack-core-2.1.1.dev20230714112410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230714101424.tar", last modified: Fri Jul 14 10:14:31 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230714112410.tar", last modified: Fri Jul 14 11:24:18 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230714101424.tar` & `localstack-core-2.1.1.dev20230714112410.tar`

### file list

```diff
@@ -1,878 +1,879 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.359307 localstack-core-2.1.1.dev20230714101424/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-14 10:14:31.359307 localstack-core-2.1.1.dev20230714101424/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-14 10:14:24.000000 localstack-core-2.1.1.dev20230714101424/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4217 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86365 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.263306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.263306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.263306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   760042 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   134355 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29093 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65777 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15100 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    78643 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19981 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.283306 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3628 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.283306 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12364 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61875 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9733 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.287307 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21376 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2559 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7281 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2267 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5740 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21384 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3288 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9386 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27391 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3311 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2004 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4654 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4953 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1251 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3692 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13431 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6773 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8750 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5037 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10780 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5772 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41269 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.287307 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15563 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.287307 localstack-core-2.1.1.dev20230714101424/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.287307 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4428 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5958 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24178 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    83531 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34301 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/provider_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68151 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15009 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15025 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43100 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54568 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.315307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.315307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.315307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.315307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.319307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.319307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.319307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.319307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3890 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.327307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.327307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.327307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10826 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4102 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5244 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7413 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3954 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4137 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13659 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69946 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.351307 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26930 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.351307 localstack-core-2.1.1.dev20230714101424/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17402 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7639 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23586 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    46654 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33137 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33236 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.359307 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39252 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 10:14:27.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-14 10:14:27.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-14 10:14:31.359307 localstack-core-2.1.1.dev20230714101424/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.664443 localstack-core-2.1.1.dev20230714112410/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-14 11:24:10.000000 localstack-core-2.1.1.dev20230714112410/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4217 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86365 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.668443 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   760042 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   134355 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.696442 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.700442 localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.700442 localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29093 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.700442 localstack-core-2.1.1.dev20230714112410/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.700442 localstack-core-2.1.1.dev20230714112410/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.700442 localstack-core-2.1.1.dev20230714112410/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.700442 localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.700442 localstack-core-2.1.1.dev20230714112410/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.700442 localstack-core-2.1.1.dev20230714112410/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.704442 localstack-core-2.1.1.dev20230714112410/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.704442 localstack-core-2.1.1.dev20230714112410/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.704442 localstack-core-2.1.1.dev20230714112410/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.704442 localstack-core-2.1.1.dev20230714112410/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.704442 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65777 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15100 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    78643 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.708442 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.708442 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.708442 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19981 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.708442 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.708442 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3628 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.712442 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12364 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61875 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9733 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.716442 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21376 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2559 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7281 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2267 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5740 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21384 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3288 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9386 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27391 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3311 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2004 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4654 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4953 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1251 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3692 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13431 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6773 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8750 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5037 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10780 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5772 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41269 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.716442 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15563 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.716442 localstack-core-2.1.1.dev20230714112410/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.716442 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.724442 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4428 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5958 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.724442 localstack-core-2.1.1.dev20230714112410/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.724442 localstack-core-2.1.1.dev20230714112410/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.724442 localstack-core-2.1.1.dev20230714112410/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24178 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.724442 localstack-core-2.1.1.dev20230714112410/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.724442 localstack-core-2.1.1.dev20230714112410/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.724442 localstack-core-2.1.1.dev20230714112410/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.724442 localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.728442 localstack-core-2.1.1.dev20230714112410/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    83531 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34301 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/provider_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68151 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15009 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15025 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43100 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54568 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.732442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1379 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.736442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.740442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.740442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.744442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.744442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.744442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.748442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.748442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.748442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.748442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.748442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.752442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.752442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.752442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.752442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.752442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.752442 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10836 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.756441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.760441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.760441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4916 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8018 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9121 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.760441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.760441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.760441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.764441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.764441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.764441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.764441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.764441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.764441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.776441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.776441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.776441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7185 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13697 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69946 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.780441 localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26930 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.784441 localstack-core-2.1.1.dev20230714112410/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17402 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7639 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23586 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    46654 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33137 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33236 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 11:24:18.788441 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-14 11:24:18.000000 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39367 2023-07-14 11:24:18.000000 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 11:24:18.000000 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-14 11:24:18.000000 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 11:24:14.000000 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-14 11:24:14.000000 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-14 11:24:18.000000 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-14 11:24:18.000000 localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-14 11:24:18.792441 localstack-core-2.1.1.dev20230714112410/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-14 10:50:21.000000 localstack-core-2.1.1.dev20230714112410/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230714101424/LICENSE.txt` & `localstack-core-2.1.1.dev20230714112410/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/Makefile` & `localstack-core-2.1.1.dev20230714112410/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/README.md` & `localstack-core-2.1.1.dev20230714112410/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/bin/localstack` & `localstack-core-2.1.1.dev20230714112410/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230714112410/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230714112410/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230714112410/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230714112410/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230714112410/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230714112410/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230714112410/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/config.py` & `localstack-core-2.1.1.dev20230714112410/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/constants.py` & `localstack-core-2.1.1.dev20230714112410/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230714112410/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230714112410/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/client.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/request.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/response.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/http/router.py` & `localstack-core-2.1.1.dev20230714112410/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230714112410/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230714112410/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230714112410/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230714112410/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230714112410/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230714112410/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230714112410/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230714112410/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/plugins.py` & `localstack-core-2.1.1.dev20230714112410/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230714112410/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230714112410/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230714112410/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230714112410/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230714112410/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/types.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/provider_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-2.1.1.dev20230714112410/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/provider_stream.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/provider_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-2.1.1.dev20230714112410/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
     ExecutionAbortedEventDetails,
     ExecutionFailedEventDetails,
     ExecutionSucceededEventDetails,
     HistoryEventExecutionDataDetails,
     HistoryEventType,
 )
 from localstack.services.stepfunctions.asl.component.common.comment import Comment
+from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
+    FailureEventException,
+)
 from localstack.services.stepfunctions.asl.component.common.flow.start_at import StartAt
 from localstack.services.stepfunctions.asl.component.eval_component import EvalComponent
 from localstack.services.stepfunctions.asl.component.state.state import CommonStateField
 from localstack.services.stepfunctions.asl.component.states import States
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
 from localstack.services.stepfunctions.asl.eval.programstate.program_ended import ProgramEnded
@@ -42,16 +45,24 @@
         super().eval(env=env)
 
     def _eval_body(self, env: Environment) -> None:
         try:
             while env.is_running():
                 next_state: CommonStateField = self._get_state(env.next_state_name)
                 next_state.eval(env)
+        except FailureEventException as ex:
+            env.set_error(error=ex.get_execution_failed_event_details())
         except Exception as ex:
-            LOG.debug(f"Stepfunctions computation ended with exception '{ex}'.")
+            cause = f"{type(ex)}({str(ex)})"
+            LOG.error(f"Stepfunctions computation ended with exception '{cause}'.")
+            env.set_error(
+                ExecutionFailedEventDetails(
+                    error="Internal Error", cause=f"Internal Error due to '{cause}'"
+                )
+            )
 
         program_state: ProgramState = env.program_state()
         if isinstance(program_state, ProgramError):
             exec_failed_event_details = select_from_typed_dict(
                 typed_dict=ExecutionFailedEventDetails, obj=program_state.error
             )
             env.event_history.add_event(
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import abc
 import copy
 import logging
 import threading
 from threading import Thread
 from typing import Any, Optional
 
-from localstack.aws.api.stepfunctions import (
-    ExecutionFailedEventDetails,
-    HistoryEventType,
-    TaskFailedEventDetails,
-)
+from localstack.aws.api.stepfunctions import HistoryEventType, TaskFailedEventDetails
 from localstack.services.stepfunctions.asl.component.common.catch.catch_decl import CatchDecl
 from localstack.services.stepfunctions.asl.component.common.catch.catch_outcome import (
     CatchOutcome,
     CatchOutcomeNotCaught,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
     FailureEvent,
+    FailureEventException,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name import (
     StatesErrorName,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name_type import (
     StatesErrorNameType,
 )
@@ -122,21 +119,25 @@
 
         if timeout is not None:
             self.timeout = timeout
         if heartbeat is not None:
             self.heartbeat = heartbeat
 
     def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
-        LOG.warning("State Task executed generic failure event reporting logic.")
+        if isinstance(ex, FailureEventException):
+            return ex.failure_event
+        LOG.warning(
+            "State Task encountered an unhandled exception that lead to a State.Runtime error."
+        )
         return FailureEvent(
-            error_name=StatesErrorName(typ=StatesErrorNameType.StatesTaskFailed),
+            error_name=StatesErrorName(typ=StatesErrorNameType.StatesRuntime),
             event_type=HistoryEventType.TaskFailed,
             event_details=EventDetails(
                 taskFailedEventDetails=TaskFailedEventDetails(
-                    error="Unsupported Error Handling",
+                    error=StatesErrorNameType.StatesRuntime.to_name(),
                     cause=str(ex),
                 )
             ),
         )
 
     @abc.abstractmethod
     def _eval_execution(self, env: Environment) -> None:
@@ -180,18 +181,15 @@
             hist_type_event=state_failure_event.event_type,
             event_detail=state_failure_event.event_details,
         )
         self._terminate_with_event(state_failure_event, env)
 
     @staticmethod
     def _terminate_with_event(failure_event: FailureEvent, env: Environment) -> None:
-        # Halt execution with the given failure event.
-        env.set_error(
-            ExecutionFailedEventDetails(**(list(failure_event.event_details.values())[0]))
-        )
+        raise FailureEventException(failure_event=failure_event)
 
     def _evaluate_with_timeout(self, env: Environment) -> None:
         self.timeout.eval(env=env)
         timeout_seconds: int = env.stack.pop()
 
         frame: Environment = env.open_frame()
         frame.inp = copy.deepcopy(env.inp)
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from localstack.services.stepfunctions.asl.component.component import Component
 from localstack.utils.aws import aws_stack
 
 
 class ResourceCondition(str):
     WaitForTaskToken = "waitForTaskToken"
+    Sync = "sync"
 
 
 class ResourceARN(TypedDict):
     partition: str
     service: str
     region: str
     account: str
@@ -117,9 +118,11 @@
         self.api_action = tail_parts[0]
 
         self.condition = None
         if len(tail_parts) > 1:
             match tail_parts[-1]:
                 case "waitForTaskToken":
                     self.condition = ResourceCondition.WaitForTaskToken
+                case "sync":
+                    self.condition = ResourceCondition.Sync
                 case unsupported:
                     raise RuntimeError(f"Unsupported condition '{unsupported}'.")
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,10 +61,16 @@
                 return StateTaskServiceLambda()
             case "sqs":
                 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service_sqs import (
                     StateTaskServiceSqs,
                 )
 
                 return StateTaskServiceSqs()
+            case "states":
+                from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service_sfn import (
+                    StateTaskServiceSfn,
+                )
+
+                return StateTaskServiceSfn()
 
             case unknown:
                 raise NotImplementedError(f"Unsupported service: '{unknown}'.")  # noqa
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from botocore.config import Config
 from botocore.exceptions import ClientError
 
 from localstack.aws.api.stepfunctions import HistoryEventType, TaskFailedEventDetails
 from localstack.aws.protocol.service_router import get_service_catalog
 from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
     FailureEvent,
 )
@@ -11,15 +12,14 @@
 from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name_type import (
     StatesErrorNameType,
 )
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service_callback import (
     StateTaskServiceCallback,
 )
 from localstack.services.stepfunctions.asl.component.state.state_props import StateProps
-from localstack.services.stepfunctions.asl.eval.callback.callback import CallbackOutcomeFailureError
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
 from localstack.utils.aws import aws_stack
 from localstack.utils.common import camel_to_snake_case
 
 
 class StateTaskServiceAwsSdk(StateTaskServiceCallback):
@@ -71,41 +71,35 @@
                     error=error,
                     cause=cause,
                 )
             ),
         )
 
     def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
-        if isinstance(ex, CallbackOutcomeFailureError):
-            return self._get_callback_outcome_failure_event(ex=ex)
-        if isinstance(ex, TimeoutError):
-            return self._get_timed_out_failure_event()
-
-        norm_service_name: str = self._normalise_service_name(self.resource.api_name)
-        error: str = self._normalise_exception_name(norm_service_name, ex)
         if isinstance(ex, ClientError):
+            norm_service_name: str = self._normalise_service_name(self.resource.api_name)
+            error: str = self._normalise_exception_name(norm_service_name, ex)
+
             error_message: str = ex.response["Error"]["Message"]
             cause_details = [
                 f"Service: {norm_service_name}",
                 f"Status Code: {ex.response['ResponseMetadata']['HTTPStatusCode']}",
                 f"Request ID: {ex.response['ResponseMetadata']['RequestId']}",
             ]
             if "HostId" in ex.response["ResponseMetadata"]:
                 cause_details.append(
                     f'Extended Request ID: {ex.response["ResponseMetadata"]["HostId"]}'
                 )
 
             cause: str = f"{error_message} ({', '.join(cause_details)})"
             failure_event = self._get_task_failure_event(error=error, cause=cause)
             return failure_event
-
-        failure_event = self._get_task_failure_event(
-            error=error, cause=str(ex)  # TODO: update cause decoration.
-        )
-        return failure_event
+        return super()._from_error(env=env, ex=ex)
 
     def _eval_service_task(self, env: Environment, parameters: dict) -> None:
-        api_client = aws_stack.create_external_boto_client(service_name=self._normalised_api_name)
+        api_client = aws_stack.create_external_boto_client(
+            service_name=self._normalised_api_name, config=Config(parameter_validation=False)
+        )
         response = getattr(api_client, self._normalised_api_action)(**parameters) or dict()
         if response:
             response.pop("ResponseMetadata", None)
         env.stack.append(response)
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,14 +82,19 @@
             outcome_output = json.loads(outcome.output)
             env.stack.append(outcome_output)
         elif isinstance(outcome, CallbackOutcomeFailure):
             raise CallbackOutcomeFailureError(callback_outcome_failure=outcome)
         else:
             raise NotImplementedError(f"Unsupported CallbackOutcome type '{type(outcome)}'.")
 
+    def _sync(self, env: Environment) -> None:
+        raise RuntimeError(
+            f"Unsupported .sync callback procedure in resource {self.resource.resource_arn}"
+        )
+
     def _is_condition(self):
         return self.resource.condition is not None
 
     def _get_callback_outcome_failure_event(self, ex: CallbackOutcomeFailureError) -> FailureEvent:
         callback_outcome_failure: CallbackOutcomeFailure = ex.callback_outcome_failure
         error: str = callback_outcome_failure.error
         return FailureEvent(
@@ -101,14 +106,19 @@
                     resource=self._get_sfn_resource(),
                     error=error,
                     cause=callback_outcome_failure.cause,
                 )
             ),
         )
 
+    def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
+        if isinstance(ex, CallbackOutcomeFailureError):
+            return self._get_callback_outcome_failure_event(ex=ex)
+        return super()._from_error(env=env, ex=ex)
+
     def _eval_execution(self, env: Environment) -> None:
         parameters = self._eval_parameters(env=env)
         parameters_str = to_json_str(parameters)
 
         scheduled_event_details = TaskScheduledEventDetails(
             resource=self._get_sfn_resource(),
             resourceType=self._get_sfn_resource_type(),
@@ -133,32 +143,35 @@
             event_detail=EventDetails(
                 taskStartedEventDetails=TaskStartedEventDetails(
                     resource=self._get_sfn_resource(), resourceType=self._get_sfn_resource_type()
                 )
             ),
         )
 
-        self._eval_service_task(env=env, parameters=parameters)
+        normalised_parameters = self._normalised_parameters_bindings(parameters)
+        self._eval_service_task(env=env, parameters=normalised_parameters)
 
         if self._is_condition():
-            output = env.stack.pop()
+            output = env.stack[-1]
             env.event_history.add_event(
                 hist_type_event=HistoryEventType.TaskSubmitted,
                 event_detail=EventDetails(
                     taskSubmittedEventDetails=TaskSubmittedEventDetails(
                         resource=self._get_sfn_resource(),
                         resourceType=self._get_sfn_resource_type(),
                         output=to_json_str(output),
                         outputDetails=HistoryEventExecutionDataDetails(truncated=False),
                     )
                 ),
             )
             match self.resource.condition:
                 case ResourceCondition.WaitForTaskToken:
                     self._wait_for_task_token(env=env)
+                case ResourceCondition.Sync:
+                    self._sync(env=env)
                 case unsupported:
                     raise NotImplementedError(f"Unsupported callback type '{unsupported}'.")
 
         output = env.stack[-1]
         env.event_history.add_event(
             hist_type_event=HistoryEventType.TaskSucceeded,
             event_detail=EventDetails(
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,27 +5,20 @@
 from localstack.aws.api.stepfunctions import HistoryEventType, TaskFailedEventDetails
 from localstack.services.stepfunctions.asl.component.common.error_name.custom_error_name import (
     CustomErrorName,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
     FailureEvent,
 )
-from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name import (
-    StatesErrorName,
-)
-from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name_type import (
-    StatesErrorNameType,
-)
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task import (
     lambda_eval_utils,
 )
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service_callback import (
     StateTaskServiceCallback,
 )
-from localstack.services.stepfunctions.asl.eval.callback.callback import CallbackOutcomeFailureError
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
 
 
 class StateTaskServiceLambda(StateTaskServiceCallback):
     _SUPPORTED_API_PARAM_BINDINGS: Final[dict[str, set[str]]] = {
         "invoke": {
@@ -56,31 +49,23 @@
             ]
         )
         error = f"Lambda.{error_code}"
         cause = f"{error_msg} ({response_details})"
         return error, cause
 
     def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
-        if isinstance(ex, CallbackOutcomeFailureError):
-            return self._get_callback_outcome_failure_event(ex=ex)
-        if isinstance(ex, TimeoutError):
-            return self._get_timed_out_failure_event()
-
         if isinstance(ex, lambda_eval_utils.LambdaFunctionErrorException):
             error = "Exception"
             error_name = CustomErrorName(error)
             cause = ex.payload
         elif isinstance(ex, ClientError):
             error, cause = self._error_cause_from_client_error(ex)
             error_name = CustomErrorName(error)
         else:
-            error = "Exception"
-            error_name = StatesErrorName(typ=StatesErrorNameType.StatesTaskFailed)
-            cause = str(ex)
-
+            return super()._from_error(env=env, ex=ex)
         return FailureEvent(
             error_name=error_name,
             event_type=HistoryEventType.TaskFailed,
             event_details=EventDetails(
                 taskFailedEventDetails=TaskFailedEventDetails(
                     error=error,
                     cause=cause,
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Final, Optional
 
+from botocore.config import Config
 from botocore.exceptions import ClientError
 
 from localstack.aws.api.stepfunctions import HistoryEventType, TaskFailedEventDetails
 from localstack.services.stepfunctions.asl.component.common.error_name.custom_error_name import (
     CustomErrorName,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
     FailureEvent,
 )
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service_callback import (
     StateTaskServiceCallback,
 )
-from localstack.services.stepfunctions.asl.eval.callback.callback import CallbackOutcomeFailureError
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
 from localstack.services.stepfunctions.asl.utils.encoding import to_json_str
 from localstack.utils.aws import aws_stack
 from localstack.utils.strings import camel_to_snake_case
 
 
@@ -35,19 +35,14 @@
         }
     }
 
     def _get_supported_parameters(self) -> Optional[set[str]]:
         return self._SUPPORTED_API_PARAM_BINDINGS.get(self.resource.api_action.lower())
 
     def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
-        if isinstance(ex, CallbackOutcomeFailureError):
-            return self._get_callback_outcome_failure_event(ex=ex)
-        if isinstance(ex, TimeoutError):
-            return self._get_timed_out_failure_event()
-
         if isinstance(ex, ClientError):
             return FailureEvent(
                 error_name=CustomErrorName(self._ERROR_NAME_CLIENT),
                 event_type=HistoryEventType.TaskFailed,
                 event_details=EventDetails(
                     taskFailedEventDetails=TaskFailedEventDetails(
                         error=self._ERROR_NAME_CLIENT,
@@ -55,34 +50,22 @@
                             "Message"
                         ],  # TODO: update to report expected cause.
                         resource=self._get_sfn_resource(),
                         resourceType=self._get_sfn_resource_type(),
                     )
                 ),
             )
-        else:
-            return FailureEvent(
-                error_name=CustomErrorName(self._ERROR_NAME_AWS),
-                event_type=HistoryEventType.TaskFailed,
-                event_details=EventDetails(
-                    taskFailedEventDetails=TaskFailedEventDetails(
-                        error=self._ERROR_NAME_AWS,
-                        cause=str(ex),  # TODO: update to report expected cause.
-                        resource=self._get_sfn_resource(),
-                        resourceType=self._get_sfn_resource_type(),
-                    )
-                ),
-            )
+        return super()._from_error(env=env, ex=ex)
 
     def _eval_service_task(self, env: Environment, parameters: dict) -> None:
         # TODO: Stepfunctions automatically dumps to json MessageBody's definitions.
         #  Are these other similar scenarios?
         if "MessageBody" in parameters:
             message_body = parameters["MessageBody"]
             if message_body is not None and not isinstance(message_body, str):
                 parameters["MessageBody"] = to_json_str(message_body)
 
         api_action = camel_to_snake_case(self.resource.api_action)
-        sqs_client = aws_stack.create_external_boto_client("sqs")
+        sqs_client = aws_stack.connect_to_service("sqs", config=Config(parameter_validation=False))
         response = getattr(sqs_client, api_action)(**parameters)
         response.pop("ResponseMetadata", None)
         env.stack.append(response)
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 from __future__ import annotations
 
 import abc
+import copy
 from typing import Optional
 
-from localstack.aws.api.stepfunctions import HistoryEventType
+from localstack.aws.api.stepfunctions import HistoryEventType, TaskTimedOutEventDetails
+from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
+    FailureEvent,
+)
+from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name import (
+    StatesErrorName,
+)
+from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name_type import (
+    StatesErrorNameType,
+)
 from localstack.services.stepfunctions.asl.component.common.parameters import Parameters
 from localstack.services.stepfunctions.asl.component.state.state_execution.execute_state import (
     ExecutionState,
 )
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.resource import (
     Resource,
 )
 from localstack.services.stepfunctions.asl.component.state.state_props import StateProps
 from localstack.services.stepfunctions.asl.eval.environment import Environment
+from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
 
 
 class StateTask(ExecutionState, abc.ABC):
     resource: Resource
 
     def __init__(self):
         super(StateTask, self).__init__(
@@ -51,14 +62,42 @@
 
     def _get_supported_parameters(self) -> Optional[set[str]]:  # noqa
         return None
 
     def _get_parameters_normalising_bindings(self) -> dict[str, str]:  # noqa
         return dict()
 
+    def _normalised_parameters_bindings(self, parameters: dict[str, str]) -> dict[str, str]:
+        normalised_parameters = copy.deepcopy(parameters)
+        # Normalise bindings.
+        parameter_normalisers = self._get_parameters_normalising_bindings()
+        for parameter_key in list(normalised_parameters.keys()):
+            norm_parameter_key = parameter_normalisers.get(parameter_key, None)
+            if norm_parameter_key:
+                tmp = normalised_parameters[parameter_key]
+                del normalised_parameters[parameter_key]
+                normalised_parameters[norm_parameter_key] = tmp
+        return normalised_parameters
+
+    def _get_timed_out_failure_event(self) -> FailureEvent:
+        return FailureEvent(
+            error_name=StatesErrorName(typ=StatesErrorNameType.StatesTimeout),
+            event_type=HistoryEventType.TaskTimedOut,
+            event_details=EventDetails(
+                taskTimedOutEventDetails=TaskTimedOutEventDetails(
+                    error=StatesErrorNameType.StatesTimeout.to_name(),
+                )
+            ),
+        )
+
+    def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
+        if isinstance(ex, TimeoutError):
+            return self._get_timed_out_failure_event()
+        return super()._from_error(env=env, ex=ex)
+
     def _eval_parameters(self, env: Environment) -> dict:
         # Eval raw parameters.
         parameters = dict()
         if self.parameters:
             self.parameters.eval(env=env)
             parameters = env.stack.pop()
 
@@ -69,21 +108,12 @@
                 parameter
                 for parameter in parameters.keys()
                 if parameter not in supported_parameters
             ]
             for unsupported_parameter in unsupported_parameters:
                 parameters.pop(unsupported_parameter, None)
 
-        # Normalise bindings.
-        parameter_normalisers = self._get_parameters_normalising_bindings()
-        for parameter_key in list(parameters.keys()):
-            norm_parameter_key = parameter_normalisers.get(parameter_key, None)
-            if norm_parameter_key:
-                tmp = parameters[parameter_key]
-                del parameters[parameter_key]
-                parameters[norm_parameter_key] = tmp
-
         return parameters
 
     def _eval_body(self, env: Environment) -> None:
         super(StateTask, self)._eval_body(env=env)
         env.context_object_manager.context_object["Task"] = None
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from typing import Optional
-
 from localstack.aws.api.stepfunctions import HistoryEventType
-from localstack.services.stepfunctions.asl.component.common.cause_decl import CauseDecl
-from localstack.services.stepfunctions.asl.component.common.error_decl import ErrorDecl
+from localstack.services.stepfunctions.asl.component.common.flow.end import End
+from localstack.services.stepfunctions.asl.component.common.flow.next import Next
 from localstack.services.stepfunctions.asl.component.state.state import CommonStateField
+from localstack.services.stepfunctions.asl.component.state.state_continue_with import (
+    ContinueWithSuccess,
+)
 from localstack.services.stepfunctions.asl.component.state.state_props import StateProps
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 
 
-class StateFail(CommonStateField):
+class StateSucceed(CommonStateField):
     def __init__(self):
         super().__init__(
-            state_entered_event_type=HistoryEventType.FailStateEntered,
-            state_exited_event_type=None,
+            state_entered_event_type=HistoryEventType.SucceedStateEntered,
+            state_exited_event_type=HistoryEventType.SucceedStateExited,
         )
-        self.cause: Optional[CauseDecl] = None
-        self.error: Optional[ErrorDecl] = None
 
     def from_state_props(self, state_props: StateProps) -> None:
-        super(StateFail, self).from_state_props(state_props)
-        self.cause = state_props.get(CauseDecl)
-        self.error = state_props.get(ErrorDecl)
+        super(StateSucceed, self).from_state_props(state_props)
+        # TODO: assert all other fields are undefined?
+
+        # No Next or End field: Succeed states are terminal states.
+        if state_props.get(Next) or state_props.get(End):
+            raise ValueError(
+                f"No Next or End field: Succeed states are terminal states: with state '{self}'."
+            )
+        self.continue_with = ContinueWithSuccess()
 
     def _eval_state(self, env: Environment) -> None:
-        # TODO.
-        env.set_error(self)
+        pass
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,43 @@
-from localstack.aws.api.stepfunctions import HistoryEventType
-from localstack.services.stepfunctions.asl.component.common.flow.end import End
-from localstack.services.stepfunctions.asl.component.common.flow.next import Next
-from localstack.services.stepfunctions.asl.component.state.state import CommonStateField
-from localstack.services.stepfunctions.asl.component.state.state_continue_with import (
-    ContinueWithSuccess,
+from typing import Optional
+
+from localstack.aws.api.stepfunctions import HistoryEventType, TaskFailedEventDetails
+from localstack.services.stepfunctions.asl.component.common.cause_decl import CauseDecl
+from localstack.services.stepfunctions.asl.component.common.error_decl import ErrorDecl
+from localstack.services.stepfunctions.asl.component.common.error_name.custom_error_name import (
+    CustomErrorName,
+)
+from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
+    FailureEvent,
+    FailureEventException,
 )
+from localstack.services.stepfunctions.asl.component.state.state import CommonStateField
 from localstack.services.stepfunctions.asl.component.state.state_props import StateProps
 from localstack.services.stepfunctions.asl.eval.environment import Environment
+from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
 
 
-class StateSucceed(CommonStateField):
+class StateFail(CommonStateField):
     def __init__(self):
         super().__init__(
-            state_entered_event_type=HistoryEventType.SucceedStateEntered,
-            state_exited_event_type=HistoryEventType.SucceedStateExited,
+            state_entered_event_type=HistoryEventType.FailStateEntered,
+            state_exited_event_type=None,
         )
+        self.cause: Optional[CauseDecl] = None
+        self.error: Optional[ErrorDecl] = None
 
     def from_state_props(self, state_props: StateProps) -> None:
-        super(StateSucceed, self).from_state_props(state_props)
-        # TODO: assert all other fields are undefined?
-
-        # No Next or End field: Succeed states are terminal states.
-        if state_props.get(Next) or state_props.get(End):
-            raise ValueError(
-                f"No Next or End field: Succeed states are terminal states: with state '{self}'."
-            )
-        self.continue_with = ContinueWithSuccess()
+        super(StateFail, self).from_state_props(state_props)
+        self.cause = state_props.get(CauseDecl)
+        self.error = state_props.get(ErrorDecl)
 
     def _eval_state(self, env: Environment) -> None:
-        pass
+        failure_event = FailureEvent(
+            error_name=CustomErrorName(self.error.error),
+            event_type=HistoryEventType.TaskFailed,
+            event_details=EventDetails(
+                taskFailedEventDetails=TaskFailedEventDetails(
+                    error=self.error.error, cause=self.cause.cause
+                )
+            ),
+        )
+        raise FailureEventException(failure_event=failure_event)
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/execution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import datetime
-import json
 from typing import Final, Optional
 
 from localstack.aws.api.stepfunctions import (
     Arn,
     CloudWatchEventsExecutionDataDetails,
     DescribeExecutionOutput,
     ExecutionListItem,
     ExecutionStatus,
     GetExecutionHistoryOutput,
     HistoryEventList,
     InvalidName,
+    SensitiveCause,
     SensitiveData,
+    SensitiveError,
     StartExecutionOutput,
     Timestamp,
     TraceHeader,
 )
 from localstack.services.stepfunctions.asl.eval.contextobject.contex_object import (
     ContextObjectInitData,
 )
@@ -41,21 +42,25 @@
     class BaseExecutionWorkerComm(ExecutionWorkerComm):
         def __init__(self, execution: Execution):
             self.execution: Execution = execution
 
         def terminated(self) -> None:
             exit_program_state: ProgramState = self.execution.exec_worker.env.program_state()
             self.execution.stop_date = datetime.datetime.now()
-            self.execution.output = to_json_str(self.execution.exec_worker.env.inp)
             if isinstance(exit_program_state, ProgramEnded):
                 self.execution.exec_status = ExecutionStatus.SUCCEEDED
+                self.execution.output = to_json_str(
+                    self.execution.exec_worker.env.inp, separators=(",", ":")
+                )
             elif isinstance(exit_program_state, ProgramStopped):
                 self.execution.exec_status = ExecutionStatus.ABORTED
             elif isinstance(exit_program_state, ProgramError):
                 self.execution.exec_status = ExecutionStatus.FAILED
+                self.execution.error = exit_program_state.error["error"]
+                self.execution.cause = exit_program_state.error["cause"]
             else:
                 raise RuntimeWarning(
                     f"Execution ended with unsupported ProgramState type '{type(exit_program_state)}'."
                 )
 
     name: Final[str]
     role_arn: Final[Arn]
@@ -68,58 +73,68 @@
 
     exec_status: Optional[ExecutionStatus]
     stop_date: Optional[Timestamp]
 
     output: Optional[SensitiveData]
     output_details: Optional[CloudWatchEventsExecutionDataDetails]
 
+    error: Optional[SensitiveError]
+    cause: Optional[SensitiveCause]
+
     exec_worker: Optional[ExecutionWorker]
 
     def __init__(
         self,
         name: str,
         role_arn: Arn,
         exec_arn: Arn,
         state_machine: StateMachine,
         start_date: Timestamp,
         input_data: Optional[dict] = None,
-        input_details: Optional[CloudWatchEventsExecutionDataDetails] = None,
         trace_header: Optional[TraceHeader] = None,
     ):
         self.name = name
         self.role_arn = role_arn
         self.exec_arn = exec_arn
         self.state_machine = state_machine
         self.start_date = start_date
         self.input_data = input_data
-        self.input_details = input_details
+        self.input_details = CloudWatchEventsExecutionDataDetails(included=True)
         self.trace_header = trace_header
         self.exec_status = None
         self.stop_date = None
         self.output = None
-        self.output_details = None
+        self.output_details = CloudWatchEventsExecutionDataDetails(included=True)
         self.exec_worker = None
+        self.error = None
+        self.cause = None
 
     def to_start_output(self) -> StartExecutionOutput:
         return StartExecutionOutput(executionArn=self.exec_arn, startDate=self.start_date)
 
     def to_describe_output(self) -> DescribeExecutionOutput:
-        return DescribeExecutionOutput(
+        describe_output = DescribeExecutionOutput(
             executionArn=self.exec_arn,
             stateMachineArn=self.state_machine.arn,
-            name=self.state_machine.name,
+            name=self.name,
             status=self.exec_status,
             startDate=self.start_date,
             stopDate=self.stop_date,
-            input=json.dumps(self.input_data),
+            input=to_json_str(self.input_data, separators=(",", ":")),
             inputDetails=self.input_details,
-            output=self.output,
-            outputDetails=self.output_details,
             traceHeader=self.trace_header,
         )
+        if describe_output["status"] == ExecutionStatus.SUCCEEDED:
+            describe_output["output"] = self.output
+            describe_output["outputDetails"] = self.output_details
+        if self.error is not None:
+            describe_output["error"] = self.error
+        if self.cause is not None:
+            describe_output["cause"] = self.cause
+        return describe_output
 
     def to_execution_list_item(self) -> ExecutionListItem:
         return ExecutionListItem(
             executionArn=self.exec_arn,
             stateMachineArn=self.state_machine.arn,
             name=self.name,
             status=self.exec_status,
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/provider_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             input_data = None
         else:
             try:
                 input_data = json.loads(input)
             except Exception as ex:
                 raise InvalidExecutionInput(str(ex))  # TODO: report parsing error like AWS.
 
-        exec_name = long_uid()
+        exec_name = name or long_uid()  # TODO: validate name format
         arn_data: ArnData = parse_arn(state_machine_arn)
         exec_arn = ":".join(
             [
                 "arn",
                 arn_data["partition"],
                 arn_data["service"],
                 arn_data["region"],
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230714112410/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/state/core.py` & `localstack-core-2.1.1.dev20230714112410/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230714112410/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230714112410/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230714112410/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230714112410/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230714112410/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -542,14 +542,15 @@
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
 localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
 localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
 localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
 localstack/services/stepfunctions/asl/component/state/state_pass/result.py
 localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
 localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7744107744107743%*

 * *Differences: {"'localstack.cloudformation.resource_providers'": '{insert: [(1, '*

 * *                                                   "'AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user:IAMUserProviderPlugin')], "*

 * *                                                   'delete: [0]}',*

 * * "'localstack.hooks.configure_localstack_container'": '{insert: [(1, '*

 * *                                                      "'configure_edge_port=localstack.plugins:configure_edge_port')], "*

 * *                                  […]*

```diff
@@ -43,52 +43,52 @@
         "stepfunctions:v2=localstack.services.providers:stepfunctions_v2",
         "sts:default=localstack.services.providers:sts",
         "support:default=localstack.services.providers:support",
         "swf:default=localstack.services.providers:swf",
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.cloudformation.resource_providers": [
-        "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user:IAMUserProviderPlugin",
-        "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin"
+        "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin",
+        "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user:IAMUserProviderPlugin"
     ],
     "localstack.hooks.configure_localstack_container": [
-        "configure_edge_port=localstack.plugins:configure_edge_port",
-        "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file"
+        "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file",
+        "configure_edge_port=localstack.plugins:configure_edge_port"
     ],
     "localstack.hooks.on_infra_ready": [
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
     ],
     "localstack.hooks.on_infra_start": [
-        "deprecation_warnings=localstack.plugins:deprecation_warnings",
-        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
-        "_publish_container_info=localstack.runtime.analytics:_publish_container_info"
+        "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
+        "deprecation_warnings=localstack.plugins:deprecation_warnings",
+        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
         "terraform/community=localstack.packages.plugins:terraform_package",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package"
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230714112410/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/pyproject.toml` & `localstack-core-2.1.1.dev20230714112410/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714101424/setup.cfg` & `localstack-core-2.1.1.dev20230714112410/setup.cfg`

 * *Files identical despite different names*

