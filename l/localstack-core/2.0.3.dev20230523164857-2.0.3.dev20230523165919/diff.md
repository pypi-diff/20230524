# Comparing `tmp/localstack-core-2.0.3.dev20230523164857.tar.gz` & `tmp/localstack-core-2.0.3.dev20230523165919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.0.3.dev20230523164857.tar", last modified: Tue May 23 16:49:03 2023, max compression
+gzip compressed data, was "localstack-core-2.0.3.dev20230523165919.tar", last modified: Tue May 23 16:59:27 2023, max compression
```

## Comparing `localstack-core-2.0.3.dev20230523164857.tar` & `localstack-core-2.0.3.dev20230523165919.tar`

### file list

```diff
@@ -1,850 +1,850 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10815 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.865745 localstack-core-2.0.3.dev20230523164857/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.865745 localstack-core-2.0.3.dev20230523164857/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-05-23 16:48:57.000000 localstack-core-2.0.3.dev20230523164857/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.865745 localstack-core-2.0.3.dev20230523164857/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.865745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   125427 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   755668 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48662 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71916 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.869745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.873745 localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27499 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.877745 localstack-core-2.0.3.dev20230523164857/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18437 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49625 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7805 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.877745 localstack-core-2.0.3.dev20230523164857/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15553 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/contrib/thundra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.877745 localstack-core-2.0.3.dev20230523164857/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.877745 localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.877745 localstack-core-2.0.3.dev20230523164857/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.877745 localstack-core-2.0.3.dev20230523164857/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.877745 localstack-core-2.0.3.dev20230523164857/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.877745 localstack-core-2.0.3.dev20230523164857/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.881745 localstack-core-2.0.3.dev20230523164857/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.881745 localstack-core-2.0.3.dev20230523164857/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.881745 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41169 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12745 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12099 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67662 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.881745 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24219 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.885745 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8832 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.885745 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17789 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21256 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28278 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12461 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91859 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72195 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.885745 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155097 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.885745 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.885745 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17238 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    64554 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8781 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2316 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.889745 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30467 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20947 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7009 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2126 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5391 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22846 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2585 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8984 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28326 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3062 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5327 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11295 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6426 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8745 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3812 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5502 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34840 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.889745 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.889745 localstack-core-2.0.3.dev20230523164857/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.889745 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.889745 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.889745 localstack-core-2.0.3.dev20230523164857/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.889745 localstack-core-2.0.3.dev20230523164857/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22448 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19454 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35686 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.893745 localstack-core-2.0.3.dev20230523164857/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2979 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61444 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9218 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26931 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5648 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47737 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1666 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54186 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7059 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.897745 localstack-core-2.0.3.dev20230523164857/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.901745 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.901745 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.901745 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.901745 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.901745 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.905745 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.905745 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.905745 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.921744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.921744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.921744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.921744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.921744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.921744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.921744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.921744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.929744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.929744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.929744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.929744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.933744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.933744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.933744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.941744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.945744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.957744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.957744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.957744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.957744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.957744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.957744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.957744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/transcribe/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/transcribe/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12950 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.961744 localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.965744 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67425 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.965744 localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.969744 localstack-core-2.0.3.dev20230523164857/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.969744 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13471 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13278 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23998 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4512 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43017 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28846 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31840 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10057 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-05-23 16:49:03.000000 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37732 2023-05-23 16:49:03.000000 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 16:49:03.000000 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4968 2023-05-23 16:49:03.000000 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 16:49:00.000000 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5055 2023-05-23 16:49:00.000000 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2023-05-23 16:49:03.000000 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-05-23 16:49:03.000000 localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3145 2023-05-23 16:49:03.973744 localstack-core-2.0.3.dev20230523164857/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-05-23 16:18:28.000000 localstack-core-2.0.3.dev20230523164857/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.752204 localstack-core-2.0.3.dev20230523165919/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-05-23 16:59:27.752204 localstack-core-2.0.3.dev20230523165919/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10815 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.576207 localstack-core-2.0.3.dev20230523165919/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-05-23 16:59:19.000000 localstack-core-2.0.3.dev20230523165919/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   125427 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.580207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   755668 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48662 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71916 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.584207 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.588207 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.588207 localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.588207 localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27499 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.588207 localstack-core-2.0.3.dev20230523165919/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18437 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49625 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7805 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.588207 localstack-core-2.0.3.dev20230523165919/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15553 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/contrib/thundra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.588207 localstack-core-2.0.3.dev20230523165919/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.592207 localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.592207 localstack-core-2.0.3.dev20230523165919/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.592207 localstack-core-2.0.3.dev20230523165919/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.592207 localstack-core-2.0.3.dev20230523165919/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.592207 localstack-core-2.0.3.dev20230523165919/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.592207 localstack-core-2.0.3.dev20230523165919/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.592207 localstack-core-2.0.3.dev20230523165919/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.596207 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41169 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12745 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12099 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67662 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.596207 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24219 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.596207 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8832 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.600206 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17789 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21256 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28278 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12461 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91859 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72195 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.600206 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155097 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.600206 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.600206 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17238 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    64554 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8781 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2316 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.604206 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30467 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20947 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7009 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2126 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5391 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22846 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2585 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8984 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28326 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3062 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5327 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11295 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6426 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8745 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3812 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5502 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34840 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.604206 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.604206 localstack-core-2.0.3.dev20230523165919/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.604206 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.604206 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.604206 localstack-core-2.0.3.dev20230523165919/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.604206 localstack-core-2.0.3.dev20230523165919/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.604206 localstack-core-2.0.3.dev20230523165919/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22448 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19454 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35686 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.608206 localstack-core-2.0.3.dev20230523165919/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.612206 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2979 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61444 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9218 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.612206 localstack-core-2.0.3.dev20230523165919/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.612206 localstack-core-2.0.3.dev20230523165919/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26931 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.612206 localstack-core-2.0.3.dev20230523165919/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.612206 localstack-core-2.0.3.dev20230523165919/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5648 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47737 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.612206 localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1666 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54186 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7059 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.612206 localstack-core-2.0.3.dev20230523165919/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.616206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.620206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.620206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.620206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.620206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.620206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.624206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.624206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.624206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.624206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.624206 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.660205 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.728204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.728204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.728204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.728204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.728204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.728204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.728204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.728204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.736204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/transcribe/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/transcribe/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12950 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.740204 localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.744204 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67425 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.744204 localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.748204 localstack-core-2.0.3.dev20230523165919/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.748204 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.748204 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13471 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13278 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23998 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.748204 localstack-core-2.0.3.dev20230523165919/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4512 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.748204 localstack-core-2.0.3.dev20230523165919/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    44447 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33085 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.752204 localstack-core-2.0.3.dev20230523165919/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10057 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.752204 localstack-core-2.0.3.dev20230523165919/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 16:59:27.752204 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-05-23 16:59:27.000000 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37732 2023-05-23 16:59:27.000000 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 16:59:27.000000 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4968 2023-05-23 16:59:27.000000 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 16:59:23.000000 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5055 2023-05-23 16:59:23.000000 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2023-05-23 16:59:27.000000 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-05-23 16:59:27.000000 localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3145 2023-05-23 16:59:27.752204 localstack-core-2.0.3.dev20230523165919/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-05-23 16:23:58.000000 localstack-core-2.0.3.dev20230523165919/setup.py
```

### Comparing `localstack-core-2.0.3.dev20230523164857/LICENSE.txt` & `localstack-core-2.0.3.dev20230523165919/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/Makefile` & `localstack-core-2.0.3.dev20230523165919/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/README.md` & `localstack-core-2.0.3.dev20230523165919/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/bin/localstack` & `localstack-core-2.0.3.dev20230523165919/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/bin/localstack-supervisor` & `localstack-core-2.0.3.dev20230523165919/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/accounts.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/acm/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/config/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/core.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/es/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/events/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/iam/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/kms/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/logs/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/route53/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/s3/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ses/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sns/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/sts/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/support/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/swf/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/app.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/chain.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/client.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/connect.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/forwarder.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/gateway.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/analytics.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/auth.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/codec.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/cors.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/fallback.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/internal.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/legacy.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/logging.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/proxy.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/region.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/routes.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/service.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/mocking.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/op_router.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/parser.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/serializer.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/service_router.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/protocol/validate.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/proxy.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/scaffold.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/asgi.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/edge.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/hypercorn.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/werkzeug.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/serving/wsgi.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/skeleton.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/spec-patches.json` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/spec.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/aws/trace.py` & `localstack-core-2.0.3.dev20230523165919/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/cli/localstack.py` & `localstack-core-2.0.3.dev20230523165919/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/cli/lpm.py` & `localstack-core-2.0.3.dev20230523165919/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/cli/plugin.py` & `localstack-core-2.0.3.dev20230523165919/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/cli/plugins.py` & `localstack-core-2.0.3.dev20230523165919/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/cli/profiles.py` & `localstack-core-2.0.3.dev20230523165919/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/config.py` & `localstack-core-2.0.3.dev20230523165919/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/constants.py` & `localstack-core-2.0.3.dev20230523165919/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/contrib/thundra.py` & `localstack-core-2.0.3.dev20230523165919/localstack/contrib/thundra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/deprecations.py` & `localstack-core-2.0.3.dev20230523165919/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/aws.py` & `localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/extensions/api/extension.py` & `localstack-core-2.0.3.dev20230523165919/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/adapters.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/asgi.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/client.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/dispatcher.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/hypercorn.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/proxy.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/request.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/resource.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/response.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/http/router.py` & `localstack-core-2.0.3.dev20230523165919/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/logging/format.py` & `localstack-core-2.0.3.dev20230523165919/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/logging/setup.py` & `localstack-core-2.0.3.dev20230523165919/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/packages/__init__.py` & `localstack-core-2.0.3.dev20230523165919/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/packages/api.py` & `localstack-core-2.0.3.dev20230523165919/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/packages/core.py` & `localstack-core-2.0.3.dev20230523165919/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/packages/debugpy.py` & `localstack-core-2.0.3.dev20230523165919/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/packages/terraform.py` & `localstack-core-2.0.3.dev20230523165919/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/plugins.py` & `localstack-core-2.0.3.dev20230523165919/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/runtime/analytics.py` & `localstack-core-2.0.3.dev20230523165919/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/runtime/hooks.py` & `localstack-core-2.0.3.dev20230523165919/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/runtime/init.py` & `localstack-core-2.0.3.dev20230523165919/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/runtime/main.py` & `localstack-core-2.0.3.dev20230523165919/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/runtime/shutdown.py` & `localstack-core-2.0.3.dev20230523165919/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/acm/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/context.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/helpers.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/integration.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/invocations.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/patches.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/router_asf.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/apigateway/templates.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/api_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/hooks.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/packages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/plugins.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/deploy.html` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/events.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/packages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/service_models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudformation/stores.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/cloudwatch/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/packages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/server.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodb/utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/ec2/exceptions.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/ec2/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/ec2/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/edge.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/es/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/events/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/events/scheduler.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/firehose/mappers.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/firehose/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/firehose/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/generic_proxy.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/iam/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/infra.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/internal.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/packages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kinesis/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kms/local_kms_server.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kms/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kms/packages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kms/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/kms/utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/logs/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/logs/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/messages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/moto.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/motoserver.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/cluster.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/packages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/opensearch/versions.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/plugins.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/providers.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/redshift/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/route53/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/route53resolver/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/route53resolver/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/route53resolver/utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/constants.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/cors.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/multipart_content.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/notifications.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/presigned_url.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/s3_listener.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/s3_starter.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/s3_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/virtual_host.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/s3/website_hosting.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/secretsmanager/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/ses/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sns/constants.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sns/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sns/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sns/publisher.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/constants.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/exceptions.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/query_api.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sqs/utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/ssm/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/packages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/stores.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/sts/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/transcribe/packages.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/transcribe/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/services/transcribe/provider.py` & `localstack-core-2.0.3.dev20230523165919/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/state/core.py` & `localstack-core-2.0.3.dev20230523165919/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/state/inspect.py` & `localstack-core-2.0.3.dev20230523165919/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/state/pickle.py` & `localstack-core-2.0.3.dev20230523165919/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/state/snapshot.py` & `localstack-core-2.0.3.dev20230523165919/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/asf_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/aws/util.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/filters.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/fixtures.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/snapshot.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/pytest/util.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/prototype.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/report.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/transformer.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.0.3.dev20230523165919/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/cli.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/client.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/events.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/logger.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/metadata.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/publisher.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/analytics/usage.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/archives.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/asyncio.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/auth.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/arns.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/aws_models.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/aws_responses.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/aws_stack.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/client.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/client_types.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/queries.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/request_context.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/resources.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/aws/templating.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/bootstrap.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/collections.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/common.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/config_listener.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/container_networking.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/container_utils/container_client.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/container_utils/container_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 from localstack import config
 from localstack.utils.collections import HashableList
 from localstack.utils.files import TMP_FILES, rm_rf, save_file
 from localstack.utils.strings import short_uid
 
 LOG = logging.getLogger(__name__)
 
