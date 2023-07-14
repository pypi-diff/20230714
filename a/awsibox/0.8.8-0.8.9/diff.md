# Comparing `tmp/awsibox-0.8.8.tar.gz` & `tmp/awsibox-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsibox-0.8.8.tar", last modified: Mon Jul 10 13:54:48 2023, max compression
+gzip compressed data, was "awsibox-0.8.9.tar", last modified: Fri Jul 14 09:59:16 2023, max compression
```

## Comparing `awsibox-0.8.8.tar` & `awsibox-0.8.9.tar`

### file list

```diff
@@ -1,286 +1,290 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.686881 awsibox-0.8.8/
--rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.8/.gitignore
--rw-r--r--   0 mello     (1000) mello     (1000)    10297 2022-03-14 08:29:15.000000 awsibox-0.8.8/LICENSE
--rw-r--r--   0 mello     (1000) mello     (1000)      257 2023-06-16 08:09:06.000000 awsibox-0.8.8/MANIFEST.in
--rw-r--r--   0 mello     (1000) mello     (1000)      877 2023-07-10 13:54:48.686881 awsibox-0.8.8/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.8/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.510878 awsibox-0.8.8/awsibox/
--rw-r--r--   0 mello     (1000) mello     (1000)    19454 2023-07-08 15:37:21.000000 awsibox-0.8.8/awsibox/RP.py
--rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-07-10 13:54:21.000000 awsibox-0.8.8/awsibox/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.8/awsibox/args.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.510878 awsibox-0.8.8/awsibox/aws/
--rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/aws/CloudFormationResourceSpecification.json
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.478878 awsibox-0.8.8/awsibox/cfg/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.490878 awsibox-0.8.8/awsibox/cfg/ibox/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.546879 awsibox-0.8.8/awsibox/cfg/ibox/com/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.550879 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     5582 2023-07-04 07:34:22.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/capacity.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1252 2023-06-16 09:13:11.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.550879 awsibox-0.8.8/awsibox/cfg/ibox/com/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.554879 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudformation/
--rw-r--r--   0 mello     (1000) mello     (1000)      658 2023-06-06 14:25:53.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.554879 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2023-07-06 14:25:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1656 2023-07-03 12:08:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/for-services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      197 2023-07-06 10:29:30.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.558879 awsibox-0.8.8/awsibox/cfg/ibox/com/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1935 2023-07-06 08:02:40.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/common.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.558879 awsibox-0.8.8/awsibox/cfg/ibox/com/dynamodb/
--rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.558879 awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/securitygroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.566879 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1414 2023-06-14 16:05:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3156 2023-07-03 10:17:08.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5739 2023-07-03 14:54:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      899 2023-06-14 16:05:02.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.566879 awsibox-0.8.8/awsibox/cfg/ibox/com/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.570879 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.574879 awsibox-0.8.8/awsibox/cfg/ibox/com/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-05-01 13:36:02.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-05-01 13:33:03.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/spot_advisor.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.582879 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.582879 awsibox-0.8.8/awsibox/cfg/ibox/com/kms/
--rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.586879 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/layers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/py-packager.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.586879 awsibox-0.8.8/awsibox/cfg/ibox/com/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.586879 awsibox-0.8.8/awsibox/cfg/ibox/com/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)      566 2023-07-07 19:35:03.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/s3/bucket-log.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.590880 awsibox-0.8.8/awsibox/cfg/ibox/com/servicediscovery/
--rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.590880 awsibox-0.8.8/awsibox/cfg/ibox/com/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.590880 awsibox-0.8.8/awsibox/cfg/ibox/com/ssm/
--rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.490878 awsibox-0.8.8/awsibox/cfg/ibox/res/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.594879 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/
--rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/deployments.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/domain-names.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.594879 awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2965 2023-06-14 15:41:11.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.598879 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-06-14 15:45:22.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5218 2023-07-10 08:40:23.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.598879 awsibox-0.8.8/awsibox/cfg/ibox/res/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.602880 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     5910 2023-07-07 08:35:38.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      504 2023-07-06 09:46:36.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/origin-access-controls.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.602880 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/
--rw-r--r--   0 mello     (1000) mello     (1000)     7805 2023-07-03 12:27:14.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1041 2023-06-14 15:57:15.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.602880 awsibox-0.8.8/awsibox/cfg/ibox/res/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1081 2023-06-14 16:01:55.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.606880 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)      604 2023-07-10 12:57:50.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1794 2023-07-04 07:39:01.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      346 2023-06-29 13:36:52.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/securitygroups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      438 2023-07-10 13:10:42.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/subnet-routetable-associations.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1245 2023-07-10 13:15:14.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/subnets.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.610880 awsibox-0.8.8/awsibox/cfg/ibox/res/ecr/
--rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-06-29 14:55:24.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ecr/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.610880 awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     9924 2023-06-14 16:06:44.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1021 2023-06-06 14:25:53.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.610880 awsibox-0.8.8/awsibox/cfg/ibox/res/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/efs/filesystems.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1961 2023-07-03 12:08:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/efs/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.614880 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticache/
--rw-r--r--   0 mello     (1000) mello     (1000)     5327 2023-05-31 09:04:53.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.618880 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     3978 2023-07-03 13:48:39.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5049 2023-07-04 07:33:41.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-07-03 12:17:05.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3618 2023-07-04 07:33:55.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.618880 awsibox-0.8.8/awsibox/cfg/ibox/res/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/events/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.622880 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     3064 2023-07-04 13:41:29.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/instance-profiles.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.626880 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-07-03 12:08:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/functions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2591 2023-06-14 16:23:01.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/versions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.630880 awsibox-0.8.8/awsibox/cfg/ibox/res/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      576 2023-07-04 15:47:10.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     9062 2023-07-04 16:14:49.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/rds/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.630880 awsibox-0.8.8/awsibox/cfg/ibox/res/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/route53/hostedzones.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/route53/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     7296 2023-07-03 09:40:54.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/route53/recordsets.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.634880 awsibox-0.8.8/awsibox/cfg/ibox/res/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)       41 2023-07-05 12:35:38.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/s3/bucket-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    12432 2023-07-07 20:33:32.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/s3/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.634880 awsibox-0.8.8/awsibox/cfg/ibox/res/scheduler/
--rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.634880 awsibox-0.8.8/awsibox/cfg/ibox/res/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      449 2023-06-14 16:29:21.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/sns/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/sns/subscriptions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.638880 awsibox-0.8.8/awsibox/cfg/ibox/res/sqs/
--rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/sqs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/sqs/queue-policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.494878 awsibox-0.8.8/awsibox/cfg/ibox/stacks/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.638880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/
--rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/infra-info.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.638880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/cch/
--rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/cch/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.638880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/clf/
--rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/clf/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.642880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     4610 2023-07-03 10:16:46.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3411 2023-07-03 13:32:23.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.642880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-15 07:56:29.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2401 2023-07-03 15:45:53.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-15 07:55:51.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.642880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/lbd/
--rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.642880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      241 2023-07-04 15:47:16.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/rds/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.654880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/
--rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-06-15 07:57:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-event-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      559 2023-06-16 09:17:19.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      749 2023-07-04 10:04:47.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4070 2023-07-10 13:18:33.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/vpc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.654880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/tsk/
--rw-r--r--   0 mello     (1000) mello     (1000)     2459 2023-06-14 16:36:55.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/tsk/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    17352 2023-07-10 10:25:27.000000 awsibox-0.8.8/awsibox/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6346 2023-07-10 13:32:50.000000 awsibox-0.8.8/awsibox/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/discover.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2315 2023-07-05 16:08:18.000000 awsibox-0.8.8/awsibox/generate.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.670881 awsibox-0.8.8/awsibox/lambdas/
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/ASGSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/AtEdgeAddHeaders.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.8/awsibox/lambdas/CCRFargateSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.8/awsibox/lambdas/CCRLightHouse.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.8/awsibox/lambdas/CCRStackReplicator.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.8/awsibox/lambdas/CloudWatchAlarmStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.8/awsibox/lambdas/CloudWatchRepeatedNotify.code
--rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/EC2StartStopTagged.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.8/awsibox/lambdas/ECSClusterAutoscale.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.8/awsibox/lambdas/ECSDrainInstance.code
--rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.8/awsibox/lambdas/ECSDrainTasks.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.8/awsibox/lambdas/ECSEventTaskStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.8/awsibox/lambdas/ECSEventsSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.8/awsibox/lambdas/ECSRaiseASGAlarm.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.8/awsibox/lambdas/ECSRunTask.code
--rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/ECSUpdateDesiredCount.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/ElasticSearchSnapShot.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5370 2023-06-07 12:49:30.000000 awsibox-0.8.8/awsibox/lambdas/InfraInfo.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.8/awsibox/lambdas/ManageService.code
--rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/PaidApi.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.8/awsibox/lambdas/PyPackager.code
--rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/Python37SSM.layer
--rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.8/awsibox/lambdas/R53RecordInstanceId.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.8/awsibox/lambdas/ServiceDiscovery.code
--rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.8/awsibox/lambdas/ServiceUnavailable.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.8/awsibox/lambdas/StacksOps.code
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.674881 awsibox-0.8.8/awsibox/mod/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.682881 awsibox-0.8.8/awsibox/mod/__pycache__/
--rw-r--r--   0 mello     (1000) mello     (1000)     5503 2023-07-10 12:23:40.000000 awsibox-0.8.8/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     6051 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     3330 2023-07-10 12:23:40.000000 awsibox-0.8.8/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)    17996 2023-07-10 12:23:40.000000 awsibox-0.8.8/awsibox/mod/__pycache__/ec2.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     6211 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     4581 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/iam.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     3491 2023-07-10 12:23:40.000000 awsibox-0.8.8/awsibox/mod/__pycache__/joker.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     6017 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/rds.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     3068 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/s3.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)    14961 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/waf.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     3950 2023-07-03 14:09:13.000000 awsibox-0.8.8/awsibox/mod/autoscaling.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3746 2023-06-16 09:25:14.000000 awsibox-0.8.8/awsibox/mod/cloudformation.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1941 2023-07-08 12:36:18.000000 awsibox-0.8.8/awsibox/mod/cloudfront.py
--rw-r--r--   0 mello     (1000) mello     (1000)     9175 2023-07-10 13:33:26.000000 awsibox-0.8.8/awsibox/mod/ec2.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2946 2023-07-07 20:01:28.000000 awsibox-0.8.8/awsibox/mod/joker.py
--rw-r--r--   0 mello     (1000) mello     (1000)    46519 2023-07-10 12:54:00.000000 awsibox-0.8.8/awsibox/shared.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.682881 awsibox-0.8.8/awsibox/user-data/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.686881 awsibox-0.8.8/awsibox/user-data/SCRIPTS/
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/ELBCHECK.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/END.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/INIT.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/PACKAGE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/SERVICE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/SETUP.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.8/awsibox/user-data/ecs-cluster.sh
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.478878 awsibox-0.8.8/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.478878 awsibox-0.8.8/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.502878 awsibox-0.8.8/build/lib/awsibox.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      877 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)     9428 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.686881 awsibox-0.8.8/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)     3350 2023-06-15 12:57:11.000000 awsibox-0.8.8/scripts/ibox_generate_templates.py
--rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-07-10 13:54:48.690881 awsibox-0.8.8/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      536 2023-06-16 08:09:19.000000 awsibox-0.8.8/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.235693 awsibox-0.8.9/
+-rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.9/.gitignore
+-rw-r--r--   0 mello     (1000) mello     (1000)    10297 2022-03-14 08:29:15.000000 awsibox-0.8.9/LICENSE
+-rw-r--r--   0 mello     (1000) mello     (1000)      257 2023-06-16 08:09:06.000000 awsibox-0.8.9/MANIFEST.in
+-rw-r--r--   0 mello     (1000) mello     (1000)      877 2023-07-14 09:59:16.235693 awsibox-0.8.9/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.9/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.051690 awsibox-0.8.9/awsibox/
+-rw-r--r--   0 mello     (1000) mello     (1000)    19454 2023-07-08 15:37:21.000000 awsibox-0.8.9/awsibox/RP.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-07-14 09:58:45.000000 awsibox-0.8.9/awsibox/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.9/awsibox/args.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.051690 awsibox-0.8.9/awsibox/aws/
+-rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/aws/CloudFormationResourceSpecification.json
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.015689 awsibox-0.8.9/awsibox/cfg/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.031690 awsibox-0.8.9/awsibox/cfg/ibox/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.099691 awsibox-0.8.9/awsibox/cfg/ibox/com/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.107691 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5580 2023-07-13 13:05:17.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/capacity.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1252 2023-06-16 09:13:11.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.107691 awsibox-0.8.9/awsibox/cfg/ibox/com/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.111691 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2023-07-06 14:25:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1656 2023-07-03 12:08:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/for-services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      197 2023-07-06 10:29:30.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.111691 awsibox-0.8.9/awsibox/cfg/ibox/com/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2002 2023-07-13 20:06:15.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/common.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.111691 awsibox-0.8.9/awsibox/cfg/ibox/com/dynamodb/
+-rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.115691 awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/securitygroup.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.119691 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1435 2023-07-11 11:57:43.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1369 2023-07-13 09:22:24.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3201 2023-07-13 12:23:53.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      905 2023-07-13 13:05:23.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5739 2023-07-03 14:54:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      734 2023-07-13 13:05:29.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.119691 awsibox-0.8.9/awsibox/cfg/ibox/com/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.123691 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.131691 awsibox-0.8.9/awsibox/cfg/ibox/com/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2890 2023-07-13 13:04:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6911 2023-07-13 13:05:02.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1568 2023-07-13 13:04:53.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1201 2023-07-13 13:05:09.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/spot_advisor.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.131691 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-07-13 13:05:44.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.135691 awsibox-0.8.9/awsibox/cfg/ibox/com/kms/
+-rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.139691 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/layers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/py-packager.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.139691 awsibox-0.8.9/awsibox/cfg/ibox/com/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.139691 awsibox-0.8.9/awsibox/cfg/ibox/com/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)      566 2023-07-07 19:35:03.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/s3/bucket-log.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.139691 awsibox-0.8.9/awsibox/cfg/ibox/com/servicediscovery/
+-rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.143691 awsibox-0.8.9/awsibox/cfg/ibox/com/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      950 2023-07-13 13:05:35.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.143691 awsibox-0.8.9/awsibox/cfg/ibox/com/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.031690 awsibox-0.8.9/awsibox/cfg/ibox/res/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.147691 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/
+-rw-r--r--   0 mello     (1000) mello     (1000)      146 2023-07-13 13:10:32.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/deployments.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/domain-names.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.147691 awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2925 2023-07-13 13:15:35.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.151691 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2401 2023-07-13 13:08:29.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5129 2023-07-13 12:23:49.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.151691 awsibox-0.8.9/awsibox/cfg/ibox/res/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.151691 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudformation/
+-rw-r--r--   0 mello     (1000) mello     (1000)      706 2023-07-13 13:10:28.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudformation/custom-resources.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      528 2023-07-13 21:39:37.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudformation/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.155691 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5910 2023-07-07 08:35:38.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      504 2023-07-06 09:46:36.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/origin-access-controls.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.155691 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/
+-rw-r--r--   0 mello     (1000) mello     (1000)     7798 2023-07-13 13:11:33.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1041 2023-06-14 15:57:15.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.159691 awsibox-0.8.9/awsibox/cfg/ibox/res/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1076 2023-07-13 13:15:55.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.163691 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      602 2023-07-13 13:07:25.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1794 2023-07-04 07:39:01.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      346 2023-06-29 13:36:52.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/securitygroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      438 2023-07-10 13:10:42.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/subnet-routetable-associations.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1245 2023-07-10 13:15:14.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/subnets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.163691 awsibox-0.8.9/awsibox/cfg/ibox/res/ecr/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-06-29 14:55:24.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ecr/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.163691 awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)    10167 2023-07-13 15:52:54.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1020 2023-07-13 13:08:36.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.167692 awsibox-0.8.9/awsibox/cfg/ibox/res/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/efs/filesystems.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1961 2023-07-03 12:08:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/efs/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.167692 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticache/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5325 2023-07-13 13:07:56.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.171692 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3978 2023-07-03 13:48:39.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5049 2023-07-04 07:33:41.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2828 2023-07-13 13:10:06.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3613 2023-07-13 13:10:19.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.171692 awsibox-0.8.9/awsibox/cfg/ibox/res/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1860 2023-07-13 13:07:34.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/events/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.175692 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3064 2023-07-04 13:41:29.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/instance-profiles.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3686 2023-07-13 13:10:37.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.175692 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-07-03 12:08:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/functions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2591 2023-06-14 16:23:01.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/versions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.175692 awsibox-0.8.9/awsibox/cfg/ibox/res/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      576 2023-07-04 15:47:10.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     9059 2023-07-13 13:09:53.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/rds/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.179692 awsibox-0.8.9/awsibox/cfg/ibox/res/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1426 2023-07-13 13:07:50.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/route53/hostedzones.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/route53/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     7294 2023-07-13 13:07:43.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/route53/recordsets.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.179692 awsibox-0.8.9/awsibox/cfg/ibox/res/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)       41 2023-07-05 12:35:38.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/s3/bucket-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    12432 2023-07-11 12:34:02.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/s3/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.179692 awsibox-0.8.9/awsibox/cfg/ibox/res/scheduler/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1574 2023-07-13 13:08:03.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.183692 awsibox-0.8.9/awsibox/cfg/ibox/res/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      449 2023-06-14 16:29:21.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/sns/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/sns/subscriptions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.183692 awsibox-0.8.9/awsibox/cfg/ibox/res/sqs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/sqs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/sqs/queue-policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.183692 awsibox-0.8.9/awsibox/cfg/ibox/res/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)       57 2023-07-13 15:07:21.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ssm/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      227 2023-07-13 15:48:42.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ssm/parameters.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.035689 awsibox-0.8.9/awsibox/cfg/ibox/stacks/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.183692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/infra-info.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.187692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/cch/
+-rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/cch/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.187692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/clf/
+-rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/clf/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.187692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4605 2023-07-13 13:06:47.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3590 2023-07-13 13:06:56.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.187692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-15 07:56:29.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2399 2023-07-11 12:06:08.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-15 07:55:51.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.191692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/lbd/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1289 2023-07-13 13:07:11.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.191692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      241 2023-07-04 15:47:16.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/rds/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.199692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/
+-rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-06-15 07:57:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1542 2023-07-13 13:07:03.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-event-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      559 2023-06-16 09:17:19.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      749 2023-07-04 10:04:47.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4070 2023-07-10 13:18:33.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/vpc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.199692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/tsk/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2890 2023-07-13 13:06:26.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/tsk/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    17392 2023-07-13 20:36:17.000000 awsibox-0.8.9/awsibox/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6633 2023-07-13 20:39:31.000000 awsibox-0.8.9/awsibox/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/discover.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2315 2023-07-05 16:08:18.000000 awsibox-0.8.9/awsibox/generate.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.219692 awsibox-0.8.9/awsibox/lambdas/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/ASGSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/AtEdgeAddHeaders.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4305 2023-07-11 08:26:15.000000 awsibox-0.8.9/awsibox/lambdas/CCRFargateSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.9/awsibox/lambdas/CCRLightHouse.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.9/awsibox/lambdas/CCRStackReplicator.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.9/awsibox/lambdas/CloudWatchAlarmStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.9/awsibox/lambdas/CloudWatchRepeatedNotify.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/EC2StartStopTagged.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.9/awsibox/lambdas/ECSClusterAutoscale.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.9/awsibox/lambdas/ECSDrainInstance.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.9/awsibox/lambdas/ECSDrainTasks.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.9/awsibox/lambdas/ECSEventTaskStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.9/awsibox/lambdas/ECSEventsSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.9/awsibox/lambdas/ECSRaiseASGAlarm.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.9/awsibox/lambdas/ECSRunTask.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/ECSUpdateDesiredCount.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/ElasticSearchSnapShot.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5370 2023-06-07 12:49:30.000000 awsibox-0.8.9/awsibox/lambdas/InfraInfo.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.9/awsibox/lambdas/ManageService.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/PaidApi.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.9/awsibox/lambdas/PyPackager.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/Python37SSM.layer
+-rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.9/awsibox/lambdas/R53RecordInstanceId.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.9/awsibox/lambdas/ServiceDiscovery.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.9/awsibox/lambdas/ServiceUnavailable.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.9/awsibox/lambdas/StacksOps.code
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.223692 awsibox-0.8.9/awsibox/mod/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.227692 awsibox-0.8.9/awsibox/mod/__pycache__/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5503 2023-07-10 12:23:40.000000 awsibox-0.8.9/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     6051 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3330 2023-07-10 12:23:40.000000 awsibox-0.8.9/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)    17996 2023-07-10 12:23:40.000000 awsibox-0.8.9/awsibox/mod/__pycache__/ec2.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     6211 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     4581 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/iam.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3491 2023-07-10 12:23:40.000000 awsibox-0.8.9/awsibox/mod/__pycache__/joker.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     6017 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/rds.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3068 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/s3.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)    14961 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/waf.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3685 2023-07-13 20:39:15.000000 awsibox-0.8.9/awsibox/mod/autoscaling.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3557 2023-07-13 20:39:15.000000 awsibox-0.8.9/awsibox/mod/cloudformation.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1941 2023-07-08 12:36:18.000000 awsibox-0.8.9/awsibox/mod/cloudfront.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     9160 2023-07-13 19:22:10.000000 awsibox-0.8.9/awsibox/mod/ec2.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3076 2023-07-13 19:22:00.000000 awsibox-0.8.9/awsibox/mod/joker.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    45364 2023-07-14 09:57:33.000000 awsibox-0.8.9/awsibox/shared.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.231692 awsibox-0.8.9/awsibox/user-data/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.235693 awsibox-0.8.9/awsibox/user-data/SCRIPTS/
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/ELBCHECK.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/END.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/INIT.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/PACKAGE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/SERVICE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/SETUP.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.9/awsibox/user-data/ecs-cluster.sh
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.015689 awsibox-0.8.9/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.015689 awsibox-0.8.9/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.043690 awsibox-0.8.9/build/lib/awsibox.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      877 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)     9546 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.235693 awsibox-0.8.9/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     3350 2023-06-15 12:57:11.000000 awsibox-0.8.9/scripts/ibox_generate_templates.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-07-14 09:59:16.239693 awsibox-0.8.9/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      536 2023-06-16 08:09:19.000000 awsibox-0.8.9/setup.py
```

### Comparing `awsibox-0.8.8/.gitignore` & `awsibox-0.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/LICENSE` & `awsibox-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/PKG-INFO` & `awsibox-0.8.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.8
+Version: 0.8.9
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
```

### Comparing `awsibox-0.8.8/awsibox/RP.py` & `awsibox-0.8.9/awsibox/RP.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/args.py` & `awsibox-0.8.9/awsibox/args.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/aws/CloudFormationResourceSpecification.json` & `awsibox-0.8.9/awsibox/aws/CloudFormationResourceSpecification.json`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml`

 * *Files 6% similar despite different names*

