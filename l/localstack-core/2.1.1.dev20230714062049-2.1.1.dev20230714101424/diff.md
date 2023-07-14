# Comparing `tmp/localstack-core-2.1.1.dev20230714062049.tar.gz` & `tmp/localstack-core-2.1.1.dev20230714101424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230714062049.tar", last modified: Fri Jul 14 06:20:59 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230714101424.tar", last modified: Fri Jul 14 10:14:31 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230714062049.tar` & `localstack-core-2.1.1.dev20230714101424.tar`

### file list

```diff
@@ -1,878 +1,878 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.654628 localstack-core-2.1.1.dev20230714062049/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-14 06:20:59.654628 localstack-core-2.1.1.dev20230714062049/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.542628 localstack-core-2.1.1.dev20230714062049/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.546628 localstack-core-2.1.1.dev20230714062049/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-14 06:20:49.000000 localstack-core-2.1.1.dev20230714062049/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.546628 localstack-core-2.1.1.dev20230714062049/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4217 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.546628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86365 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   760042 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.550628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   134355 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.554628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.558628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.558628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.558628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.558628 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9183 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.558628 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.562628 localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.562628 localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29093 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.562628 localstack-core-2.1.1.dev20230714062049/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.562628 localstack-core-2.1.1.dev20230714062049/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.562628 localstack-core-2.1.1.dev20230714062049/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.566628 localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.566628 localstack-core-2.1.1.dev20230714062049/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.566628 localstack-core-2.1.1.dev20230714062049/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.570628 localstack-core-2.1.1.dev20230714062049/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.570628 localstack-core-2.1.1.dev20230714062049/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.570628 localstack-core-2.1.1.dev20230714062049/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.574628 localstack-core-2.1.1.dev20230714062049/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.574628 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65824 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40232 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15121 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    78643 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.578628 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.578628 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.578628 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19981 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72344 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.578628 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.582628 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.582628 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12364 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61886 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7957 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9733 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.586628 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21531 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7311 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2283 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5756 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21650 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3340 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9484 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27850 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3365 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4684 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5007 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2735 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1513 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3727 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13537 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6852 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8861 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5059 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10780 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5845 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41308 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.586628 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.586628 localstack-core-2.1.1.dev20230714062049/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.586628 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73285 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.590628 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.590628 localstack-core-2.1.1.dev20230714062049/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.590628 localstack-core-2.1.1.dev20230714062049/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.590628 localstack-core-2.1.1.dev20230714062049/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24178 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.590628 localstack-core-2.1.1.dev20230714062049/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.590628 localstack-core-2.1.1.dev20230714062049/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20375 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.590628 localstack-core-2.1.1.dev20230714062049/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.594628 localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.594628 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.594628 localstack-core-2.1.1.dev20230714062049/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.594628 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.594628 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.594628 localstack-core-2.1.1.dev20230714062049/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.598628 localstack-core-2.1.1.dev20230714062049/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.598628 localstack-core-2.1.1.dev20230714062049/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.598628 localstack-core-2.1.1.dev20230714062049/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.598628 localstack-core-2.1.1.dev20230714062049/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.598628 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    83531 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34301 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/provider_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15011 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.602628 localstack-core-2.1.1.dev20230714062049/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.602628 localstack-core-2.1.1.dev20230714062049/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.602628 localstack-core-2.1.1.dev20230714062049/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22742 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.602628 localstack-core-2.1.1.dev20230714062049/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43100 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.602628 localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.602628 localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16684 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.602628 localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.606628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.606628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.606628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.606628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.606628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.606628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.606628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.610628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.610628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.610628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.610628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.610628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.610628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.610628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.614628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.614628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.614628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.614628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.614628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.614628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.618628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.618628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.618628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.618628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.618628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.618628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.618628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.622628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.622628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.622628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.622628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3890 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.622628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.622628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.622628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.622628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.626628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.626628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10826 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.626628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.626628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.626628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.630628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2069 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.630628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4102 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5244 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7413 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3954 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4137 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.630628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.630628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.630628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.630628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.630628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.630628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.634628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.634628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.634628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.634628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13659 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13605 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.638628 localstack-core-2.1.1.dev20230714062049/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.642628 localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.642628 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69946 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.642628 localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26930 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.646628 localstack-core-2.1.1.dev20230714062049/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.650628 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.650628 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13775 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11852 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23586 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.650628 localstack-core-2.1.1.dev20230714062049/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.650628 localstack-core-2.1.1.dev20230714062049/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    46654 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33137 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33236 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.654628 localstack-core-2.1.1.dev20230714062049/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.654628 localstack-core-2.1.1.dev20230714062049/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23661 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 06:20:59.654628 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-14 06:20:59.000000 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39252 2023-07-14 06:20:59.000000 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 06:20:59.000000 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-14 06:20:59.000000 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 06:20:54.000000 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-14 06:20:54.000000 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-14 06:20:59.000000 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-14 06:20:59.000000 localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-14 06:20:59.654628 localstack-core-2.1.1.dev20230714062049/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-14 05:47:53.000000 localstack-core-2.1.1.dev20230714062049/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.359307 localstack-core-2.1.1.dev20230714101424/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-14 10:14:31.359307 localstack-core-2.1.1.dev20230714101424/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-14 10:14:24.000000 localstack-core-2.1.1.dev20230714101424/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4217 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86365 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.251306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.263306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.263306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.263306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   760042 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   134355 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.267306 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29093 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.271306 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.275307 localstack-core-2.1.1.dev20230714101424/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65777 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15100 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    78643 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19981 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.279307 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.283306 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3628 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.283306 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12364 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61875 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9733 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.287307 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21376 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2559 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7281 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2267 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5740 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21384 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3288 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9386 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27391 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3311 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2004 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4654 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4953 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1251 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3692 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13431 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6773 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8750 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5037 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10780 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5772 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41269 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.287307 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15563 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.287307 localstack-core-2.1.1.dev20230714101424/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.287307 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4428 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5958 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24178 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.291307 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.295307 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    83531 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34301 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/provider_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68151 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15009 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15025 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43100 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54568 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.299307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.303307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.307307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.315307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.315307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.315307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.315307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.319307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.319307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.319307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.319307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.323307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3890 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.327307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.327307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.327307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10826 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4102 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5244 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7413 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3954 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4137 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.331307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.339307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.343307 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13659 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.347307 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69946 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.351307 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26930 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.351307 localstack-core-2.1.1.dev20230714101424/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17402 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7639 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23586 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    46654 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33137 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33236 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.355307 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 10:14:31.359307 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39252 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 10:14:27.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-14 10:14:27.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-14 10:14:31.000000 localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-14 10:14:31.359307 localstack-core-2.1.1.dev20230714101424/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-14 09:37:55.000000 localstack-core-2.1.1.dev20230714101424/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230714062049/LICENSE.txt` & `localstack-core-2.1.1.dev20230714101424/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/Makefile` & `localstack-core-2.1.1.dev20230714101424/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/PKG-INFO` & `localstack-core-2.1.1.dev20230714101424/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230714062049
+Version: 2.1.1.dev20230714101424
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230714062049/README.md` & `localstack-core-2.1.1.dev20230714101424/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/bin/localstack` & `localstack-core-2.1.1.dev20230714101424/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230714101424/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/forwarder.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     Request,
     RequestContext,
     ServiceRequest,
     ServiceRequestHandler,
     ServiceResponse,
 )
 from localstack.aws.client import parse_response, raise_service_exception
+from localstack.aws.connect import connect_to
 from localstack.aws.skeleton import DispatchTable, create_dispatch_table
 from localstack.aws.spec import load_service
 from localstack.http import Response
 from localstack.http.proxy import forward
-from localstack.utils.aws import aws_stack
 from localstack.utils.strings import to_str
 
 
 def ForwardingFallbackDispatcher(
     provider: object, request_forwarder: ServiceRequestHandler
 ) -> DispatchTable:
     """
@@ -156,15 +156,15 @@
 
     service = load_service(service_name)
     operation = service.operation_model(action)
 
     # we re-use botocore internals here to serialize the HTTP request,
     # but deactivate validation (validation errors should be handled by the backend)
     # and don't send it yet
-    client = aws_stack.connect_to_service(
+    client = connect_to.get_client(
         service_name,
         endpoint_url=endpoint_url,
         region_name=region,
         config=_non_validating_boto_config,
     )
     request_context = {
         "client_region": region,
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230714101424/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230714101424/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230714101424/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230714101424/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230714101424/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230714101424/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/config.py` & `localstack-core-2.1.1.dev20230714101424/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/constants.py` & `localstack-core-2.1.1.dev20230714101424/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230714101424/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230714101424/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/client.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/request.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/response.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/http/router.py` & `localstack-core-2.1.1.dev20230714101424/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230714101424/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230714101424/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230714101424/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230714101424/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230714101424/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230714101424/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230714101424/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230714101424/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/plugins.py` & `localstack-core-2.1.1.dev20230714101424/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230714101424/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230714101424/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230714101424/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230714101424/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230714101424/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     ConnectionType,
     DocumentationPart,
     DocumentationPartLocation,
     IntegrationType,
     Model,
     RequestValidator,
 )
+from localstack.aws.connect import connect_to
 from localstack.constants import (
     APPLICATION_JSON,
     HEADER_LOCALSTACK_EDGE_URL,
     LOCALHOST_HOSTNAME,
     PATH_USER_REQUEST,
 )
 from localstack.services.apigateway.context import ApiInvocationContext
@@ -524,15 +525,15 @@
     if is_test_invoke_method(context.method, context.path):
         return None
 
     if not context.stage:
         return {}
 
     _, region_name = get_api_account_id_and_region(context.api_id)
-    api_gateway_client = aws_stack.connect_to_service("apigateway", region_name=region_name)
+    api_gateway_client = connect_to(region_name=region_name).apigateway
     try:
         response = api_gateway_client.get_stage(restApiId=context.api_id, stageName=context.stage)
         return response.get("variables")
     except Exception:
         LOG.info("Failed to get stage %s for API id %s", context.stage, context.api_id)
         return {}
 
@@ -613,15 +614,15 @@
     response.headers["Access-Control-Allow-Methods"] = "GET, POST, PUT, DELETE, PATCH"
     response.headers["Access-Control-Allow-Headers"] = "*"
     response._content = ""
     return response
 
 
 def get_rest_api_paths(rest_api_id, region_name=None):
-    apigateway = aws_stack.connect_to_service(service_name="apigateway", region_name=region_name)
+    apigateway = connect_to(region_name=region_name).apigateway
     resources = apigateway.get_resources(restApiId=rest_api_id, limit=100)
     resource_map = {}
     for resource in resources["items"]:
         path = resource.get("path")
         # TODO: check if this is still required in the general case (can we rely on "path" being
         #  present?)
         path = path or queries.get_apigateway_path_for_resource(
@@ -1463,15 +1464,15 @@
                 responses = dict.fromkeys(integration_responses, {})
                 spec.path(path=path, operations={method: {"responses": responses}})
 
     def _swagger_export(self, api_id: str, stage: str, export_format: str) -> str:
         """
         https://github.com/OAI/OpenAPI-Specification/blob/main/versions/2.0.md
         """
-        apigateway_client = aws_stack.connect_to_service("apigateway")
+        apigateway_client = connect_to().apigateway
 
         rest_api = apigateway_client.get_rest_api(restApiId=api_id)
         resources = apigateway_client.get_resources(restApiId=api_id)
 
         spec = APISpec(
             title=rest_api.get("name"),
             version=timestamp(rest_api.get("createdDate"), format=TIMESTAMP_FORMAT_TZ),
@@ -1484,15 +1485,15 @@
 
         return getattr(spec, self.export_formats.get(export_format))()
 
     def _oas30_export(self, api_id: str, stage: str, export_format: str) -> str:
         """
         https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md
         """
-        apigateway_client = aws_stack.connect_to_service("apigateway")
+        apigateway_client = connect_to().apigateway
 
         rest_api = apigateway_client.get_rest_api(restApiId=api_id)
         resources = apigateway_client.get_resources(restApiId=api_id)
 
         spec = APISpec(
             title=rest_api.get("name"),
             version=timestamp(rest_api.get("createdDate"), format=TIMESTAMP_FORMAT_TZ),
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -569,15 +569,15 @@
     def invoke(self, invocation_context: ApiInvocationContext):
         invocation_path = invocation_context.path_with_query_string
         integration = invocation_context.integration
         path_params = invocation_context.path_params
         relative_path, query_string_params = extract_query_string_params(path=invocation_path)
         uri = integration.get("uri") or integration.get("integrationUri") or ""
 
-        s3 = aws_stack.connect_to_service("s3")
+        s3 = connect_to().s3
         uri = apply_request_parameters(
             uri,
             integration=integration,
             path_params=path_params,
             query_params=query_string_params,
         )
         uri_match = re.match(self.TARGET_REGEX_PATH_S3_URI, uri) or re.match(
@@ -615,15 +615,15 @@
         method = invocation_context.method
         headers = invocation_context.headers
         relative_path, query_string_params = extract_query_string_params(path=invocation_path)
         uri = integration.get("uri") or integration.get("integrationUri") or ""
 
         if ":servicediscovery:" in uri:
             # check if this is a servicediscovery integration URI
-            client = aws_stack.connect_to_service("servicediscovery")
+            client = connect_to().servicediscovery
             service_id = uri.split("/")[-1]
             instances = client.list_instances(ServiceId=service_id)["Instances"]
             instance = (instances or [None])[0]
             if instance and instance.get("Id"):
                 uri = "http://%s/%s" % (instance["Id"], invocation_path.lstrip("/"))
 
         # apply custom request template
@@ -748,15 +748,15 @@
             payload = self._create_request_parameters(invocation_context)
         elif APPLICATION_JSON in invocation_context.integration.get("requestTemplates", {}):
             payload = self.request_templates.render(invocation_context)
             payload = json.loads(payload)
         else:
             payload = json.loads(invocation_context.data)
 
-        client = aws_stack.connect_to_service("stepfunctions")
+        client = connect_to().stepfunctions
         if isinstance(payload.get("input"), dict):
             payload["input"] = json.dumps(payload["input"])
 
         # Hot fix since step functions local package responses: Unsupported Operation: 'StartSyncExecution'
         method_name = (
             camel_to_snake_case(action) if action != "StartSyncExecution" else "start_execution"
         )
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/invocations.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 def run_authorizer(invocation_context: ApiInvocationContext, authorizer: Dict):
     # TODO implement authorizers
     pass
 
 
 def authorize_invocation(invocation_context: ApiInvocationContext):
     region_name = invocation_context.region_name or aws_stack.get_region()
-    client = aws_stack.connect_to_service("apigateway", region_name=region_name)
+    client = connect_to(region_name=region_name).apigateway
     authorizers = client.get_authorizers(restApiId=invocation_context.api_id, limit=100).get(
         "items", []
     )
     for authorizer in authorizers:
         run_authorizer(invocation_context, authorizer)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from urllib.parse import urlparse
 
 from flask import Flask, Response, jsonify, request
 from flask_cors import CORS
 
 from localstack import config, constants
 from localstack.aws.accounts import get_aws_account_id
+from localstack.aws.connect import connect_to
 from localstack.constants import APPLICATION_JSON
 from localstack.http import Request
 from localstack.http import Response as HttpResponse
 from localstack.services.awslambda import lambda_executors
 from localstack.services.awslambda.event_source_listeners.event_source_listener import (
     EventSourceListener,
 )
@@ -428,15 +429,15 @@
     if context is None:
         context = {}
 
     # Ensure that the service provider has been initialized. This is required to ensure all lifecycle hooks
     # (e.g., persistence) have been executed when the run_lambda(..) function gets called (e.g., from API GW).
     LOG.debug("Running lambda %s", func_arn)
     if not hasattr(run_lambda, "_provider_initialized"):
-        aws_stack.connect_to_service("lambda").list_functions()
+        connect_to().awslambda.list_functions()
         run_lambda._provider_initialized = True
 
     store = get_awslambda_store_for_arn(func_arn)
     if suppress_output:
         stdout_ = sys.stdout
         stderr_ = sys.stderr
         stream = StringIO()
@@ -905,15 +906,15 @@
     Lambda to the configured URL."""
     if not config.LAMBDA_FALLBACK_URL:
         return
 
     lambda_name = arns.lambda_function_name(func_arn)
     if config.LAMBDA_FALLBACK_URL.startswith("dynamodb://"):
         table_name = urlparse(config.LAMBDA_FALLBACK_URL.replace("dynamodb://", "http://")).netloc
-        dynamodb = aws_stack.connect_to_service("dynamodb")
+        dynamodb = connect_to().dynamodb
         item = {
             "id": {"S": short_uid()},
             "timestamp": {"N": str(now_utc())},
             "payload": {"S": data},
             "function_name": {"S": lambda_name},
         }
         resources.create_dynamodb_table(table_name, partition_key="id")
@@ -934,15 +935,15 @@
             pass
 
         return content
     raise ClientError("Unexpected value for LAMBDA_FALLBACK_URL: %s" % config.LAMBDA_FALLBACK_URL)
 
 
 def get_lambda_policy(function, qualifier=None):
-    iam_client = aws_stack.connect_to_service("iam")
+    iam_client = connect_to().iam
     policies = iam_client.list_policies(Scope="Local", MaxItems=500)["Policies"]
     docs = []
     for p in policies:
         # !TODO: Cache policy documents instead of running N+1 API calls here!
         versions = iam_client.list_policy_versions(PolicyArn=p["Arn"])["Versions"]
         default_version = [v for v in versions if v.get("IsDefaultVersion")]
         versions = default_version or versions
@@ -1627,15 +1628,15 @@
 
 
 def add_permission_policy_statement(
     resource_name, resource_arn, resource_arn_qualified, qualifier=None
 ):
     store = get_awslambda_store_for_arn(resource_arn)
     data = json.loads(to_str(request.data))
-    iam_client = aws_stack.connect_to_service("iam")
+    iam_client = connect_to().iam
     sid = data.get("StatementId")
     action = data.get("Action")
     principal = data.get("Principal")
     sourcearn = data.get("SourceArn")
     function_url_auth_type = data.get("FunctionUrlAuthType")
     previous_policy = get_lambda_policy(resource_name, qualifier)
 
@@ -1686,15 +1687,15 @@
 
     return jsonify(result)
 
 
 @app.route("%s/functions/<function>/policy/<statement>" % API_PATH_ROOT, methods=["DELETE"])
 def remove_permission(function, statement):
     qualifier = request.args.get("Qualifier")
-    iam_client = aws_stack.connect_to_service("iam")
+    iam_client = connect_to().iam
     policy = get_lambda_policy(function, qualifier=qualifier)
     if not policy:
         return not_found_error('Unable to find policy for Lambda function "%s"' % function)
 
     statement_index = next(
         (i for i, item in enumerate(policy["Statement"]) if item["Sid"] == statement), None
     )
@@ -1838,15 +1839,15 @@
             os.path.join(
                 stepfunctions_local_package.get_installed_dir(),
                 "localstack-internal-awssdk",
                 "awssdk.zip",
             ),
             mode="rb",
         )
-        lambda_client = aws_stack.connect_to_service("lambda")
+        lambda_client = connect_to().awslambda
         lambda_client.create_function(
             FunctionName="localstack-internal-awssdk",
             Runtime=LAMBDA_RUNTIME_NODEJS14X,
             Handler="index.handler",
             Code={"ZipFile": code},
             Role=LAMBDA_TEST_ROLE.format(account_id=get_aws_account_id()),
             Timeout=30,
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_executors.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import time
 import traceback
 import uuid
 from multiprocessing import Process, Queue
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from localstack import config
+from localstack.aws.connect import connect_to
 from localstack.constants import DEFAULT_LAMBDA_CONTAINER_REGISTRY
 from localstack.runtime.hooks import hook_spec
 from localstack.services.awslambda.lambda_utils import (
     API_PATH_ROOT,
     LAMBDA_RUNTIME_PROVIDED,
     get_main_container_network_for_lambda,
     get_main_endpoint_from_container,
@@ -874,15 +875,15 @@
         self,
         lambda_function: LambdaFunction,
         inv_context: InvocationContext,
         lambda_docker_ip=None,
     ) -> InvocationResult:
         full_url = self._get_lambda_stay_open_url(lambda_docker_ip)
 
-        client = aws_stack.connect_to_service("lambda", endpoint_url=full_url)
+        client = connect_to(endpoint_url=full_url).awslambda
         event = inv_context.event or "{}"
 
         LOG.debug(f"Calling {full_url} to run invocation in docker-reuse Lambda container")
         response = client.invoke(
             FunctionName=lambda_function.name(),
             InvocationType=inv_context.invocation_type,
             Payload=to_bytes(event),
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_starter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 
 from moto.awslambda import models as moto_awslambda_models
 
 from localstack import config
+from localstack.aws.connect import connect_to
 from localstack.services.awslambda.lambda_api import handle_lambda_url_invocation
 from localstack.services.awslambda.lambda_utils import get_default_executor_mode
 from localstack.services.edge import ROUTER
 from localstack.services.plugins import ServiceLifecycleHook
 from localstack.utils.analytics import log
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.aws.request_context import AWS_REGION_REGEX
 from localstack.utils.patch import patch
 from localstack.utils.platform import is_linux
 from localstack.utils.strings import to_bytes
 
 LOG = logging.getLogger(__name__)
 
@@ -73,26 +74,23 @@
     cleanup()
 
 
 def check_lambda(expect_shutdown=False, print_error=False):
     out = None
     try:
         from localstack.services.infra import PROXY_LISTENERS
-        from localstack.utils.aws import aws_stack
         from localstack.utils.common import wait_for_port_open
 
         # wait for port to be opened
         # TODO get lambda port in a cleaner way
         port = PROXY_LISTENERS.get("lambda")[1]
         wait_for_port_open(port, sleep_time=0.5, retries=20)
 
         endpoint_url = f"http://127.0.0.1:{port}"
-        out = aws_stack.connect_to_service(
-            service_name="lambda", endpoint_url=endpoint_url
-        ).list_functions()
+        out = connect_to(endpoint_url=endpoint_url).awslambda.list_functions()
     except Exception:
         if print_error:
             LOG.exception("Lambda health check failed")
     if expect_shutdown:
         assert out is None
     else:
         assert out and isinstance(out.get("Functions"), list)
@@ -100,24 +98,24 @@
 
 @patch(moto_awslambda_models.LambdaBackend.get_function)
 def get_function(fn, self, *args, **kwargs):
     result = fn(self, *args, **kwargs)
     if result:
         return result
 
-    client = aws_stack.connect_to_service("lambda")
+    client = connect_to().awslambda
     lambda_name = arns.lambda_function_name(args[0])
     response = client.get_function(FunctionName=lambda_name)
 
     spec = response["Configuration"]
     spec["Code"] = {"ZipFile": "ZW1wdHkgc3RyaW5n"}
     region = arns.extract_region_from_arn(spec["FunctionArn"])
     new_function = moto_awslambda_models.LambdaFunction(spec, region)
 
     return new_function
 
 
 @patch(moto_awslambda_models.LambdaFunction.invoke)
 def invoke(fn, self, *args, **kwargs):
     payload = to_bytes(args[0])
-    client = aws_stack.connect_to_service("lambda")
+    client = connect_to().awslambda
     return client.invoke(FunctionName=self.function_name, Payload=payload)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/api_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import re
 from urllib.parse import urlparse
 
 from requests.structures import CaseInsensitiveDict
 
 from localstack import config, constants
+from localstack.aws.connect import connect_to
 from localstack.services.s3 import s3_listener, s3_utils
-from localstack.utils.aws import aws_stack
 from localstack.utils.functions import run_safe
 from localstack.utils.http import safe_requests
 from localstack.utils.strings import to_str
 
 LOG = logging.getLogger(__name__)
 
 
@@ -41,15 +41,15 @@
         status_code = 0 if response is None else response.status_code
         if response is None or status_code == 301 or status_code >= 400:
             # check if this is an S3 URL, then get the file directly from there
             url = convert_s3_to_local_url(url)
             if is_local_service_url(url):
                 parsed_path = urlparse(url).path.lstrip("/")
                 parts = parsed_path.partition("/")
-                client = aws_stack.connect_to_service("s3")
+                client = connect_to().s3
                 LOG.debug(
                     "Download CloudFormation template content from local S3: %s - %s",
                     parts[0],
                     parts[2],
                 )
                 result = client.get_object(Bucket=parts[0], Key=parts[2])
                 body = to_str(result["Body"].read())
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import uuid
 from typing import Any, Callable, Literal, Optional, Type, TypedDict
 
 import botocore
 
 from localstack import config
 from localstack.aws.accounts import get_aws_account_id
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation import usage
 from localstack.services.cloudformation.deployment_utils import (
     PLACEHOLDER_AWS_NO_VALUE,
     dump_resource_as_json,
     fix_boto_parameters_based_on_report,
     get_action_name_for_resource_change,
     log_not_available_message,
@@ -336,18 +337,18 @@
         dynamic_ref_match = REGEX_DYNAMIC_REF.match(result)
         if dynamic_ref_match:
             service_name = dynamic_ref_match[1]
             reference_key = dynamic_ref_match[2]
 
             # only these 3 services are supported for dynamic references right now
             if service_name == "ssm":
-                ssm_client = aws_stack.connect_to_service("ssm")
+                ssm_client = connect_to().ssm
                 return ssm_client.get_parameter(Name=reference_key)["Parameter"]["Value"]
             elif service_name == "ssm-secure":
-                ssm_client = aws_stack.connect_to_service("ssm")
+                ssm_client = connect_to().ssm
                 return ssm_client.get_parameter(Name=reference_key, WithDecryption=True)[
                     "Parameter"
                 ]["Value"]
             elif service_name == "secretsmanager":
                 # reference key needs to be parsed further
                 # because {{resolve:secretsmanager:secret-id:secret-string:json-key:version-stage:version-id}}
                 # we match for "secret-id:secret-string:json-key:version-stage:version-id"
@@ -365,15 +366,15 @@
 
                 kwargs = {}  # optional args for get_secret_value
                 if version_id:
                     kwargs["VersionId"] = version_id
                 if version_stage:
                     kwargs["VersionStage"] = version_stage
 
-                secretsmanager_client = aws_stack.connect_to_service("secretsmanager")
+                secretsmanager_client = connect_to().secretsmanager
                 secret_value = secretsmanager_client.get_secret_value(SecretId=secret_id, **kwargs)[
                     "SecretString"
                 ]
                 if json_key:
                     json_secret = json.loads(secret_value)
                     if json_key not in json_secret:
                         raise DependencyNotYetSatisfied(
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 
 import boto3
 from samtranslator.translator.transform import transform as transform_sam
 
 from localstack.aws.accounts import get_aws_account_id
 from localstack.aws.api import CommonServiceException
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.engine import yaml_parser
 from localstack.services.cloudformation.engine.policy_loader import create_policy_loader
 from localstack.services.cloudformation.engine.transformers import (
     apply_transform_intrinsic_functions,
 )
 from localstack.services.cloudformation.stores import get_cloudformation_store
 from localstack.utils.aws import aws_stack
@@ -107,15 +108,15 @@
         "fragment": parsed_template,
         "transformId": transformation_id,
         "params": formatted_transform_parameters,
         "requestId": long_uid(),
         "templateParameterValues": formatted_stack_parameters,
     }
 
-    client = aws_stack.connect_to_service("lambda")
+    client = connect_to().awslambda
     invocation = client.invoke(
         FunctionName=macro_definition["FunctionName"], Payload=json.dumps(event)
     )
     if invocation.get("StatusCode") != 200 or invocation.get("FunctionError") == "Unhandled":
         raise FailedTransformationException(
             transformation=macro["Name"],
             message=f"Received malformed response from transform {transformation_id}. Rollback requested by user.",
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/types.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/awslambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from localstack.services.awslambda.lambda_utils import get_handler_file_from_name
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     select_parameters,
 )
 from localstack.services.cloudformation.packages import cloudformation_package
 from localstack.services.cloudformation.service_models import LOG, GenericBaseModel
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.common import (
     cp_r,
     is_base64,
     is_zip_file,
     mkdir,
     new_tmp_dir,
     rm_rf,
@@ -35,15 +35,15 @@
 
     def fetch_state(self, stack_name, resources):
         func_name = self.props["FunctionName"]
         return connect_to().awslambda.get_function(FunctionName=func_name)
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
-        client = aws_stack.connect_to_service("lambda")
+        client = connect_to().awslambda
         config_keys = [
             "Description",
             "Environment",
             "FunctionName",
             "Handler",
             "ImageConfig",
             "Layers",
@@ -233,15 +233,15 @@
 
         def _matches(m):
             return m["FunctionArn"] == lambda_arn and (
                 m.get("EventSourceArn") == source_arn
                 or m.get("SelfManagedEventSource") == self_managed_src
             )
 
-        client = aws_stack.connect_to_service("lambda")
+        client = connect_to().awslambda
         lambda_arn = client.get_function(FunctionName=function_name)["Configuration"]["FunctionArn"]
         kwargs = {"EventSourceArn": source_arn} if source_arn else {}
         mappings = client.list_event_source_mappings(FunctionName=function_name, **kwargs)
         mapping = list(filter(lambda m: _matches(m), mappings["EventSourceMappings"]))
         if not mapping:
             raise Exception("ResourceNotFound")
         return mapping[0]
@@ -268,15 +268,15 @@
 
     def fetch_state(self, stack_name, resources):
         if not self.physical_resource_id:
             return None
 
         props = self.props
         func_name = props.get("FunctionName")
-        lambda_client = aws_stack.connect_to_service("lambda")
+        lambda_client = connect_to().awslambda
         policy = lambda_client.get_policy(FunctionName=func_name)
         if not policy:
             return None
 
         loaded_policy = json.loads(policy["Policy"])
         statements = loaded_policy.get("Statement", [])
         matched_statements = [s for s in statements if s["Sid"] == self.physical_resource_id]
@@ -286,15 +286,15 @@
         return statements[0]
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
         parameters_to_select = ["FunctionName", "Action", "Principal", "SourceArn"]
         update_config_props = select_attributes(props, parameters_to_select)
 
-        client = aws_stack.connect_to_service("lambda")
+        client = connect_to().awslambda
         client.remove_permission(
             FunctionName=update_config_props["FunctionName"], StatementId=self.physical_resource_id
         )
         return client.add_permission(StatementId=self.physical_resource_id, **update_config_props)
 
     @staticmethod
     def get_deploy_templates():
@@ -337,15 +337,15 @@
 
 class LambdaEventInvokeConfig(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Lambda::EventInvokeConfig"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("lambda")
+        client = connect_to().awslambda
         props = self.props
         result = client.get_function_event_invoke_config(
             FunctionName=props.get("FunctionName"),
             Qualifier=props.get("FunctionName", "$LATEST"),
         )
         return result
 
@@ -374,15 +374,15 @@
 
 class LambdaUrl(GenericBaseModel):
     @classmethod
     def cloudformation_type(cls):
         return "AWS::Lambda::Url"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("lambda")
+        client = connect_to().awslambda
 
         kwargs = {"FunctionName": self.props.get("TargetFunctionArn")}
         qualifier = self.props.get("Qualifier")
         if qualifier:
             kwargs["Qualifier"] = qualifier
 
         return client.get_function_url_config(**kwargs)
@@ -424,15 +424,15 @@
 
 class LambdaAlias(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Lambda::Alias"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("lambda")
+        client = connect_to().awslambda
         props = self.props
         result = client.get_alias(FunctionName=props.get("FunctionName"), Name=props.get("Name"))
         return result
 
     @staticmethod
     def get_deploy_templates():
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
@@ -455,15 +455,15 @@
     def cloudformation_type():
         return "AWS::Lambda::CodeSigningConfig"
 
     def fetch_state(self, stack_name, resources):
         if not self.physical_resource_id:
             return None
 
-        client = aws_stack.connect_to_service("lambda")
+        client = connect_to().awslambda
         result = client.get_code_signing_config(CodeSigningConfigArn=self.physical_resource_id)[
             "CodeSigningConfig"
         ]
         return result
 
     @classmethod
     def get_deploy_templates(cls):
@@ -489,15 +489,15 @@
     @staticmethod
     def cloudformation_type():
         return "AWS::Lambda::LayerVersion"
 
     def fetch_state(self, stack_name, resources):
         layer_name = self.props.get("LayerName")
         # TODO extract region name if layer_name is an ARN
-        client = aws_stack.connect_to_service("lambda")
+        client = connect_to().awslambda
         layers = client.list_layer_versions(LayerName=layer_name).get("LayerVersions", [])
         return layers[-1] if layers else None
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         resource["Properties"]["LayerName"] = (
             resource["Properties"].get("LayerName") or f"layer-{short_uid()}"
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 from localstack.utils.common import select_attributes
 
 
 class CertificateManagerCertificate(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::CertificateManager::Certificate"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("acm")
+        client = connect_to().acm
         result = client.list_certificates().get("CertificateSummaryList", [])
         domain_name = self.props.get("DomainName")
         result = [c for c in result if c["DomainName"] == domain_name]
         return (result or [None])[0]
 
     @classmethod
     def get_deploy_templates(cls):
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cloudformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 import uuid
 
 from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import generate_default_name
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.services.cloudformation.stores import get_cloudformation_store
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 
 LOG = logging.getLogger(__name__)
 
 
 class CloudFormationStack(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::CloudFormation::Stack"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("cloudformation")
+        client = connect_to().cloudformation
         child_stack_name = self.props["StackName"]
         result = client.describe_stacks(StackName=child_stack_name)
         result = (result.get("Stacks") or [None])[0]
         return result
 
     def get_cfn_attribute(self, attribute_name: str):
         if attribute_name.startswith("Outputs."):
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import generate_default_name
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 
 
 class CloudWatchAlarm(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::CloudWatch::Alarm"
 
@@ -17,15 +17,15 @@
         return "MetricAlarms"
 
     @classmethod
     def _create_function_name(self):
         return "put_metric_alarm"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("cloudwatch")
+        client = connect_to().cloudwatch
         alarm_name = self.props["AlarmName"]
         result = client.describe_alarms(AlarmNames=[alarm_name]).get(self._response_name(), [])
         return (result or [None])[0]
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         role_name = resource.get("Properties", {}).get("AlarmName")
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import (
     PLACEHOLDER_AWS_NO_VALUE,
     generate_default_name,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils import common
-from localstack.utils.aws import aws_stack
 
 
 def get_ddb_provisioned_throughput(
     properties: dict, logical_resource_id: str, resource: dict, stack_name: str
 ) -> dict | None:
     # see https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-dynamodb-table.html#cfn-dynamodb-table-provisionedthroughput
     args = properties.get("ProvisionedThroughput")
@@ -84,15 +84,15 @@
         if value:
             return value
 
         return super(DynamoDBTable, self).get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         table_name = self.props.get("TableName") or self.logical_resource_id
-        return aws_stack.connect_to_service("dynamodb").describe_table(TableName=table_name)
+        return connect_to().dynamodb.describe_table(TableName=table_name)
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         table_name = resource.get("Properties", {}).get("TableName")
         resource["Properties"]["TableName"] = table_name or generate_default_name(
             stack_name, resource["LogicalResourceId"]
         )
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ec2.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class EC2RouteTable(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::RouteTable"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         if not self.physical_resource_id:
             return None
         result = client.describe_route_tables(RouteTableIds=[self.physical_resource_id])
         return (result["RouteTables"] or [None])[0]
 
     @staticmethod
     def get_deploy_templates():
@@ -45,15 +45,15 @@
 
 class EC2Route(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::Route"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         props = self.props
         dst_cidr = props.get("DestinationCidrBlock")
         dst_cidr6 = props.get("DestinationIpv6CidrBlock")
         table_id = props.get("RouteTableId")
         route_tables = client.describe_route_tables()["RouteTables"]
         route_table = ([t for t in route_tables if t["RouteTableId"] == table_id] or [None])[0]
         if route_table:
@@ -94,15 +94,15 @@
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::InternetGateway"
 
     def fetch_state(self, stack_name, resources):
         if not self.physical_resource_id:
             return None
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         gateways = client.describe_internet_gateways(
             InternetGatewayIds=[self.physical_resource_id]
         )["InternetGateways"]
         return gateways[0] if gateways else None
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "InternetGatewayId":
@@ -128,15 +128,15 @@
 
 class EC2SubnetRouteTableAssociation(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::SubnetRouteTableAssociation"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         props = self.props
         table_id = props.get("RouteTableId")
         gw_id = props.get("GatewayId")
         route_tables = client.describe_route_tables()["RouteTables"]
         route_table = ([t for t in route_tables if t["RouteTableId"] == table_id] or [None])[0]
         subnet_id = props.get("SubnetId")
         if route_table:
@@ -170,15 +170,15 @@
 
 class EC2VPCGatewayAttachment(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::VPCGatewayAttachment"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         props = self.props
         igw_id = props.get("InternetGatewayId")
         vpngw_id = props.get("VpnGatewayId")
         gateways = []
         if igw_id:
             gateways = client.describe_internet_gateways()["InternetGateways"]
             gateways = [g for g in gateways if g["InternetGatewayId"] == igw_id]
@@ -190,15 +190,15 @@
         result = [a for a in attachments if a.get("State") in ("attached", "available")]
         if result:
             return gateway
 
     @classmethod
     def get_deploy_templates(cls):
         def _attach_gateway(logical_resource_id: str, resource: dict, stack_name: str):
-            client = aws_stack.connect_to_service("ec2")
+            client = connect_to().ec2
             resource_provider = cls(resource)
             props = resource_provider.props
             igw_id = props.get("InternetGatewayId")
             vpngw_id = props.get("VpnGatewayId")
             vpc_id = props.get("VpcId")
             if igw_id:
                 return client.attach_internet_gateway(VpcId=vpc_id, InternetGatewayId=igw_id)
@@ -271,15 +271,15 @@
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::Subnet"
 
     def fetch_state(self, stack_name, resources) -> dict:
         if not self.physical_resource_id:
             return None
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         props = self.props
         filters = [
             {"Name": "cidr-block", "Values": [props["CidrBlock"]]},
             {"Name": "vpc-id", "Values": [props["VpcId"]]},
         ]
         subnets = client.describe_subnets(Filters=filters)["Subnets"]
         return (subnets or [None])[0]
@@ -288,15 +288,15 @@
         if attribute_name == "SubnetId":
             return self.props.get("SubnetId")
         return super(EC2Subnet, self).get_cfn_attribute(attribute_name)
 
     @classmethod
     def get_deploy_templates(cls):
         def _post_create(logical_resource_id: str, resource: dict, stack_name: str):
-            client = aws_stack.connect_to_service("ec2")
+            client = connect_to().ec2
             resource_provider = cls(resource)
             props = resource_provider.props
 
             bool_attrs = [
                 "AssignIpv6AddressOnCreation",
                 "EnableDns64",
                 "MapPublicIpOnLaunch",
@@ -356,22 +356,22 @@
 class EC2VPC(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::VPC"
 
     def fetch_state(self, stack_name, resources):
         if self.physical_resource_id:
-            client = aws_stack.connect_to_service("ec2")
+            client = connect_to().ec2
             resp = client.describe_vpcs(
                 Filters=[{"Name": "vpc-id", "Values": [self.physical_resource_id]}]
             )
             return (resp["Vpcs"] or [None])[0]
 
     def get_cfn_attribute(self, attribute_name):
-        ec2_client = aws_stack.connect_to_service("ec2")
+        ec2_client = connect_to().ec2
         vpc_id = self.props["VpcId"]
 
         if attribute_name == "DefaultSecurityGroup":
             sgs = ec2_client.describe_security_groups(
                 Filters=[
                     {"Name": "group-name", "Values": ["default"]},
                     {"Name": "vpc-id", "Values": [vpc_id]},
@@ -397,15 +397,15 @@
 
     @classmethod
     def get_deploy_templates(cls):
         def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
             res = cls(resource)
             vpc_id = res.state.get("VpcId")
             if vpc_id:
-                ec2_client = aws_stack.connect_to_service("ec2")
+                ec2_client = connect_to().ec2
                 resp = ec2_client.describe_route_tables(
                     Filters=[
                         {"Name": "vpc-id", "Values": [vpc_id]},
                         {"Name": "association.main", "Values": ["false"]},
                     ]
                 )
                 for rt in resp["RouteTables"]:
@@ -444,15 +444,15 @@
 
 class EC2NatGateway(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::NatGateway"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         props = self.props
         subnet_id = props.get("SubnetId")
         assoc_id = props.get("AllocationId")
         result = client.describe_nat_gateways(
             Filters=[{"Name": "subnet-id", "Values": [subnet_id]}]
         )
         result = result["NatGateways"]
@@ -497,28 +497,28 @@
         return self._get_state()
 
     def update_resource(self, new_resource, stack_name, resources):
         instance_id = self.physical_resource_id
         props = new_resource["Properties"]
         groups = props.get("SecurityGroups", props.get("SecurityGroupIds"))
 
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         kwargs = {}
         if groups:
             kwargs["Groups"] = groups
         client.modify_instance_attribute(
             InstanceId=instance_id,
             InstanceType={"Value": props["InstanceType"]},
             **kwargs,
         )
         return self._get_state(client)
 
     def _get_state(self, client=None):
         instance_id = self.physical_resource_id
-        client = client or aws_stack.connect_to_service("ec2")
+        client = client or connect_to().ec2
         resp = client.describe_instances(InstanceIds=[instance_id])
         reservation = (resp.get("Reservations") or [{}])[0]
         result = (reservation.get("Instances") or [None])[0]
         return result
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from localstack.aws.api.es import CreateElasticsearchDomainRequest
 from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import remove_none_values
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.collections import convert_to_typed_dict
 
 
 def es_add_tags_params(properties: dict, logical_resource_id: str, resource: dict, stack_name: str):
     es_arn = arns.es_domain_arn(properties.get("DomainName"))
     tags = properties.get("Tags", [])
     return {"ARN": es_arn, "TagList": tags}
@@ -26,17 +26,15 @@
             result = domain_status.get("Endpoint")
             if result:
                 return result
         return super(ElasticsearchDomain, self).get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         domain_name = self._domain_name()
-        return aws_stack.connect_to_service("es").describe_elasticsearch_domain(
-            DomainName=domain_name
-        )
+        return connect_to().es.describe_elasticsearch_domain(DomainName=domain_name)
 
     def _domain_name(self):
         return self.props.get("DomainName") or self.logical_resource_id
 
     @staticmethod
     def get_deploy_templates():
         def _create_params(
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import json
 
 from botocore.exceptions import ClientError
 
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     select_parameters,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils import common
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.common import short_uid
 
 
 class EventConnection(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Events::Connection"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("events")
+        client = connect_to().events
         conn_name = self.props.get("Name")
         return client.describe_connection(Name=conn_name)
 
     def get_cfn_attribute(self, attribute_name):
         props = self.props
         if attribute_name == "Name":
             return props.get("Name")
@@ -45,15 +46,15 @@
 class EventBus(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Events::EventBus"
 
     def fetch_state(self, stack_name, resources):
         event_bus_name = self.props.get("Name")
-        client = aws_stack.connect_to_service("events")
+        client = connect_to().events
         return client.describe_event_bus(Name=event_bus_name)
 
     def get_cfn_attribute(self, attribute_name):
         props = self.props
         if attribute_name == "Name":
             return props.get("Name")
         if attribute_name == "Arn":
@@ -89,15 +90,15 @@
     def fetch_state(self, stack_name, resources):
         rule_name = self.props.get("Name")
 
         kwargs = {"Name": rule_name}
         if bus_name := self.props.get("EventBusName"):
             kwargs["EventBusName"] = bus_name
 
-        result = aws_stack.connect_to_service("events").describe_rule(**kwargs) or {}
+        result = connect_to().events.describe_rule(**kwargs) or {}
         return result if result.get("Name") else None
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         role_name = resource.get("Properties", {}).get("Name")
         if not role_name:
             resource["Properties"]["Name"] = generate_default_name(
@@ -136,25 +137,25 @@
             pattern = result.get("EventPattern")
             if isinstance(pattern, dict):
                 wrapped = common.recurse_object(pattern, wrap_in_lists)
                 result["EventPattern"] = json.dumps(wrapped)
             return result
 
         def _delete_rule(logical_resource_id: str, resource: dict, stack_name: str):
-            events = aws_stack.connect_to_service("events")
+            events = connect_to().events
             props = resource["Properties"]
             rule_name = props["Name"]
             targets = events.list_targets_by_rule(Rule=rule_name)["Targets"]
             target_ids = [tgt["Id"] for tgt in targets]
             if targets:
                 events.remove_targets(Rule=rule_name, Ids=target_ids, Force=True)
             events.delete_rule(Name=rule_name)
 
         def _put_targets(logical_resource_id: str, resource: dict, stack_name: str):
-            events = aws_stack.connect_to_service("events")
+            events = connect_to().events
             props = resource["Properties"]
             rule_name = props["Name"]
             event_bus_name = props.get("EventBusName")
             targets = props.get("Targets") or []
             if len(targets) > 0 and event_bus_name:
                 events.put_targets(Rule=rule_name, EventBusName=event_bus_name, Targets=targets)
             elif len(targets) > 0:
@@ -182,15 +183,15 @@
     @classmethod
     def cloudformation_type(cls):
         return "AWS::Events::EventBusPolicy"
 
     @classmethod
     def get_deploy_templates(cls):
         def _create(logical_resource_id: str, resource: dict, stack_name: str):
-            events = aws_stack.connect_to_service("events")
+            events = connect_to().events
             props = resource["Properties"]
 
             resource["PhysicalResourceId"] = f"EventBusPolicy-{short_uid()}"
 
             statement_id = props["StatementId"]  # required
             event_bus_name = props.get("EventBusName")  # optional
             statement = props.get(
@@ -218,15 +219,15 @@
                     Action=props["Action"],
                     Principal=props["Principal"],
                     **optional_event_bus_name,
                     **optional_condition,
                 )
 
         def _delete(logical_resource_id: str, resource: dict, stack_name: str):
-            events = aws_stack.connect_to_service("events")
+            events = connect_to().events
             props = resource["Properties"]
             statement_id = props["StatementId"]
             event_bus_name = props.get("EventBusName")
             optional_event_bus_name = {"EventBusName": event_bus_name} if event_bus_name else {}
             try:
                 events.remove_permission(
                     StatementId=statement_id, RemoveAllPermissions=False, **optional_event_bus_name
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/iam.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     generate_default_name,
     param_defaults,
     remove_none_values,
     select_parameters,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.services.iam.provider import SERVICE_LINKED_ROLE_PATH_PREFIX
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.common import ensure_list
 from localstack.utils.functions import call_safe
 
 LOG = logging.getLogger(__name__)
 
 
 class IAMManagedPolicy(GenericBaseModel):
@@ -39,15 +39,15 @@
             resource["Properties"]["ManagedPolicyName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
         def _create(logical_resource_id: str, resource: dict, stack_name: str):
-            iam = aws_stack.connect_to_service("iam")
+            iam = connect_to().iam
             props = resource["Properties"]
 
             policy_doc = json.dumps(remove_none_values(props["PolicyDocument"]))
             policy = iam.create_policy(
                 PolicyName=props["ManagedPolicyName"], PolicyDocument=policy_doc
             )
             policy_arn = policy["Policy"]["Arn"]
@@ -68,28 +68,28 @@
 class IAMUser(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::IAM::User"
 
     def fetch_state(self, stack_name, resources):
         user_name = self.props.get("UserName")
-        return aws_stack.connect_to_service("iam").get_user(UserName=user_name)["User"]
+        return connect_to().iam.get_user(UserName=user_name)["User"]
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         role_name = resource["Properties"].get("UserName")
         if not role_name:
             resource["Properties"]["UserName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
         def _post_create(logical_resource_id: str, resource: dict, stack_name: str):
-            client = aws_stack.connect_to_service("iam")
+            client = connect_to().iam
             props = resource["Properties"]
             username = props["UserName"]
 
             for group in props.get("Groups", []):
                 client.add_user_to_group(UserName=username, GroupName=group)
             for managed_policy in props.get("ManagedPolicyArns", []):
                 client.attach_user_policy(UserName=username, PolicyArn=managed_policy)
@@ -105,15 +105,15 @@
                 client.create_login_profile(
                     UserName=username,
                     Password=login_profile.get("Password"),
                     PasswordResetRequired=login_profile.get("PasswordResetRequired"),
                 )
 
         def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
-            client = aws_stack.connect_to_service("iam")
+            client = connect_to().iam
             props = resource["Properties"]
             user_name = props["UserName"]
 
             for managed_policy in props.get("ManagedPolicyArns", []):
                 client.detach_user_policy(UserName=user_name, PolicyArn=managed_policy)
 
             for inline_policy in props.get("Policies", []):
@@ -163,33 +163,31 @@
         if attribute_name == "SecretAccessKey":
             return self.props.get("SecretAccessKey")
 
     def fetch_state(self, stack_name, resources):
         user_name = self.props.get("UserName")
         access_key_id = self.physical_resource_id
         if access_key_id:
-            keys = aws_stack.connect_to_service("iam").list_access_keys(UserName=user_name)[
-                "AccessKeyMetadata"
-            ]
+            keys = connect_to().iam.list_access_keys(UserName=user_name)["AccessKeyMetadata"]
             return [key for key in keys if key["AccessKeyId"] == access_key_id][0]
 
     def update_resource(self, new_resource, stack_name, resources):
         access_key_id = self.physical_resource_id
         new_props = new_resource["Properties"]
         user_name = new_props.get("UserName")
         status = new_props.get("Status")
 
-        aws_stack.connect_to_service("iam").update_access_key(
+        connect_to().iam.update_access_key(
             UserName=user_name, AccessKeyId=access_key_id, Status=status
         )
 
     @staticmethod
     def get_deploy_templates():
         def _delete(logical_resource_id: str, resource: dict, stack_name: str):
-            iam_client = aws_stack.connect_to_service("iam")
+            iam_client = connect_to().iam
             props = resource["Properties"]
             user_name = props["UserName"]
             access_key_id = resource["PhysicalResourceId"]
 
             try:
                 iam_client.delete_access_key(UserName=user_name, AccessKeyId=access_key_id)
             except ClientError as err:
@@ -199,15 +197,15 @@
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
             access_key_id = result["AccessKey"]["AccessKeyId"]
             resource["PhysicalResourceId"] = access_key_id
             resource["Properties"]["SecretAccessKey"] = result["AccessKey"]["SecretAccessKey"]
             status = resource["Properties"].get("Status", "Active")
             if status == "Inactive":
                 user_name = resource["Properties"]["UserName"]
-                client = aws_stack.connect_to_service("iam")
+                client = connect_to().iam
                 client.update_access_key(
                     UserName=user_name, AccessKeyId=access_key_id, Status="Inactive"
                 )
 
         return {
             "create": {
                 "function": "create_access_key",
@@ -233,15 +231,15 @@
         client = connect_to().iam
         return client.get_role(RoleName=role_name)["Role"]
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
         # _states contains the old state of the resource
         _states = new_resource.get("_state_", None)
-        client = aws_stack.connect_to_service("iam")
+        client = connect_to().iam
         if _states:
             props_policy = props.get("AssumeRolePolicyDocument")
             name_changed = props.get("RoleName") != _states.get("RoleName")
             policy_changed = props_policy and props_policy != _states.get(
                 "AssumeRolePolicyDocument", ""
             )
             if name_changed or policy_changed:
@@ -269,15 +267,15 @@
             )
 
     @classmethod
     def _post_create(cls, logical_resource_id: str, resource: dict, stack_name: str):
         """attaches managed policies from the template to the role"""
 
         properties = resource["Properties"]
-        iam = aws_stack.connect_to_service("iam")
+        iam = connect_to().iam
         role_name = properties["RoleName"]
 
         # attach managed policies
         policy_arns = properties.get("ManagedPolicyArns", [])
         for arn in policy_arns:
             iam.attach_role_policy(RoleName=role_name, PolicyArn=arn)
 
@@ -314,15 +312,15 @@
                 PolicyName=pol_name,
                 PolicyDocument=doc,
             )
 
     @staticmethod
     def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
         """detach managed policies from role before deleting"""
-        iam_client = aws_stack.connect_to_service("iam")
+        iam_client = connect_to().iam
         props = resource["Properties"]
         role_name = props["RoleName"]
 
         try:
             # TODO: this should probably only remove the policies that are specified in the stack (verify with AWS)
             # detach managed policies
             for policy in iam_client.list_attached_role_policies(RoleName=role_name).get(
@@ -392,15 +390,15 @@
 
 class IAMServiceLinkedRole(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::IAM::ServiceLinkedRole"
 
     def fetch_state(self, stack_name, resources):
-        iam = aws_stack.connect_to_service("iam")
+        iam = connect_to().iam
         service_name = self.props["AWSServiceName"]
         path = f"{SERVICE_LINKED_ROLE_PATH_PREFIX}/{service_name}"
         roles = iam.list_roles(PathPrefix=path)["Roles"]
         for role in roles:
             policy = role.get("AssumeRolePolicyDocument") or "{}"
             policy = json.loads(policy or "{}") if isinstance(policy, str) else policy
             statements = policy.get("Statement")
@@ -423,15 +421,15 @@
 
 class IAMPolicy(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::IAM::Policy"
 
     def update_resource(self, new_resource, stack_name, resources):
-        client = aws_stack.connect_to_service("iam")
+        client = connect_to().iam
         props = new_resource["Properties"]
         _states = new_resource.get("_state_")
         if _states:
             policy_doc = json.dumps(remove_none_values(props["PolicyDocument"]))
             policy_name = props["PolicyName"]
             for role in props.get("Roles", []):
                 client.put_role_policy(
@@ -454,15 +452,15 @@
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
             # the physical resource ID here has a bit of a weird format
             # e.g. 'stack-fnSe-1OKWZIBB89193' where fnSe are the first 4 characters of the LogicalResourceId (or name?)
             suffix = "".join(random.choices(string.ascii_uppercase + string.digits, k=13))
             resource["PhysicalResourceId"] = f"stack-{resource.get('PolicyName', '')[:4]}-{suffix}"
 
         def _create(logical_resource_id: str, resource: dict, stack_name: str):
-            iam = aws_stack.connect_to_service("iam")
+            iam = connect_to().iam
             props = resource["Properties"]
             policy_doc = json.dumps(remove_none_values(props["PolicyDocument"]))
             policy_name = props["PolicyName"]
             for role in props.get("Roles", []):
                 iam.put_role_policy(
                     RoleName=role, PolicyName=policy_name, PolicyDocument=policy_doc
                 )
@@ -489,15 +487,15 @@
         }
 
     @classmethod
     def get_policy_state(cls, obj, stack_name, resources, managed_policy=False):
         def _filter(pols):
             return [p for p in pols["AttachedPolicies"] if p["PolicyName"] == policy_name]
 
-        iam = aws_stack.connect_to_service("iam")
+        iam = connect_to().iam
         props = obj.props
         result = {}
         # Note: util function reused for both IAM::Policy and IAM::ManagedPolicy
         policy_name = props.get("PolicyName") or props.get("ManagedPolicyName")
         roles = props.get("Roles", [])
         users = props.get("Users", [])
         groups = props.get("Groups", [])
@@ -533,42 +531,42 @@
     def cloudformation_type():
         return "AWS::IAM::InstanceProfile"
 
     def fetch_state(self, stack_name, resources):
         instance_profile_name = self.physical_resource_id
         if not instance_profile_name:
             return None
-        client = aws_stack.connect_to_service("iam")
+        client = connect_to().iam
         resp = client.get_instance_profile(InstanceProfileName=instance_profile_name)
         return resp["InstanceProfile"]
 
     @staticmethod
     def add_defaults(resource, stack_name):
         role_name = resource.get("Properties", {}).get("InstanceProfileName")
         if not role_name:
             resource["Properties"]["InstanceProfileName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
         def _add_roles(logical_resource_id: str, resource: dict, stack_name: str):
-            client = aws_stack.connect_to_service("iam")
+            client = connect_to().iam
             props = resource["Properties"]
             roles = props.get("Roles")
             if roles:
                 if len(roles) > 1:
                     raise Exception("Roles has too many elements. The limit is 1.")
                 client.add_role_to_instance_profile(
                     InstanceProfileName=props["InstanceProfileName"],
                     RoleName=roles[0],
                 )
 
         def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
-            iam_client = aws_stack.connect_to_service("iam")
+            iam_client = connect_to().iam
             props = resource["Properties"]
             roles = props.get("Roles")
             assert len(roles) == 1
             try:
                 iam_client.remove_role_from_instance_profile(
                     InstanceProfileName=props["InstanceProfileName"],
                     RoleName=roles[0],
@@ -605,28 +603,28 @@
 class IAMGroup(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::IAM::Group"
 
     def fetch_state(self, stack_name, resources):
         group_name = self.props.get("GroupName")
-        return aws_stack.connect_to_service("iam").get_group(GroupName=group_name)["Group"]
+        return connect_to().iam.get_group(GroupName=group_name)["Group"]
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
-        return aws_stack.connect_to_service("iam").update_group(
+        return connect_to().iam.update_group(
             GroupName=props.get("GroupName"),
             NewPath=props.get("NewPath") or "",
             NewGroupName=props.get("NewGroupName") or "",
         )
 
     @staticmethod
     def get_deploy_templates():
         def _post_create(logical_resource_id: str, resource: dict, stack_name: str):
-            client = aws_stack.connect_to_service("iam")
+            client = connect_to().iam
             props = resource["Properties"]
             group_name = props["GroupName"]
 
             for managed_policy in props.get("ManagedPolicyArns", []):
                 client.attach_group_policy(GroupName=group_name, PolicyArn=managed_policy)
 
             for inline_policy in props.get("Policies", []):
@@ -634,15 +632,15 @@
                 client.put_group_policy(
                     GroupName=group_name,
                     PolicyName=inline_policy.get("PolicyName"),
                     PolicyDocument=doc,
                 )
 
         def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
-            client = aws_stack.connect_to_service("iam")
+            client = connect_to().iam
             props = resource["Properties"]
             group_name = props["GroupName"]
 
             for managed_policy in props.get("ManagedPolicyArns", []):
                 client.detach_group_policy(GroupName=group_name, PolicyArn=managed_policy)
 
             for inline_policy in props.get("Policies", []):
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kinesis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import generate_default_name
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 
 
 class KinesisStreamConsumer(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Kinesis::StreamConsumer"
 
     def fetch_state(self, stack_name, resources):
         props = self.props
         stream_arn = props["StreamARN"]
-        result = aws_stack.connect_to_service("kinesis").list_stream_consumers(StreamARN=stream_arn)
+        result = connect_to().kinesis.list_stream_consumers(StreamARN=stream_arn)
         result = [r for r in result["Consumers"] if r["ConsumerName"] == props["ConsumerName"]]
         return (result or [None])[0]
 
     @staticmethod
     def get_deploy_templates():
         def _handle_result(result, resource_id, resources, resource_type):
             resource = resources[resource_id]
@@ -35,15 +35,15 @@
 class KinesisStream(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Kinesis::Stream"
 
     def fetch_state(self, stack_name, resources):
         stream_name = self.props["Name"]
-        result = aws_stack.connect_to_service("kinesis").describe_stream(StreamName=stream_name)
+        result = connect_to().kinesis.describe_stream(StreamName=stream_name)
         return result
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         props = resource["Properties"]
         name = props.get("Name")
         if not name:
@@ -57,15 +57,15 @@
     def get_deploy_templates():
         def get_delete_params(
             properties: dict, logical_resource_id: str, resource: dict, stack_name: str
         ) -> dict:
             return {"StreamName": properties["Name"], "EnforceConsumerDeletion": True}
 
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
-            client = aws_stack.connect_to_service("kinesis")
+            client = connect_to().kinesis
             stream_name = resource["Properties"]["Name"]
 
             description = client.describe_stream(StreamName=stream_name)
             while description["StreamDescription"]["StreamStatus"] != "ACTIVE":
                 description = client.describe_stream(StreamName=stream_name)
 
             resource["PhysicalResourceId"] = stream_name
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import select_parameters
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 
 
 class FirehoseDeliveryStream(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::KinesisFirehose::DeliveryStream"
 
     def fetch_state(self, stack_name, resources):
         stream_name = self.props.get("DeliveryStreamName") or self.logical_resource_id
-        return aws_stack.connect_to_service("firehose").describe_delivery_stream(
-            DeliveryStreamName=stream_name
-        )
+        return connect_to().firehose.describe_delivery_stream(DeliveryStreamName=stream_name)
 
     @staticmethod
     def get_deploy_templates():
         def _handle_result(result, resource_id, resources, resource_type):
             resources[resource_id]["Properties"]["Arn"] = result["DeliveryStreamARN"]
             resources[resource_id]["PhysicalResourceId"] = resources[resource_id]["Properties"][
                 "DeliveryStreamName"
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/kms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 
 
 class KMSKey(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::KMS::Key"
 
@@ -39,15 +39,15 @@
         if not physical_res_id:
             return
         return client.describe_key(KeyId=physical_res_id)
 
     @classmethod
     def get_deploy_templates(cls):
         def _create(logical_resource_id: str, resource: dict, stack_name: str):
-            kms_client = aws_stack.connect_to_service("kms")
+            kms_client = connect_to().kms
             resource_provider = cls(resource)
             props = resource_provider.props
             params = {}
             if props.get("KeyPolicy"):
                 params["Policy"] = json.dumps(props["KeyPolicy"])
 
             if props.get("Tags"):
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import generate_default_name
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 
 
 class LogsLogGroup(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Logs::LogGroup"
 
@@ -12,15 +12,15 @@
         props = self.props
         if attribute_name == "Arn":
             return props.get("arn")
         return super(LogsLogGroup, self).get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         group_name = self.props.get("LogGroupName")
-        logs = aws_stack.connect_to_service("logs")
+        logs = connect_to().logs
         groups = logs.describe_log_groups(logGroupNamePrefix=group_name)["logGroups"]
         return ([g for g in groups if g["logGroupName"] == group_name] or [None])[0]
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         name = resource.get("Properties", {}).get("LogGroupName")
         if not name:
@@ -53,15 +53,15 @@
 
     def get_cfn_attribute(self, attribute_name):
         return super(LogsLogStream, self).get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         group_name = self.props.get("LogGroupName")
         stream_name = self.props.get("LogStreamName")
-        logs = aws_stack.connect_to_service("logs")
+        logs = connect_to().logs
         streams = logs.describe_log_streams(
             logGroupName=group_name, logStreamNamePrefix=stream_name
         )["logStreams"]
         return ([s for s in streams if s["logStreamName"] == stream_name] or [None])[0]
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
@@ -94,15 +94,15 @@
     def cloudformation_type():
         return "AWS::Logs::SubscriptionFilter"
 
     def fetch_state(self, stack_name, resources):
         props = self.props
         group_name = props.get("LogGroupName")
         filter_pattern = props.get("FilterPattern")
-        logs = aws_stack.connect_to_service("logs")
+        logs = connect_to().logs
         groups = logs.describe_subscription_filters(logGroupName=group_name)["subscriptionFilters"]
         groups = [g for g in groups if g.get("filterPattern") == filter_pattern]
         return (groups or [None])[0]
 
     @staticmethod
     def get_deploy_templates():
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/opensearch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from localstack.aws.api.opensearch import (
     CreateDomainRequest,
     OpenSearchPartitionInstanceType,
     OpenSearchWarmPartitionInstanceType,
 )
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import remove_none_values
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.collections import convert_to_typed_dict
 
 
 # OpenSearch still uses "es" ARNs
 # See examples in:
 # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-opensearchservice-domain.html
 def opensearch_add_tags_params(
@@ -23,15 +24,15 @@
 class OpenSearchDomain(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::OpenSearchService::Domain"
 
     def fetch_state(self, stack_name, resources):
         domain_name = self._domain_name()
-        return aws_stack.connect_to_service("opensearch").describe_domain(DomainName=domain_name)
+        return connect_to().opensearch.describe_domain(DomainName=domain_name)
 
     def _domain_name(self):
         return self.props.get("DomainName") or self.logical_resource_id
 
     @staticmethod
     def get_deploy_templates():
         def _create_params(
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/redshift.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import generate_default_name
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 
 
 class RedshiftCluster(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Redshift::Cluster"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("redshift")
+        client = connect_to().redshift
         cluster_id = self.props.get("ClusterIdentifier")
         result = client.describe_clusters(ClusterIdentifier=cluster_id)["Clusters"]
         return (result or [None])[0]
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         role_name = resource.get("Properties", {}).get("ClusterIdentifier")
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import params_list_to_dict
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 
 
 class ResourceGroupsGroup(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ResourceGroups::Group"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("resource-groups")
+        client = connect_to().resource_groups
         result = client.list_groups().get("Groups", [])
         result = [g for g in result if g["Name"] == self.props["Name"]]
         return (result or [None])[0]
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "Arn":
             return self.props.get("GroupArn")
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/route53.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 from localstack.utils.common import select_attributes
 
 
 class Route53RecordSet(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Route53::RecordSet"
 
     def fetch_state(self, stack_name, resources):
-        route53 = aws_stack.connect_to_service("route53")
+        route53 = connect_to().route53
         props = self.props
         result = route53.list_resource_record_sets(HostedZoneId=props["HostedZoneId"])[
             "ResourceRecordSets"
         ]
         result = [r for r in result if r["Name"] == props["Name"] and r["Type"] == props["Type"]]
         return (result or [None])[0]
 
@@ -49,15 +49,15 @@
                 "Comment": properties.get("Comment", ""),
                 "Changes": [{"Action": "CREATE", "ResourceRecordSet": attrs}],
             }
 
         def hosted_zone_id_change_batch(
             properties: dict, logical_resource_id: str, resource: dict, stack_name: str
         ):
-            route53 = aws_stack.connect_to_service("route53")
+            route53 = connect_to().route53
             hosted_zone_id = properties.get("HostedZoneId")
             if not hosted_zone_id:
                 hosted_zone_name = properties.get("HostedZoneName")
                 # https://docs.aws.amazon.com/Route53/latest/APIReference/API_ChangeResourceRecordSets.html"
                 # "Specify either HostedZoneName or HostedZoneId, but not both. If you have multiple hosted zones with
                 # the same domain name, you must specify the hosted zone using HostedZoneId."
                 if not hosted_zone_name:
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/s3.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from botocore.exceptions import ClientError
 
+from localstack.aws.connect import connect_to
 from localstack.config import get_edge_port_http
 from localstack.constants import S3_STATIC_WEBSITE_HOSTNAME, S3_VIRTUAL_HOSTNAME
 from localstack.services.cloudformation.cfn_utils import rename_params
 from localstack.services.cloudformation.deployment_utils import (
     dump_json_params,
     generate_default_name,
 )
@@ -19,15 +20,15 @@
 class S3BucketPolicy(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::S3::BucketPolicy"
 
     def fetch_state(self, stack_name, resources):
         bucket_name = self.props.get("Bucket") or self.logical_resource_id
-        return aws_stack.connect_to_service("s3").get_bucket_policy(Bucket=bucket_name)
+        return connect_to().s3.get_bucket_policy(Bucket=bucket_name)
 
     @staticmethod
     def get_deploy_templates():
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
             resource["PhysicalResourceId"] = md5(
                 canonical_json(resource["Properties"]["PolicyDocument"])
             )
@@ -165,15 +166,15 @@
             }
             return result
 
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
             resource["PhysicalResourceId"] = resource["Properties"]["BucketName"]
 
         def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
-            s3 = aws_stack.connect_to_service("s3")
+            s3 = connect_to().s3
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             try:
                 s3.delete_bucket_policy(Bucket=bucket_name)
             except Exception:
                 pass
             s3_listener.remove_bucket_notification(resource["PhysicalResourceId"])
@@ -181,62 +182,62 @@
             try:
                 delete_all_s3_objects(bucket_name)
             except Exception as e:
                 if "NoSuchBucket" not in str(e):
                     raise
 
         def _add_bucket_tags(logical_resource_id: str, resource: dict, stack_name: str):
-            s3 = aws_stack.connect_to_service("s3")
+            s3 = connect_to().s3
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             tags = props.get("Tags", [])
             if len(tags) > 0:
                 s3.put_bucket_tagging(Bucket=bucket_name, Tagging={"TagSet": tags})
 
         def _put_bucket_versioning(logical_resource_id: str, resource: dict, stack_name: str):
-            s3_client = aws_stack.connect_to_service("s3")
+            s3_client = connect_to().s3
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             versioning_config = props.get("VersioningConfiguration")
             if versioning_config:
                 s3_client.put_bucket_versioning(
                     Bucket=bucket_name,
                     VersioningConfiguration={
                         "Status": versioning_config.get("Status", "Disabled"),
                     },
                 )
 
         def _put_bucket_cors_configuration(
             logical_resource_id: str, resource: dict, stack_name: str
         ):
-            s3_client = aws_stack.connect_to_service("s3")
+            s3_client = connect_to().s3
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             cors_configuration = transform_cfn_cors(props.get("CorsConfiguration"))
             if cors_configuration:
                 s3_client.put_bucket_cors(
                     Bucket=bucket_name,
                     CORSConfiguration=cors_configuration,
                 )
 
         def _put_bucket_website_configuration(
             logical_resource_id: str, resource: dict, stack_name: str
         ):
-            s3_client = aws_stack.connect_to_service("s3")
+            s3_client = connect_to().s3
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             website_config = transform_website_configuration(props.get("WebsiteConfiguration"))
             if website_config:
                 s3_client.put_bucket_website(
                     Bucket=bucket_name,
                     WebsiteConfiguration=website_config,
                 )
 
         def _create_bucket(logical_resource_id: str, resource: dict, stack_name: str):
-            s3_client = aws_stack.connect_to_service("s3")
+            s3_client = connect_to().s3
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             try:
                 s3_client.head_bucket(Bucket=bucket_name)
             except ClientError as e:
                 if e.response["Error"]["Message"] == "Not Found":
                     bucket_name = props.get("BucketName")
@@ -272,15 +273,15 @@
         }
         return result
 
     def fetch_state(self, stack_name, resources):
         props = self.props
         bucket_name = self._get_bucket_name()
         bucket_name = self.normalize_bucket_name(bucket_name)
-        s3_client = aws_stack.connect_to_service("s3")
+        s3_client = connect_to().s3
         response = s3_client.get_bucket_location(Bucket=bucket_name)
         notifs = props.get("NotificationConfiguration")
         if not response or not notifs:
             return response
         configs = s3_client.get_bucket_notification_configuration(Bucket=bucket_name)
         has_notifs = (
             configs.get("TopicConfigurations")
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import random
 import string
 
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import generate_default_name
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 from localstack.utils.common import select_attributes
 
 LOG = logging.getLogger(__name__)
 
 
 class SecretsManagerSecret(GenericBaseModel):
     @staticmethod
@@ -21,17 +21,15 @@
             case "Id":
                 return self.props.get("ARN")
 
         return super(SecretsManagerSecret, self).get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         secret_name = self.props.get("Name") or self.logical_resource_id
-        result = aws_stack.connect_to_service("secretsmanager").describe_secret(
-            SecretId=secret_name
-        )
+        result = connect_to().secretsmanager.describe_secret(SecretId=secret_name)
         return result
 
     @staticmethod
     def generate_secret_value(
         length: int,
         excl_lower: bool,
         excl_upper: bool,
@@ -150,17 +148,15 @@
 class SecretsManagerResourcePolicy(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SecretsManager::ResourcePolicy"
 
     def fetch_state(self, stack_name, resources):
         secret_id = self.props.get("SecretId")
-        result = aws_stack.connect_to_service("secretsmanager").get_resource_policy(
-            SecretId=secret_id
-        )
+        result = connect_to().secretsmanager.get_resource_policy(SecretId=secret_id)
         return result
 
     @staticmethod
     def get_deploy_templates():
         def create_params(
             properties: dict, logical_resource_id: str, resource: dict, stack_name: str
         ) -> dict:
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/sns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 
 from botocore.exceptions import ClientError
 
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     is_none_or_empty_value,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 from localstack.utils.common import canonicalize_bool_to_str
 
 
 class SNSTopic(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SNS::Topic"
 
     def fetch_state(self, stack_name, resources):
         topic_name = self.props["TopicName"]
-        topics = aws_stack.connect_to_service("sns").list_topics()
+        topics = connect_to().sns.list_topics()
         result = list(
             filter(
                 lambda item: item["TopicArn"].split(":")[-1] == topic_name,
                 topics.get("Topics", []),
             )
         )
         return result[0] if result else None
@@ -73,15 +73,15 @@
                 rs = sns_client.list_topics(NextToken=key)
                 topics.extend(rs.get("Topics", []))
                 key = rs.get("NextToken")
 
             return topics
 
         def _add_topics(logical_resource_id: str, resource: str, stack_name: str):
-            sns_client = aws_stack.connect_to_service("sns")
+            sns_client = connect_to().sns
             topics = _list_all_topics(sns_client)
             topics_by_name = {t["TopicArn"].split(":")[-1]: t for t in topics}
 
             provider = cls(resource)
             props = provider.props
 
             subscriptions = props.get("Subscription", [])
@@ -120,15 +120,15 @@
         return "AWS::SNS::Subscription"
 
     def fetch_state(self, stack_name, resources):
         props = self.props
         topic_arn = props.get("TopicArn")
         if topic_arn is None:
             return
-        subs = aws_stack.connect_to_service("sns").list_subscriptions_by_topic(TopicArn=topic_arn)
+        subs = connect_to().sns.list_subscriptions_by_topic(TopicArn=topic_arn)
         result = [
             sub
             for sub in subs["Subscriptions"]
             if props.get("Protocol") == sub["Protocol"] and props.get("Endpoint") == sub["Endpoint"]
         ]
         # TODO: use get_subscription_attributes to compare FilterPolicy
         return result[0] if result else None
@@ -178,15 +178,15 @@
 
 class SNSTopicPolicy(GenericBaseModel):
     @classmethod
     def cloudformation_type(cls):
         return "AWS::SNS::TopicPolicy"
 
     def fetch_state(self, stack_name, resources):
-        sns_client = aws_stack.connect_to_service("sns")
+        sns_client = connect_to().sns
         result = {}
         props = self.props
         for topic_arn in props["Topics"]:
             result[topic_arn] = None
             attrs = sns_client.get_topic_attributes(TopicArn=topic_arn)
             policy = attrs["Attributes"].get("Policy")
             if not policy:
@@ -199,28 +199,28 @@
             # return None if not all policies for all topics are properly deployed yet
             return None
         return result
 
     @classmethod
     def get_deploy_templates(cls):
         def _create(logical_resource_id: str, resource: dict, stack_name: str):
-            sns_client = aws_stack.connect_to_service("sns")
+            sns_client = connect_to().sns
             provider = cls(resource)
             props = provider.props
 
             resource["PhysicalResourceId"] = generate_default_name(stack_name, logical_resource_id)
 
             policy = json.dumps(props["PolicyDocument"])
             for topic_arn in props["Topics"]:
                 sns_client.set_topic_attributes(
                     TopicArn=topic_arn, AttributeName="Policy", AttributeValue=policy
                 )
 
         def _delete(logical_resource_id: str, resource: dict, stack_name: str):
-            sns_client = aws_stack.connect_to_service("sns")
+            sns_client = connect_to().sns
             provider = cls(resource)
             props = provider.props
 
             for topic_arn in props["Topics"]:
                 try:
                     sns_client.set_topic_attributes(
                         TopicArn=topic_arn, AttributeName="Policy", AttributeValue=""
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/sqs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 import logging
 
 from botocore.exceptions import ClientError
 
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     params_list_to_dict,
     params_select_attributes,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.common import short_uid
 
 LOG = logging.getLogger(__name__)
 
 
 class QueuePolicy(GenericBaseModel):
     @classmethod
@@ -23,30 +24,30 @@
     def fetch_state(self, stack_name, resources):
         if self.resource_json.get("PhysicalResourceId"):
             return {"something": "something"}  # gotta return <something> since {} is falsey :)
 
     @classmethod
     def get_deploy_templates(cls):
         def _create(logical_resource_id: str, resource: dict, stack_name: str):
-            sqs_client = aws_stack.connect_to_service("sqs")
+            sqs_client = connect_to().sqs
             resource_provider = cls(resource)
             props = resource_provider.props
 
             resource["PhysicalResourceId"] = "%s-%s-%s" % (
                 stack_name,
                 logical_resource_id,
                 short_uid(),
             )
 
             policy = json.dumps(props["PolicyDocument"])
             for queue in props["Queues"]:
                 sqs_client.set_queue_attributes(QueueUrl=queue, Attributes={"Policy": policy})
 
         def _delete(logical_resource_id: str, resource: dict, stack_name: str):
-            sqs_client = aws_stack.connect_to_service("sqs")
+            sqs_client = connect_to().sqs
             resource_provider = cls(resource)
             props = resource_provider.props
 
             for queue in props["Queues"]:
                 try:
                     sqs_client.set_queue_attributes(QueueUrl=queue, Attributes={"Policy": ""})
                 except ClientError as err:
@@ -69,15 +70,15 @@
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "Arn":
             return arns.sqs_queue_arn(self.properties["QueueName"])
         return super().get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         queue_name = self.props["QueueName"]
-        sqs_client = aws_stack.connect_to_service("sqs")
+        sqs_client = connect_to().sqs
         queues = sqs_client.list_queues()
         result = list(
             filter(
                 lambda item:
                 # TODO possibly find a better way to compare resource_id with queue URLs
                 item.endswith("/%s" % queue_name),
                 queues.get("QueueUrls", []),
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import logging
 import re
 from typing import Dict
 
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import generate_default_name
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack
 from localstack.utils.common import to_str
 
 LOG = logging.getLogger(__name__)
 
 
 class SFNActivity(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::StepFunctions::Activity"
 
     def fetch_state(self, stack_name, resources):
         activity_arn = self.physical_resource_id
         if not activity_arn:
             return None
-        client = aws_stack.connect_to_service("stepfunctions")
+        client = connect_to().stepfunctions
         result = client.describe_activity(activityArn=activity_arn)
         return result
 
     @staticmethod
     def get_deploy_templates():
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
             resource["Properties"]["Arn"] = result["activityArn"]
@@ -52,25 +52,25 @@
             return self.props.get("Arn")
         if attribute_name == "Name":
             return self.props.get("StateMachineName")
         return super(SFNStateMachine, self).get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         sm_name = self.props.get("StateMachineName") or self.logical_resource_id
-        sfn_client = aws_stack.connect_to_service("stepfunctions")
+        sfn_client = connect_to().stepfunctions
         state_machines = sfn_client.list_state_machines()["stateMachines"]
         sm_arn = [m["stateMachineArn"] for m in state_machines if m["name"] == sm_name]
         if not sm_arn:
             return None
         result = sfn_client.describe_state_machine(stateMachineArn=sm_arn[0])
         return result
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
-        client = aws_stack.connect_to_service("stepfunctions")
+        client = connect_to().stepfunctions
         sm_arn = self.props.get("stateMachineArn")
         if not sm_arn:
             self.state = self.fetch_state(stack_name=stack_name, resources=resources)
             sm_arn = self.state["stateMachineArn"]
         kwargs = {
             "stateMachineArn": sm_arn,
             "definition": props["DefinitionString"],
@@ -96,15 +96,15 @@
         ) -> dict:
             def _get_definition(properties):
                 # TODO: support "Definition" parameter
                 definition_str = properties.get("DefinitionString")
                 s3_location = properties.get("DefinitionS3Location")
                 if not definition_str and s3_location:
                     # TODO: currently not covered by tests - add a test to mimick the behavior of "sam deploy ..."
-                    s3_client = aws_stack.connect_to_service("s3")
+                    s3_client = connect_to().s3
                     LOG.debug("Fetching state machine definition from S3: %s", s3_location)
                     result = s3_client.get_object(
                         Bucket=s3_location["Bucket"], Key=s3_location["Key"]
                     )
                     definition_str = to_str(result["Body"].read())
                 substitutions = properties.get("DefinitionSubstitutions")
                 if substitutions is not None:
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     UpdateStackOutput,
     UpdateStackSetInput,
     UpdateStackSetOutput,
     UpdateTerminationProtectionOutput,
     ValidateTemplateInput,
     ValidateTemplateOutput,
 )
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation import api_utils
 from localstack.services.cloudformation.engine import parameters as param_resolver
 from localstack.services.cloudformation.engine import template_deployer, template_preparer
 from localstack.services.cloudformation.engine.entities import (
     Stack,
     StackChangeSet,
     StackInstance,
@@ -87,15 +88,14 @@
 )
 from localstack.services.cloudformation.engine.template_utils import resolve_stack_conditions
 from localstack.services.cloudformation.stores import (
     find_change_set,
     find_stack,
     get_cloudformation_store,
 )
-from localstack.utils.aws import aws_stack
 from localstack.utils.collections import (
     remove_attributes,
     select_attributes,
     select_from_typed_dict,
 )
 from localstack.utils.json import clone
 from localstack.utils.strings import long_uid, short_uid
@@ -961,15 +961,15 @@
         regions = request["Regions"]
 
         stacks_to_await = []
         for account in accounts:
             for region in regions:
                 # deploy new stack
                 LOG.debug('Deploying instance for stack set "%s" in region "%s"', set_name, region)
-                cf_client = aws_stack.connect_to_service("cloudformation", region_name=region)
+                cf_client = connect_to(region_name=region).cloudformation
                 kwargs = select_attributes(sset_meta, ["TemplateBody"]) or select_attributes(
                     sset_meta, ["TemplateURL"]
                 )
                 stack_name = f"sset-{set_name}-{account}"
 
                 # skip creation of existing stacks
                 if find_stack(stack_name, region=region):
@@ -988,15 +988,15 @@
                     "StackInstanceStatus": {"DetailedStatus": "SUCCEEDED"},
                 }
                 instance = StackInstance(instance)
                 stack_set.stack_instances.append(instance)
 
         # wait for completion of stack
         for stack in stacks_to_await:
-            client = aws_stack.connect_to_service("cloudformation", region_name=stack[1])
+            client = connect_to(region_name=stack[1]).cloudformation
             client.get_waiter("stack_create_complete").wait(StackName=stack[0])
 
         # record operation
         operation = {
             "OperationId": op_id,
             "StackSetId": stack_set.metadata["StackSetId"],
             "Action": "CREATE",
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/provider_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import math
 import threading
 from datetime import datetime, timedelta, timezone
 from typing import TYPE_CHECKING, List, Optional
 
 from localstack.aws.api.cloudwatch import MetricAlarm, MetricDataQuery, StateValue
+from localstack.aws.connect import connect_to
 from localstack.utils.aws import arns, aws_stack
 from localstack.utils.scheduler import Scheduler
 
 if TYPE_CHECKING:
     from mypy_boto3_cloudwatch import CloudWatchClient
 
 LOG = logging.getLogger(__name__)
@@ -92,15 +93,15 @@
 
     def restart_existing_alarms(self) -> None:
         """
         Only used re-create persistent state. Reschedules alarms that already exist
         """
         service = "cloudwatch"
         for region in aws_stack.get_valid_regions_for_service(service):
-            client = aws_stack.connect_to_service(service, region_name=region)
+            client = connect_to(region_name=region).get_client(service)
             result = client.describe_alarms()
             for metric_alarm in result["MetricAlarms"]:
                 arn = metric_alarm["AlarmArn"]
                 self.schedule_metric_alarm(alarm_arn=arn)
 
     def _is_alarm_supported(self, alarm_details: MetricAlarm) -> bool:
         required_parameters = ["Period", "Statistic", "MetricName", "Threshold"]
@@ -123,15 +124,15 @@
     client = get_cloudwatch_client_for_region_of_alarm(alarm_arn)
     metric_alarms = client.describe_alarms(AlarmNames=[alarm_name])["MetricAlarms"]
     return metric_alarms[0] if metric_alarms else None
 
 
 def get_cloudwatch_client_for_region_of_alarm(alarm_arn: str) -> "CloudWatchClient":
     region = arns.extract_region_from_arn(alarm_arn)
-    return aws_stack.connect_to_service("cloudwatch", region_name=region)
+    return connect_to(region_name=region).cloudwatch
 
 
 def generate_metric_query(alarm_details: MetricAlarm) -> MetricDataQuery:
     """Creates the dict with the required data for MetricDataQueries when calling client.get_metric_data"""
 
     metric = {
         "MetricName": alarm_details["MetricName"],
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/cloudwatch/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     PutMetricAlarmInput,
     StateValue,
     TagKeyList,
     TagList,
     TagResourceOutput,
     UntagResourceOutput,
 )
+from localstack.aws.connect import connect_to
 from localstack.constants import DEFAULT_AWS_ACCOUNT_ID
 from localstack.deprecations import deprecated_endpoint
 from localstack.http import Request
 from localstack.services import moto
 from localstack.services.cloudwatch.alarm_scheduler import AlarmScheduler
 from localstack.services.edge import ROUTER
 from localstack.services.plugins import SERVICE_PLUGINS, ServiceLifecycleHook
@@ -66,15 +67,15 @@
         actions = self.alarm_actions
     else:
         actions = self.insufficient_data_actions
     for action in actions:
         data = arns.parse_arn(action)
         # test for sns - can this be done in a more generic way?
         if data["service"] == "sns":
-            service = aws_stack.connect_to_service(data["service"])
+            service = connect_to.get_client(data["service"])
             subject = f"""{self.state_value}: "{self.name}" in {self.region_name}"""
             message = create_message_response_update_state(self, old_state)
             service.publish(TopicArn=action, Subject=subject, Message=message)
         else:
             # TODO: support other actions
             LOG.warning(
                 "Action for service %s not implemented, action '%s' will not be triggered.",
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     UpdateGlobalTableOutput,
     UpdateItemInput,
     UpdateItemOutput,
     UpdateTableInput,
     UpdateTableOutput,
     UpdateTimeToLiveOutput,
 )
+from localstack.aws.connect import connect_to
 from localstack.aws.forwarder import get_request_forwarder_http
 from localstack.constants import AUTH_CREDENTIAL_REGEX, LOCALHOST, TEST_AWS_SECRET_ACCESS_KEY
 from localstack.http import Response
 from localstack.services.dynamodb.models import DynamoDBStore, dynamodb_stores
 from localstack.services.dynamodb.server import DynamodbServer
 from localstack.services.dynamodb.utils import (
     ItemFinder,
@@ -148,15 +149,15 @@
 ]
 THROTTLED_ACTIONS = READ_THROTTLED_ACTIONS + WRITE_THROTTLED_ACTIONS
 
 MANAGED_KMS_KEYS = {}
 
 
 def dynamodb_table_exists(table_name, client=None):
-    client = client or aws_stack.connect_to_service("dynamodb")
+    client = client or connect_to().dynamodb
     paginator = client.get_paginator("list_tables")
     pages = paginator.paginate(PaginationConfig={"PageSize": 100})
     for page in pages:
         table_names = page["TableNames"]
         if to_str(table_name) in table_names:
             return True
     return False
@@ -202,20 +203,19 @@
             record.pop("eventSourceARN", None)
             record["dynamodb"].pop("StreamViewType", None)
             hash_keys = list(filter(lambda key: key["KeyType"] == "HASH", table_def["KeySchema"]))
             partition_key = hash_keys[0]["AttributeName"]
 
             stream_account_id = extract_account_id_from_arn(stream_arn)
             stream_region_name = extract_region_from_arn(stream_arn)
-            kinesis = aws_stack.connect_to_service(
-                "kinesis",
+            kinesis = connect_to(
                 aws_access_key_id=stream_account_id,
                 aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY,
                 region_name=stream_region_name,
-            )
+            ).kinesis
             kinesis.put_record(
                 StreamName=stream_name,
                 Data=json.dumps(record, cls=BytesEncoder),
                 PartitionKey=partition_key,
             )
 
     @classmethod
@@ -242,20 +242,19 @@
         return records
 
     @classmethod
     def is_kinesis_stream_exists(cls, stream_arn):
         account_id = extract_account_id_from_arn(stream_arn)
         region_name = extract_region_from_arn(stream_arn)
 
-        kinesis = aws_stack.connect_to_service(
-            "kinesis",
+        kinesis = connect_to(
             aws_access_key_id=account_id,
             aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY,
             region_name=region_name,
-        )
+        ).kinesis
         stream_name_from_arn = stream_arn.split("/", 1)[1]
         # check if the stream exists in kinesis for the user
         filtered = list(
             filter(
                 lambda stream_name: stream_name == stream_name_from_arn,
                 kinesis.list_streams()["StreamNames"],
             )
@@ -269,20 +268,19 @@
     @classmethod
     def get_sse_kms_managed_key(cls, account_id: str, region_name: str):
         from localstack.services.kms import provider
 
         existing_key = MANAGED_KMS_KEYS.get(region_name)
         if existing_key:
             return existing_key
-        kms_client = aws_stack.connect_to_service(
-            "kms",
+        kms_client = connect_to(
             aws_access_key_id=account_id,
             aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY,
             region_name=region_name,
-        )
+        ).kms
         key_data = kms_client.create_key(
             Description="Default key that protects my DynamoDB data when no other key is defined"
         )
         key_id = key_data["KeyMetadata"]["KeyId"]
 
         provider.set_key_managed(key_id, account_id, region_name)
         MANAGED_KMS_KEYS[aws_stack.get_region()] = key_id
@@ -1316,20 +1314,19 @@
 
         return region_name
 
     @staticmethod
     def table_exists(account_id: str, region_name: str, table_name: str) -> bool:
         region_name = DynamoDBProvider.ddb_region_name(region_name)
 
-        client = aws_stack.connect_to_service(
-            "dynamodb",
+        client = connect_to(
             aws_access_key_id=account_id,
             aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY,
             region_name=region_name,
-        )
+        ).dynamodb
         return dynamodb_table_exists(table_name, client)
 
     @staticmethod
     def ensure_table_exists(account_id: str, region_name: str, table_name: str):
         """
         Raise ResourceNotFoundException if the given table does not exist.
 
@@ -1654,15 +1651,15 @@
         cache = {}
     if not table_name:
         return
     table_arn = arns.dynamodb_table_arn(table_name)
     cached = cache.get(table_arn)
     if isinstance(cached, bool):
         return cached
-    lambda_client = aws_stack.connect_to_service("lambda")
+    lambda_client = connect_to().awslambda
     sources = lambda_client.list_event_source_mappings(EventSourceArn=table_arn)[
         "EventSourceMappings"
     ]
     result = False
     if sources:
         result = True
     if not result and dynamodbstreams_api.get_stream_for_table(table_arn):
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 import threading
 
 from localstack import config
+from localstack.aws.connect import connect_externally_to
 from localstack.config import is_env_true
 from localstack.services.dynamodb.packages import dynamodblocal_package
-from localstack.utils.aws import aws_stack
 from localstack.utils.common import TMP_THREADS, ShellCommandThread, get_free_tcp_port, mkdir
 from localstack.utils.functions import run_safe
 from localstack.utils.net import wait_for_port_closed
 from localstack.utils.run import FuncThread, run
 from localstack.utils.serving import Server
 from localstack.utils.sync import retry, synchronized
 
@@ -162,15 +162,15 @@
 
     def check_dynamodb(self, expect_shutdown: bool = False, print_error: bool = False) -> None:
         """Checks if DynamoDB server is up"""
         out = None
 
         try:
             self.wait_is_up()
-            out = aws_stack.connect_to_service("dynamodb", endpoint_url=self.url).list_tables()
+            out = connect_externally_to(endpoint_url=self.url).dynamodb.list_tables()
         except Exception:
             if print_error:
                 LOG.exception("DynamoDB health check failed")
         if expect_shutdown:
             assert out is None
         else:
             assert isinstance(out["TableNames"], list)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodb/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict, List, Mapping, Optional
 
 from cachetools import TTLCache
 from moto.core.exceptions import JsonRESTError
 
 from localstack.aws.accounts import get_aws_account_id
 from localstack.aws.api.dynamodb import ResourceNotFoundException
+from localstack.aws.connect import connect_to
 from localstack.constants import TEST_AWS_SECRET_ACCESS_KEY
 from localstack.utils.aws import aws_stack
 from localstack.utils.aws.arns import dynamodb_table_arn
 from localstack.utils.json import canonical_json
 from localstack.utils.testutil import list_all_resources
 
 LOG = logging.getLogger(__name__)
@@ -95,20 +96,19 @@
         region_name = region_name or aws_stack.get_region()
         key = dynamodb_table_arn(
             table_name=table_name, account_id=account_id, region_name=region_name
         )
         schema = SCHEMA_CACHE.get(key)
         if not schema:
             # TODO: consider making in-memory lookup instead of API call
-            ddb_client = aws_stack.connect_to_service(
-                "dynamodb",
+            ddb_client = connect_to(
                 aws_access_key_id=account_id,
                 aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY,
                 region_name=region_name,
-            )
+            ).dynamodb
             try:
                 schema = ddb_client.describe_table(TableName=table_name)
                 SCHEMA_CACHE[key] = schema
             except Exception as e:
                 if "ResourceNotFoundException" in str(e):
                     raise ResourceNotFoundException(f"Unknown table: {table_name}") from e
                 raise
@@ -119,20 +119,19 @@
     @staticmethod
     def find_existing_item(
         put_item: Dict, table_name: str = None, account_id: str = None, region_name: str = None
     ) -> Optional[Dict]:
         from localstack.services.dynamodb.provider import ValidationException
 
         table_name = table_name or put_item["TableName"]
-        ddb_client = aws_stack.connect_to_service(
-            "dynamodb",
+        ddb_client = connect_to(
             aws_access_key_id=account_id or get_aws_account_id(),
             aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY,
             region_name=region_name or aws_stack.get_region(),
-        )
+        ).dynamodb
 
         search_key = {}
         if "Key" in put_item:
             search_key = put_item["Key"]
         else:
             schema = SchemaExtractor.get_table_schema(table_name)
             schemas = [schema["Table"]["KeySchema"]]
@@ -176,20 +175,19 @@
         if not table_name:
             return []
         all_items = cls.get_all_table_items(table_name)
         return all_items
 
     @staticmethod
     def get_all_table_items(table_name: str) -> List:
-        ddb_client = aws_stack.connect_to_service(
-            "dynamodb",
+        ddb_client = connect_to(
             aws_access_key_id=get_aws_account_id(),
             aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY,
             region_name=aws_stack.get_region(),
-        )
+        ).dynamodb
         dynamodb_kwargs = {"TableName": table_name}
         all_items = list_all_resources(
             lambda kwargs: ddb_client.scan(**{**kwargs, **dynamodb_kwargs}),
             last_token_attr_name="LastEvaluatedKey",
             next_token_attr_name="ExclusiveStartKey",
             list_attr_name="Items",
         )
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 from typing import Dict
 
 from bson.json_util import dumps
 
 from localstack.aws.accounts import get_aws_account_id
 from localstack.aws.api.dynamodbstreams import StreamStatus, StreamViewType
+from localstack.aws.connect import connect_to
 from localstack.services.dynamodbstreams.models import DynamoDbStreamsStore, dynamodbstreams_stores
 from localstack.utils.aws import arns, aws_stack, resources
 from localstack.utils.common import now_utc
 
 DDB_KINESIS_STREAM_NAME_PREFIX = "__ddb_stream_"
 
 LOG = logging.getLogger(__name__)
@@ -66,15 +67,15 @@
 def get_stream_for_table(table_arn: str) -> dict:
     store = get_dynamodbstreams_store()
     table_name = table_name_from_stream_arn(table_arn)
     return store.ddb_streams.get(table_name)
 
 
 def forward_events(records: dict) -> None:
-    kinesis = aws_stack.connect_to_service("kinesis")
+    kinesis = connect_to().kinesis
     for record in records:
         table_arn = record.pop("eventSourceARN", "")
         if stream := get_stream_for_table(table_arn):
             table_name = table_name_from_stream_arn(stream["StreamArn"])
             stream_name = get_kinesis_stream_name(table_name)
             kinesis.put_record(
                 StreamName=stream_name,
@@ -85,15 +86,15 @@
 
 def delete_streams(table_arn: str) -> None:
     store = get_dynamodbstreams_store()
     table_name = table_name_from_table_arn(table_arn)
     if store.ddb_streams.pop(table_name, None):
         stream_name = get_kinesis_stream_name(table_name)
         with contextlib.suppress(Exception):
-            aws_stack.connect_to_service("kinesis").delete_stream(StreamName=stream_name)
+            connect_to().kinesis.delete_stream(StreamName=stream_name)
             # sleep a bit, as stream deletion can take some time ...
             time.sleep(1)
 
 
 def get_kinesis_stream_name(table_name: str) -> str:
     return DDB_KINESIS_STREAM_NAME_PREFIX + table_name
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/dynamodbstreams/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     get_kinesis_stream_name,
     get_shard_id,
     kinesis_shard_id,
     stream_name_from_stream_arn,
     table_name_from_stream_arn,
 )
 from localstack.services.plugins import ServiceLifecycleHook
-from localstack.utils.aws import aws_stack
 from localstack.utils.collections import select_from_typed_dict
 
 LOG = logging.getLogger(__name__)
 
 STREAM_STATUS_MAP = {
     "ACTIVE": StreamStatus.ENABLED,
     "CREATING": StreamStatus.ENABLING,
@@ -51,19 +50,19 @@
         self,
         context: RequestContext,
         stream_arn: StreamArn,
         limit: PositiveIntegerObject = None,
         exclusive_start_shard_id: ShardId = None,
     ) -> DescribeStreamOutput:
         store = get_dynamodbstreams_store(context.account_id, context.region)
-        kinesis = aws_stack.connect_to_service("kinesis")
+        kinesis = connect_to().kinesis
         for stream in store.ddb_streams.values():
             if stream["StreamArn"] == stream_arn:
                 # get stream details
-                dynamodb = aws_stack.connect_to_service("dynamodb")
+                dynamodb = connect_to().dynamodb
                 table_name = table_name_from_stream_arn(stream["StreamArn"])
                 stream_name = get_kinesis_stream_name(table_name)
                 stream_details = kinesis.describe_stream(StreamName=stream_name)
                 table_details = dynamodb.describe_table(TableName=table_name)
                 stream["KeySchema"] = table_details["Table"]["KeySchema"]
                 stream["StreamStatus"] = STREAM_STATUS_MAP.get(
                     stream_details["StreamDescription"]["StreamStatus"]
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/ec2/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,22 +69,22 @@
     Tenancy,
     VpcEndpointId,
     VpcEndpointRouteTableIdList,
     VpcEndpointSecurityGroupIdList,
     VpcEndpointSubnetIdList,
     scope,
 )
+from localstack.aws.connect import connect_to
 from localstack.services.ec2.exceptions import (
     InvalidLaunchTemplateIdError,
     InvalidLaunchTemplateNameError,
     MissingParameterError,
 )
 from localstack.services.ec2.models import get_ec2_backend
 from localstack.services.moto import call_moto
-from localstack.utils.aws import aws_stack
 from localstack.utils.patch import patch
 from localstack.utils.strings import first_char_to_upper, long_uid, short_uid
 
 # additional subnet attributes not yet supported upstream
 ADDITIONAL_SUBNET_ATTRS = ("private_dns_name_options_on_launch", "enable_dns64")
 
 
@@ -382,15 +382,15 @@
             try:
                 template.versions[int(request["DefaultVersion"]) - 1]
             except IndexError:
                 raise InvalidLaunchTemplateIdError()
 
         template.default_version_number = int(request["DefaultVersion"])
 
-        client = aws_stack.connect_to_service("ec2")
+        client = connect_to().ec2
         retrieved_template = client.describe_launch_templates(LaunchTemplateIds=[template.id])
 
         result: ModifyLaunchTemplateResult = {
             "LaunchTemplate": retrieved_template["LaunchTemplates"][0],
         }
 
         return result
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/firehose/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,17 +139,15 @@
     :param domain_arn: ARN of the cluster.
     :returns: cluster endpoint
     :raises: ValueError if the domain_arn is malformed
     """
     region_name = extract_region_from_arn(domain_arn)
     if region_name is None:
         raise ValueError("unable to parse region from opensearch domain ARN")
-    opensearch_client = aws_stack.connect_to_service(
-        service_name="opensearch", region_name=region_name
-    )
+    opensearch_client = connect_to(region_name=region_name).opensearch
     domain_name = opensearch_domain_name(domain_arn)
     info = opensearch_client.describe_domain(DomainName=domain_name)
     base_domain = info["DomainStatus"]["Endpoint"]
     # Add the URL scheme "http" if it's not set yet. https might not be enabled for all instances
     # f.e. when the endpoint strategy is PORT or there is a custom opensearch/elasticsearch instance
     endpoint = base_domain if base_domain.startswith("http") else f"http://{base_domain}"
     return endpoint
@@ -679,17 +677,15 @@
             for record in records:
                 if "data" in record:
                     record["data"] = to_str(record["data"])
                 if "Data" in record:
                     record["Data"] = to_str(record["Data"])
             event = {"records": records}
             event = to_bytes(json.dumps(event))
-            client = aws_stack.connect_to_service(
-                "lambda", region_name=extract_region_from_arn(lambda_arn)
-            )
+            client = connect_to(region_name=extract_region_from_arn(lambda_arn)).awslambda
             response = client.invoke(FunctionName=lambda_arn, Payload=event)
             result = response.get("Payload").read()
             result = json.loads(to_str(result))
             records = result.get("records", []) if result else []
         else:
             LOG.warning("Unsupported Firehose processor type '%s'", proc_type)
         return records
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/iam/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     policyDocumentType,
     roleDescriptionType,
     roleNameType,
     tagKeyListType,
     tagListType,
     userNameType,
 )
+from localstack.aws.connect import connect_to
 from localstack.constants import INTERNAL_AWS_SECRET_ACCESS_KEY
 from localstack.services.moto import call_moto
-from localstack.utils.aws import aws_stack
 from localstack.utils.aws.aws_stack import extract_access_key_id_from_auth_header
 from localstack.utils.common import short_uid
 from localstack.utils.patch import patch
 
 SERVICE_LINKED_ROLE_PATH_PREFIX = "/aws-service-role"
 
 ADDITIONAL_MANAGED_POLICIES = {
@@ -386,19 +386,18 @@
     ) -> GetUserResponse:
         response = call_moto(context=context)
         moto_user_name = response["User"]["UserName"]
         moto_user = get_iam_backend(context).users.get(moto_user_name)
         # if the user does not exist or is no user
         if not moto_user and not user_name:
             access_key_id = extract_access_key_id_from_auth_header(context.request.headers)
-            sts_client = aws_stack.connect_to_service(
-                "sts",
+            sts_client = connect_to(
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=INTERNAL_AWS_SECRET_ACCESS_KEY,
-            )
+            ).sts
             caller_identity = sts_client.get_caller_identity()
             caller_arn = caller_identity["Arn"]
             if caller_arn.endswith(":root"):
                 return GetUserResponse(
                     User=User(
                         UserId=context.account_id,
                         Arn=caller_arn,
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-2.1.1.dev20230714101424/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kinesis/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,29 +22,30 @@
     StartingPosition,
     StreamARN,
     StreamName,
     SubscribeToShardEvent,
     SubscribeToShardEventStream,
     SubscribeToShardOutput,
 )
+from localstack.aws.connect import connect_to
 from localstack.constants import LOCALHOST
 from localstack.services.kinesis.kinesis_mock_server import KinesisServerManager
 from localstack.services.kinesis.models import KinesisStore, kinesis_stores
 from localstack.services.plugins import ServiceLifecycleHook
 from localstack.state import AssetDirectory, StateVisitor
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.time import now_utc
 
 LOG = logging.getLogger(__name__)
 MAX_SUBSCRIPTION_SECONDS = 300
 SERVER_STARTUP_TIMEOUT = 120
 
 
 def find_stream_for_consumer(consumer_arn):
-    kinesis = aws_stack.connect_to_service("kinesis")
+    kinesis = connect_to().kinesis
     for stream_name in kinesis.list_streams()["StreamNames"]:
         stream_arn = arns.kinesis_stream_arn(stream_name)
         for cons in kinesis.list_stream_consumers(StreamARN=stream_arn)["Consumers"]:
             if cons["ConsumerARN"] == consumer_arn:
                 return stream_name
     raise Exception("Unable to find stream for stream consumer %s" % consumer_arn)
 
@@ -83,15 +84,15 @@
     def subscribe_to_shard(
         self,
         context: RequestContext,
         consumer_arn: ConsumerARN,
         shard_id: ShardId,
         starting_position: StartingPosition,
     ) -> SubscribeToShardOutput:
-        kinesis = aws_stack.connect_to_service("kinesis")
+        kinesis = connect_to().kinesis
         stream_name = find_stream_for_consumer(consumer_arn)
         iter_type = starting_position["Type"]
         kwargs = {}
         starting_sequence_number = starting_position.get("SequenceNumber") or "0"
         if iter_type in ["AT_SEQUENCE_NUMBER", "AFTER_SEQUENCE_NUMBER"]:
             kwargs["StartingSequenceNumber"] = starting_sequence_number
         elif iter_type in ["AT_TIMESTAMP"]:
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/logs/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,30 +31,31 @@
     PutLogEventsResponse,
     ResourceNotFoundException,
     SequenceToken,
     TagKeyList,
     TagList,
     Tags,
 )
+from localstack.aws.connect import connect_to
 from localstack.services import moto
 from localstack.services.logs.models import get_moto_logs_backend, logs_stores
 from localstack.services.moto import call_moto
 from localstack.services.plugins import ServiceLifecycleHook
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.aws.arns import extract_region_from_arn
 from localstack.utils.common import is_number
 from localstack.utils.patch import patch
 
 LOG = logging.getLogger(__name__)
 
 
 class LogsProvider(LogsApi, ServiceLifecycleHook):
     def __init__(self):
         super().__init__()
-        self.cw_client = aws_stack.connect_to_service("cloudwatch")
+        self.cw_client = connect_to().cloudwatch
 
     def put_log_events(
         self,
         context: RequestContext,
         log_group_name: LogGroupName,
         log_stream_name: LogStreamName,
         log_events: InputLogEvents,
@@ -247,38 +248,36 @@
 
     log_group = self.groups.get(log_group_name)
 
     if not log_group:
         raise ResourceNotFoundException("The specified log group does not exist.")
 
     if ":lambda:" in destination_arn:
-        client = aws_stack.connect_to_service(
-            "lambda", region_name=extract_region_from_arn(destination_arn)
-        )
+        client = connect_to(region_name=extract_region_from_arn(destination_arn)).awslambda
         lambda_name = arns.lambda_function_name(destination_arn)
         try:
             client.get_function(FunctionName=lambda_name)
         except Exception:
             raise InvalidParameterException(
                 "destinationArn for vendor lambda cannot be used with roleArn"
             )
 
     elif ":kinesis:" in destination_arn:
-        client = aws_stack.connect_to_service("kinesis")
+        client = connect_to().kinesis
         stream_name = arns.kinesis_stream_name(destination_arn)
         try:
             client.describe_stream(StreamName=stream_name)
         except Exception:
             raise InvalidParameterException(
                 "Could not deliver test message to specified Kinesis stream. "
                 "Check if the given kinesis stream is in ACTIVE state. "
             )
 
     elif ":firehose:" in destination_arn:
-        client = aws_stack.connect_to_service("firehose")
+        client = connect_to().firehose
         firehose_name = arns.firehose_name(destination_arn)
         try:
             client.describe_delivery_stream(DeliveryStreamName=firehose_name)
         except Exception:
             raise InvalidParameterException(
                 "Could not deliver test message to specified Firehose stream. "
                 "Check if the given Firehose stream is in ACTIVE state."
@@ -338,29 +337,27 @@
         output = io.BytesIO()
         with GzipFile(fileobj=output, mode="w") as f:
             f.write(json.dumps(data, separators=(",", ":")).encode("utf-8"))
         payload_gz_encoded = output.getvalue()
         event = {"awslogs": {"data": base64.b64encode(output.getvalue()).decode("utf-8")}}
 
         if ":lambda:" in self.destination_arn:
-            client = aws_stack.connect_to_service(
-                "lambda", region_name=extract_region_from_arn(self.destination_arn)
-            )
+            client = connect_to(region_name=extract_region_from_arn(self.destination_arn)).awslambda
             lambda_name = arns.lambda_function_name(self.destination_arn)
             client.invoke(FunctionName=lambda_name, Payload=json.dumps(event))
         if ":kinesis:" in self.destination_arn:
-            client = aws_stack.connect_to_service("kinesis")
+            client = connect_to().kinesis
             stream_name = arns.kinesis_stream_name(self.destination_arn)
             client.put_record(
                 StreamName=stream_name,
                 Data=payload_gz_encoded,
                 PartitionKey=log_group_name,
             )
         if ":firehose:" in self.destination_arn:
-            client = aws_stack.connect_to_service("firehose")
+            client = connect_to().firehose
             firehose_name = arns.firehose_name(self.destination_arn)
             client.put_record(
                 DeliveryStreamName=firehose_name,
                 Record={"Data": payload_gz_encoded},
             )
     return "{:056d}".format(self.upload_sequence_token)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/provider_stream.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/provider_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from botocore.client import ClientError
 from moto.s3.exceptions import InvalidFilterRuleName, MissingBucket
 from moto.s3.models import FakeBucket
 from requests.models import Request, Response
 
 from localstack import config, constants
 from localstack.aws.api import CommonServiceException
+from localstack.aws.connect import connect_to
 from localstack.aws.protocol.serializer import gen_amzn_requestid
 from localstack.config import get_protocol as get_service_protocol
 from localstack.services.generic_proxy import ProxyListener
 from localstack.services.generic_proxy import append_cors_headers as _append_default_cors_headers
 from localstack.services.generic_proxy import is_cors_origin_allowed
 from localstack.services.s3 import multipart_content
 from localstack.services.s3.s3_utils import (
@@ -324,15 +325,15 @@
     if not event_type_matches(notification["Event"], action, api_method) or not filter_rules_match(
         notification.get("Filter"), object_path
     ):
         return
 
     key = unquote(object_path.replace("//", "/"))[1:]
 
-    s3_client = aws_stack.connect_to_service("s3")
+    s3_client = connect_to().s3
     object_data = {}
     try:
         object_data = s3_client.head_object(Bucket=bucket_name, Key=key)
     except botocore.exceptions.ClientError:
         pass
 
     source_ip = headers.get("X-Forwarded-For", "127.0.0.1").split(",")[0]
@@ -348,29 +349,29 @@
         config_id=notification["Id"],
         source_ip=source_ip,
     )
     message = json.dumps(message)
 
     if notification.get("Queue"):
         region = arns.extract_region_from_arn(notification["Queue"])
-        sqs_client = aws_stack.connect_to_service("sqs", region_name=region)
+        sqs_client = connect_to(region_name=region).sqs
         try:
             queue_url = arns.sqs_queue_url_for_arn(notification["Queue"])
             sqs_client.send_message(
                 QueueUrl=queue_url,
                 MessageBody=message,
                 MessageSystemAttributes=create_sqs_system_attributes(headers),
             )
         except Exception as e:
             LOGGER.warning(
                 f"Unable to send notification for S3 bucket \"{bucket_name}\" to SQS queue \"{notification['Queue']}\": {e}",
             )
     if notification.get("Topic"):
         region = arns.extract_region_from_arn(notification["Topic"])
-        sns_client = aws_stack.connect_to_service("sns", region_name=region)
+        sns_client = connect_to(region_name=region).sns
         try:
             sns_client.publish(
                 TopicArn=notification["Topic"],
                 Message=message,
                 Subject="Amazon S3 Notification",
             )
         except Exception as e:
@@ -379,35 +380,33 @@
             )
     # CloudFunction and LambdaFunction are semantically identical
     lambda_function_config = notification.get("CloudFunction") or notification.get("LambdaFunction")
     if lambda_function_config:
         # make sure we don't run into a socket timeout
         region = arns.extract_region_from_arn(lambda_function_config)
         connection_config = botocore.config.Config(read_timeout=300)
-        lambda_client = aws_stack.connect_to_service(
-            "lambda", config=connection_config, region_name=region
-        )
+        lambda_client = connect_to(config=connection_config, region_name=region).awslambda
         try:
             lambda_client.invoke(
                 FunctionName=lambda_function_config,
                 InvocationType="Event",
                 Payload=message,
             )
         except Exception:
             LOGGER.warning(
                 f'Unable to send notification for S3 bucket "{bucket_name}" to Lambda function "{lambda_function_config}".'
             )
 
     if "EventBridge" in notification:
-        s3api_client = aws_stack.connect_to_service("s3")
+        s3api_client = connect_to().s3
         region = (
             s3api_client.get_bucket_location(Bucket=bucket_name)["LocationConstraint"]
             or config.DEFAULT_REGION
         )
-        events_client = aws_stack.connect_to_service("events", region_name=region)
+        events_client = connect_to(region_name=region).events
 
         entry = {
             "Source": "aws.s3",
             "Resources": [f"arn:aws:s3:::{bucket_name}"],
             "Detail": {
                 "version": version_id or "0",
                 "bucket": {"name": bucket_name},
@@ -778,15 +777,15 @@
     # Fix content type for Range requests - https://github.com/localstack/localstack/issues/1259
     if "Range" not in headers:
         return
 
     if response.status_code >= 400:
         return
 
-    s3_client = aws_stack.connect_to_service("s3")
+    s3_client = connect_to().s3
     path = urlparse(unquote(path)).path
     key_name = extract_key_name(headers, path)
     result = s3_client.head_object(Bucket=bucket_name, Key=key_name)
     content_type = result["ContentType"]
     if response.headers.get("Content-Type") == "text/html; charset=utf-8":
         response.headers["Content-Type"] = content_type
 
@@ -1016,15 +1015,15 @@
 
 def bucket_exists(bucket_name):
     """Tests for the existence of the specified bucket. Returns the error code
     if the bucket does not exist (200 if the bucket does exist).
     """
     bucket_name = normalize_bucket_name(bucket_name)
 
-    s3_client = aws_stack.connect_to_service("s3")
+    s3_client = connect_to().s3
     try:
         s3_client.head_bucket(Bucket=bucket_name)
     except ClientError as err:
         error_code = err.response.get("Error").get("Code")
         return False, error_code
 
     return True, 200
@@ -1790,15 +1789,15 @@
                 response.headers["Content-Length"] = str(len(response._content or ""))
 
             # convert to chunked encoding, for compatibility with certain SDKs (e.g., AWS PHP SDK)
             convert_to_chunked_encoding(method, path, response)
 
 
 def serve_static_website(headers, path, bucket_name):
-    s3_client = aws_stack.connect_to_service("s3")
+    s3_client = connect_to().s3
 
     # check if bucket exists
     try:
         s3_client.head_bucket(Bucket=bucket_name)
     except ClientError:
         return no_such_bucket(bucket_name, headers.get("x-amz-request-id"), 404)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_starter.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from moto.s3 import models as s3_models
 from moto.s3 import responses as s3_responses
 from moto.s3.exceptions import MissingBucket, S3ClientError
 from moto.s3.responses import S3_ALL_MULTIPARTS, MalformedXML, minidom
 from moto.s3.utils import undo_clean_key_name
 
 from localstack import config
+from localstack.aws.connect import connect_to
 from localstack.services.infra import start_moto_server
 from localstack.services.s3 import constants as s3_constants
 from localstack.services.s3 import s3_listener, s3_utils
-from localstack.utils.aws import aws_stack
 from localstack.utils.collections import get_safe
 from localstack.utils.common import get_free_tcp_port, wait_for_port_open
 from localstack.utils.patch import patch
 from localstack.utils.server import multiserver
 
 LOG = logging.getLogger(__name__)
 
@@ -35,17 +35,15 @@
 def check_s3(expect_shutdown=False, print_error=False):
     out = None
     try:
         # wait for port to be opened
         wait_for_port_open(s3_listener.PORT_S3_BACKEND)
         # check S3
         endpoint_url = f"http://127.0.0.1:{s3_listener.PORT_S3_BACKEND}"
-        out = aws_stack.connect_to_service(
-            service_name="s3", endpoint_url=endpoint_url
-        ).list_buckets()
+        out = connect_to(endpoint_url=endpoint_url).s3.list_buckets()
     except Exception:
         if print_error:
             LOG.exception("S3 health check failed")
     if expect_shutdown:
         assert out is None
     else:
         assert out and isinstance(out.get("Buckets"), list)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,22 @@
     LifecycleRule,
     LifecycleRules,
     MethodNotAllowed,
     NoSuchBucket,
     NoSuchKey,
     ObjectKey,
 )
+from localstack.aws.connect import connect_to
 from localstack.services.s3.constants import (
     S3_VIRTUAL_HOST_FORWARDED_HEADER,
     SIGNATURE_V2_PARAMS,
     SIGNATURE_V4_PARAMS,
     VALID_CANNED_ACLS_BUCKET,
 )
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.aws.arns import parse_arn
 from localstack.utils.strings import checksum_crc32, checksum_crc32c, hash_sha1, hash_sha256
 
 checksum_keys = ["ChecksumSHA1", "ChecksumSHA256", "ChecksumCRC32", "ChecksumCRC32C"]
 
 BUCKET_NAME_REGEX = (
     r"(?=^.{3,63}$)(?!^(\d+\.)+\d+$)"
@@ -311,15 +312,15 @@
         # recreate the ARN manually with the bucket region and bucket owner
         # if the KMS key is cross-account, user should provide an ARN and not a KeyId
         kms_key = arns.kms_key_arn(
             key_id=key_id, account_id=bucket.account_id, region_name=bucket.region_name
         )
 
     # the KMS key should be in the same region as the bucket, create the client in the bucket region
-    kms_client = aws_stack.connect_to_service("kms", region_name=bucket.region_name)
+    kms_client = connect_to(region_name=bucket.region_name).kms
     try:
         key = kms_client.describe_key(KeyId=kms_key)
         if not key["KeyMetadata"]["Enabled"]:
             if key["KeyMetadata"]["KeyState"] == "PendingDeletion":
                 raise CommonServiceException(
                     code="KMS.KMSInvalidStateException",
                     message=f'{key["KeyMetadata"]["Arn"]} is pending deletion.',
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/secretsmanager/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,17 @@
     UpdateSecretRequest,
     UpdateSecretResponse,
     UpdateSecretVersionStageRequest,
     UpdateSecretVersionStageResponse,
     ValidateResourcePolicyRequest,
     ValidateResourcePolicyResponse,
 )
+from localstack.aws.connect import connect_to
 from localstack.services.moto import call_moto
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.patch import patch
 from localstack.utils.strings import short_uid
 from localstack.utils.time import today_no_time
 
 # Constants.
 AWSPREVIOUS: Final[str] = "AWSPREVIOUS"
 AWSPENDING: Final[str] = "AWSPENDING"
@@ -561,15 +562,15 @@
             rotation_period = rotation_rules[rotation_days]
             if rotation_period < 1 or rotation_period > 1000:
                 msg = "RotationRules.AutomaticallyAfterDays " "must be within 1-1000."
                 raise InvalidParameterException(msg)
 
     rotation_func = None
     try:
-        lm_client = aws_stack.connect_to_service("lambda", region_name=self.region_name)
+        lm_client = connect_to(region_name=self.region_name).awslambda
         get_func_res = lm_client.get_function(FunctionName=rotation_lambda_arn)
         lm_spec = get_func_res["Configuration"]
         lm_spec["Code"] = {"ZipFile": str(short_uid())}
         rotation_func = LambdaFunction(self.account_id, lm_spec, self.region_name)
     except Exception:
         # Fall through to ResourceNotFoundException.
         pass
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/ses/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,22 @@
     SendTemplatedEmailResponse,
     SesApi,
     TemplateData,
     TemplateName,
     VerificationAttributes,
     VerificationStatus,
 )
+from localstack.aws.connect import connect_to
 from localstack.constants import TEST_AWS_SECRET_ACCESS_KEY
 from localstack.http import Resource, Response
 from localstack.services.internal import DeprecatedResource, get_internal_apis
 from localstack.services.moto import call_moto
 from localstack.services.plugins import ServiceLifecycleHook
 from localstack.services.ses.models import SentEmail, SentEmailBody
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import arns
 from localstack.utils.files import mkdir
 from localstack.utils.strings import long_uid, to_str
 from localstack.utils.time import timestamp, timestamp_millis
 
 if TYPE_CHECKING:
     from mypy_boto3_sns import SNSClient
 
@@ -641,13 +642,12 @@
 
     @staticmethod
     def _client_for_topic(topic_arn: str) -> "SNSClient":
         arn_parameters = arns.parse_arn(topic_arn)
         region = arn_parameters["region"]
         access_key_id = arn_parameters["account"]
 
-        return aws_stack.connect_to_service(
-            "sns",
+        return connect_to(
             region_name=region,
             aws_access_key_id=access_key_id,
             aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY,
-        )
+        ).sns
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sns/publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from localstack.services.sns import constants as sns_constants
 from localstack.services.sns.models import (
     SnsApplicationPlatforms,
     SnsMessage,
     SnsStore,
     SnsSubscription,
 )
-from localstack.utils.aws import aws_stack
 from localstack.utils.aws.arns import (
     extract_region_from_arn,
     extract_resource_from_arn,
     parse_arn,
     sqs_queue_url_for_arn,
 )
 from localstack.utils.aws.aws_responses import create_sqs_system_attributes
@@ -701,15 +700,15 @@
 
 def get_attributes_for_application_endpoint(endpoint_arn: str) -> Tuple[Dict, Dict]:
     """
     Retrieve the attributes necessary to send a message directly to the platform (credentials and token)
     :param endpoint_arn:
     :return:
     """
-    sns_client = aws_stack.connect_to_service("sns")
+    sns_client = connect_to().sns
     # TODO: we should access this from the moto store directly
     endpoint_attributes = sns_client.get_endpoint_attributes(EndpointArn=endpoint_arn)
 
     app_platform_arn = get_application_platform_arn_from_endpoint_arn(endpoint_arn)
     app = sns_client.get_platform_application_attributes(PlatformApplicationArn=app_platform_arn)
 
     return app.get("Attributes", {}), endpoint_attributes.get("Attributes", {})
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
     RegisterTargetWithMaintenanceWindowResult,
     RegisterTaskWithMaintenanceWindowResult,
     ServiceRole,
     SsmApi,
     TagList,
     Targets,
 )
+from localstack.aws.connect import connect_to
 from localstack.services.moto import call_moto, call_moto_with_request
-from localstack.utils.aws import aws_stack
 from localstack.utils.collections import remove_attributes
 from localstack.utils.objects import keys_to_lower
 from localstack.utils.patch import patch
 
 PARAM_PREFIX_SECRETSMANAGER = "/aws/reference/secretsmanager"
 
 
@@ -352,15 +352,15 @@
             param_name = "/%s" % param_name
         return param_name
 
     @staticmethod
     def _get_secrets_information(
         name: ParameterName, resource_name: str
     ) -> Optional[GetParameterResult]:
-        client = aws_stack.connect_to_service("secretsmanager")
+        client = connect_to().secretsmanager
         try:
             secret_info = client.get_secret_value(SecretId=resource_name)
             secret_info.pop("ResponseMetadata", None)
             created_date_timestamp = time.mktime(secret_info["CreatedDate"].timetuple())
             secret_info["CreatedDate"] = created_date_timestamp
             secret_info_lower = keys_to_lower(
                 remove_attributes(copy.deepcopy(secret_info), ["ARN"])
@@ -377,15 +377,15 @@
             }
             return GetParameterResult(**result)
         except client.exceptions.ResourceNotFoundException:
             return None
 
     @staticmethod
     def _get_params_and_secrets(names: ParameterNameList) -> GetParametersResult:
-        ssm_client = aws_stack.connect_to_service("ssm")
+        ssm_client = connect_to().ssm
         result = {"Parameters": [], "InvalidParameters": []}
 
         for name in names:
             if name.startswith(PARAM_PREFIX_SECRETSMANAGER):
                 secret = SsmProvider._get_secrets_information(
                     name, name[len(PARAM_PREFIX_SECRETSMANAGER) + 1 :]
                 )
@@ -405,33 +405,33 @@
                     result["InvalidParameters"].append(name)
 
         return GetParametersResult(**result)
 
     @staticmethod
     def _notify_event_subscribers(name: ParameterName, operation: str):
         """Publish an EventBridge event to notify subscribers of changes."""
-        events = aws_stack.connect_to_service("events")
+        events = connect_to().events
         detail = {"name": name, "operation": operation}
         event = {
             "Source": "aws.ssm",
             "Detail": json.dumps(detail),
             "DetailType": "Parameter Store Change",
         }
         events.put_events(Entries=[event])
 
 
 @patch(SimpleSystemManagerBackend.get_maintenance_window)
 def get_maintenance_window(fn, self, window_id):
     """Get a maintenance window by ID."""
-    store = ssm_backends[aws_stack.get_aws_account_id()][aws_stack.get_region()]
+    store = ssm_backends[self.account_id][self.region_name]
     if not store.windows.get(window_id):
         raise DoesNotExistException(window_id)
     return fn(self, window_id)
 
 
 @patch(SimpleSystemManagerBackend.delete_maintenance_window)
 def delete_maintenance_window(fn, self, window_id):
     """Delete a maintenance window by ID."""
-    store = ssm_backends[aws_stack.get_aws_account_id()][aws_stack.get_region()]
+    store = ssm_backends[self.account_id][self.region_name]
     if not store.windows.get(window_id):
         raise DoesNotExistException(window_id)
     return fn(self, window_id)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-2.1.1.dev20230714101424/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from json import JSONDecodeError
 from typing import Any, Final, Optional
 
 from localstack.aws.api.lambda_ import InvocationResponse
+from localstack.aws.connect import connect_to
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.utils.encoding import to_json_str
-from localstack.utils.aws.aws_stack import connect_to_service
 from localstack.utils.collections import select_from_typed_dict
 from localstack.utils.run import to_str
 from localstack.utils.strings import to_bytes
 
 
 class LambdaFunctionErrorException(Exception):
     function_error: Final[Optional[str]]
@@ -17,15 +17,15 @@
 
     def __init__(self, function_error: Optional[str], payload: str):
         self.function_error = function_error
         self.payload = payload
 
 
 def exec_lambda_function(env: Environment, parameters: dict) -> None:
-    lambda_client = connect_to_service("lambda")
+    lambda_client = connect_to().awslambda
     invocation_resp: InvocationResponse = lambda_client.invoke(**parameters)
 
     func_error: Optional[str] = invocation_resp.get("FunctionError")
     if func_error:
         payload = json.loads(to_str(invocation_resp["Payload"].read()))
         payload_str = json.dumps(payload, separators=(",", ":"))
         raise LambdaFunctionErrorException(func_error, payload_str)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import subprocess
 
 from localstack import config
 from localstack.aws.accounts import get_aws_account_id
+from localstack.aws.connect import connect_to
 from localstack.services.infra import do_run, log_startup_message
 from localstack.services.stepfunctions.packages import stepfunctions_local_package
 from localstack.utils.aws import aws_stack
 from localstack.utils.common import wait_for_port_open
 from localstack.utils.net import wait_for_port_closed
 from localstack.utils.run import ShellCommandThread, wait_for_process_to_be_killed
 from localstack.utils.sync import retry
@@ -109,17 +110,15 @@
 
 
 def check_stepfunctions(expect_shutdown: bool = False, print_error: bool = False) -> None:
     out = None
     try:
         wait_for_port_open(config.LOCAL_PORT_STEPFUNCTIONS, sleep_time=2)
         endpoint_url = f"http://127.0.0.1:{config.LOCAL_PORT_STEPFUNCTIONS}"
-        out = aws_stack.connect_to_service(
-            service_name="stepfunctions", endpoint_url=endpoint_url
-        ).list_state_machines()
+        out = connect_to(endpoint_url=endpoint_url).stepfunctions.list_state_machines()
     except Exception:
         if print_error:
             LOG.exception("StepFunctions health check failed")
 
     if expect_shutdown:
         assert out is None
     else:
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230714101424/localstack/services/transcribe/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from localstack.packages.ffmpeg import ffmpeg_package
 from localstack.services.plugins import ServiceLifecycleHook
 from localstack.services.s3.utils import (
     get_bucket_and_key_from_presign_url,
     get_bucket_and_key_from_s3_uri,
 )
 from localstack.services.transcribe.models import TranscribeStore, transcribe_stores
-from localstack.utils.aws import aws_stack
 from localstack.utils.files import new_tmp_file
 from localstack.utils.http import download
 from localstack.utils.run import run
 from localstack.utils.threads import start_thread
 
 LOG = logging.getLogger(__name__)
 
@@ -259,15 +258,15 @@
         failure_reason = None
 
         try:
             LOG.debug("Starting transcription: %s", job_name)
 
             # Get file from S3
             file_path = new_tmp_file()
-            s3_client = aws_stack.connect_to_service("s3")
+            s3_client = connect_to().s3
             s3_path = job["Media"]["MediaFileUri"]
             bucket, _, key = s3_path.removeprefix("s3://").partition("/")
             s3_client.download_file(Bucket=bucket, Key=key, Filename=file_path)
 
             ffmpeg_bin = ffmpeg_package.get_installer().get_ffmpeg_path()
             ffprobe_bin = ffmpeg_package.get_installer().get_ffprobe_path()
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/state/core.py` & `localstack-core-2.1.1.dev20230714101424/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230714101424/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230714101424/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230714101424/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230714101424/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/arns.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import re
 from functools import cache
 from typing import Optional, TypedDict
 
 from botocore.utils import ArnParser, InvalidArnException
 
 from localstack.aws.accounts import DEFAULT_AWS_ACCOUNT_ID, get_aws_account_id
-from localstack.constants import INTERNAL_AWS_ACCESS_KEY_ID, INTERNAL_AWS_SECRET_ACCESS_KEY
-from localstack.utils.aws.aws_stack import connect_to_service, get_region, get_valid_regions
+from localstack.aws.connect import connect_to
+from localstack.utils.aws.aws_stack import get_region, get_valid_regions
 
 # set up logger
 LOG = logging.getLogger(__name__)
 
 # TODO: extract ARN utils into separate file!
 
 _arn_parser = ArnParser()
@@ -31,20 +31,15 @@
         region_name = arn["region"]
         queue_name = arn["resource"]
     except InvalidArnException:
         account_id = DEFAULT_AWS_ACCOUNT_ID
         region_name = None
         queue_name = queue_arn
 
-    sqs_client = connect_to_service(
-        "sqs",
-        region_name=region_name,
-        aws_access_key_id=INTERNAL_AWS_ACCESS_KEY_ID,
-        aws_secret_access_key=INTERNAL_AWS_SECRET_ACCESS_KEY,
-    )
+    sqs_client = connect_to(region_name=region_name).sqs
     result = sqs_client.get_queue_url(QueueName=queue_name, QueueOwnerAWSAccountId=account_id)[
         "QueueUrl"
     ]
     return result
 
 
 # TODO: remove and merge with sqs_queue_url_for_arn(..) above!!
@@ -194,15 +189,15 @@
 def lambda_function_or_layer_arn(
     type, entity_name, version=None, account_id=None, region_name=None
 ):
     pattern = "arn:([a-z-]+):lambda:.*:.*:(function|layer):.*"
     if re.match(pattern, entity_name):
         return entity_name
     if ":" in entity_name:
-        client = connect_to_service("lambda")
+        client = connect_to().awslambda
         entity_name, _, alias = entity_name.rpartition(":")
         try:
             alias_response = client.get_alias(FunctionName=entity_name, Name=alias)
             version = alias_response["FunctionVersion"]
 
         except Exception as e:
             msg = f"Alias {alias} of {entity_name} not found"
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/aws_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from localstack.aws.accounts import get_aws_access_key_id, get_aws_account_id
 from localstack.constants import (
     APPLICATION_AMZ_JSON_1_0,
     APPLICATION_AMZ_JSON_1_1,
     APPLICATION_X_WWW_FORM_URLENCODED,
     ENV_DEV,
     HEADER_LOCALSTACK_ACCOUNT_ID,
+    INTERNAL_AWS_ACCESS_KEY_ID,
     LOCALHOST,
     MAX_POOL_CONNECTIONS,
     REGION_LOCAL,
     S3_VIRTUAL_HOSTNAME,
     TEST_AWS_ACCESS_KEY_ID,
     TEST_AWS_SECRET_ACCESS_KEY,
 )
@@ -189,18 +190,26 @@
 
 
 def get_boto3_region() -> str:
     """Return the region name, as determined from the environment when creating a new boto3 session"""
     return boto3.session.Session().region_name
 
 
-def is_internal_call_context(headers):
+# TODO: remove this and use the `is_internal_call` property of RequestContext
+def is_internal_call_context(headers) -> bool:
     """Return whether we are executing in the context of an internal API call, i.e.,
     the case where one API uses a boto3 client to call another API internally."""
-    return HEADER_LOCALSTACK_ACCOUNT_ID in headers.keys()
+    if HEADER_LOCALSTACK_ACCOUNT_ID in headers.keys():
+        # TODO: Used by the old client, marked for removal
+        return True
+
+    if INTERNAL_AWS_ACCESS_KEY_ID in headers.get("Authorization", ""):
+        return True
+
+    return False
 
 
 def get_local_service_url(service_name_or_port: Union[str, int]) -> str:
     """Return the local service URL for the given service name or port."""
     if isinstance(service_name_or_port, int):
         return f"{config.get_protocol()}://{LOCALHOST}:{service_name_or_port}"
     service_name = service_name_or_port
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/message_forwarding.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from localstack.utils import collections
 from localstack.utils.aws.arns import (
     extract_account_id_from_arn,
     extract_region_from_arn,
     firehose_name,
     get_sqs_queue_url,
 )
-from localstack.utils.aws.aws_stack import connect_to_service
 from localstack.utils.http import add_path_parameters_to_url, add_query_params_to_url
 from localstack.utils.http import safe_requests as requests
 from localstack.utils.strings import to_bytes, to_str
 from localstack.utils.time import now_utc
 
 LOG = logging.getLogger(__name__)
 
@@ -71,15 +70,15 @@
         )
         queue_url = get_sqs_queue_url(target_arn)
         msg_group_id = collections.get_safe(target_attributes, "$.SqsParameters.MessageGroupId")
         kwargs = {"MessageGroupId": msg_group_id} if msg_group_id else {}
         sqs_client.send_message(QueueUrl=queue_url, MessageBody=json.dumps(event), **kwargs)
 
     elif ":states:" in target_arn:
-        stepfunctions_client = connect_to_service("stepfunctions", region_name=region)
+        stepfunctions_client = connect_to(region_name=region).stepfunctions
         stepfunctions_client.start_execution(stateMachineArn=target_arn, input=json.dumps(event))
 
     elif ":firehose:" in target_arn:
         delivery_stream_name = firehose_name(target_arn)
         firehose_client = clients.firehose.request_metadata(
             service_principal=source_service, source_arn=source_arn
         )
@@ -208,15 +207,15 @@
 def send_event_to_api_destination(target_arn, event, http_parameters: Optional[Dict] = None):
     """Send an event to an EventBridge API destination
     See https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-api-destinations.html"""
 
     # ARN format: ...:api-destination/{name}/{uuid}
     region = extract_region_from_arn(target_arn)
     api_destination_name = target_arn.split(":")[-1].split("/")[1]
-    events_client = connect_to_service("events", region_name=region)
+    events_client = connect_to(region_name=region).events
     destination = events_client.describe_api_destination(Name=api_destination_name)
 
     # get destination endpoint details
     method = destination.get("HttpMethod", "GET")
     endpoint = destination.get("InvocationEndpoint")
     state = destination.get("ApiDestinationState") or "ACTIVE"
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/queries.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,23 @@
+from localstack.aws.connect import connect_to
 from localstack.utils.aws.arns import extract_region_from_arn, get_sqs_queue_url
-from localstack.utils.aws.aws_stack import connect_to_service
 from localstack.utils.strings import to_str
 
 
 def sqs_receive_message(queue_arn):
     region_name = extract_region_from_arn(queue_arn)
-    client = connect_to_service("sqs", region_name=region_name)
+    client = connect_to(region_name=region_name).sqs
     queue_url = get_sqs_queue_url(queue_arn)
     response = client.receive_message(QueueUrl=queue_url)
     return response
 
 
-def get_apigateway_integration(api_id, method, path, env=None):
-    apigateway = connect_to_service(service_name="apigateway", client=True, env=env)
-
-    resources = apigateway.get_resources(restApiId=api_id, limit=100)
-    resource_id = None
-    for r in resources["items"]:
-        if r["path"] == path:
-            resource_id = r["id"]
-    if not resource_id:
-        raise Exception('Unable to find apigateway integration for path "%s"' % path)
-
-    integration = apigateway.get_integration(
-        restApiId=api_id, resourceId=resource_id, httpMethod=method
-    )
-    return integration
-
-
 def get_apigateway_resource_for_path(api_id, path, parent=None, resources=None):
     if resources is None:
-        apigateway = connect_to_service(service_name="apigateway")
+        apigateway = connect_to().apigateway
         resources = apigateway.get_resources(restApiId=api_id, limit=100)
     if not isinstance(path, list):
         path = path.split("/")
     if not path:
         return parent
     for resource in resources:
         if resource["pathPart"] == path[0] and (not parent or parent["id"] == resource["parentId"]):
@@ -44,15 +27,15 @@
     return None
 
 
 def get_apigateway_path_for_resource(
     api_id, resource_id, path_suffix="", resources=None, region_name=None
 ):
     if resources is None:
-        apigateway = connect_to_service(service_name="apigateway", region_name=region_name)
+        apigateway = connect_to(region_name=region_name).apigateway
         resources = apigateway.get_resources(restApiId=api_id, limit=100)["items"]
     target_resource = list(filter(lambda res: res["id"] == resource_id, resources))[0]
     path_part = target_resource.get("pathPart", "")
     if path_suffix:
         if path_part:
             path_suffix = "%s/%s" % (path_part, path_suffix)
     else:
@@ -65,16 +48,16 @@
         parent_id,
         path_suffix=path_suffix,
         resources=resources,
         region_name=region_name,
     )
 
 
-def kinesis_get_latest_records(stream_name, shard_id, count=10, env=None, client=None):
-    kinesis = client or connect_to_service("kinesis", env=env)
+def kinesis_get_latest_records(stream_name, shard_id, count=10, client=None):
+    kinesis = client or connect_to().kinesis
     result = []
     response = kinesis.get_shard_iterator(
         StreamName=stream_name, ShardId=shard_id, ShardIteratorType="TRIM_HORIZON"
     )
     shard_iterator = response["ShardIterator"]
     while shard_iterator:
         records_response = kinesis.get_records(ShardIterator=shard_iterator)
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,31 @@
+from localstack.aws.connect import connect_to
 from localstack.constants import AWS_REGION_US_EAST_1
 from localstack.utils.aws.aws_models import KinesisStream
-from localstack.utils.aws.aws_stack import (
-    LOG,
-    connect_to_resource,
-    connect_to_service,
-    get_environment,
-)
+from localstack.utils.aws.aws_stack import LOG, connect_to_resource
 from localstack.utils.functions import run_safe
 from localstack.utils.sync import poll_condition
 
 
-def create_sqs_queue(queue_name, env=None):
-    env = get_environment(env)
-    # queue
-    conn = connect_to_service("sqs", env=env)
-    return conn.create_queue(QueueName=queue_name)
+def create_sqs_queue(queue_name):
+    return connect_to().sqs.create_queue(QueueName=queue_name)
 
 
 def get_or_create_bucket(bucket_name: str, s3_client=None):
-    s3_client = s3_client or connect_to_service("s3")
+    s3_client = s3_client or connect_to().s3
     try:
         return s3_client.head_bucket(Bucket=bucket_name)
     except Exception:
         return create_s3_bucket(bucket_name, s3_client=s3_client)
 
 
 def create_s3_bucket(bucket_name: str, s3_client=None):
     """Creates a bucket in the region that is associated with the current request
     context, or with the given boto3 S3 client, if specified."""
-    s3_client = s3_client or connect_to_service("s3")
+    s3_client = s3_client or connect_to().s3
     region = s3_client.meta.region_name
     kwargs = {}
     if region != AWS_REGION_US_EAST_1:
         kwargs = {"CreateBucketConfiguration": {"LocationConstraint": region}}
     return s3_client.create_bucket(Bucket=bucket_name, **kwargs)
 
 
@@ -42,15 +35,15 @@
     stream_view_type: str = None,
     region_name: str = None,
     client=None,
     wait_for_active: bool = True,
 ):
     """Utility method to create a DynamoDB table"""
 
-    dynamodb = client or connect_to_service("dynamodb", region_name=region_name)
+    dynamodb = client or connect_to(region_name=region_name).dynamodb
     stream_spec = {"StreamEnabled": False}
     key_schema = [{"AttributeName": partition_key, "KeyType": "HASH"}]
     attr_defs = [{"AttributeName": partition_key, "AttributeType": "S"}]
     if stream_view_type is not None:
         stream_spec = {"StreamEnabled": True, "StreamViewType": stream_view_type}
     table = None
     try:
@@ -79,24 +72,23 @@
 
 def create_api_gateway(
     name,
     description=None,
     resources=None,
     stage_name=None,
     enabled_api_keys=None,
-    env=None,
     usage_plan_name=None,
     region_name=None,
     auth_creator_func=None,  # function that receives an api_id and returns an authorizer_id
     client=None,
 ):
     if enabled_api_keys is None:
         enabled_api_keys = []
     if not client:
-        client = connect_to_service("apigateway", env=env, region_name=region_name)
+        client = connect_to(region_name=region_name).apigateway
     resources = resources or []
     stage_name = stage_name or "testing"
     usage_plan_name = usage_plan_name or "Basic Usage"
     description = description or 'Test description for API "%s"' % name
 
     LOG.info('Creating API resources under API Gateway "%s".', name)
     api = client.create_rest_api(name=name, description=description)
@@ -133,30 +125,29 @@
             # create integrations for this API resource/method
             integrations = method["integrations"]
             create_api_gateway_integrations(
                 api_id,
                 api_resource["id"],
                 method,
                 integrations,
-                env=env,
                 region_name=region_name,
                 client=client,
             )
     # deploy the API gateway
     client.create_deployment(restApiId=api_id, stageName=stage_name)
     return api
 
 
 def create_api_gateway_integrations(
-    api_id, resource_id, method, integrations=None, env=None, region_name=None, client=None
+    api_id, resource_id, method, integrations=None, region_name=None, client=None
 ):
     if integrations is None:
         integrations = []
     if not client:
-        client = connect_to_service("apigateway", env=env, region_name=region_name)
+        client = connect_to(region_name=region_name).apigateway
     for integration in integrations:
         req_templates = integration.get("requestTemplates") or {}
         res_templates = integration.get("responseTemplates") or {}
         success_code = integration.get("successCode") or "200"
         client_error_code = integration.get("clientErrorCode") or "400"
         server_error_code = integration.get("serverErrorCode") or "500"
         request_parameters = integration.get("requestParameters") or {}
@@ -192,17 +183,16 @@
                 restApiId=api_id,
                 resourceId=resource_id,
                 httpMethod=method["httpMethod"],
                 statusCode=response_config["code"],
             )
 
 
-def create_kinesis_stream(stream_name, shards=1, env=None, delete=False):
-    env = get_environment(env)
+def create_kinesis_stream(stream_name, shards=1, delete=False):
     stream = KinesisStream(id=stream_name, num_shards=shards)
-    conn = connect_to_service("kinesis", env=env)
+    conn = connect_to().kinesis
     stream.connect(conn)
     if delete:
         run_safe(lambda: stream.destroy(), print_error=False)
     stream.create()
     # Note: Returning the stream without awaiting its creation (via wait_for()) to avoid API call timeouts/retries.
     return stream
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from datetime import datetime, timezone
 from typing import Optional
 
 from flask import Response
 
 from localstack import config
 from localstack.aws.connect import connect_to
-from localstack.utils.aws import aws_stack
 from localstack.utils.strings import to_str
 from localstack.utils.time import now_utc
 
 LOG = logging.getLogger(__name__)
 
 
 # ---------------
@@ -53,15 +52,15 @@
     See also: https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-available-cloudwatch-metrics.html
     :param region The region that should be used for CloudWatch
     :param queue_name The name of the queue
     :param metric The metric name to be used
     :param value The value of the metric data, default: 1
     :param unit The unit of the metric data, default: "Count"
     """
-    cw_client = aws_stack.connect_to_service("cloudwatch", region_name=region)
+    cw_client = connect_to(region_name=region).cloudwatch
     try:
         cw_client.put_metric_data(
             Namespace="AWS/SQS",
             MetricData=[
                 {
                     "MetricName": metric,
                     "Dimensions": [{"Name": "QueueName", "Value": queue_name}],
@@ -96,15 +95,15 @@
     log_stream_name,
     log_output,
     start_time=None,
     auto_create_group: Optional[bool] = True,
     logs_client=None,
 ):
     start_time = start_time or int(time.time() * 1000)
-    logs_client = logs_client or aws_stack.connect_to_service("logs")
+    logs_client = logs_client or connect_to().logs
     log_output = to_str(log_output)
 
     if auto_create_group:
         # make sure that the log group exists, create it if not
         try:
             logs_client.create_log_group(logGroupName=log_group_name)
         except Exception as e:
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/testutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 import shutil
 import tempfile
 import time
 from contextlib import contextmanager
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
-from localstack.aws.connect import connect_externally_to
+from localstack.aws.connect import connect_externally_to, connect_to
 from localstack.testing.aws.util import is_aws_cloud
 from localstack.utils.aws import arns
 from localstack.utils.aws import resources as resource_utils
 
 try:
     from typing import Literal
 except ImportError:
@@ -120,16 +120,17 @@
                         rm_rf(full_name)
 
         # create zip file
         result = create_zip_file(tmp_dir, get_content=get_content)
         return result
 
 
-def delete_lambda_function(name, region_name: str = None):  # TODO: remove all occurrences
-    client = aws_stack.connect_to_service("lambda", region_name=region_name)
+# TODO: remove all occurrences
+def delete_lambda_function(name, region_name: str = None):
+    client = connect_externally_to(region_name=region_name).awslambda
     client.delete_function(FunctionName=name)
 
 
 def create_zip_file(
     file_path: str,
     zip_file: str = None,
     get_content: bool = False,
@@ -206,15 +207,15 @@
     if tags is None:
         tags = {}
     if libs is None:
         libs = []
 
     starting_position = starting_position or LAMBDA_DEFAULT_STARTING_POSITION
     runtime = runtime or LAMBDA_DEFAULT_RUNTIME
-    client = client or aws_stack.connect_to_service("lambda", region_name=region_name)
+    client = client or connect_to(region_name=region_name).awslambda
 
     # load zip file content if handler_file is specified
     if not zip_file and handler_file:
         file_content = load_file(handler_file) if os.path.exists(handler_file) else handler_file
         if libs or not handler:
             zip_file = create_lambda_archive(
                 file_content,
@@ -431,15 +432,15 @@
 
 
 def list_all_s3_objects():
     return map_all_s3_objects().values()
 
 
 def delete_all_s3_objects(buckets):
-    s3_client = aws_stack.connect_to_service("s3")
+    s3_client = connect_to().s3
     buckets = ensure_list(buckets)
     for bucket in buckets:
         keys = all_s3_object_keys(bucket)
         deletes = [{"Key": key} for key in keys]
         if deletes:
             s3_client.delete_objects(Bucket=bucket, Delete={"Objects": deletes})
 
@@ -542,15 +543,15 @@
             )
         )
     assert len(events) == expected_length
     return events
 
 
 def list_all_log_events(log_group_name: str, logs_client=None) -> List[Dict]:
-    logs = logs_client or aws_stack.connect_to_service("logs")
+    logs = logs_client or connect_to().logs
     return list_all_resources(
         lambda kwargs: logs.filter_log_events(logGroupName=log_group_name, **kwargs),
         last_token_attr_name="nextToken",
         list_attr_name="events",
     )
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230714101424/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230714062049
+Version: 2.1.1.dev20230714101424
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9534313725490198%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(2, '*

 * *                                      "'_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser')], "*

 * *                                      'delete: [0]}',*

 * * "'localstack.packages'": '{insert: [(0, '*

 * *                          "'cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package'), "*

 * *                          '(5, '*

 * *                          "'kinesis-mock/community=localstack.services.kin […]*

```diff
@@ -59,36 +59,36 @@
         "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
         "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
         "terraform/community=localstack.packages.plugins:terraform_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package"
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230714062049/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230714101424/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/pyproject.toml` & `localstack-core-2.1.1.dev20230714101424/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230714062049/setup.cfg` & `localstack-core-2.1.1.dev20230714101424/setup.cfg`

 * *Files identical despite different names*