+# list of well-known image repo prefixes that should be stripped off to canonicalize image names
+WELL_KNOWN_IMAGE_REPO_PREFIXES = ("localhost/", "docker.io/library/")
+
 
 @unique
 class DockerContainerStatus(Enum):
     DOWN = -1
     NON_EXISTENT = 0
     UP = 1
     PAUSED = 2
@@ -418,26 +421,28 @@
     platform: Optional[DockerPlatform]
     privileged: Optional[bool]
     ports: Optional[PortMappings]
     ulimits: Optional[List[Ulimit]]
     user: Optional[str]
 
 
+# TODO: remove Docker/Podman compatibility switches (in particular strip_wellknown_repo_prefixes=...)
+#  from the container client base interface and introduce derived Podman client implementations instead!
 class ContainerClient(metaclass=ABCMeta):
     STOP_TIMEOUT = 0
 
     @abstractmethod
     def get_container_status(self, container_name: str) -> DockerContainerStatus:
         """Returns the status of the container with the given name"""
         pass
 
     def get_networks(self, container_name: str) -> List[str]:
         LOG.debug("Getting networks for container: %s", container_name)
         container_attrs = self.inspect_container(container_name_or_id=container_name)
-        return list(container_attrs["NetworkSettings"]["Networks"].keys())
+        return list(container_attrs["NetworkSettings"].get("Networks", {}).keys())
 
     def get_container_ipv4_for_network(
         self, container_name_or_id: str, container_network: str
     ) -> str:
         """
         Returns the IPv4 address for the container on the interface connected to the given network
         :param container_name_or_id: Container to inspect
@@ -448,15 +453,15 @@
             "Getting ipv4 address for container %s in network %s.",
             container_name_or_id,
             container_network,
         )
         # we always need the ID for this
         container_id = self.get_container_id(container_name=container_name_or_id)
         network_attrs = self.inspect_network(container_network)
-        containers = network_attrs["Containers"]
+        containers = network_attrs.get("Containers") or {}
         if container_id not in containers:
             raise ContainerException(
                 "Container %s is not connected to target network %s",
                 container_name_or_id,
                 container_network,
             )
         try:
@@ -470,15 +475,14 @@
     @abstractmethod
     def stop_container(self, container_name: str, timeout: int = None):
         """Stops container with given name
         :param container_name: Container identifier (name or id) of the container to be stopped
         :param timeout: Timeout after which SIGKILL is sent to the container.
                         If not specified, defaults to `STOP_TIMEOUT`
         """
-        pass
 
     @abstractmethod
     def restart_container(self, container_name: str, timeout: int = 10):
         """Restarts a container with the given name.
         :param container_name: Container identifier
         :param timeout: Seconds to wait for stop before killing the container
         """
@@ -490,32 +494,29 @@
     @abstractmethod
     def unpause_container(self, container_name: str):
         """Unpauses a container with the given name."""
 
     @abstractmethod
     def remove_container(self, container_name: str, force=True, check_existence=False) -> None:
         """Removes container with given name"""
-        pass
 
     @abstractmethod
     def remove_image(self, image: str, force: bool = True) -> None:
         """Removes an image with given name
 
         :param image: Image name and tag
         :param force: Force removal
         """
-        pass
 
     @abstractmethod
     def list_containers(self, filter: Union[List[str], str, None] = None, all=True) -> List[dict]:
         """List all containers matching the given filters
 
         :return: A list of dicts with keys id, image, name, labels, status
         """
-        pass
 
     def get_running_container_names(self) -> List[str]:
         """Returns a list of the names of all running containers"""
         result = self.list_containers(all=False)
         result = list(map(lambda container: container["name"], result))
         return result
 
@@ -524,32 +525,28 @@
         return container_name in self.get_running_container_names()
 
     @abstractmethod
     def copy_into_container(
         self, container_name: str, local_path: str, container_path: str
     ) -> None:
         """Copy contents of the given local path into the container"""
-        pass
 
     @abstractmethod
     def copy_from_container(
         self, container_name: str, local_path: str, container_path: str
     ) -> None:
         """Copy contents of the given container to the host"""
-        pass
 
     @abstractmethod
     def pull_image(self, docker_image: str, platform: Optional[DockerPlatform] = None) -> None:
         """Pulls an image with a given name from a Docker registry"""
-        pass
 
     @abstractmethod
     def push_image(self, docker_image: str) -> None:
         """Pushes an image with a given name to a Docker registry"""
-        pass
 
     @abstractmethod
     def build_image(
         self,
         dockerfile_path: str,
         image_name: str,
         context_path: str = None,
@@ -558,122 +555,121 @@
         """Builds an image from the given Dockerfile
 
         :param dockerfile_path: Path to Dockerfile, or a directory that contains a Dockerfile
         :param image_name: Name of the image to be built
         :param context_path: Path for build context (defaults to dirname of Dockerfile)
         :param platform: Target platform for build (defaults to platform of Docker host)
         """
-        pass
 
     @abstractmethod
     def tag_image(self, source_ref: str, target_name: str) -> None:
         """Tags an image with a new name
 
         :param source_ref: Name or ID of the image to be tagged
         :param target_name: New name (tag) of the tagged image
         """
-        pass
 
     @abstractmethod
-    def get_docker_image_names(self, strip_latest=True, include_tags=True) -> List[str]:
+    def get_docker_image_names(
+        self,
+        strip_latest: bool = True,
+        include_tags: bool = True,
+        strip_wellknown_repo_prefixes: bool = True,
+    ) -> List[str]:
         """
         Get all names of docker images available to the container engine
         :param strip_latest: return images both with and without :latest tag