```diff
@@ -77,20 +77,20 @@
               And(
                 Condition(f"CloudWatchAlarm{IBOX_TITLE}Backend5XX"),
                 Condition(getattr(cfg, IBOX_RESNAME)["Condition"]))
     - EC2ClassicExternal:
         IBOX_TITLE: LoadBalancerClassicExternal
         Condition: LoadBalancerExternal
         Scheme: 'internet-facing'
-        Subnets: Split(',', get_expvalue('SubnetsPublic'))
+        Subnets: Split(',', ImportValue('SubnetsPublic'))
     - EC2ClassicInternal:
         IBOX_TITLE: LoadBalancerClassicInternal
         Condition: LoadBalancerInternal
         Scheme: 'internal'
-        Subnets: Split(',', get_expvalue('SubnetsPrivate'))
+        Subnets: Split(',', ImportValue('SubnetsPrivate'))
   ElasticLoadBalancingV2LoadBalancer:
     - IBOX_BASE:
         IBOX_LINKED_OBJ:
           Alarm:
             Key: CloudWatchAlarm
             Name: IBOX_TITLE.Target5XX
             Type: IBOX_TITLE.Target5XX
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/capacity.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/capacity.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/for-services.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/for-services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/common.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/common.yml`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     - res/rds/ibox_base.yml
     - res/route53/ibox_base.yml
     - res/s3/ibox_base.yml
     - res/cloudfront/ibox_base.yml
     - res/application-autoscaling/ibox_base.yml
     - res/autoscaling/ibox_base.yml
     - res/apigateway/ibox_base.yml
+    - res/cloudformation/ibox_base.yml
+    - res/ssm/ibox_base.yml
 
 global:
   Parameter:
     - Env:
         Description: Environment
         AllowedValues: ['dev', 'stg', 'prod']
         Default: dev
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/bottlerocket.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/bottlerocket.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/capacityprovider.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/capacityprovider.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     - DaemonReserveCpu:
         Description: 'Empty for mapped value'
         AllowedValues: ['', 'yes', 'no']
   Condition:
     - DaemonReserveCpu:
         get_condition('', 'equals', 'yes', 'DaemonReserveCpu')
   Output:
-    - ClusterStack:
-        Value: Ref("AWS::StackName")
     - DaemonReserveCpu:
         Value: get_endvalue('DaemonReserveCpu')
   DaemonReserveCpu: 'no'
   EC2SecurityGroup:
     - EcsService:
         IBOX_ENABLED: False
   # Included yaml ecs/task.yml have changed ParameterStore Roles to RoleTask, need to restore it.
@@ -30,14 +28,16 @@
   LogsLogGroup: IBOX_SKIP_FUNC
   IAMRole:
     - Task:
         Condition: DaemonReserveCpu
   ECSService:
     - Base:
         IBOX_ENABLED: False
+        ClusterStackName.IBOX_AUTO_PO:
+          Value: Ref("AWS::StackName")
     - Daemon:
         IBOX_ENABLED: True
         Condition: DaemonReserveCpu
         Cluster: Ref('Cluster')
         LoadBalancers: IBOX_SKIP_FUNC
         NetworkConfiguration: IBOX_SKIP_FUNC
         Role: Ref("AWS::NoValue")
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/fargate-spot.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/fargate-spot.yml`

 * *Files 19% similar despite different names*

```diff
@@ -14,30 +14,31 @@
           Condition('ECSTasksLaunchOnFargate'),
           get_condition('', 'equals', 'no', 'FargateSpot')
         )
   ApplicationAutoScalingScalableTarget:
     - ECSService:
         ResourceId:
           If('FargateSpot',
-            get_subvalue('service/${1E}/${ECSServiceSpot.Name}', 'Cluster', 'ClusterStack'),
-            get_subvalue('service/${1E}/${Service.Name}', 'Cluster', 'ClusterStack')
+            Select(5, Split(":", Ref("ECSServiceSpot"))),
+            Select(5, Split(":", Ref("Service"))),
           )
-  CloudFormationCustomResource:
-    - FargateSpot:
-        Condition: FargateSpot
-        DependsOn: ECSServiceSpot
-        ServiceToken: get_expvalue("LambdaCCRFargateSpot")
-        ServiceArn: Ref("ECSServiceSpot")
-        ServiceBase: GetAtt("Service", "Name")
-        ServiceSpot: GetAtt("ECSServiceSpot", "Name")
-        Cluster: get_expvalue("Cluster", "ClusterStack")
-        ScalingPolicy: Ref("ApplicationAutoScalingScalingPolicyCpu")
   ECSService:
-    - Spot:
-        IBOX_ENABLED: True
-        Condition: FargateSpot
-        DependsOn: Service
-        Tags:
-          - ServiceBase:
-              Key: IBOXFARGATESPOTServiceBase
-              Value: GetAtt('Service', 'Name')
+    - Base:
+        IBOX_LINKED_OBJ:
+          CloudFormationCustomResource:
+            Key: CloudFormationCustomResource
+            Name: FargateSpot
+            Type: FargateSpot
+            Conf:
+              IBOX_LINKED_OBJ_NAME: IBOX_TITLE
+          ServiceSpot:
+            Key: ECSService
+            Name: Spot
+            Type: Spot
+            Conf:
+              Condition: FargateSpot
+              DependsOn: IBOX_TITLE
+              Tags:
+                - ServiceBase:
+                    Key: IBOXFARGATESPOTServiceBase
+                    Value: GetAtt(IBOX_TITLE, 'Name')
   FargateSpot: 'no'
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,18 @@
       - com/ecs/daemon-reserver-cpu.yml
       - com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
   - !include
       - stacks/ec2/i_type.yml
       - stacks/ec2/ecs-cluster.yml
 
 global:
-  IBOX_LAUNCH_TEMPLATE_NO_SG_EXTRA: True
   IBOX_ROLE_EX: ecs-cluster
   Output:
     - StackType:
         Value: ec2 ecs
-    - ClusterStack:
-        Value: Ref("AWS::StackName")
   ApplicationAutoScalingScalableTarget:
     - ECSService:
         ResourceId: Sub('service/${Cluster}/${Service.Name}')
   ApplicationAutoScalingScalingPolicy:
     - Cpu:
         IBOX_ENABLED: False
     - Custom:
@@ -82,15 +79,18 @@
     - ParameterStore:
         Roles:
           - Ref('RoleTask')
   LaunchTemplate:
     - Data:
         NetworkInterfaces:
           - eth0:
-              Groups++:
+              Groups:
+                - GetAtt('SecurityGroupInstancesRules', 'GroupId')
                 - ImportValue('SecurityGroupBaseInstance')
   LoadBalancerType: Application
   RecordSet: ['External', 'Internal']
   ECSService:
     - Base:
         DependsOn: ECSClusterCapacityProviderAssociationsBase
         Cluster: Ref('Cluster')
+        ClusterStackName.IBOX_AUTO_PO:
+          Value: Ref("AWS::StackName")
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/task.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/task.yml`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,19 @@
   - com/iam/policy-parameterstore.yml
   - com/iam/policy-ecs-exec.yml
   - com/ec2/securitygroup.yml
 
 
 global:
   Parameter:
-    - ClusterStack:
-        Description: 'Cluster Stack Name used to launch service on - empty for default based on env/role'
     - DockerLabelLastUpdate:
         Description: 'Use to force redeploy - can use: $(date +%F_%T)'
-  Output:
-    - ClusterStack:
-        Value: get_endvalue('ClusterStack')
-  ClusterStack: ecs-a
+  ECSService:
+    - Base:
+        ClusterStackName: ecs-a
   ECSTaskDefinition:
     - Base:
         IBOX_ENABLED: True
   LogsLogGroup:
     - Base:
         IBOX_TITLE: LogsLogGroup
         LogGroupName: Sub('/aws/ecs/${AWS::StackName}')
@@ -25,9 +22,9 @@
   IAMPolicy:
     - ParameterStore:
         Roles:
           - Ref('RoleTask')
   IAMRole:
     - Task:
         ManagedPolicyArns:
-          - get_expvalue('IAMPolicyCloudWatchPutMetric')
+          - ImportValue('IAMPolicyCloudWatchPutMetric')
         Principal: ecs-tasks.amazonaws.com
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
           ZipFile: str(IBOX_INDEXNAME)
         Layers:
           - LambdaLayerVersionPython37SSM
         Runtime: python3.9
         Timeout: 30
         Environment:
           Variables:
-            - SNSTopic: get_expvalue('SNSTopicCloudWatchAlarm')
+            - SNSTopic: ImportValue('SNSTopicCloudWatchAlarm')
     - CloudWatchAlarmStateChange:
         IBOX_ENABLED: False
         Architectures: ['arm64']
         Description: 'CloudWatch Alarm State change to Alarm'
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Layers:
@@ -64,15 +64,15 @@
                 Action:
                   - 'cloudwatch:DescribeAlarms'
                 Effect: Allow
                 Resource: '*'
             - 2:
                 Action: 'sns:Publish'
                 Effect: Allow
-                Resource: get_expvalue('SNSTopicCloudWatchAlarm')
+                Resource: ImportValue('SNSTopicCloudWatchAlarm')
     - LambdaCloudWatchAlarmStateChange:
         IBOX_ENABLED: False
         Roles:
           - Ref('RoleLambdaCloudWatchAlarmStateChange')
         PolicyDocument:
           Statement:
             - 1:
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/events/cluster-autoscale.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/events/cluster-autoscale.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/events/ec2.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/events/ec2.yml`

 * *Files 2% similar despite different names*

```diff
@@ -77,30 +77,30 @@
         Architectures:
           - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'ServiceDiscovery'
         Environment:
           Variables:
-            - NameSpaceID: get_expvalue('ServiceDiscoveryPublicDnsNamespaceId')
+            - NameSpaceID: ImportValue('ServiceDiscoveryPublicDnsNamespaceId')
             - PublicDnsNamespaceName: Sub(f'find.{cfg.HostedZoneNameEnv}')
-            - HostedZoneId: get_expvalue('HostedZoneIdEnv')
+            - HostedZoneId: ImportValue('HostedZoneIdEnv')
         MemorySize: 256
         Runtime: python3.9
         Timeout: 30
     - R53RecordInstanceId:
         Architectures:
           - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'R53 Record InstanceId Automatic Creation'
         Environment:
           Variables:
             - HostedZoneName: get_endvalue('HostedZoneNamePrivate')
-            - HostedZoneId: get_expvalue('HostedZoneIdPrivate')
+            - HostedZoneId: ImportValue('HostedZoneIdPrivate')
             - Topic: Ref('SNSTopicASGNotificationR53')
         MemorySize: 256
         Runtime: python3.9
         Timeout: 30
   LambdaPermission:
     - EC2StartStopTaggedEventsRuleEC2StartTagged:
         FunctionName: GetAtt('LambdaEC2StartStopTagged', 'Arn')
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs-spot.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,21 @@
         Layers:
           - LambdaLayerVersionPython37SSM
           - LambdaLayerVersionPythonArm64SlackClient
         Runtime: python3.9
         Timeout: 30
         Environment:
           Variables:
-            - SNSTopic: get_expvalue('SNSTopicCloudWatchAlarm')
+            - SNSTopic: ImportValue('SNSTopicCloudWatchAlarm')
   IAMPolicy:
     - LambdaECSEventTaskStateChange:
         Roles:
           - Ref('RoleLambdaECSEventTaskStateChange')
         PolicyDocument:
           Statement:
             - 1:
                 Action: 'sns:Publish'
                 Effect: Allow
-                Resource: get_expvalue('SNSTopicCloudWatchAlarm')
+                Resource: ImportValue('SNSTopicCloudWatchAlarm')
     - ParameterStore:
         Roles++:
           - Ref('RoleLambdaECSEventTaskStateChange')
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/events/spot_advisor.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/events/spot_advisor.yml`

 * *Files 25% similar despite different names*