-        :param include_tags: Include tags of the images in the names
+        :param include_tags: include tags of the images in the names
+        :param strip_wellknown_repo_prefixes: whether to strip off well-known repo prefixes like
+               "localhost/" or "docker.io/library/" which are added by the Podman API, but not by Docker
         :return: List of image names
         """
-        pass
 
     @abstractmethod
-    def get_container_logs(self, container_name_or_id: str, safe=False) -> str:
+    def get_container_logs(self, container_name_or_id: str, safe: bool = False) -> str:
         """Get all logs of a given container"""
-        pass
 
     @abstractmethod
     def stream_container_logs(self, container_name_or_id: str) -> CancellableStream:
         """Returns a blocking generator you can iterate over to retrieve log output as it happens."""
-        pass
 
     @abstractmethod
     def inspect_container(self, container_name_or_id: str) -> Dict[str, Union[Dict, str]]:
         """Get detailed attributes of a container.
 
         :return: Dict containing docker attributes as returned by the daemon
         """
-        pass
 
     def inspect_container_volumes(self, container_name_or_id) -> List[VolumeInfo]:
         """Return information about the volumes mounted into the given container.
 
         :param container_name_or_id: the container name or id
         :return: a list of volumes
         """
         volumes = []
         for doc in self.inspect_container(container_name_or_id)["Mounts"]:
             volumes.append(VolumeInfo(**{k.lower(): v for k, v in doc.items()}))
 
         return volumes
 
     @abstractmethod
-    def inspect_image(self, image_name: str, pull: bool = True) -> Dict[str, Union[Dict, str]]:
+    def inspect_image(
+        self, image_name: str, pull: bool = True, strip_wellknown_repo_prefixes: bool = True
+    ) -> Dict[str, Union[dict, list, str]]:
         """Get detailed attributes of an image.
 
         :param image_name: Image name to inspect
         :param pull: Whether to pull image if not existent