```diff
@@ -17,22 +17,22 @@
           S3Bucket: Sub(cfg.BucketNameAppRepository)
           S3Key: ibox-tools/spot-advisor/spot-advisor.zip
         Description: 'Advise if ASG is using a spot instance type with a high frequency of interruption'
         Runtime: python3.9
         Timeout: 300
         Environment:
           Variables:
-            - SNSTopic: get_expvalue('SNSTopicCloudWatchAlarm')
+            - SNSTopic: ImportValue('SNSTopicCloudWatchAlarm')
   IAMPolicy:
     - LambdaSpotAdvisor:
         Roles:
           - Ref('RoleLambdaSpotAdvisor')
         PolicyDocument:
           Statement:
             - 1:
                 Action: 'sns:Publish'
                 Effect: Allow
-                Resource: get_expvalue('SNSTopicCloudWatchAlarm')
+                Resource: ImportValue('SNSTopicCloudWatchAlarm')
             - 2:
                 Action: 'pricing:GetProducts'
                 Effect: Allow
                 Resource: '*'
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/managed-policies.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   IAMPolicy:
     - ParameterStore:
         PolicyDocument:
           Statement:
             - Decrypt:
                 Action: 'kms:Decrypt'
                 Effect: Allow
-                Resource: get_expvalue('KeyParameterStore')
+                Resource: ImportValue('KeyParameterStore')
             - Describe:
                 Action: 'ssm:DescribeParameters'
                 Effect: Allow
                 Resource: Sub('arn:aws:ssm:${AWS::Region}:${AWS::AccountId}:*')
             - Get:
                 Action: 'ssm:GetParameters'
                 Effect: Allow
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-update_stack.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-update_stack.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/roles.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/py-packager.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/py-packager.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/service-unavailable.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/service-unavailable.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/s3/bucket-log.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/s3/bucket-log.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,10 +21,10 @@
                 Resource: '*'
   SQSQueue:
     - ASGNotificationR53:
         MessageRetentionPeriod: 360
   SNSSubscription:
     - ASGNotificationR53SQSASGNotificationR53:
         IBOX_SOURCE_OBJ: SNSSubscriptionSQS
-        TopicArn: get_expvalue('SNSTopicASGNotificationR53')
+        TopicArn: ImportValue('SNSTopicASGNotificationR53')
         Endpoint: GetAtt('SQSQueueASGNotificationR53', 'Arn')
         Protocol: sqs
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 global:
   ApplicationAutoScalingScalableTarget:
     - ECSService:
         IBOX_ENABLED: False
         MaxCapacity: get_endvalue('CapacityMax')
         MinCapacity: get_endvalue('CapacityMin')
-        ResourceId: get_subvalue('service/${1E}/${Service.Name}', 'Cluster', 'ClusterStack')
-        RoleARN: get_expvalue('RoleEC2ContainerServiceAutoscale', '')
+        ResourceId: Select(5, Split(":", Ref("Service")))
+        RoleARN: ImportValue('RoleEC2ContainerServiceAutoscale')
         ScalableDimension: 'ecs:service:DesiredCount'
         ServiceNamespace: ecs
         ScheduledActions:
           - IBOX_BASE:
               IBOX_PARAMETER:
                 - IBOX_REFNAME.Enabled:
                     Description: 'Empty for mapped value'
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml`

 * *Files 2% similar despite different names*

```diff
@@ -60,8 +60,8 @@
               - HealthCheck
               - ReplaceUnhealthy
               - AlarmNotification
               - ScheduledActions
             WaitOnResourceSignals: true
           AutoScalingScheduledAction:
             IgnoreUnmodifiedGroupSizeProperties: true
-        VPCZoneIdentifier: Split(',', get_expvalue('SubnetsPrivate'))
+        VPCZoneIdentifier: Split(',', ImportValue('SubnetsPrivate'))
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,14 @@
         KeyName: none
         Monitoring:
           Enabled: false
         NetworkInterfaces:
           - eth0:
               AssociatePublicIpAddress: false
               DeviceIndex: 0
-              Groups:
-                - GetAtt('SecurityGroupInstancesRules', 'GroupId')
         TagSpecifications:
           - instance:
               ResourceType: instance
               Tags:
                 - Name:
                     Key: Name
                     Value: Ref('EnvRole')
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/policies.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/alarms.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/alarms.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Target5XX: &target5xx
-  AlarmActions: [get_expvalue('SNSTopicCloudWatchAlarm')]
+  AlarmActions: [ImportValue('SNSTopicCloudWatchAlarm')]
   EvaluationPeriods: 2
   MetricName: HTTPCode_Target_5XX_Count
   Statistic: Sum
   ComparisonOperator: 'GreaterThanThreshold'
   Threshold: '50'
   TreatMissingData: 'notBreaching'
   Namespace: 'AWS/ApplicationELB'
 
 LoadBalancerApplication5XX: &alb5xx
-  AlarmActions: [get_expvalue('SNSTopicCloudWatchAlarm')]
+  AlarmActions: [ImportValue('SNSTopicCloudWatchAlarm')]
   EvaluationPeriods: 2
   MetricName: HTTPCode_ELB_5XX_Count
   Statistic: Sum
   ComparisonOperator: 'GreaterThanThreshold'
   Threshold: '50'
   TreatMissingData: 'notBreaching'
   Namespace: 'AWS/ApplicationELB'
 
 Backend5XX: &backend5xx
-  AlarmActions: [get_expvalue('SNSTopicCloudWatchAlarm')]
+  AlarmActions: [ImportValue('SNSTopicCloudWatchAlarm')]
   EvaluationPeriods: 2
   MetricName: HTTPCode_Backend_5XX
   Statistic: Sum
   ComparisonOperator: GreaterThanThreshold
   Threshold: '50'
   TreatMissingData: 'notBreaching'
   Namespace: 'AWS/ELB'
@@ -95,15 +95,15 @@
         Value: Ref('AutoScalingGroup')
   Namespace: 'AWS/EC2'
 
 ECS: &ecs
   Dimensions:
     - Cluster:
         Name: ClusterName
-        Value: get_expvalue('Cluster', 'ClusterStack')
+        Value: Select(1, Split("/", Ref("Service")))
     - Service:
         Name: ServiceName
         Value: GetAtt('Service', 'Name')
   Namespace: 'AWS/ECS'
 
 
 CPU: &cpu
@@ -230,16 +230,16 @@
         Statistic: 'Maximum'
         Threshold: '80'
         Unit: Percent
     - SQSQueueDeadLetter:
         IBOX_PARAMETER:
           - _Threshold:
               AllowedValues: ['', '1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
-              AlarmActions: [get_expvalue('SNSTopicCloudWatchAlarm')]
-        AlarmActions: [get_expvalue('SNSTopicCloudWatchAlarm')]
+              AlarmActions: [ImportValue('SNSTopicCloudWatchAlarm')]
+        AlarmActions: [ImportValue('SNSTopicCloudWatchAlarm')]
         EvaluationPeriods: 1
         ComparisonOperator: GreaterThanThreshold
         Dimensions:
           - SQSQueue:
               Name: QueueName
               Value: GetAtt(IBOX_LINKED_OBJ_NAME, 'QueueName')
         MetricName: ApproximateNumberOfMessagesVisible
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,8 @@
               Bucket: Sub(cfg.BucketNameAppRepository)
               BundleType: tgz
               Key: Join('', [
                   get_endvalue(f"{IBOX_RESNAME}ApplicationName"), "/", get_endvalue(f"{IBOX_RESNAME}ApplicationName"), "-",
                   Sub(getattr(cfg, f'{IBOX_CURNAME}Suffix')),
                 ])
         DeploymentGroupName: get_subvalue("${AWS::StackName}.${EnvRole}-${1M}", f"{IBOX_RESNAME}ApplicationName")
-        ServiceRoleArn: get_expvalue("RoleCodeDeploy", "")
+        ServiceRoleArn: ImportValue("RoleCodeDeploy")
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/ibox_base.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
   - res/ec2/securitygroups.yml
   - res/ec2/securitygroupingresses.yml
 
 global:
   EC2VPCEndpoint:
     - IBOX_BASE:
         Create: 'no'
-        RouteTableIds: [get_expvalue("RouteTablePrivate")]
-        VpcId: get_expvalue("VpcId")
+        RouteTableIds: [ImportValue("RouteTablePrivate")]
+        VpcId: ImportValue("VpcId")
   EC2Subnet:
     - IBOX_BASE:
         IBOX_ENABLED: False
         Condition: str(f"Zone{IBOX_LINKED_OBJ_NAME}")
         AvailabilityZone: Sub("${AWS::Region}%s" % IBOX_LINKED_OBJ_NAME.lower())
         VpcId: Ref("VPC")
   EC2SubnetRouteTableAssociation:
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/subnets.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/subnets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/ecr/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/ecr/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/ibox_base.yml`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,21 @@
               Value: ${NetworkMode}
         IBOX_TITLE: TaskDefinition
         ContainerDefinitions:
           - IBOX_BASE:
               IBOX_PARAMETER:
                 - EnvApp.IBOX_PROPNAME.Version:
                     IBOX_ENABLED_IF: hasattr(cfg, f"{IBOX_REFNAME}ImageSuffix")
+                    IBOX_LINKED_OBJ:
+                      SSMParameter:
+                        Key: SSMParameter
+                        Name: EnvApp.IBOX_PROPNAME.Version
+                        Type: EnvAppVersion
+                        Conf:
+                          IBOX_LINKED_OBJ_NAME: EnvApp.IBOX_PROPNAME.Version
                     Description: str(f'EnvApp{IBOX_PROPNAME}Version')
                     Default: "1"
                     AllowedPattern: '^[a-zA-Z0-9-_.]+$'
                 - IBOX_REFNAME.Cpu:
                     Description: 'Cpu Share - empty for mapped value'
                 - IBOX_REFNAME.Memory:
                     Description: 'Memory hard limit - empty for mapped value'
@@ -110,17 +117,14 @@
                     Value: Ref('AWS::StackName')
                 - EnvRegion:
                     Name: EnvRegion
                     Value: Ref('AWS::Region')
                 - EnvBrand:
                     Name: EnvBrand
                     Value: cfg.BrandDomain
-                - EnvClusterStackName:
-                    Name: EnvClusterStackName
-                    Value: get_endvalue('ClusterStack')
               Essential: true
               HostPort: none
               Image: Join('', [
                   get_endvalue('EcrAccount'), '.dkr.ecr.', Ref('AWS::Region'), '.amazonaws.com/',
                   Sub(getattr(cfg, f'{IBOX_REFNAME}ImageSuffix'))
                 ])
               LinuxParameters:
@@ -161,26 +165,27 @@
               StopTimeout: 30
               UseTaskDefinition:
                 Cpu: 'yes'
                 Memory: 'yes'
         # End ContainerDefinitions
         Cpu.IBOX_CODE: If(IBOX_CURNAME, get_endvalue(IBOX_CURNAME), Ref('AWS::NoValue'))
         Cpu: none
-        ExecutionRoleArn: If('ECSTasksLaunchOnFargate', get_expvalue('RoleECSTaskExecution'), Ref('AWS::NoValue'))
+        ExecutionRoleArn: If('ECSTasksLaunchOnFargate', ImportValue('RoleECSTaskExecution'), Ref('AWS::NoValue'))
         Memory.IBOX_CODE: If(IBOX_CURNAME, get_endvalue(IBOX_CURNAME), Ref('AWS::NoValue'))
         Memory: none
         NetworkMode.IBOX_CODE: If("ECSTasksLaunchOnFargate", "awsvpc", get_endvalue(IBOX_CURNAME))
         NetworkMode: bridge
         RequiresCompatibilities: If('ECSTasksLaunchOnFargate', ['EC2', 'FARGATE'], ['EC2'])
         TaskRoleArn: Ref('RoleTask')
 
   ECSService:
     - IBOX_BASE:
         IBOX_ENABLED: False
-        Cluster: get_expvalue('Cluster', 'ClusterStack')
+        ClusterStackName.IBOX_AUTO_PO: {}
+        Cluster: get_expvalue('Cluster', f'{IBOX_RESNAME}ClusterStackName')
         EnableExecuteCommand.IBOX_CODE: If(
             f'{IBOX_RESNAME}EnableExecuteCommandOverride',
             Ref(f'{IBOX_RESNAME}EnableExecuteCommand'),
             If('ECSTasksLaunchOnFargate', True, get_endvalue(f'{IBOX_RESNAME}EnableExecuteCommand', add_override=False)))
         EnableExecuteCommand.IBOX_AUTO_PO:
           Description: 'empty for mapped value - Default to "true" for FARGATE'
           AllowedValues: ['', 'true', 'false']
@@ -194,10 +199,10 @@
         NetworkConfiguration:
           IBOX_IF:
             - ECSTaskDefinitionBaseNetworkModeAwsVpc
             - IBOX_IFVALUE
             - Ref('AWS::NoValue')
           AwsvpcConfiguration:
             SecurityGroups: list([GetAtt('SecurityGroupEcsService', 'GroupId')]) + cfg.SecurityGroupsImport