+        :param strip_wellknown_repo_prefixes: whether to strip off well-known repo prefixes like
+               "localhost/" or "docker.io/library/" which are added by the Podman API, but not by Docker
         :return: Dict containing docker attributes as returned by the daemon
         """
-        pass
 
     @abstractmethod
     def create_network(self, network_name: str) -> str:
         """
         Creates a network with the given name
         :param network_name: Name of the network
         :return Network ID
         """
-        pass
 
     @abstractmethod
     def delete_network(self, network_name: str) -> None:
         """
         Delete a network with the given name
         :param network_name: Name of the network
         """
-        pass
 
     @abstractmethod
     def inspect_network(self, network_name: str) -> Dict[str, Union[Dict, str]]:
         """Get detailed attributes of an network.
 
         :return: Dict containing docker attributes as returned by the daemon
         """
-        pass
 
     @abstractmethod
     def connect_container_to_network(
         self, network_name: str, container_name_or_id: str, aliases: Optional[List] = None
     ) -> None:
         """
         Connects a container to a given network
         :param network_name: Network to connect the container to
         :param container_name_or_id: Container to connect to the network
         :param aliases: List of dns names the container should be available under in the network
         """
-        pass
 
     @abstractmethod
     def disconnect_container_from_network(
         self, network_name: str, container_name_or_id: str
     ) -> None:
         """
         Disconnects a container from a given network
         :param network_name: Network to disconnect the container from
         :param container_name_or_id: Container to disconnect from the network
         """
-        pass
 
     def get_container_name(self, container_id: str) -> str:
         """Get the name of a container by a given identifier"""
         return self.inspect_container(container_id)["Name"].lstrip("/")
 
     def get_container_id(self, container_name: str) -> str:
         """Get the id of a container by a given name"""
@@ -681,15 +677,14 @@
 
     @abstractmethod
     def get_container_ip(self, container_name_or_id: str) -> str:
         """Get the IP address of a given container
 
         If container has multiple networks, it will return the IP of the first
         """
-        pass
 
     def get_image_cmd(self, docker_image: str, pull: bool = True) -> List[str]:
         """Get the command for the given image
         :param docker_image: Docker image to inspect
         :param pull: Whether to pull if image is not present
         :return: Image command in its array form
         """
@@ -699,36 +694,34 @@
     def get_image_entrypoint(self, docker_image: str, pull: bool = True) -> str:
         """Get the entry point for the given image
         :param docker_image: Docker image to inspect
         :param pull: Whether to pull if image is not present
         :return: Image entrypoint
         """
         LOG.debug("Getting the entrypoint for image: %s", docker_image)
-        entrypoint_list = self.inspect_image(docker_image, pull)["Config"]["Entrypoint"] or []
+        entrypoint_list = self.inspect_image(docker_image, pull)["Config"].get("Entrypoint") or []
         return shlex.join(entrypoint_list)
 
     @abstractmethod
     def has_docker(self) -> bool:
         """Check if system has docker available"""
-        pass
 
     @abstractmethod
     def commit(
         self,
         container_name_or_id: str,
         image_name: str,
         image_tag: str,
     ):
         """Create an image from a running container.
 
         :param container_name_or_id: Source container
         :param image_name: Destination image name
         :param image_tag: Destination image tag
         """
-        pass
 
     def create_container_from_config(self, container_config: ContainerConfiguration) -> str:
         """
         Similar to create_container, but allows passing the whole ContainerConfiguration
         :param container_config: ContainerConfiguration how to start the container
         :return: Container ID
         """
@@ -783,15 +776,14 @@
         labels: Optional[Dict[str, str]] = None,
         platform: Optional[DockerPlatform] = None,
     ) -> str:
         """Creates a container with the given image
 
         :return: Container ID
         """
-        pass
 
     @abstractmethod
     def run_container(
         self,
         image_name: str,
         stdin: bytes = None,
         *,
@@ -817,15 +809,14 @@
         privileged: Optional[bool] = None,
         ulimits: Optional[List[Ulimit]] = None,
     ) -> Tuple[bytes, bytes]:
         """Creates and runs a given docker container
 
         :return: A tuple (stdout, stderr)
         """
-        pass
 
     @abstractmethod
     def exec_in_container(
         self,
         container_name_or_id: str,
         command: Union[List[str], str],
         interactive: bool = False,
@@ -835,41 +826,38 @@
         user: Optional[str] = None,
         workdir: Optional[str] = None,
     ) -> Tuple[bytes, bytes]:
         """Execute a given command in a container
 
         :return: A tuple (stdout, stderr)
         """
-        pass
 
     @abstractmethod
     def start_container(
         self,
         container_name_or_id: str,
         stdin: bytes = None,
         interactive: bool = False,
         attach: bool = False,
         flags: Optional[str] = None,
     ) -> Tuple[bytes, bytes]:
         """Start a given, already created container
 
         :return: A tuple (stdout, stderr) if attach or interactive is set, otherwise a tuple (b"container_name_or_id", b"")
         """
-        pass
 
     @abstractmethod
     def login(self, username: str, password: str, registry: Optional[str] = None) -> None:
         """
         Login into an OCI registry
 
         :param username: Username for the registry
         :param password: Password / token for the registry
         :param registry: Registry url
         """
-        pass
 
 
 class Util:
     MAX_ENV_ARGS_LENGTH = 20000
 
     @staticmethod
     def format_env_vars(key: str, value: Optional[str]):
@@ -912,22 +900,39 @@
     @staticmethod
     def mountable_tmp_file():
         f = os.path.join(config.dirs.tmp, short_uid())
         TMP_FILES.append(f)
         return f
 
     @staticmethod
-    def append_without_latest(image_names):
+    def append_without_latest(image_names: List[str]):
         suffix = ":latest"
         for image in list(image_names):
             if image.endswith(suffix):
                 image_names.append(image[: -len(suffix)])
 
     @staticmethod
-    def tar_path(path, target_path, is_dir: bool):
+    def strip_wellknown_repo_prefixes(image_names: List[str]) -> List[str]:
+        """
+        Remove well-known repo prefixes like `localhost/` or `docker.io/library/` from the list of given
+        image names. This is mostly to ensure compatibility of our Docker client with Podman API responses.
+        :return: a copy of the list of image names, with well-known repo prefixes removed
+        """
+        result = []
+        for image in image_names:
+            for prefix in WELL_KNOWN_IMAGE_REPO_PREFIXES:
+                if image.startswith(prefix):
+                    image = image.removeprefix(prefix)
+                    # strip only one of the matching prefixes (avoid multi-stripping)
+                    break
+            result.append(image)
+        return result
+
+    @staticmethod
+    def tar_path(path: str, target_path: str, is_dir: bool):
         f = tempfile.NamedTemporaryFile()
         with tarfile.open(mode="w", fileobj=f) as t:
             abs_path = os.path.abspath(path)
             arcname = (
                 os.path.basename(path)
                 if is_dir
                 else (os.path.basename(target_path) or os.path.basename(path))
```

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import re
 import shlex
 import subprocess
 from typing import Dict, List, Optional, Tuple, Union
 
 from localstack import config
+from localstack.utils.collections import ensure_list
 from localstack.utils.container_utils.container_client import (
     AccessDenied,
     CancellableStream,
     ContainerClient,
     ContainerException,
     DockerContainerStatus,
     DockerPlatform,
@@ -23,15 +24,15 @@
     RegistryConnectionError,
     SimpleVolumeBind,
     Ulimit,
     Util,
     VolumeBind,
 )
 from localstack.utils.run import run
-from localstack.utils.strings import to_str
+from localstack.utils.strings import first_char_to_upper, to_str
 
 LOG = logging.getLogger(__name__)
 
 
 class CancellableProcessStream(CancellableStream):
     process: subprocess.Popen
 
@@ -49,15 +50,21 @@
         return line
 
     def close(self):
         return self.process.terminate()
 
 
 class CmdDockerClient(ContainerClient):
-    """Class for managing docker containers using the command line executable"""
+    """
+    Class for managing Docker (or Podman) containers using the command line executable.
+
+    The client also supports targeting Podman engines, as Podman is almost a drop-in replacement
+    for Docker these days. The majority of compatibility switches in this class is to handle slightly
+    different response payloads or error messages returned by the `docker` vs `podman` commands.
+    """
 
     default_run_outfile: Optional[str] = None
 
     def _docker_cmd(self) -> List[str]:
         """Return the string to be used for running Docker commands."""
         return config.DOCKER_CMD.split()
 
@@ -90,78 +97,71 @@
             timeout = self.STOP_TIMEOUT
         cmd = self._docker_cmd()
         cmd += ["stop", "--time", str(timeout), container_name]
         LOG.debug("Stopping container with cmd %s", cmd)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name, error=e)
+            raise ContainerException(
+                f"Docker process returned with errorcode {e.returncode}", e.stdout, e.stderr
+            ) from e
 
     def restart_container(self, container_name: str, timeout: int = 10) -> None:
         cmd = self._docker_cmd()
         cmd += ["restart", "--time", str(timeout), container_name]
         LOG.debug("Restarting container with cmd %s", cmd)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name, error=e)
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def pause_container(self, container_name: str) -> None:
         cmd = self._docker_cmd()
         cmd += ["pause", container_name]
         LOG.debug("Pausing container with cmd %s", cmd)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name, error=e)
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def unpause_container(self, container_name: str) -> None:
         cmd = self._docker_cmd()
         cmd += ["unpause", container_name]
         LOG.debug("Unpausing container with cmd %s", cmd)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name, error=e)
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def remove_image(self, image: str, force: bool = True) -> None:
         cmd = self._docker_cmd()
         cmd += ["rmi", image]
         if force:
             cmd += ["--force"]
         LOG.debug("Removing image %s %s", image, "(forced)" if force else "")
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such image" in to_str(e.stdout):
+            # handle different error messages for Docker and podman
+            error_messages = ["No such image", "image not known"]
+            if any(msg in to_str(e.stdout) for msg in error_messages):
                 raise NoSuchImage(image, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def commit(
         self,
         container_name_or_id: str,
         image_name: str,
         image_tag: str,
     ):
@@ -169,38 +169,34 @@
         cmd += ["commit", container_name_or_id, f"{image_name}:{image_tag}"]
         LOG.debug(
             "Creating image from container %s as %s:%s", container_name_or_id, image_name, image_tag
         )
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name_or_id, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name_or_id, error=e)
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def remove_container(self, container_name: str, force=True, check_existence=False) -> None:
         if check_existence and container_name not in self.get_running_container_names():
             return
         cmd = self._docker_cmd() + ["rm"]
         if force:
             cmd.append("-f")
         cmd.append(container_name)
         LOG.debug("Removing container with cmd %s", cmd)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name, error=e)
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def list_containers(self, filter: Union[List[str], str, None] = None, all=True) -> List[dict]:
         filter = [filter] if isinstance(filter, str) else filter
         cmd = self._docker_cmd()
         cmd.append("ps")
         if all:
             cmd.append("-a")
@@ -222,17 +218,19 @@
                 container_list = json.loads(cmd_result)
             else:
                 container_list = [json.loads(line) for line in cmd_result.splitlines()]
         result = []
         for container in container_list:
             result.append(
                 {
-                    "id": container["ID"],
+                    # support both, Docker and podman API response formats (`ID` vs `Id`)
+                    "id": container.get("ID") or container["Id"],
                     "image": container["Image"],
-                    "name": container["Names"],
+                    # Docker returns a single string for `Names`, whereas podman returns a list of names
+                    "name": ensure_list(container["Names"])[0],
                     "status": container["State"],
                     "labels": container["Labels"],
                 }
             )
         return result
 
     def copy_into_container(
@@ -240,46 +238,53 @@
     ) -> None:
         cmd = self._docker_cmd()
         cmd += ["cp", local_path, f"{container_name}:{container_path}"]
         LOG.debug("Copying into container with cmd: %s", cmd)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name)
+            self._check_and_raise_no_such_container_error(container_name, error=e)
+            if "does not exist" in to_str(e.stdout):
+                raise NoSuchContainer(container_name, stdout=e.stdout, stderr=e.stderr)
             raise ContainerException(
                 f"Docker process returned with errorcode {e.returncode}", e.stdout, e.stderr
             ) from e
 
     def copy_from_container(
         self, container_name: str, local_path: str, container_path: str
     ) -> None:
         cmd = self._docker_cmd()
         cmd += ["cp", f"{container_name}:{container_path}", local_path]
         LOG.debug("Copying from container with cmd: %s", cmd)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name)
+            self._check_and_raise_no_such_container_error(container_name, error=e)
+            # additional check to support Podman CLI output
+            if re.match(".*container .+ does not exist", to_str(e.stdout)):
+                raise NoSuchContainer(container_name, stdout=e.stdout, stderr=e.stderr)
             raise ContainerException(
                 "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
             ) from e
 
     def pull_image(self, docker_image: str, platform: Optional[DockerPlatform] = None) -> None:
         cmd = self._docker_cmd()
         cmd += ["pull", docker_image]
         if platform:
             cmd += ["--platform", platform]
         LOG.debug("Pulling image with cmd: %s", cmd)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "pull access denied" in to_str(e.stdout):
-                raise NoSuchImage(docker_image)
+            stdout_str = to_str(e.stdout)
+            if "pull access denied" in stdout_str:
+                raise NoSuchImage(docker_image, stdout=e.stdout, stderr=e.stderr)
+            # note: error message 'access to the resource is denied' raised by Podman client
+            if "Trying to pull" in stdout_str and "access to the resource is denied" in stdout_str:
+                raise NoSuchImage(docker_image, stdout=e.stdout, stderr=e.stderr)
             raise ContainerException(
                 "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
             ) from e
 
     def push_image(self, docker_image: str) -> None:
         cmd = self._docker_cmd()
         cmd += ["push", docker_image]
@@ -293,14 +298,17 @@
                 raise AccessDenied(docker_image)
             if "access token has insufficient scopes" in to_str(e.stdout):
                 raise AccessDenied(docker_image)
             if "does not exist" in to_str(e.stdout):
                 raise NoSuchImage(docker_image)
             if "connection refused" in to_str(e.stdout):
                 raise RegistryConnectionError(e.stdout)
+            # note: error message 'image not known' raised by Podman client
+            if "image not known" in to_str(e.stdout):
+                raise NoSuchImage(docker_image)
             raise ContainerException(
                 f"Docker process returned with errorcode {e.returncode}", e.stdout, e.stderr
             ) from e
 
     def build_image(
         self,
         dockerfile_path: str,
@@ -326,86 +334,116 @@
     def tag_image(self, source_ref: str, target_name: str) -> None:
         cmd = self._docker_cmd()
         cmd += ["tag", source_ref, target_name]
         LOG.debug("Tagging Docker image %s as %s", source_ref, target_name)
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such image" in to_str(e.stdout):
+            # handle different error messages for Docker and podman
+            error_messages = ["No such image", "image not known"]
+            if any(msg in to_str(e.stdout) for msg in error_messages):
                 raise NoSuchImage(source_ref)
             raise ContainerException(
                 f"Docker process returned with error code {e.returncode}", e.stdout, e.stderr
             ) from e
 
-    def get_docker_image_names(self, strip_latest=True, include_tags=True):
+    def get_docker_image_names(
+        self, strip_latest=True, include_tags=True, strip_wellknown_repo_prefixes: bool = True
+    ):
         format_string = "{{.Repository}}:{{.Tag}}" if include_tags else "{{.Repository}}"
         cmd = self._docker_cmd()
         cmd += ["images", "--format", format_string]
         try:
             output = run(cmd)
 
             image_names = output.splitlines()
+            if strip_wellknown_repo_prefixes:
+                image_names = Util.strip_wellknown_repo_prefixes(image_names)
             if strip_latest:
                 Util.append_without_latest(image_names)
+
             return image_names
         except Exception as e:
             LOG.info('Unable to list Docker images via "%s": %s', cmd, e)
             return []
 
     def get_container_logs(self, container_name_or_id: str, safe=False) -> str:
         cmd = self._docker_cmd()
         cmd += ["logs", container_name_or_id]
         try:
             return run(cmd)
         except subprocess.CalledProcessError as e:
             if safe:
                 return ""
-            if "No such container" in to_str(e.stdout):
-                raise NoSuchContainer(container_name_or_id, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name_or_id, error=e)
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def stream_container_logs(self, container_name_or_id: str) -> CancellableStream:
         self.inspect_container(container_name_or_id)  # guard to check whether container is there
 
         cmd = self._docker_cmd()
         cmd += ["logs", container_name_or_id, "--follow"]
 
         process: subprocess.Popen = run(
             cmd, asynchronous=True, outfile=subprocess.PIPE, stderr=subprocess.PIPE
         )
 
         return CancellableProcessStream(process)
 
-    def _inspect_object(self, object_name_or_id: str) -> Dict[str, Union[Dict, str]]:
+    def _inspect_object(self, object_name_or_id: str) -> Dict[str, Union[dict, list, str]]:
         cmd = self._docker_cmd()
         cmd += ["inspect", "--format", "{{json .}}", object_name_or_id]
         try:
             cmd_result = run(cmd)
         except subprocess.CalledProcessError as e:
-            if "No such object" in to_str(e.stdout):
+            # note: case-insensitive comparison, to support Docker and Podman output formats
+            if "no such object" in to_str(e.stdout).lower():
                 raise NoSuchObject(object_name_or_id, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
-        image_data = json.loads(cmd_result.strip())
-        return image_data
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
+        object_data = json.loads(cmd_result.strip())
+        if isinstance(object_data, list):
+            # return first list item, for compatibility with Podman API
+            if len(object_data) == 1:
+                result = object_data[0]
+                # convert first character to uppercase (e.g., `name` -> `Name`), for Podman/Docker compatibility
+                result = {first_char_to_upper(k): v for k, v in result.items()}
+                return result
+            LOG.info(
+                "Expected a single object for `inspect` on ID %s, got %s",
+                object_name_or_id,
+                len(object_data),
+            )
+        return object_data
 
     def inspect_container(self, container_name_or_id: str) -> Dict[str, Union[Dict, str]]:
         try:
             return self._inspect_object(container_name_or_id)
         except NoSuchObject as e:
             raise NoSuchContainer(container_name_or_id=e.object_id)
 
-    def inspect_image(self, image_name: str, pull: bool = True) -> Dict[str, Union[Dict, str]]:
-        try:
-            return self._inspect_object(image_name)
+    def inspect_image(
+        self,
+        image_name: str,
+        pull: bool = True,
+        strip_wellknown_repo_prefixes: bool = True,
+    ) -> Dict[str, Union[dict, list, str]]:
+        try:
+            result = self._inspect_object(image_name)
+            if strip_wellknown_repo_prefixes:
+                if result.get("RepoDigests"):
+                    result["RepoDigests"] = Util.strip_wellknown_repo_prefixes(
+                        result["RepoDigests"]
+                    )
+                if result.get("RepoTags"):
+                    result["RepoTags"] = Util.strip_wellknown_repo_prefixes(result["RepoTags"])
+            return result
         except NoSuchObject as e:
             if pull:
                 self.pull_image(image_name)
                 return self.inspect_image(image_name, pull=False)
             raise NoSuchImage(image_name=e.object_id)
 
     def create_network(self, network_name: str) -> str:
@@ -454,59 +492,56 @@
         cmd += [network_name, container_name_or_id]
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
             stdout_str = to_str(e.stdout)
             if re.match(r".*network (.*) not found.*", stdout_str):
                 raise NoSuchNetwork(network_name=network_name)
-            elif "No such container" in stdout_str:
-                raise NoSuchContainer(container_name_or_id, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name_or_id, error=e)
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def disconnect_container_from_network(
         self, network_name: str, container_name_or_id: str
     ) -> None:
         LOG.debug(
             "Disconnecting container '%s' from network '%s'", container_name_or_id, network_name
         )
         cmd = self._docker_cmd() + ["network", "disconnect", network_name, container_name_or_id]
         try:
             run(cmd)
         except subprocess.CalledProcessError as e:
             stdout_str = to_str(e.stdout)
             if re.match(r".*network (.*) not found.*", stdout_str):
                 raise NoSuchNetwork(network_name=network_name)
-            elif "No such container" in stdout_str:
-                raise NoSuchContainer(container_name_or_id, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            self._check_and_raise_no_such_container_error(container_name_or_id, error=e)
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def get_container_ip(self, container_name_or_id: str) -> str:
         cmd = self._docker_cmd()
         cmd += [
             "inspect",
             "--format",
             "{{range .NetworkSettings.Networks}}{{.IPAddress}} {{end}}",
             container_name_or_id,
         ]
         try:
             result = run(cmd).strip()
             return result.split(" ")[0] if result else ""
         except subprocess.CalledProcessError as e:
-            if "No such object" in to_str(e.stdout):
+            self._check_and_raise_no_such_container_error(container_name_or_id, error=e)
+            # consider different error messages for Podman
+            if "no such object" in to_str(e.stdout).lower():
                 raise NoSuchContainer(container_name_or_id, stdout=e.stdout, stderr=e.stderr)
-            else:
-                raise ContainerException(
-                    "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
-                ) from e
+            raise ContainerException(
+                "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
+            ) from e
 
     def login(self, username: str, password: str, registry: Optional[str] = None) -> None:
         cmd = self._docker_cmd()
         # TODO specify password via stdin
         cmd += ["login", "-u", username, "-p", password]
         if registry:
             cmd.append(registry)
@@ -529,28 +564,34 @@
         LOG.debug("Create container with cmd: %s", cmd)
         try:
             container_id = run(cmd)
             # Note: strip off Docker warning messages like "DNS setting (--dns=127.0.0.1) may fail in containers"
             container_id = container_id.strip().split("\n")[-1]
             return container_id.strip()
         except subprocess.CalledProcessError as e:
-            if "Unable to find image" in to_str(e.stdout):
+            error_messages = ["Unable to find image", "Trying to pull"]
+            if any(msg in to_str(e.stdout) for msg in error_messages):
                 raise NoSuchImage(image_name, stdout=e.stdout, stderr=e.stderr)
             raise ContainerException(
                 "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
             ) from e
         finally:
             Util.rm_env_vars_file(env_file)
 
     def run_container(self, image_name: str, stdin=None, **kwargs) -> Tuple[bytes, bytes]:
         cmd, env_file = self._build_run_create_cmd("run", image_name, **kwargs)
         LOG.debug("Run container with cmd: %s", cmd)
-        result = self._run_async_cmd(cmd, stdin, kwargs.get("name") or "", image_name)
-        Util.rm_env_vars_file(env_file)
-        return result
+        try:
+            return self._run_async_cmd(cmd, stdin, kwargs.get("name") or "", image_name)
+        except ContainerException as e:
+            if "Trying to pull" in str(e) and "access to the resource is denied" in str(e):
+                raise NoSuchImage(image_name, stdout=e.stdout, stderr=e.stderr) from e
+            raise
+        finally:
+            Util.rm_env_vars_file(env_file)
 
     def exec_in_container(
         self,
         container_name_or_id: str,
         command: Union[List[str], str],
         interactive=False,
         detach=False,
@@ -571,18 +612,19 @@
         if workdir:
             cmd += ["--workdir", workdir]
         if env_vars:
             env_flag, env_file = Util.create_env_vars_file_flag(env_vars)
             cmd += env_flag
         cmd.append(container_name_or_id)
         cmd += command if isinstance(command, List) else [command]
-        LOG.debug("Execute in container cmd: %s", cmd)
-        result = self._run_async_cmd(cmd, stdin, container_name_or_id)
-        Util.rm_env_vars_file(env_file)
-        return result
+        LOG.debug("Execute command in container: %s", cmd)
+        try:
+            return self._run_async_cmd(cmd, stdin, container_name_or_id)
+        finally:
+            Util.rm_env_vars_file(env_file)
 
     def start_container(
         self,
         container_name_or_id: str,
         stdin=None,
         interactive: bool = False,
         attach: bool = False,
@@ -622,15 +664,17 @@
                 )
             else:
                 return stdout, stderr
         except subprocess.CalledProcessError as e:
             stderr_str = to_str(e.stderr)
             if "Unable to find image" in stderr_str:
                 raise NoSuchImage(image_name or "", stdout=e.stdout, stderr=e.stderr)
-            if "No such container" in stderr_str:
+            # consider different error messages for Docker/Podman
+            error_messages = ("No such container", "no container with name or ID")
+            if any(msg.lower() in to_str(e.stderr).lower() for msg in error_messages):
                 raise NoSuchContainer(container_name, stdout=e.stdout, stderr=e.stderr)
             raise ContainerException(
                 "Docker process returned with errorcode %s" % e.returncode, e.stdout, e.stderr
             ) from e
 
     def _build_run_create_cmd(
         self,
@@ -732,7 +776,21 @@
         :param mount_volume: Either a SimpleVolumeBind, in essence a tuple (host_dir, container_dir), or a VolumeBind object
         :return: String which is passable as parameter to the docker cli -v option
         """
         if isinstance(mount_volume, VolumeBind):
             return mount_volume.to_str()
         else:
             return f"{mount_volume[0]}:{mount_volume[1]}"
+
+    def _check_and_raise_no_such_container_error(
+        self, container_name_or_id: str, error: subprocess.CalledProcessError
+    ):
+        """
+        Check the given client invocation error and raise a `NoSuchContainer` exception if it
+        represents a `no such container` exception from Docker or Podman.
+        """
+
+        # consider different error messages for Docker/Podman
+        error_messages = ("No such container", "no container with name or ID")
+        process_stdout_lower = to_str(error.stdout).lower()
+        if any(msg.lower() in process_stdout_lower for msg in error_messages):
+            raise NoSuchContainer(container_name_or_id, stdout=error.stdout, stderr=error.stderr)
```

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,32 +37,37 @@
 from localstack.utils.threads import start_worker_thread
 
 LOG = logging.getLogger(__name__)
 SDK_ISDIR = 1 << 31
 
 
 class SdkDockerClient(ContainerClient):
-    """Class for managing docker using the python docker sdk"""
+    """
+    Class for managing Docker (or Podman) using the Python Docker SDK.
+
+    The client also supports targeting Podman engines, as Podman is almost a drop-in replacement
+    for Docker these days (with ongoing efforts to further streamline the two), and the Docker SDK
+    is doing some of the heavy lifting for us to support both target platforms.
+    """
 
     docker_client: Optional[DockerClient]
 
     def __init__(self):
         try:
             self.docker_client = self._create_client()
             logging.getLogger("urllib3").setLevel(logging.INFO)
         except DockerNotAvailable:
             self.docker_client = None
 
     def client(self):
         if self.docker_client:
             return self.docker_client
-        else:
-            # if the initialization failed before, try to initialize on-demand
-            self.docker_client = self._create_client()
-            return self.docker_client
+        # if the initialization failed before, try to initialize on-demand
+        self.docker_client = self._create_client()
+        return self.docker_client
 
     @staticmethod
     def _create_client():
         from localstack.config import DOCKER_SDK_DEFAULT_RETRIES, DOCKER_SDK_DEFAULT_TIMEOUT_SECONDS
 
         for attempt in range(0, DOCKER_SDK_DEFAULT_RETRIES + 1):
             try:
@@ -273,14 +278,17 @@
                     raise AccessDenied(docker_image)
                 if "connection refused" in to_str(result):
                     raise RegistryConnectionError(result)
                 raise ContainerException(result)
         except ImageNotFound:
             raise NoSuchImage(docker_image)
         except APIError as e:
+            # note: error message 'image not known' raised by Podman API
+            if "image not known" in str(e):
+                raise NoSuchImage(docker_image)
             raise ContainerException() from e
 
     def build_image(
         self,
         dockerfile_path: str,
         image_name: str,
         context_path: str = None,
@@ -306,27 +314,34 @@
             image = self.client().images.get(source_ref)
             image.tag(target_name)
         except APIError as e:
             if e.status_code == 404:
                 raise NoSuchImage(source_ref)
             raise ContainerException("Unable to tag Docker image") from e
 
-    def get_docker_image_names(self, strip_latest=True, include_tags=True):
+    def get_docker_image_names(
+        self,
+        strip_latest: bool = True,
+        include_tags: bool = True,
+        strip_wellknown_repo_prefixes: bool = True,
+    ):
         try:
             images = self.client().images.list()
             image_names = [tag for image in images for tag in image.tags if image.tags]
             if not include_tags:
-                image_names = list(map(lambda image_name: image_name.split(":")[0], image_names))
+                image_names = [image_name.rpartition(":")[0] for image_name in image_names]
+            if strip_wellknown_repo_prefixes:
+                image_names = Util.strip_wellknown_repo_prefixes(image_names)
             if strip_latest:
                 Util.append_without_latest(image_names)
             return image_names
         except APIError as e:
             raise ContainerException() from e
 
-    def get_container_logs(self, container_name_or_id: str, safe=False) -> str:
+    def get_container_logs(self, container_name_or_id: str, safe: bool = False) -> str:
         try:
             container = self.client().containers.get(container_name_or_id)
             return to_str(container.logs())
         except NotFound:
             if safe:
                 return ""
             raise NoSuchContainer(container_name_or_id)
@@ -348,17 +363,30 @@
         try:
             return self.client().containers.get(container_name_or_id).attrs
         except NotFound:
             raise NoSuchContainer(container_name_or_id)
         except APIError as e:
             raise ContainerException() from e
 
-    def inspect_image(self, image_name: str, pull: bool = True) -> Dict[str, Union[Dict, str]]:
-        try:
-            return self.client().images.get(image_name).attrs
+    def inspect_image(
+        self,
+        image_name: str,
+        pull: bool = True,
+        strip_wellknown_repo_prefixes: bool = True,
+    ) -> Dict[str, Union[dict, list, str]]:
+        try:
+            result = self.client().images.get(image_name).attrs
+            if strip_wellknown_repo_prefixes:
+                if result.get("RepoDigests"):
+                    result["RepoDigests"] = Util.strip_wellknown_repo_prefixes(
+                        result["RepoDigests"]
+                    )
+                if result.get("RepoTags"):
+                    result["RepoTags"] = Util.strip_wellknown_repo_prefixes(result["RepoTags"])
+            return result
         except NotFound:
             if pull:
                 self.pull_image(image_name)
                 return self.inspect_image(image_name, pull=False)
             raise NoSuchImage(image_name)
         except APIError as e:
             raise ContainerException() from e
@@ -443,14 +471,16 @@
         LOG.debug("Removing image %s %s", image, "(forced)" if force else "")
         try:
             self.client().images.remove(image=image, force=force)
         except ImageNotFound:
             if not force:
                 raise NoSuchImage(image)
         except APIError as e:
+            if "image not known" in str(e):
+                raise NoSuchImage(image)
             raise ContainerException() from e
 
     def commit(
         self,
         container_name_or_id: str,
         image_name: str,
         image_tag: str,
```

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/coverage_docs.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/crypto.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/diagnose.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/docker_utils.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/files.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/functions.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/http.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/json.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/net.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/numbers.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/objects.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/patch.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/platform.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/run.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/scheduler.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/server/http2_server.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/server/proxy_server.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/serving.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/ssl.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/strings.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/sync.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/tagging.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/tail.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/testutil.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/threads.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/time.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/urls.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/venv.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack/utils/xml.py` & `localstack-core-2.0.3.dev20230523165919/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/plux.json` & `localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.888888888888889%*

 * *Differences: {"'localstack.hooks.on_infra_shutdown'": '{insert: [(1, '*

 * *                                         "'_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown')], "*

 * *                                         'delete: [0]}',*

 * * "'localstack.hooks.on_infra_start'": '{insert: [(0, '*

 * *                                      "'_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start'), "*

 * *                                      '(6, '*

 * *                                      "'_ […]*

```diff
@@ -49,40 +49,40 @@
         "configure_edge_port=localstack.plugins:configure_edge_port"
     ],
     "localstack.hooks.on_infra_ready": [
         "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
         "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
     ],
     "localstack.hooks.on_infra_start": [
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration"
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
-        "ffmpeg/community=localstack.services.transcribe.plugins:ffmpeg_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "ffmpeg/community=localstack.services.transcribe.plugins:ffmpeg_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages"
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "terraform/community=localstack.packages.plugins:terraform_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package"
     ]
 }
```

### Comparing `localstack-core-2.0.3.dev20230523164857/localstack_core.egg-info/requires.txt` & `localstack-core-2.0.3.dev20230523165919/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/pyproject.toml` & `localstack-core-2.0.3.dev20230523165919/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230523164857/setup.cfg` & `localstack-core-2.0.3.dev20230523165919/setup.cfg`

 * *Files identical despite different names*