-            Subnets: Split(',', get_expvalue('SubnetsPrivate'))
+            Subnets: Split(',', ImportValue('SubnetsPrivate'))
         PlatformVersion: If('ECSTasksLaunchOnFargate', 'LATEST', Ref('AWS::NoValue'))
         TaskDefinition: Ref('TaskDefinition')
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/services.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,14 @@
               IBOX_ENABLED_IF: 'False'
         IBOX_BASE_SKIP: True
         IBOX_SOURCE_OBJ: ECSTaskDefinitionBase
         IBOX_TITLE: TaskDefinitionFargate
         IBOX_ENABLED: False
         Cpu.IBOX_CODE: get_endvalue(IBOX_CURNAME)
         Cpu: '256'
-        ExecutionRoleArn: get_expvalue('RoleECSTaskExecution')
+        ExecutionRoleArn: ImportValue('RoleECSTaskExecution')
         Memory.IBOX_CODE: get_endvalue(IBOX_CURNAME)
         Memory: '512'
         NetworkMode.IBOX_CODE: get_endvalue(IBOX_CURNAME)
         NetworkMode: awsvpc
         RequiresCompatibilities: ['FARGATE']
         TaskRoleArn: Ref('RoleTask')
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/efs/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/efs/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticache/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticache/ibox_base.yml`

 * *Files 4% similar despite different names*

```diff
@@ -68,18 +68,18 @@
         Condition: ReplicationGroup
         Value: get_endvalue(f'ElastiCacheReplicationGroup{IBOX_INDEXNAME}NumCacheClusters')
 
 
 Cluster: &cluster
   Condition: CacheCluster
   ## Internal
-  CacheSubnetGroupName: get_expvalue(f'CacheSubnetGroupPrivate')
+  CacheSubnetGroupName: ImportValue(f'CacheSubnetGroupPrivate')
   VpcSecurityGroupIds: [Ref('SecurityGroupCCH')]
   ## External
-  #CacheSubnetGroupName: get_expvalue(f'CacheSubnetGroupPublic')
+  #CacheSubnetGroupName: ImportValue(f'CacheSubnetGroupPublic')
   #CacheSecurityGroupNames: [Ref('SecurityGroupCCH')]
   AZMode: single-az
   AutoMinorVersionUpgrade: true
   NumCacheNodes: 1
 
 ReplicationGroup: &replication-group
   Condition: ReplicationGroup
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,24 @@
         Export: Export(Sub('%sDNS-${AWS::StackName}' % IBOX_TITLE))
     - _FullName:
         Condition: IBOX_TITLE
         Value: GetAtt(IBOX_TITLE, 'LoadBalancerFullName')
         Export: Export(Sub('%sFullName-${AWS::StackName}' % IBOX_TITLE))
   Condition: IBOX_TITLE
   SecurityGroups:
-    - get_expvalue(f'SecurityGroup{IBOX_TITLE}')
+    - ImportValue(f'SecurityGroup{IBOX_TITLE}')
     - GetAtt(f'SecurityGroup{IBOX_TITLE}', 'GroupId')
 
 External: &external
   Scheme: 'internet-facing'
-  Subnets: Split(',', get_expvalue('SubnetsPublic'))
+  Subnets: Split(',', ImportValue('SubnetsPublic'))
 
 Internal: &internal
   Scheme: 'internal'
-  Subnets: Split(',', get_expvalue('SubnetsPrivate'))
+  Subnets: Split(',', ImportValue('SubnetsPrivate'))
 
 global:
   ElasticLoadBalancingV2LoadBalancer:
     - EC2ApplicationExternal:
         IBOX_ENABLED: False
         <<: [*external, *app]
     - EC2ApplicationInternal:
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Key: 'deregistration_delay.timeout_seconds'
         Value.IBOX_AUTO_PO: {}
         Value: '30'
     - GroupCookieSticky:
         Key: 'stickiness.enabled'
         Value: If(f'{IBOX_MAPNAME}TargetGroupAttributesCookieDurationValue', 'true', 'false')
   Protocol: HTTP
-  VpcId: get_expvalue('VpcId')
+  VpcId: ImportValue('VpcId')
 
 global:
   ElasticLoadBalancingV2TargetGroup:
     - EC2LoadBalancerApplicationExternal:
         IBOX_ENABLED: False
         IBOX_LINKED_OBJ:
           Key: EC2SecurityGroupIngress
@@ -46,45 +46,45 @@
         IBOX_ENABLED: False
         IBOX_LINKED_OBJ:
           Key: EC2SecurityGroupIngress
           Name: LoadBalancerNetworkExternal
           Type: EC2LoadBalancerNetworkInstancesRule
         Port: 80
         Protocol: TCP
-        VpcId: get_expvalue('VpcId')
+        VpcId: ImportValue('VpcId')
     - EC2LoadBalancerNetworkInternal:
         IBOX_ENABLED: False
         IBOX_LINKED_OBJ:
           Key: EC2SecurityGroupIngress
           Name: LoadBalancerNetworkInternal
           Type: EC2LoadBalancerNetworkInstancesRule
         Port: 80
         Protocol: TCP
-        VpcId: get_expvalue('VpcId')
+        VpcId: ImportValue('VpcId')
     - ECSLoadBalancerApplicationDefaultExternal:
         IBOX_ENABLED: False
         IBOX_TITLE: TargetGroupServiceUnavailableExternal
         IBOX_OUTPUT:
           - TargetGroupServiceUnavailableExternal:
               Value: Ref("TargetGroupServiceUnavailableExternal")
         Condition: LoadBalancerApplicationExternal
         Targets:
           - ServiceUnavailable:
-              Id: get_expvalue(f'LambdaServiceUnavailableArn')
+              Id: ImportValue(f'LambdaServiceUnavailableArn')
         TargetType: lambda
     - ECSLoadBalancerApplicationDefaultInternal:
         IBOX_ENABLED: False
         IBOX_TITLE: TargetGroupServiceUnavailableInternal
         IBOX_OUTPUT:
           - TargetGroupServiceUnavailableInternal:
               Value: Ref("TargetGroupServiceUnavailableInternal")
         Condition: LoadBalancerApplicationInternal
         Targets:
           - ServiceUnavailable:
-              Id: get_expvalue(f'LambdaServiceUnavailableArn')
+              Id: ImportValue(f'LambdaServiceUnavailableArn')
         TargetType: lambda
     - ECSLoadBalancerApplicationExternal:
         IBOX_ENABLED: False
         <<: *base
         Port: get_endvalue('ECSTaskDefinitionBaseContainerDefinitions1ContainerPort')
         TargetType: If('ECSTaskDefinitionBaseNetworkModeAwsVpc', 'ip', Ref('AWS::NoValue'))
     - ECSLoadBalancerApplicationInternal:
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/events/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/events/ibox_base.yml`

 * *Files 16% similar despite different names*

```diff
@@ -18,23 +18,26 @@
             Conf:
               IBOX_RESNAME: LambdaPermission.IBOX_INDEXNAME.IBOX_RESNAME
               IBOX_LINKED_OBJ_NAME: getattr(cfg, f"{IBOX_RESNAME}TargetsLambda0Arn")
               IBOX_LINKED_OBJ_INDEX: GetAtt("IBOX_RESNAME", 'Arn')
     - TargetECSCluster:
         IBOX_BASE_SKIP: True
         IBOX_ENABLED: False
+        ClusterStackName.IBOX_AUTO_PO: {}
         Targets:
           - ECSCluster0:
-              Arn: 'get_subvalue("arn:aws:ecs:${AWS::Region}:${AWS::AccountId}:cluster/${1E}", "Cluster", stack="ClusterStack")'
+              Arn: >-
+                get_subvalue(
+                  "arn:aws:ecs:${AWS::Region}:${AWS::AccountId}:cluster/${1E}", "Cluster", stack=f"{IBOX_RESNAME}ClusterStackName")
               EcsParameters:
                 LaunchType: get_endvalue("ServiceBaseLaunchType")
                 NetworkConfiguration:
                   IBOX_IF:
                     - ECSTaskDefinitionBaseNetworkModeAwsVpc
                     - IBOX_IFVALUE
                     - Ref("AWS::NoValue")
                   AwsVpcConfiguration:
                     SecurityGroups: cfg.SecurityGroupsImport
-                    Subnets: Split(",", get_expvalue("SubnetsPrivate"))
+                    Subnets: Split(",", ImportValue("SubnetsPrivate"))
                 TaskDefinitionArn: Ref("TaskDefinition")
-              RoleArn: get_expvalue("RoleECSEvents")
+              RoleArn: ImportValue("RoleECSEvents")
               Id: str(f"TargetECSCluster0")
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/iam/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/iam/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/iam/managed-policies.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/iam/managed-policies.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   Effect: Allow
   Resource: '*'
 SSMParameterStoreBase02: &ssm_parameter_store_base_02
   Action:
     - 'kms:Decrypt'
     - 'kms:Encrypt'
   Effect: Allow
-  Resource: get_expvalue('KeyParameterStore')
+  Resource: ImportValue('KeyParameterStore')
 
 LogRead01: &log_read_01
   Action:
     - 'logs:Describe*'
     - 'logs:Get*'
     - 'logs:List*'
     - 'logs:StartQuery'
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/iam/policies.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/iam/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/iam/roles.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/functions.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/functions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/permissions.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/permissions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/versions.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/versions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/rds/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/rds/ibox_base.yml`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 Mysql: &mysql
   Engine: mysql
   EngineVersion: '5.7'
 
 MysqlInternal:
   <<: *mysql
   PubliclyAccessible: false
-  DBSubnetGroupName: get_expvalue('DBSubnetGroupPrivate')
+  DBSubnetGroupName: ImportValue('DBSubnetGroupPrivate')
 MysqlExternal:
   <<: *mysql
   PubliclyAccessible: true
-  DBSubnetGroupName: get_expvalue('DBSubnetGroupPublic')
+  DBSubnetGroupName: ImportValue('DBSubnetGroupPublic')
 
 global:
   RDSDBInstance:
     # Here i use IBOX_MAPNAME in place of IBOX_RESNAME because current resource name IBOX_RESNAME is simply DBInstance.
     # Instead i want to have a code that permit to create multiple rds resources in the same stack.
     - IBOX_BASE:
         IBOX_ENABLED: False
@@ -156,15 +156,15 @@
         MasterUsername: masterusername
         MasterUserPassword.IBOX_CODE: If(f"{IBOX_REFNAME}DBInstanceSkipProperties", Ref("AWS::NoValue"), get_endvalue(IBOX_CURNAME))
         MasterUserPassword: masteruserpassword
         MaxAllocatedStorage: 0
         MaxAllocatedStorage.IBOX_CODE:
           If(f'{IBOX_MAPNAME}StorageAutoScaling', get_endvalue(f'{IBOX_MAPNAME}MaxAllocatedStorage'), Ref('AWS::NoValue'))
         MonitoringInterval: 0
-        MonitoringRoleArn: If(f'{IBOX_MAPNAME}MonitoringInterval', get_expvalue('RoleRDSEnhancedMonitoring'), Ref('AWS::NoValue'))
+        MonitoringRoleArn: If(f'{IBOX_MAPNAME}MonitoringInterval', ImportValue('RoleRDSEnhancedMonitoring'), Ref('AWS::NoValue'))
         MultiAZ: false
         PerformanceInsights: 0
         PerformanceInsightsRetentionPeriod:
           If(f'{IBOX_MAPNAME}PerformanceInsights', get_endvalue(f'{IBOX_MAPNAME}PerformanceInsights'), Ref('AWS::NoValue'))
         SourceDBInstanceIdentifier.IBOX_CODE: If(IBOX_CURNAME, get_endvalue(IBOX_CURNAME), Ref("AWS::NoValue"))
         SourceDBInstanceIdentifier: none
         StorageThroughput.IBOX_CODE:
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/route53/hostedzones.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/route53/hostedzones.yml`

 * *Files 2% similar despite different names*

```diff
@@ -36,9 +36,9 @@
         <<: *private
         Enabled: 'yes'
         HostedZoneConfig:
             Comment: Sub('${EnvShort} private zone ${AWS::Region}')
         Name: Sub(cfg.HostedZoneNamePrivate)
         VPCs:
           - Vpc1:
-              VPCId: get_expvalue('VpcId')
+              VPCId: ImportValue('VpcId')
               VPCRegion: Ref('AWS::Region')
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/route53/recordsets.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/route53/recordsets.yml`

 * *Files 0% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 
 ZoneExternal: &zone_external
   HostedZoneId: >-
       If(
         "HostedZoneEnv",
         Ref("HostedZoneEnv"),
         get_endvalue("Route53HostedZoneEnvId"),
-      ) if "Env" in getattr(cfg, "Route53HostedZone", []) else get_expvalue('HostedZoneIdEnv')
+      ) if "Env" in getattr(cfg, "Route53HostedZone", []) else ImportValue('HostedZoneIdEnv')
   Name: Sub('${AWS::StackName}.${EnvRole}.%s' % cfg.HostedZoneNameRegionEnv)
 
 ZoneInternal: &zone_internal
   HostedZoneId: >-
       If(
         "HostedZonePrivate",
         Ref("HostedZonePrivate"),
         get_endvalue("Route53HostedZonePrivateId"),
-      ) if "Private" in getattr(cfg, "Route53HostedZone", []) else get_expvalue('HostedZoneIdPrivate')
+      ) if "Private" in getattr(cfg, "Route53HostedZone", []) else ImportValue('HostedZoneIdPrivate')
   Name: Sub('${AWS::StackName}.${EnvRole}.%s' % cfg.HostedZoneNamePrivate)
 
 LoadBalancer: &loadbalancer
   AliasTarget: &loadbalancer_alias_target
     HostedZoneId: get_endvalue('HostedZoneIdLBNET' if getattr("cfg", "LoadBalancerType", "") == "Network" else 'HostedZoneIdLB')
   Type: A
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/s3/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/s3/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/scheduler/ibox_base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/scheduler/ibox_base.yml`

 * *Files 18% similar despite different names*

```diff
@@ -17,21 +17,24 @@
             Conf:
               IBOX_RESNAME: LambdaPermission.IBOX_RESNAME
               IBOX_LINKED_OBJ_NAME: getattr(cfg, f"{IBOX_RESNAME}TargetArn")
               IBOX_LINKED_OBJ_INDEX: GetAtt("IBOX_RESNAME", 'Arn')
     - TargetECSCluster:
         IBOX_BASE_SKIP: True
         IBOX_ENABLED: False
+        ClusterStackName.IBOX_AUTO_PO: {}
         Target:
-          Arn: 'get_subvalue("arn:aws:ecs:${AWS::Region}:${AWS::AccountId}:cluster/${1E}", "Cluster", stack="ClusterStack")'
+          Arn: >-
+            get_subvalue(
+              "arn:aws:ecs:${AWS::Region}:${AWS::AccountId}:cluster/${1E}", "Cluster", stack=f"{IBOX_RESNAME}ClusterStackName")
           EcsParameters:
             LaunchType: get_endvalue("ServiceBaseLaunchType")
             NetworkConfiguration:
               IBOX_IF:
                 - ECSTaskDefinitionBaseNetworkModeAwsVpc
                 - IBOX_IFVALUE
                 - Ref("AWS::NoValue")
               AwsvpcConfiguration:
                 SecurityGroups: cfg.SecurityGroupsImport
-                Subnets: Split(",", get_expvalue("SubnetsPrivate"))
+                Subnets: Split(",", ImportValue("SubnetsPrivate"))
             TaskDefinitionArn: Ref("TaskDefinition")
-          RoleArn: get_expvalue("RoleECSEvents")
+          RoleArn: ImportValue("RoleECSEvents")
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/sns/subscriptions.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/sns/subscriptions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/res/sqs/queue-policies.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/res/sqs/queue-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/i_type.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/infra-info.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/infra-info.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     - ECSDrainInstance:
         IBOX_TITLE: ASGLifecycleHookECSDrainInstance
         AutoScalingGroupName: Ref('AutoScalingGroup')
         DefaultResult: 'ABANDON'
         HeartbeatTimeout.IBOX_AUTO_PO: {}
         HeartbeatTimeout: 3600
         LifecycleTransition: 'autoscaling:EC2_INSTANCE_TERMINATING'
-        NotificationTargetARN: get_expvalue('SNSTopicECSDrainInstance')
-        RoleARN: get_expvalue('RoleASGLifecycleHookECSDrainInstance')
+        NotificationTargetARN: ImportValue('SNSTopicECSDrainInstance')
+        RoleARN: ImportValue('RoleASGLifecycleHookECSDrainInstance')
   AutoScalingGroup:
     - Base:
         Tags:
           - ECSCluster:
               Key: ECSCluster
               Value: Ref('Cluster')
               PropagateAtLaunch: true
@@ -65,20 +65,20 @@
         IBOX_ENABLED: False
     - EC2CPULow:
         IBOX_ENABLED: False
   EC2SecurityGroupIngress:
     - ContainerInstanceExternal:
         FromPort: 32768
         GroupId: GetAtt('SecurityGroupInstancesRules', 'GroupId')
-        SourceSecurityGroupId: get_expvalue('SecurityGroupLoadBalancerApplicationExternal')
+        SourceSecurityGroupId: ImportValue('SecurityGroupLoadBalancerApplicationExternal')
         ToPort: 60999
     - ContainerInstanceInternal:
         FromPort: 32768
         GroupId: GetAtt('SecurityGroupInstancesRules', 'GroupId')
-        SourceSecurityGroupId: get_expvalue('SecurityGroupLoadBalancerApplicationInternal')
+        SourceSecurityGroupId: ImportValue('SecurityGroupLoadBalancerApplicationInternal')
         ToPort: 60999
   ECSCluster:
     - Base:
         IBOX_TITLE: Cluster
         IBOX_PARAMETER:
           - _ClusterAutoReduceTag:
               Description: Empty for mapped value
@@ -122,15 +122,15 @@
             - '/aws/service/bottlerocket/aws-ecs-1/x86_64/latest/image_id'
             - '/aws/service/bottlerocket/aws-ecs-1/arm64/latest/image_id'
   Listeners: []
   RecordSet: []
   IAMRole:
     - Instance:
         ManagedPolicyArns++:
-          - get_expvalue('IAMPolicyEcs')
+          - ImportValue('IAMPolicyEcs')
 
 dev: &cfg_dev
   AutoScalingLifecycleHook:
     ECSDrainInstance:
       HeartbeatTimeout: 900
   LaunchTemplateData:
     ImageId: latest
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/i_type.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/i_type.yml`

 * *Files 11% similar despite different names*

```diff
@@ -66,14 +66,19 @@
                 CustomOriginConfig:
                   HTTPSPort.IBOX_CODE: If(
                     f"{IBOX_CURNAME}Override", Ref(IBOX_CURNAME), get_endvalue("ElasticLoadBalancingV2ListenerEC2LoadBalancerApplicationExternalHttpsPort"))
   EC2SecurityGroup:
     - InstancesRules:
         IBOX_NO_OUTPUT: True
         GroupDescription: Enable Access from LoadBalancer to Instances and between Instances
+  LaunchTemplate:
+    - Data:
+        NetworkInterfaces:
+          - eth0:
+              Groups: list([GetAtt('SecurityGroupInstancesRules', 'GroupId')]) + cfg.SecurityGroupsImport
   LoadBalancerType: Classic
   IAMPolicy:
     - CloudFormation:
         Roles:
           - Ref('RoleInstance')
         PolicyDocument:
           Statement:
@@ -85,16 +90,16 @@
                 Resource: Sub('arn:aws:cloudformation:*:*:stack/${AWS::StackName}/*')
     - ParameterStore:
         Roles:
           - Ref('RoleInstance')
   IAMRole:
     - Instance:
         ManagedPolicyArns:
-          - get_expvalue('IAMPolicyBaseInstance')
-          - get_expvalue('IAMPolicySSM')
+          - ImportValue('IAMPolicyBaseInstance')
+          - ImportValue('IAMPolicySSM')
         Principal: ec2.amazonaws.com
 
 dev: &cfg_dev
   CloudWatchAlarm:
     LoadBalancerClassicExternalBackend5XX:
       EvaluationPeriods: 0
     LoadBalancerClassicInternalBackend5XX:
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/buildkite.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/buildkite.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/i_type.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/i_type.yml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         IBOX_ENABLED: True
     - Custom:
         TargetTrackingScalingPolicyConfiguration:
           CustomizedMetricSpecification:
             Dimensions:
               - Cluster:
                   Name: ClusterName
-                  Value: get_expvalue('Cluster', 'ClusterStack')
+                  Value: Select(1, Split("/", Ref("Service")))
               - Service:
                   Name: ServiceName
                   Value: GetAtt('Service', 'Name')
   CloudFrontDistribution:
     - IBOX_BASE:
         DistributionConfig:
           Origins:
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                   - 'ssm:DescribeParameters'
                   - 'kms:ListAliases'
                 Effect: Allow
                 Resource: '*'
             - KMSKey:
                 Action: 'kms:Decrypt'
                 Effect: Allow
-                Resource: get_expvalue('KeyParameterStore')
+                Resource: ImportValue('KeyParameterStore')
   Lambda:
     - StacksOps:
         Architectures:
           - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Stacks Operations'
@@ -36,9 +36,9 @@
           - LambdaLayerVersionPython37SSM
           - LambdaLayerVersionPythonArm64IboxStacksOps
           - LambdaLayerVersionPythonArm64SlackClient
         MemorySize: 512
         Runtime: python3.9
         Environment:
           Variables:
-            - CloudFormationNotificationArn: get_expvalue('SNSTopicCloudFormationNotification')
+            - CloudFormationNotificationArn: ImportValue('SNSTopicCloudFormationNotification')
         Timeout: 60
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-base.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 Resource: Sub('arn:aws:ecs:${AWS::Region}:${AWS::AccountId}:task-definition/lth-t-*')
             - 2:
                 Action:
                   - 'iam:PassRole'
                 Effect: Allow
                 Resource:
                   - Sub('arn:aws:iam::${AWS::AccountId}:role/lth-t-*')
-                  - get_expvalue('RoleECSTaskExecution')
+                  - ImportValue('RoleECSTaskExecution')
             - 3:
                 Action:
                   - 'events:ListTargetsByRule'
                 Effect: Allow
                 Resource: '*'
   Lambda:
     - CCRLightHouse:
```

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-extra-01.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-extra-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/vpc.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/vpc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/cfg/ibox/stacks/tsk/i_type.yml` & `awsibox-0.8.9/awsibox/cfg/ibox/stacks/tsk/i_type.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 IBoxLoader: !include
   - com/ecs/task.yml
 
 global:
+  Parameter:
+    - ECSRunTaskClusterStackName:
+        Description: "Empty for mapped value"
   Condition:
     - EnableExecuteCommand: Equals(True, False)
       # Need to create a "dummy" Condition for tasks that do not use EventsRuleECSRunTask, where there is the "right" one
     - ECSTasksLaunchOnFargate: Equals(True, True)
+  Output:
+    - ECSRunTaskClusterName:
+        Value: get_expvalue('Cluster', 'ECSRunTaskClusterStackName')
+    - ECSRunTaskClusterStackName:
+        Value: get_endvalue("ECSRunTaskClusterStackName")
+    - ECSRunTaskSubnetsPrivate:
+        Value: ImportValue("SubnetsPrivate")
+  ECSRunTaskClusterStackName: ecs-a
   ECSTaskDefinition:
     - Base:
         NetworkMode: awsvpc
   EventsRule:
     - ECSRunTask:
         IBOX_SOURCE_OBJ: EventsRuleTargetLambda
         Description: 'Periodically invoke LambdaECSRunTask'
@@ -28,28 +39,28 @@
         State: 'ENABLED'
         Targets:
           - Lambda0:
               Arn: ImportValue('LambdaECSRunTaskArn')
               Id: 'TargetFunction-01'
               Input: Join('"', [
                   '{',
-                  'Cluster":', get_expvalue('Cluster', 'ClusterStack'), ',',
-                  'ECSInstancesStackName":', get_endvalue('ClusterStack'), ',',
+                  'Cluster":', get_expvalue('Cluster', 'ECSRunTaskClusterStackName'), ',',
+                  'ECSInstancesStackName":', get_endvalue('ECSRunTaskClusterStackName'), ',',
                   'LaunchType":', get_endvalue('EventsRuleECSRunTaskLaunchType'), ',',
                   If('ECSTaskDefinitionBaseNetworkModeAwsVpc', 'NetworkModeAwsVpc":"awsvpc",', Ref('AWS::NoValue')),
                   'TaskDefinition":', Ref('TaskDefinition'), ',',
-                  'Subnets":', get_expvalue('SubnetsPrivate'), ',',
+                  'Subnets":', ImportValue('SubnetsPrivate'), ',',
                   'SecurityGroups":', Join(' ', cfg.SecurityGroupsImport),
                   '}',
                 ])
   IAMPolicy:
     - LambdaECSRunTaskTrigger:
         PolicyName: Sub('LambdaECSRunTaskTrigger_${AWS::StackName}')
         Roles:
-          - get_expvalue('RoleLambdaECSRunTask')
+          - ImportValue('RoleLambdaECSRunTask')
         PolicyDocument:
           Statement:
             - 1:
                 Action:
                   - 'ecs:RunTask'
                   - 'ecs:StartTask'
                 Effect: Allow
@@ -57,8 +68,8 @@
             - 2:
                 Action:
                   - 'iam:GetRole'
                   - 'iam:PassRole'
                 Effect: Allow
                 Resource: 
                   - GetAtt('RoleTask', 'Arn')
-                  - get_expvalue('RoleECSTaskExecution')
+                  - ImportValue('RoleECSTaskExecution')
```

### Comparing `awsibox-0.8.8/awsibox/cfg.py` & `awsibox-0.8.9/awsibox/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     return family_instances_list
 
 
 INSTANCE_LIST = ["default"] + build_instance_list()
 
 # Order is VERY important do not CHANGE it!
 CFG_TO_FUNC = {
-    "Parameter": {"module": "cloudformation", "func": "CFM_Parameters"},
+    "Parameter": {"module": "joker", "func": (None, "Parameter")},
     "Condition": {"module": "cloudformation", "func": "CFM_Conditions"},
     "Mapping": {"module": "cloudformation", "func": "CFM_Mappings"},
     "ApiGatewayAccount": {"module": "joker", "func": ("apigateway", "Account")},
     "ApiGatewayApiKey": {"module": "joker", "func": ("apigateway", "ApiKey")},
     "ApiGatewayBasePathMapping": {
         "module": "joker",
         "func": ("apigateway", "BasePathMapping"),
@@ -332,14 +332,15 @@
     "CertificateManagerCertificate": {
         "module": "joker",
         "func": ("certificatemanager", "Certificate"),
     },
     "CloudFormationCustomResource": {
         "module": "joker",
         "func": ("cloudformation", "CustomResource"),
+        "dep": ["ECSService"],
     },
     "CloudFrontCachePolicy": {"module": "joker", "func": ("cloudfront", "CachePolicy")},
     "CloudFrontDistribution": {
         "module": "cloudfront",
         "func": "CF_CloudFront",
         "dep": [
             "ElasticLoadBalancingV2Listener",
@@ -424,15 +425,15 @@
     "ECSClusterCapacityProviderAssociations": {
         "module": "joker",
         "func": ("ecs", "ClusterCapacityProviderAssociations"),
     },
     "ECSService": {
         "module": "joker",
         "func": ("ecs", "Service"),
-        "dep": ["SecurityGroups"],
+        "dep": ["SecurityGroups", "ECSTaskDefinition"],
     },
     "ECSTaskDefinition": {"module": "joker", "func": ("ecs", "TaskDefinition")},
     "EFSAccessPoint": {"module": "joker", "func": ("efs", "AccessPoint")},
     "EFSFileSystem": {"module": "joker", "func": ("efs", "FileSystem")},
     "EFSMountTarget": {"module": "joker", "func": ("efs", "MountTarget")},
     "ElastiCacheCacheCluster": {
         "module": "joker",
@@ -604,9 +605,9 @@
     },
     # ReplicateRegions need to be the last one
     "CCRReplicateRegions": {
         "module": "cloudformation",
         "func": "CFM_CustomResourceReplicator",
     },
     # Output need to be last line
-    "Output": {"module": "cloudformation", "func": "CFM_Outputs"},
+    "Output": {"module": "joker", "func": (None, "Output")},
 }
```

### Comparing `awsibox-0.8.8/awsibox/common.py` & `awsibox-0.8.9/awsibox/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,24 @@
     MAX_SECURITY_GROUPS,
     SECURITY_GROUPS_DEFAULT,
 )
 
 
 ### BEGIN TROPOSPHERE OVERRIDE ###
 
+# set Parameter default values
+def my_parameter_init(self, title, **kwargs):
+    super(Parameter, self).__init__(title, **kwargs)
+    if "Type" not in kwargs:
+        self.Type = "String"
+    if "Default" not in kwargs:
+        self.Default = ""
+
+
+Parameter.__init__ = my_parameter_init
 
 # Temporary fix for https://github.com/cloudtools/troposphere/issues/2146
 sso.PermissionSet.props["InlinePolicy"] = (str, False)
 
 # Temporary fix for https://github.com/cloudtools/troposphere/issues/1474
 def my_one_of(class_name, properties, property, conditionals):
     if properties.get(property) not in conditionals and not isinstance(
```

### Comparing `awsibox-0.8.8/awsibox/discover.py` & `awsibox-0.8.9/awsibox/discover.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/generate.py` & `awsibox-0.8.9/awsibox/generate.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ASGSpot.code` & `awsibox-0.8.9/awsibox/lambdas/ASGSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/AtEdgeAddHeaders.code` & `awsibox-0.8.9/awsibox/lambdas/AtEdgeAddHeaders.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/CCRFargateSpot.code` & `awsibox-0.8.9/awsibox/lambdas/CCRFargateSpot.code`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,18 @@
     # Init code goes here
     is_success = True
 except Exception as e:
     helper.init_failure(e)
 
 
 def update_alarms(res, spot):
-    alarm_prefix = "TargetTracking-service/%s-Alarm" % "/".join(
-        res["ServiceArn"].split("/")[1:3]
-    )
-    service_base = res["ServiceBase"]
-    service_spot = res["ServiceSpot"]
-    cluster = res["Cluster"]
+    service_base = res["ServiceBaseArn"].split("/")[2]
+    service_spot = res["ServiceSpotArn"].split("/")[2]
+    cluster = res["ServiceSpotArn"].split("/")[1]
+    alarm_prefix = f"TargetTracking-service/{cluster}/{service_spot}"
 
     skip_props = [
         "AlarmArn",
         "AlarmConfigurationUpdatedTimestamp",
         "StateReason",
         "StateReasonData",
         "StateUpdatedTimestamp",
```

### Comparing `awsibox-0.8.8/awsibox/lambdas/CCRLightHouse.code` & `awsibox-0.8.9/awsibox/lambdas/CCRLightHouse.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/CCRStackReplicator.code` & `awsibox-0.8.9/awsibox/lambdas/CCRStackReplicator.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/CloudWatchAlarmStateChange.code` & `awsibox-0.8.9/awsibox/lambdas/CloudWatchAlarmStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/CloudWatchRepeatedNotify.code` & `awsibox-0.8.9/awsibox/lambdas/CloudWatchRepeatedNotify.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/EC2StartStopTagged.code` & `awsibox-0.8.9/awsibox/lambdas/EC2StartStopTagged.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ECSClusterAutoscale.code` & `awsibox-0.8.9/awsibox/lambdas/ECSClusterAutoscale.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ECSDrainInstance.code` & `awsibox-0.8.9/awsibox/lambdas/ECSDrainInstance.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ECSDrainTasks.code` & `awsibox-0.8.9/awsibox/lambdas/ECSDrainTasks.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ECSEventTaskStateChange.code` & `awsibox-0.8.9/awsibox/lambdas/ECSEventTaskStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ECSEventsSpot.code` & `awsibox-0.8.9/awsibox/lambdas/ECSEventsSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ECSRaiseASGAlarm.code` & `awsibox-0.8.9/awsibox/lambdas/ECSRaiseASGAlarm.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ECSRunTask.code` & `awsibox-0.8.9/awsibox/lambdas/ECSRunTask.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ECSUpdateDesiredCount.code` & `awsibox-0.8.9/awsibox/lambdas/ECSUpdateDesiredCount.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ElasticSearchSnapShot.code` & `awsibox-0.8.9/awsibox/lambdas/ElasticSearchSnapShot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/InfraInfo.code` & `awsibox-0.8.9/awsibox/lambdas/InfraInfo.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ManageService.code` & `awsibox-0.8.9/awsibox/lambdas/ManageService.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/PaidApi.code` & `awsibox-0.8.9/awsibox/lambdas/PaidApi.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/PyPackager.code` & `awsibox-0.8.9/awsibox/lambdas/PyPackager.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/Python37SSM.layer` & `awsibox-0.8.9/awsibox/lambdas/Python37SSM.layer`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/R53RecordInstanceId.code` & `awsibox-0.8.9/awsibox/lambdas/R53RecordInstanceId.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ServiceDiscovery.code` & `awsibox-0.8.9/awsibox/lambdas/ServiceDiscovery.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/ServiceUnavailable.code` & `awsibox-0.8.9/awsibox/lambdas/ServiceUnavailable.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/lambdas/StacksOps.code` & `awsibox-0.8.9/awsibox/lambdas/StacksOps.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/ec2.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/ec2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/iam.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/iam.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/joker.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/joker.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/rds.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/rds.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/s3.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/s3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/__pycache__/waf.cpython-311.pyc` & `awsibox-0.8.9/awsibox/mod/__pycache__/waf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/autoscaling.py` & `awsibox-0.8.9/awsibox/mod/autoscaling.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,20 +21,14 @@
     LaunchTemplateData = ec2.LaunchTemplateData("LaunchTemplateData")
     auto_get_props(
         LaunchTemplateData,
         "LaunchTemplateData",
         res_obj_type="AWS::EC2::LaunchTemplate",
     )
 
-    if getattr(cfg, "IBOX_LAUNCH_TEMPLATE_NO_SG_EXTRA", False):
-        SecurityGroups = []
-    else:
-        SecurityGroups = cfg.SecurityGroupsImport
-    LaunchTemplateData.NetworkInterfaces[0].Groups.extend(SecurityGroups)
-
     R_LaunchTemplate.LaunchTemplateData = LaunchTemplateData
 
     ud_envrole = getattr(cfg, "IBOX_ROLE_EX", getattr(cfg, "envrole"))
     # try to get a complete user-data conf in package or in Ext dir
     user_data = import_user_data(ud_envrole)
 
     if not user_data:
@@ -97,17 +91,15 @@
                 "EC2InstanceUserDataELBClassicCheckLoadBalancerName",
                 Ref(f"LoadBalancerClassic{n}"),
             )
     if cfg.LoadBalancerType in ["Application", "Network"]:
         for n, v in getattr(cfg, "ElasticLoadBalancingV2TargetGroup", {}).items():
             # check for enabled only for EC2 ones
             if n.startswith("EC2") and v.get("IBOX_ENABLED", True):
-                TargetGroups.append(
-                    Ref(f"ElasticLoadBalancingV2TargetGroup{n}")
-                )
+                TargetGroups.append(Ref(f"ElasticLoadBalancingV2TargetGroup{n}"))
                 setattr(
                     cfg,
                     "EC2InstanceUserDataELBV2CheckTargetGroupArn",
                     Ref(f"ElasticLoadBalancingV2TargetGroup{n}"),
                 )
 
     # Resources
```

### Comparing `awsibox-0.8.8/awsibox/mod/cloudformation.py` & `awsibox-0.8.9/awsibox/mod/cloudformation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import troposphere.cloudformation as cfm
 
 from ..common import *
 from ..shared import (
-    Parameter,
     do_no_override,
     get_endvalue,
     get_expvalue,
     # need it even if not directly used cause eval in CFM_Conditions
     get_condition,
     add_obj,
-    auto_build_obj,
 )
 
 
 def mapping_EnvRegion():
     RP = copy.deepcopy(cfg.RP_map)
 
     for env in list(RP):
@@ -80,18 +78,14 @@
             zones[f"Zone{n}"] = "True" if nzones > n else "False"
 
         mappings["AvabilityZones"][r] = zones
 
     return mappings
 
 
-def CFM_Parameters(key):
-    auto_build_obj(Parameter(""), getattr(cfg, key))
-
-
 def CFM_Conditions(key):
     do_no_override(True)
     for n, v in getattr(cfg, key).items():
         c_Condition = {n: eval(v)}
 
         add_obj(c_Condition)
     do_no_override(False)
@@ -107,18 +101,14 @@
             c_Mapping = mapping_AZ()
         else:
             c_Mapping = {n: v}
 
         cfg.Mappings.update(c_Mapping)
 
 
-def CFM_Outputs(key):
-    auto_build_obj(Output(""), getattr(cfg, key))
-
-
 def CFM_CustomResourceReplicator(key):
     resname = "CloudFormationCustomResourceStackReplicator"
     # Parameters
     P_ReplicateRegions = Parameter(
         "CCRReplicateRegions",
         Description="Regions where to replicate - none to disable - empty for default based on env/role",
         Type="CommaDelimitedList",
```

### Comparing `awsibox-0.8.8/awsibox/mod/cloudfront.py` & `awsibox-0.8.9/awsibox/mod/cloudfront.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/mod/ec2.py` & `awsibox-0.8.9/awsibox/mod/ec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import troposphere.ec2 as ec2
 
 from ..common import *
 from ..shared import (
-    Parameter,
     get_endvalue,
     get_expvalue,
     auto_get_props,
     get_condition,
     add_obj,
 )
```

### Comparing `awsibox-0.8.8/awsibox/mod/joker.py` & `awsibox-0.8.9/awsibox/mod/joker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..common import *
-from ..shared import auto_get_props, add_obj, Parameter, get_condition, parse_ibox_key
+from ..shared import auto_get_props, add_obj, get_condition, parse_ibox_key
 from ..RP import RP_to_cfg, merge_dict
 
 
 def Joker(key, module, cls):
     for n, v in getattr(cfg, key).items():
         if not v.get("IBOX_ENABLED", True):
             continue
@@ -22,16 +22,20 @@
         if cfg.debug:
             logging.error(f"Joker processing: {resname}")
 
         # get IBOX_LINKED_OBJ keys
         linked_obj_name = v.get("IBOX_LINKED_OBJ_NAME", "")
         linked_obj_index = v.get("IBOX_LINKED_OBJ_INDEX", "")
 
-        mod = __import__(f"troposphere.{module}")
-        my_module = getattr(mod, module)
+        if module:
+            mod = __import__(f"troposphere.{module}")
+            my_module = getattr(mod, module)
+        else:
+            # for classes in troposphere __init__
+            my_module = __import__("troposphere")
         my_class = getattr(my_module, cls)
 
         obj = my_class(resname)
 
         # use IBOX_SOURCE_OBJ to prepopulate obj
         ibox_source_obj = v.get("IBOX_SOURCE_OBJ", [])
         if isinstance(ibox_source_obj, str):
```

### Comparing `awsibox-0.8.8/awsibox/shared.py` & `awsibox-0.8.9/awsibox/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,40 +21,14 @@
 
 class IBOX_Custom_Obj(AWSProperty):
     props: PropsDictType = {
         "Value": (str, True),
     }
 
 
-class Parameter(Parameter):
-    def __init__(self, title, **kwargs):
-        super().__init__(title, **kwargs)
-        if "Type" not in kwargs:
-            self.Type = "String"
-        if "Default" not in kwargs:
-            self.Default = ""
-
-        # Create SSM Parameter for EnvAppXVersion Params to have history of application versions
-        if title.startswith("EnvApp") and title.endswith("Version"):
-            add_obj(
-                [
-                    # get_condition(title, "not_equals", "", nomap=True),
-                    ssm.Parameter(
-                        f"SSMParameter{title}",
-                        Type="String",
-                        # Condition=title,
-                        Name=Sub(
-                            "/EnvAppVersions/${EnvRole}/${AWS::StackName}/%s" % title
-                        ),
-                        Value=Ref(title),
-                    ),
-                ]
-            )
-
-
 def stack_add_res():
     for n, v in cfg.Parameters.items():
         # Automatically create override conditions for parameters
         if n in list(cfg.fixedvalues) + cfg.mappedvalues:
             if n.endswith("InstanceType"):
                 default = "default"
             elif n == "SecurityGroups":
@@ -68,15 +42,14 @@
                 else {f"{n}Override": Not(Equals(Ref(n), default))}
             )
 
             add_obj(condition)
         # End
         cfg.template.add_parameter(v)
 
-
     for n, v in cfg.Conditions.items():
         cfg.template.add_condition(n, v)
 
     for n, v in cfg.Mappings.items():
         cfg.template.add_mapping(n, v)
 
     for n, v in cfg.Resources.items():
@@ -946,14 +919,16 @@
             return values
 
         def _linked_obj(linked_obj_data):
             # need to parse them here to have the right values
             lo_name = parse_ibox_key(linked_obj_data.get("Name", IBOX_RESNAME))
             lo_key = parse_ibox_key(linked_obj_data.get("Key", ""))
             lo_type = parse_ibox_key(linked_obj_data.get("Type", ""))
+            if not lo_type:
+                return
             # this way even if without key "For", for cycle will run at least one time
             lo_for_cycle = parse_ibox_key(linked_obj_data.get("For", [""]))
 
             louc_cfg = {}
             for lo_for_index in lo_for_cycle:
                 # need to copy it because it's updated
                 lo_conf = copy.deepcopy(
@@ -963,29 +938,27 @@
                 # for all lo_conf entries, if their value is a string parse it using parse_ibox_key
                 for loc_entry_key, loc_entry_value in lo_conf.items():
                     lo_conf[loc_entry_key] = parse_ibox_key(
                         loc_entry_value, conf={"IBOX_LINKED_OBJ_FOR": lo_for_index}
                     )
 
                 linked_obj_key_name = f"{lo_key}{lo_type}{lo_for_index}"
+                if not hasattr(cfg, linked_obj_key_name):
+                    # usefull when using for-cycle to have multiple targets all using the same source obj
+                    linked_obj_key_name = f"{lo_key}{lo_type}"
+
                 target_name = f"{lo_name}{lo_for_index}"
 
                 # get existing object
                 if f"{lo_key}{target_name}" == linked_obj_key_name:
                     # source and target are the same, so update the object in place
                     linked_obj = getattr(cfg, linked_obj_key_name)
                 else:
                     # copy it, first search for the full name including for index
-                    linked_obj = copy.deepcopy(
-                        getattr(
-                            cfg,
-                            linked_obj_key_name,
-                            getattr(cfg, f"{lo_key}{lo_type}", None),
-                        )
-                    )
+                    linked_obj = copy.deepcopy(getattr(cfg, linked_obj_key_name))
 
                 # update it with config from IBOX_LINKED_OBJ Conf
                 linked_obj.update(lo_conf)
 
                 lo_resname = lo_conf.get("IBOX_RESNAME", f"{lo_key}{lo_name}")
                 linked_obj["IBOX_RESNAME"] = f"{lo_resname}{lo_for_index}"
 
@@ -1186,26 +1159,14 @@
         except Exception:
             pass
 
     _populate(obj, key, mapname, rootdict)
     return obj
 
 
-def auto_build_obj(obj, key, name=None):
-    props = vars(obj)["propnames"]
-    classname = obj.__class__
-    for resname, resvalue in key.items():
-        final_obj = classname(resname)
-        if not name:
-            name = final_obj.__class__.__name__
-        auto_get_props(final_obj, f"{name}{resname}")
-
-        add_obj(final_obj)
-
-
 def change_obj_data(obj, find, value):
     if isinstance(obj, list):
         for n, v in enumerate(obj):
             change_obj_data(obj[n], find, value)
     elif isinstance(obj, If):
         obj_if = obj.data["Fn::If"]
         for n, v in enumerate(obj_if):
@@ -1260,15 +1221,16 @@
         return eval(value, globals(), conf)
     for key in IBOX_SPECIAL_KEYS:
         if key in value:
             if key in conf:
                 value = value.replace(key, str(conf[key]))
             else:
                 value = value.replace(key, globals().get(key, ""))
-    value = value.replace("_", IBOX_RESNAME)
+    if "IBOX_RESNAME" in globals():
+        value = value.replace("_", IBOX_RESNAME)
     value = value.replace(".", "")
 
     return value
 
 
 def camel_to_snake(data):
     out = ""
```

### Comparing `awsibox-0.8.8/awsibox/user-data/SCRIPTS/ELBCHECK.sh` & `awsibox-0.8.9/awsibox/user-data/SCRIPTS/ELBCHECK.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/user-data/SCRIPTS/END.sh` & `awsibox-0.8.9/awsibox/user-data/SCRIPTS/END.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/user-data/SCRIPTS/INIT.sh` & `awsibox-0.8.9/awsibox/user-data/SCRIPTS/INIT.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/user-data/SCRIPTS/PACKAGE.sh` & `awsibox-0.8.9/awsibox/user-data/SCRIPTS/PACKAGE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/user-data/SCRIPTS/SERVICE.sh` & `awsibox-0.8.9/awsibox/user-data/SCRIPTS/SERVICE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/user-data/SCRIPTS/SETUP.sh` & `awsibox-0.8.9/awsibox/user-data/SCRIPTS/SETUP.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/awsibox/user-data/ecs-cluster.sh` & `awsibox-0.8.9/awsibox/user-data/ecs-cluster.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/build/lib/awsibox.egg-info/PKG-INFO` & `awsibox-0.8.9/build/lib/awsibox.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.8
+Version: 0.8.9
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
```

### Comparing `awsibox-0.8.8/build/lib/awsibox.egg-info/SOURCES.txt` & `awsibox-0.8.9/build/lib/awsibox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
 awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
 awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
 awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
 awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
 awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
 awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
-awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
 awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
 awsibox/cfg/ibox/com/cloudfront/for-services.yml
 awsibox/cfg/ibox/com/cloudfront/i_base.yml
 awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
 awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
 awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
 awsibox/cfg/ibox/com/ec2/bottlerocket.yml
@@ -88,14 +87,16 @@
 awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
 awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
 awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
 awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
 awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
 awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
 awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+awsibox/cfg/ibox/res/cloudformation/custom-resources.yml
+awsibox/cfg/ibox/res/cloudformation/ibox_base.yml
 awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
 awsibox/cfg/ibox/res/cloudfront/origin-access-controls.yml
 awsibox/cfg/ibox/res/cloudfront/policies.yml
 awsibox/cfg/ibox/res/cloudwatch/alarms.yml
 awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
 awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
 awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
@@ -139,14 +140,16 @@
 awsibox/cfg/ibox/res/s3/bucket-policies.yml
 awsibox/cfg/ibox/res/s3/ibox_base.yml
 awsibox/cfg/ibox/res/scheduler/ibox_base.yml
 awsibox/cfg/ibox/res/sns/ibox_base.yml
 awsibox/cfg/ibox/res/sns/subscriptions.yml
 awsibox/cfg/ibox/res/sqs/ibox_base.yml
 awsibox/cfg/ibox/res/sqs/queue-policies.yml
+awsibox/cfg/ibox/res/ssm/ibox_base.yml
+awsibox/cfg/ibox/res/ssm/parameters.yml
 awsibox/cfg/ibox/stacks/agw/i_type.yml
 awsibox/cfg/ibox/stacks/agw/infra-info.yml
 awsibox/cfg/ibox/stacks/cch/i_type.yml
 awsibox/cfg/ibox/stacks/clf/i_type.yml
 awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
 awsibox/cfg/ibox/stacks/ec2/i_type.yml
 awsibox/cfg/ibox/stacks/ecs/buildkite.yml
```

### Comparing `awsibox-0.8.8/scripts/ibox_generate_templates.py` & `awsibox-0.8.9/scripts/ibox_generate_templates.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/setup.cfg` & `awsibox-0.8.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.8/setup.py` & `awsibox-0.8.9/setup.py`

 * *Files identical despite different names*

