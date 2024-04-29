# Comparing `tmp/troposphere-4.7.0.tar.gz` & `tmp/troposphere-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troposphere-4.7.0.tar", last modified: Sun Mar 10 20:55:59 2024, max compression
+gzip compressed data, was "troposphere-4.8.0.tar", last modified: Mon Apr 29 19:32:15 2024, max compression
```

## Comparing `troposphere-4.7.0.tar` & `troposphere-4.8.0.tar`

### file list

```diff
@@ -1,495 +1,503 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.979699 troposphere-4.7.0/
--rw-r--r--   0 mark       (501) staff       (20)      563 2022-06-17 14:59:33.000000 troposphere-4.7.0/.gitignore
--rw-r--r--   0 mark       (501) staff       (20)     1319 2017-04-14 00:59:43.000000 troposphere-4.7.0/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)      111 2019-05-06 00:16:28.000000 troposphere-4.7.0/MANIFEST.in
--rw-r--r--   0 mark       (501) staff       (20)     9160 2024-03-10 20:55:59.979340 troposphere-4.7.0/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     7929 2022-06-17 14:59:33.000000 troposphere-4.7.0/README.rst
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.773949 troposphere-4.7.0/examples/
--rw-r--r--   0 mark       (501) staff       (20)     5175 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/ApiGateway.py
--rw-r--r--   0 mark       (501) staff       (20)     1061 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/ApplicationAutoScalingSample.py
--rw-r--r--   0 mark       (501) staff       (20)     7076 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/ApplicationELB.py
--rw-r--r--   0 mark       (501) staff       (20)     5440 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/ApplicationLB_FixedActions.py
--rw-r--r--   0 mark       (501) staff       (20)     4339 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/AuroraServerlessRDS_SecretsManager.py
--rw-r--r--   0 mark       (501) staff       (20)     8535 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/Autoscaling.py
--rw-r--r--   0 mark       (501) staff       (20)     9383 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/AutoscalingHTTPRequests.py
--rw-r--r--   0 mark       (501) staff       (20)     2883 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/Backup.py
--rw-r--r--   0 mark       (501) staff       (20)     3607 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Batch.py
--rw-r--r--   0 mark       (501) staff       (20)    11829 2022-08-08 22:11:46.000000 troposphere-4.7.0/examples/BatchEventSnsLambda.py
--rw-r--r--   0 mark       (501) staff       (20)      508 2021-03-27 21:38:06.000000 troposphere-4.7.0/examples/CertificateManagerSample.py
--rw-r--r--   0 mark       (501) staff       (20)      549 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/ClassExtensions.py
--rw-r--r--   0 mark       (501) staff       (20)     3000 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/CloudFormation_Init_ConfigSet.py
--rw-r--r--   0 mark       (501) staff       (20)     1833 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/CloudFront_Distribution_S3.py
--rw-r--r--   0 mark       (501) staff       (20)     1558 2022-01-05 01:20:25.000000 troposphere-4.7.0/examples/CloudFront_StreamingDistribution_S3.py
--rw-r--r--   0 mark       (501) staff       (20)     2915 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/CloudTrail.py
--rw-r--r--   0 mark       (501) staff       (20)     1477 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/CloudWatchEventsSample.py
--rw-r--r--   0 mark       (501) staff       (20)      773 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/CodeBuild.py
--rw-r--r--   0 mark       (501) staff       (20)     2503 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/CodeDeploy.py
--rw-r--r--   0 mark       (501) staff       (20)     3626 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/CodePipeline.py
--rw-r--r--   0 mark       (501) staff       (20)      990 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/CustomResource.py
--rw-r--r--   0 mark       (501) staff       (20)     1544 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Dlm.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2298 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/DynamoDB_Table.py
--rw-r--r--   0 mark       (501) staff       (20)     5293 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/DynamoDB_Table_With_GSI_And_NonKeyAttributes_Projection.py
--rw-r--r--   0 mark       (501) staff       (20)     5031 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/DynamoDB_Table_With_GlobalSecondaryIndex.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2701 2021-04-24 21:53:41.000000 troposphere-4.7.0/examples/DynamoDB_Table_With_KinesisStreamSpecification.py
--rw-r--r--   0 mark       (501) staff       (20)     6897 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/DynamoDB_Tables_OnDemand.py
--rw-r--r--   0 mark       (501) staff       (20)     2064 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/EC2Conditions.py
--rw-r--r--   0 mark       (501) staff       (20)     2299 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/EC2InstanceSample.py
--rw-r--r--   0 mark       (501) staff       (20)     2710 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/EC2_Remove_Ephemeral_Drive.py
--rw-r--r--   0 mark       (501) staff       (20)     1253 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/ECRSample.py
--rw-r--r--   0 mark       (501) staff       (20)     8934 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/ECSCluster.py
--rw-r--r--   0 mark       (501) staff       (20)     1272 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/ECSFargate.py
--rw-r--r--   0 mark       (501) staff       (20)     4271 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/EFS.py
--rw-r--r--   0 mark       (501) staff       (20)     4835 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/ELBSample.py
--rw-r--r--   0 mark       (501) staff       (20)     8958 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/EMR_Cluster.py
--rwxr-xr-x   0 mark       (501) staff       (20)    25606 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/ElastiCacheRedis.py
--rw-r--r--   0 mark       (501) staff       (20)     5587 2021-07-04 20:54:52.000000 troposphere-4.7.0/examples/ElasticBeanstalk_Nodejs_Sample.py
--rw-r--r--   0 mark       (501) staff       (20)     1596 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/ElasticsearchDomain.py
--rw-r--r--   0 mark       (501) staff       (20)     2134 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Firehose_with_Redshift.py
--rw-r--r--   0 mark       (501) staff       (20)     1413 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/IAM_Policies_SNS_Publish_To_SQS.py
--rw-r--r--   0 mark       (501) staff       (20)      838 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/IAM_Roles_and_InstanceProfiles.py
--rw-r--r--   0 mark       (501) staff       (20)     1919 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/IAM_Users_Groups_and_Policies.py
--rw-r--r--   0 mark       (501) staff       (20)     1943 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/IAM_Users_snippet.py
--rw-r--r--   0 mark       (501) staff       (20)     2670 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/IoTAnalytics.py
--rw-r--r--   0 mark       (501) staff       (20)     1852 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/IoTSample.py
--rw-r--r--   0 mark       (501) staff       (20)      441 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/Kinesis_Stream.py
--rw-r--r--   0 mark       (501) staff       (20)     5327 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/Lambda.py
--rw-r--r--   0 mark       (501) staff       (20)      829 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/Mediapackage.py
--rw-r--r--   0 mark       (501) staff       (20)      317 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/Metadata.py
--rw-r--r--   0 mark       (501) staff       (20)     1564 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/MskCluster.py
--rw-r--r--   0 mark       (501) staff       (20)     3181 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/NatGateway.py
--rw-r--r--   0 mark       (501) staff       (20)     5651 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/NetworkLB.py
--rw-r--r--   0 mark       (501) staff       (20)     4834 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/OpenStack_AutoScaling.py
--rw-r--r--   0 mark       (501) staff       (20)     1962 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/OpenStack_Server.py
--rw-r--r--   0 mark       (501) staff       (20)     5280 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/OpsWorksSnippet.py
--rw-r--r--   0 mark       (501) staff       (20)     1407 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/RDS_Snapshot_On_Delete.py
--rw-r--r--   0 mark       (501) staff       (20)     5097 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/RDS_VPC.py
--rw-r--r--   0 mark       (501) staff       (20)     1989 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/RDS_with_DBParameterGroup.py
--rw-r--r--   0 mark       (501) staff       (20)     3514 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Redshift.py
--rw-r--r--   0 mark       (501) staff       (20)     4876 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/RedshiftClusterInVpc.py
--rwxr-xr-x   0 mark       (501) staff       (20)     1722 2022-11-26 19:34:19.000000 troposphere-4.7.0/examples/RedshiftServerless.py
--rw-r--r--   0 mark       (501) staff       (20)     1962 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/Route53_A.py
--rw-r--r--   0 mark       (501) staff       (20)     1329 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/Route53_CNAME.py
--rw-r--r--   0 mark       (501) staff       (20)     2491 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/Route53_RoundRobin.py
--rw-r--r--   0 mark       (501) staff       (20)      815 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/S3_Bucket.py
--rw-r--r--   0 mark       (501) staff       (20)     1081 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/S3_Bucket_With_AccelerateConfiguration.py
--rw-r--r--   0 mark       (501) staff       (20)     2580 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/S3_Bucket_With_Versioning_And_Lifecycle_Rules.py
--rw-r--r--   0 mark       (501) staff       (20)     1420 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/S3_Website_Bucket_With_Retain_On_Delete.py
--rw-r--r--   0 mark       (501) staff       (20)     1530 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/SQSDLQ.py
--rw-r--r--   0 mark       (501) staff       (20)     1021 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/SQSEncrypt.py
--rw-r--r--   0 mark       (501) staff       (20)     2312 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/SQS_With_CloudWatch_Alarms.py
--rw-r--r--   0 mark       (501) staff       (20)     2559 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/SSMExample.py
--rw-r--r--   0 mark       (501) staff       (20)      550 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Secretsmanager.py
--rw-r--r--   0 mark       (501) staff       (20)     1441 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Secretsmanager_Rds.py
--rw-r--r--   0 mark       (501) staff       (20)     1946 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Serverless_Api_Backend.py
--rw-r--r--   0 mark       (501) staff       (20)      814 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Serverless_Deployment_Preference.py
--rw-r--r--   0 mark       (501) staff       (20)      969 2022-03-02 00:34:16.000000 troposphere-4.7.0/examples/Serverless_S3_Processor.py
--rw-r--r--   0 mark       (501) staff       (20)     5077 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/VPC_EC2_Instance_With_Multiple_Dynamic_IPAddresses.py
--rw-r--r--   0 mark       (501) staff       (20)     6446 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/VPC_With_VPN_Connection.py
--rw-r--r--   0 mark       (501) staff       (20)    15713 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/VPC_single_instance_in_subnet.py
--rw-r--r--   0 mark       (501) staff       (20)     1054 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/VpnEndpoint.py
--rw-r--r--   0 mark       (501) staff       (20)     5454 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/WAF_Common_Attacks_Sample.py
--rw-r--r--   0 mark       (501) staff       (20)     5462 2022-06-17 14:59:33.000000 troposphere-4.7.0/examples/WAF_Regional_Common_Attacks_Sample.py
--rw-r--r--   0 mark       (501) staff       (20)     1511 2021-03-27 21:20:49.000000 troposphere-4.7.0/examples/WaitObject.py
--rw-r--r--   0 mark       (501) staff       (20)      565 2023-12-21 21:43:55.000000 troposphere-4.7.0/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)      115 2019-05-06 00:16:28.000000 troposphere-4.7.0/requirements.txt
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.774929 troposphere-4.7.0/scripts/
--rwxr-xr-x   0 mark       (501) staff       (20)     6100 2022-07-22 22:21:38.000000 troposphere-4.7.0/scripts/cfn
--rwxr-xr-x   0 mark       (501) staff       (20)    12048 2022-06-17 14:59:33.000000 troposphere-4.7.0/scripts/cfn2py
--rw-r--r--   0 mark       (501) staff       (20)     1569 2024-03-10 20:55:59.980697 troposphere-4.7.0/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)       38 2021-03-27 20:52:28.000000 troposphere-4.7.0/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.804416 troposphere-4.7.0/tests/
--rw-r--r--   0 mark       (501) staff       (20)     1945 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_apigateway.py
--rw-r--r--   0 mark       (501) staff       (20)     2724 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_apigatewayv2.py
--rw-r--r--   0 mark       (501) staff       (20)     1680 2023-02-24 15:58:15.000000 troposphere-4.7.0/tests/test_appconfig.py
--rw-r--r--   0 mark       (501) staff       (20)     1609 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_appsync.py
--rw-r--r--   0 mark       (501) staff       (20)     4598 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_asg.py
--rw-r--r--   0 mark       (501) staff       (20)     8412 2023-02-27 00:23:50.000000 troposphere-4.7.0/tests/test_awslambda.py
--rw-r--r--   0 mark       (501) staff       (20)    20416 2023-11-10 16:04:26.000000 troposphere-4.7.0/tests/test_basic.py
--rw-r--r--   0 mark       (501) staff       (20)     1072 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_cloudformation.py
--rw-r--r--   0 mark       (501) staff       (20)      886 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_cloudfront.py
--rw-r--r--   0 mark       (501) staff       (20)     1665 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_cloudwatch.py
--rw-r--r--   0 mark       (501) staff       (20)     4112 2023-02-24 15:58:15.000000 troposphere-4.7.0/tests/test_codebuild.py
--rw-r--r--   0 mark       (501) staff       (20)     1231 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_codecommit.py
--rw-r--r--   0 mark       (501) staff       (20)      642 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_config.py
--rw-r--r--   0 mark       (501) staff       (20)     2613 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_dict.py
--rw-r--r--   0 mark       (501) staff       (20)      585 2023-02-24 15:58:15.000000 troposphere-4.7.0/tests/test_dlm.py
--rw-r--r--   0 mark       (501) staff       (20)     4714 2023-08-13 20:05:24.000000 troposphere-4.7.0/tests/test_ec2.py
--rw-r--r--   0 mark       (501) staff       (20)      308 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_ecr.py
--rw-r--r--   0 mark       (501) staff       (20)     8500 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_ecs.py
--rw-r--r--   0 mark       (501) staff       (20)     1988 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_efs.py
--rw-r--r--   0 mark       (501) staff       (20)     1803 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_eks.py
--rw-r--r--   0 mark       (501) staff       (20)     4712 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_elasticloadbalancerv2.py
--rw-r--r--   0 mark       (501) staff       (20)    11735 2023-02-24 16:29:02.000000 troposphere-4.7.0/tests/test_emr.py
--rw-r--r--   0 mark       (501) staff       (20)     1549 2022-01-17 22:13:33.000000 troposphere-4.7.0/tests/test_examples.py
--rw-r--r--   0 mark       (501) staff       (20)     1773 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_examples_template_generator.py
--rwxr-xr-x   0 mark       (501) staff       (20)     1264 2023-10-25 14:19:18.000000 troposphere-4.7.0/tests/test_findinmap.py
--rw-r--r--   0 mark       (501) staff       (20)      616 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_fsx.py
--rw-r--r--   0 mark       (501) staff       (20)     1576 2023-12-06 22:15:23.000000 troposphere-4.7.0/tests/test_guardduty.py
--rw-r--r--   0 mark       (501) staff       (20)     1876 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_int_type.py
--rw-r--r--   0 mark       (501) staff       (20)      846 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_iot1click.py
--rw-r--r--   0 mark       (501) staff       (20)      622 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_iottwinmaker.py
--rw-r--r--   0 mark       (501) staff       (20)     2131 2022-10-24 14:32:59.000000 troposphere-4.7.0/tests/test_language_extensions.py
--rw-r--r--   0 mark       (501) staff       (20)     2530 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_logs.py
--rw-r--r--   0 mark       (501) staff       (20)      843 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_mappings.py
--rw-r--r--   0 mark       (501) staff       (20)      612 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_networkfirewall.py
--rw-r--r--   0 mark       (501) staff       (20)      809 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_opensearchservice.py
--rw-r--r--   0 mark       (501) staff       (20)     1671 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_opsworks.py
--rw-r--r--   0 mark       (501) staff       (20)     1323 2023-10-25 14:19:18.000000 troposphere-4.7.0/tests/test_parameters.py
--rw-r--r--   0 mark       (501) staff       (20)     5150 2022-06-17 14:59:34.000000 troposphere-4.7.0/tests/test_policies.py
--rw-r--r--   0 mark       (501) staff       (20)    14858 2024-02-14 23:42:50.000000 troposphere-4.7.0/tests/test_rds.py
--rw-r--r--   0 mark       (501) staff       (20)     1336 2022-06-17 14:59:35.000000 troposphere-4.7.0/tests/test_resiliencehub.py
--rw-r--r--   0 mark       (501) staff       (20)      409 2022-06-17 14:59:35.000000 troposphere-4.7.0/tests/test_route53.py
--rw-r--r--   0 mark       (501) staff       (20)     2130 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_s3.py
--rw-r--r--   0 mark       (501) staff       (20)      775 2023-01-28 23:24:40.000000 troposphere-4.7.0/tests/test_scheduler.py
--rw-r--r--   0 mark       (501) staff       (20)    15112 2023-08-13 20:05:24.000000 troposphere-4.7.0/tests/test_serverless.py
--rw-r--r--   0 mark       (501) staff       (20)      782 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_sqs.py
--rw-r--r--   0 mark       (501) staff       (20)      527 2022-07-22 22:21:38.000000 troposphere-4.7.0/tests/test_ssm.py
--rw-r--r--   0 mark       (501) staff       (20)      828 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_stepfunctions.py
--rw-r--r--   0 mark       (501) staff       (20)     2653 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_tags.py
--rw-r--r--   0 mark       (501) staff       (20)     6943 2023-10-26 21:02:29.000000 troposphere-4.7.0/tests/test_template.py
--rw-r--r--   0 mark       (501) staff       (20)     4214 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_template_generator.py
--rw-r--r--   0 mark       (501) staff       (20)     1795 2021-03-27 21:20:49.000000 troposphere-4.7.0/tests/test_userdata.py
--rw-r--r--   0 mark       (501) staff       (20)     9703 2022-06-17 14:59:35.000000 troposphere-4.7.0/tests/test_validators.py
--rw-r--r--   0 mark       (501) staff       (20)     4353 2022-06-17 14:59:35.000000 troposphere-4.7.0/tests/test_wafv2.py
--rw-r--r--   0 mark       (501) staff       (20)     2044 2022-06-17 14:59:35.000000 troposphere-4.7.0/tests/test_yaml.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.933699 troposphere-4.7.0/troposphere/
--rw-r--r--   0 mark       (501) staff       (20)    37341 2024-03-10 20:51:26.000000 troposphere-4.7.0/troposphere/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     2053 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/accessanalyzer.py
--rw-r--r--   0 mark       (501) staff       (20)    10858 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/acmpca.py
--rw-r--r--   0 mark       (501) staff       (20)     4704 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/amazonmq.py
--rw-r--r--   0 mark       (501) staff       (20)     5587 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/amplify.py
--rw-r--r--   0 mark       (501) staff       (20)     8774 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/analytics.py
--rw-r--r--   0 mark       (501) staff       (20)    17726 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/apigateway.py
--rw-r--r--   0 mark       (501) staff       (20)    13938 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/apigatewayv2.py
--rw-r--r--   0 mark       (501) staff       (20)     5482 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/appconfig.py
--rw-r--r--   0 mark       (501) staff       (20)    42057 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/appflow.py
--rw-r--r--   0 mark       (501) staff       (20)     2252 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/appintegrations.py
--rw-r--r--   0 mark       (501) staff       (20)     7355 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/applicationautoscaling.py
--rw-r--r--   0 mark       (501) staff       (20)     6982 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/applicationinsights.py
--rw-r--r--   0 mark       (501) staff       (20)    46906 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/appmesh.py
--rw-r--r--   0 mark       (501) staff       (20)     9596 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/apprunner.py
--rw-r--r--   0 mark       (501) staff       (20)    12585 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/appstream.py
--rw-r--r--   0 mark       (501) staff       (20)    15117 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/appsync.py
--rw-r--r--   0 mark       (501) staff       (20)     1359 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/aps.py
--rw-r--r--   0 mark       (501) staff       (20)     1517 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/arczonalshift.py
--rw-r--r--   0 mark       (501) staff       (20)     1610 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ask.py
--rw-r--r--   0 mark       (501) staff       (20)     5770 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/athena.py
--rw-r--r--   0 mark       (501) staff       (20)     3045 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/auditmanager.py
--rw-r--r--   0 mark       (501) staff       (20)    24067 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/autoscaling.py
--rw-r--r--   0 mark       (501) staff       (20)     5587 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/autoscalingplans.py
--rw-r--r--   0 mark       (501) staff       (20)    17344 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/awslambda.py
--rw-r--r--   0 mark       (501) staff       (20)     3544 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/b2bi.py
--rw-r--r--   0 mark       (501) staff       (20)    11634 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/backup.py
--rw-r--r--   0 mark       (501) staff       (20)      711 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/backupgateway.py
--rw-r--r--   0 mark       (501) staff       (20)    22321 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/batch.py
--rw-r--r--   0 mark       (501) staff       (20)     5549 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/billingconductor.py
--rw-r--r--   0 mark       (501) staff       (20)     6713 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/budgets.py
--rw-r--r--   0 mark       (501) staff       (20)     5681 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cassandra.py
--rw-r--r--   0 mark       (501) staff       (20)     2311 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ce.py
--rw-r--r--   0 mark       (501) staff       (20)     2028 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/certificatemanager.py
--rw-r--r--   0 mark       (501) staff       (20)     1653 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/chatbot.py
--rw-r--r--   0 mark       (501) staff       (20)    11185 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cleanrooms.py
--rw-r--r--   0 mark       (501) staff       (20)     1200 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cloud9.py
--rw-r--r--   0 mark       (501) staff       (20)    10879 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cloudformation.py
--rw-r--r--   0 mark       (501) staff       (20)    37095 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cloudfront.py
--rw-r--r--   0 mark       (501) staff       (20)     4985 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cloudtrail.py
--rw-r--r--   0 mark       (501) staff       (20)     8353 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cloudwatch.py
--rw-r--r--   0 mark       (501) staff       (20)     1258 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codeartifact.py
--rw-r--r--   0 mark       (501) staff       (20)    12123 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codebuild.py
--rw-r--r--   0 mark       (501) staff       (20)     1772 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codecommit.py
--rw-r--r--   0 mark       (501) staff       (20)    13982 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codedeploy.py
--rw-r--r--   0 mark       (501) staff       (20)     1336 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codeguruprofiler.py
--rw-r--r--   0 mark       (501) staff       (20)      725 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codegurureviewer.py
--rw-r--r--   0 mark       (501) staff       (20)    10552 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codepipeline.py
--rw-r--r--   0 mark       (501) staff       (20)     1389 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codestar.py
--rw-r--r--   0 mark       (501) staff       (20)     1724 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codestarconnections.py
--rw-r--r--   0 mark       (501) staff       (20)     1173 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/codestarnotifications.py
--rw-r--r--   0 mark       (501) staff       (20)    25006 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cognito.py
--rw-r--r--   0 mark       (501) staff       (20)      803 2023-08-13 20:05:24.000000 troposphere-4.7.0/troposphere/compat.py
--rw-r--r--   0 mark       (501) staff       (20)     5786 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/comprehend.py
--rw-r--r--   0 mark       (501) staff       (20)    15661 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/config.py
--rw-r--r--   0 mark       (501) staff       (20)    24075 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/connect.py
--rw-r--r--   0 mark       (501) staff       (20)     2980 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/connectcampaigns.py
--rw-r--r--   0 mark       (501) staff       (20)    43847 2023-10-26 21:12:57.000000 troposphere-4.7.0/troposphere/constants.py
--rw-r--r--   0 mark       (501) staff       (20)     2132 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/controltower.py
--rw-r--r--   0 mark       (501) staff       (20)      973 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/cur.py
--rw-r--r--   0 mark       (501) staff       (20)    16498 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/customerprofiles.py
--rw-r--r--   0 mark       (501) staff       (20)    22007 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/databrew.py
--rw-r--r--   0 mark       (501) staff       (20)     2692 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/datapipeline.py
--rw-r--r--   0 mark       (501) staff       (20)    15902 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/datasync.py
--rw-r--r--   0 mark       (501) staff       (20)    10006 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/datazone.py
--rw-r--r--   0 mark       (501) staff       (20)     2113 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/dax.py
--rw-r--r--   0 mark       (501) staff       (20)     1354 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/detective.py
--rw-r--r--   0 mark       (501) staff       (20)     3286 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/devopsguru.py
--rw-r--r--   0 mark       (501) staff       (20)     1626 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/directoryservice.py
--rw-r--r--   0 mark       (501) staff       (20)    10001 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/dlm.py
--rw-r--r--   0 mark       (501) staff       (20)    24459 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/dms.py
--rw-r--r--   0 mark       (501) staff       (20)     3666 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/docdb.py
--rw-r--r--   0 mark       (501) staff       (20)      930 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/docdbelastic.py
--rw-r--r--   0 mark       (501) staff       (20)    12563 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/dynamodb.py
--rw-r--r--   0 mark       (501) staff       (20)   107097 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ec2.py
--rw-r--r--   0 mark       (501) staff       (20)     5266 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ecr.py
--rw-r--r--   0 mark       (501) staff       (20)    28821 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ecs.py
--rw-r--r--   0 mark       (501) staff       (20)     4954 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/efs.py
--rw-r--r--   0 mark       (501) staff       (20)    11430 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/eks.py
--rw-r--r--   0 mark       (501) staff       (20)    13035 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/elasticache.py
--rw-r--r--   0 mark       (501) staff       (20)     5696 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/elasticbeanstalk.py
--rw-r--r--   0 mark       (501) staff       (20)     4393 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/elasticloadbalancing.py
--rw-r--r--   0 mark       (501) staff       (20)    16923 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/elasticloadbalancingv2.py
--rw-r--r--   0 mark       (501) staff       (20)     6672 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/elasticsearch.py
--rw-r--r--   0 mark       (501) staff       (20)    19238 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/emr.py
--rw-r--r--   0 mark       (501) staff       (20)     1495 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/emrcontainers.py
--rw-r--r--   0 mark       (501) staff       (20)     6774 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/emrserverless.py
--rw-r--r--   0 mark       (501) staff       (20)     6337 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/entityresolution.py
--rw-r--r--   0 mark       (501) staff       (20)    16239 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/events.py
--rw-r--r--   0 mark       (501) staff       (20)     1842 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/eventschemas.py
--rw-r--r--   0 mark       (501) staff       (20)     8771 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/evidently.py
--rw-r--r--   0 mark       (501) staff       (20)     1963 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/finspace.py
--rw-r--r--   0 mark       (501) staff       (20)    25627 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/firehose.py
--rw-r--r--   0 mark       (501) staff       (20)     4491 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/fis.py
--rw-r--r--   0 mark       (501) staff       (20)     3508 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/fms.py
--rw-r--r--   0 mark       (501) staff       (20)     2279 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/forecast.py
--rw-r--r--   0 mark       (501) staff       (20)     6791 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/frauddetector.py
--rw-r--r--   0 mark       (501) staff       (20)    15293 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/fsx.py
--rw-r--r--   0 mark       (501) staff       (20)    13795 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/gamelift.py
--rw-r--r--   0 mark       (501) staff       (20)     3208 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/globalaccelerator.py
--rw-r--r--   0 mark       (501) staff       (20)    32645 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/glue.py
--rw-r--r--   0 mark       (501) staff       (20)     3374 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/grafana.py
--rw-r--r--   0 mark       (501) staff       (20)    18307 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/greengrass.py
--rw-r--r--   0 mark       (501) staff       (20)    10421 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/greengrassv2.py
--rw-r--r--   0 mark       (501) staff       (20)    10694 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/groundstation.py
--rw-r--r--   0 mark       (501) staff       (20)     7073 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/guardduty.py
--rw-r--r--   0 mark       (501) staff       (20)      575 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/healthimaging.py
--rw-r--r--   0 mark       (501) staff       (20)     2499 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/healthlake.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.937496 troposphere-4.7.0/troposphere/helpers/
--rw-r--r--   0 mark       (501) staff       (20)        0 2017-01-20 05:47:11.000000 troposphere-4.7.0/troposphere/helpers/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     1382 2021-06-13 00:15:44.000000 troposphere-4.7.0/troposphere/helpers/userdata.py
--rw-r--r--   0 mark       (501) staff       (20)     7747 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iam.py
--rw-r--r--   0 mark       (501) staff       (20)     1227 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/identitystore.py
--rw-r--r--   0 mark       (501) staff       (20)    20496 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/imagebuilder.py
--rw-r--r--   0 mark       (501) staff       (20)     1446 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/inspector.py
--rw-r--r--   0 mark       (501) staff       (20)     6843 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/inspectorv2.py
--rw-r--r--   0 mark       (501) staff       (20)     2566 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/internetmonitor.py
--rw-r--r--   0 mark       (501) staff       (20)    44436 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iot.py
--rw-r--r--   0 mark       (501) staff       (20)     2101 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iot1click.py
--rw-r--r--   0 mark       (501) staff       (20)    18061 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iotanalytics.py
--rw-r--r--   0 mark       (501) staff       (20)     1511 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iotcoredeviceadvisor.py
--rw-r--r--   0 mark       (501) staff       (20)    13364 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iotevents.py
--rw-r--r--   0 mark       (501) staff       (20)      631 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iotfleethub.py
--rw-r--r--   0 mark       (501) staff       (20)    11514 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iotfleetwise.py
--rw-r--r--   0 mark       (501) staff       (20)    12508 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iotsitewise.py
--rw-r--r--   0 mark       (501) staff       (20)      946 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iotthingsgraph.py
--rw-r--r--   0 mark       (501) staff       (20)     9082 2024-03-08 22:53:50.000000 troposphere-4.7.0/troposphere/iottwinmaker.py
--rw-r--r--   0 mark       (501) staff       (20)    15493 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/iotwireless.py
--rw-r--r--   0 mark       (501) staff       (20)     3765 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ivs.py
--rw-r--r--   0 mark       (501) staff       (20)     2968 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ivschat.py
--rw-r--r--   0 mark       (501) staff       (20)     6902 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/kafkaconnect.py
--rw-r--r--   0 mark       (501) staff       (20)    29289 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/kendra.py
--rw-r--r--   0 mark       (501) staff       (20)     1020 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/kendraranking.py
--rw-r--r--   0 mark       (501) staff       (20)     1771 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/kinesis.py
--rw-r--r--   0 mark       (501) staff       (20)    19659 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/kinesisanalyticsv2.py
--rw-r--r--   0 mark       (501) staff       (20)     1133 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/kinesisvideo.py
--rw-r--r--   0 mark       (501) staff       (20)     1865 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/kms.py
--rw-r--r--   0 mark       (501) staff       (20)    10866 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/lakeformation.py
--rw-r--r--   0 mark       (501) staff       (20)    34001 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/lex.py
--rw-r--r--   0 mark       (501) staff       (20)     3834 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/licensemanager.py
--rw-r--r--   0 mark       (501) staff       (20)    16575 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/lightsail.py
--rw-r--r--   0 mark       (501) staff       (20)     4462 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/location.py
--rw-r--r--   0 mark       (501) staff       (20)     6224 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/logs.py
--rw-r--r--   0 mark       (501) staff       (20)     2834 2024-03-08 22:53:50.000000 troposphere-4.7.0/troposphere/lookoutequipment.py
--rw-r--r--   0 mark       (501) staff       (20)     7958 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/lookoutmetrics.py
--rw-r--r--   0 mark       (501) staff       (20)      498 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/lookoutvision.py
--rw-r--r--   0 mark       (501) staff       (20)     3121 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/m2.py
--rw-r--r--   0 mark       (501) staff       (20)     3472 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/macie.py
--rw-r--r--   0 mark       (501) staff       (20)     4756 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/managedblockchain.py
--rw-r--r--   0 mark       (501) staff       (20)    11226 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/mediaconnect.py
--rw-r--r--   0 mark       (501) staff       (20)     2375 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/mediaconvert.py
--rw-r--r--   0 mark       (501) staff       (20)    81298 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/medialive.py
--rw-r--r--   0 mark       (501) staff       (20)    15907 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/mediapackage.py
--rw-r--r--   0 mark       (501) staff       (20)     7207 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/mediapackagev2.py
--rw-r--r--   0 mark       (501) staff       (20)     1963 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/mediastore.py
--rw-r--r--   0 mark       (501) staff       (20)    10750 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/mediatailor.py
--rw-r--r--   0 mark       (501) staff       (20)     3659 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/memorydb.py
--rw-r--r--   0 mark       (501) staff       (20)    15935 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/msk.py
--rw-r--r--   0 mark       (501) staff       (20)     2793 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/mwaa.py
--rw-r--r--   0 mark       (501) staff       (20)     4431 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/neptune.py
--rw-r--r--   0 mark       (501) staff       (20)     1600 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/neptunegraph.py
--rw-r--r--   0 mark       (501) staff       (20)    16133 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/networkfirewall.py
--rw-r--r--   0 mark       (501) staff       (20)    10773 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/networkmanager.py
--rw-r--r--   0 mark       (501) staff       (20)     8804 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/nimblestudio.py
--rw-r--r--   0 mark       (501) staff       (20)      891 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/oam.py
--rw-r--r--   0 mark       (501) staff       (20)     4565 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/omics.py
--rw-r--r--   0 mark       (501) staff       (20)     3233 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/opensearchserverless.py
--rw-r--r--   0 mark       (501) staff       (20)     9376 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/opensearchservice.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.939679 troposphere-4.7.0/troposphere/openstack/
--rw-r--r--   0 mark       (501) staff       (20)       91 2021-03-27 15:02:50.000000 troposphere-4.7.0/troposphere/openstack/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     1798 2021-03-27 21:04:46.000000 troposphere-4.7.0/troposphere/openstack/heat.py
--rw-r--r--   0 mark       (501) staff       (20)     8723 2023-08-13 20:37:09.000000 troposphere-4.7.0/troposphere/openstack/neutron.py
--rw-r--r--   0 mark       (501) staff       (20)     5593 2022-06-17 14:59:35.000000 troposphere-4.7.0/troposphere/openstack/nova.py
--rw-r--r--   0 mark       (501) staff       (20)    12555 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/opsworks.py
--rw-r--r--   0 mark       (501) staff       (20)     1713 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/opsworkscm.py
--rw-r--r--   0 mark       (501) staff       (20)     2193 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/organizations.py
--rw-r--r--   0 mark       (501) staff       (20)     2754 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/osis.py
--rw-r--r--   0 mark       (501) staff       (20)     2826 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/panorama.py
--rw-r--r--   0 mark       (501) staff       (20)    16599 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/pcaconnectorad.py
--rw-r--r--   0 mark       (501) staff       (20)     6121 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/personalize.py
--rw-r--r--   0 mark       (501) staff       (20)    26131 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/pinpoint.py
--rw-r--r--   0 mark       (501) staff       (20)     5976 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/pinpointemail.py
--rw-r--r--   0 mark       (501) staff       (20)    23116 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/pipes.py
--rw-r--r--   0 mark       (501) staff       (20)     2038 2022-06-17 14:59:35.000000 troposphere-4.7.0/troposphere/policies.py
--rw-r--r--   0 mark       (501) staff       (20)     1804 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/proton.py
--rw-r--r--   0 mark       (501) staff       (20)     1505 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/qldb.py
--rw-r--r--   0 mark       (501) staff       (20)   260523 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/quicksight.py
--rw-r--r--   0 mark       (501) staff       (20)     1152 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ram.py
--rw-r--r--   0 mark       (501) staff       (20)    19205 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/rds.py
--rw-r--r--   0 mark       (501) staff       (20)    10165 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/redshift.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4946 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/redshiftserverless.py
--rw-r--r--   0 mark       (501) staff       (20)     3966 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/refactorspaces.py
--rw-r--r--   0 mark       (501) staff       (20)     4387 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/rekognition.py
--rw-r--r--   0 mark       (501) staff       (20)     3435 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/resiliencehub.py
--rw-r--r--   0 mark       (501) staff       (20)     1863 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/resourceexplorer2.py
--rw-r--r--   0 mark       (501) staff       (20)     2343 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/resourcegroups.py
--rw-r--r--   0 mark       (501) staff       (20)     4196 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/robomaker.py
--rw-r--r--   0 mark       (501) staff       (20)     2688 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/rolesanywhere.py
--rw-r--r--   0 mark       (501) staff       (20)     8103 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/route53.py
--rw-r--r--   0 mark       (501) staff       (20)     3233 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/route53recoverycontrol.py
--rw-r--r--   0 mark       (501) staff       (20)     3654 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/route53recoveryreadiness.py
--rw-r--r--   0 mark       (501) staff       (20)     6588 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/route53resolver.py
--rw-r--r--   0 mark       (501) staff       (20)     2543 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/rum.py
--rw-r--r--   0 mark       (501) staff       (20)    36935 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/s3.py
--rw-r--r--   0 mark       (501) staff       (20)      932 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/s3express.py
--rw-r--r--   0 mark       (501) staff       (20)     3223 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/s3objectlambda.py
--rw-r--r--   0 mark       (501) staff       (20)     4439 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/s3outposts.py
--rw-r--r--   0 mark       (501) staff       (20)    94881 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/sagemaker.py
--rw-r--r--   0 mark       (501) staff       (20)     7106 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/scheduler.py
--rw-r--r--   0 mark       (501) staff       (20)      475 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/sdb.py
--rw-r--r--   0 mark       (501) staff       (20)     4391 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/secretsmanager.py
--rw-r--r--   0 mark       (501) staff       (20)     7777 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/securityhub.py
--rw-r--r--   0 mark       (501) staff       (20)    27801 2023-08-13 20:05:24.000000 troposphere-4.7.0/troposphere/serverless.py
--rw-r--r--   0 mark       (501) staff       (20)    11569 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/servicecatalog.py
--rw-r--r--   0 mark       (501) staff       (20)     1886 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/servicecatalogappregistry.py
--rw-r--r--   0 mark       (501) staff       (20)     4974 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/servicediscovery.py
--rw-r--r--   0 mark       (501) staff       (20)    15107 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ses.py
--rw-r--r--   0 mark       (501) staff       (20)     2979 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/shield.py
--rw-r--r--   0 mark       (501) staff       (20)     1441 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/signer.py
--rw-r--r--   0 mark       (501) staff       (20)      985 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/simspaceweaver.py
--rw-r--r--   0 mark       (501) staff       (20)     3082 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/sns.py
--rw-r--r--   0 mark       (501) staff       (20)     2172 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/sqs.py
--rw-r--r--   0 mark       (501) staff       (20)    14745 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ssm.py
--rw-r--r--   0 mark       (501) staff       (20)     4909 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ssmcontacts.py
--rw-r--r--   0 mark       (501) staff       (20)     5642 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/ssmincidents.py
--rw-r--r--   0 mark       (501) staff       (20)     3272 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/sso.py
--rw-r--r--   0 mark       (501) staff       (20)     4645 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/stepfunctions.py
--rw-r--r--   0 mark       (501) staff       (20)     1605 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/supportapp.py
--rw-r--r--   0 mark       (501) staff       (20)     4149 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/synthetics.py
--rw-r--r--   0 mark       (501) staff       (20)     1110 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/systemsmanagersap.py
--rw-r--r--   0 mark       (501) staff       (20)    17841 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/template_generator.py
--rw-r--r--   0 mark       (501) staff       (20)     7732 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/timestream.py
--rw-r--r--   0 mark       (501) staff       (20)    11970 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/transfer.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.941156 troposphere-4.7.0/troposphere/type_defs/
--rw-r--r--   0 mark       (501) staff       (20)       24 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/type_defs/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)      156 2023-10-25 14:19:18.000000 troposphere-4.7.0/troposphere/type_defs/compat.py
--rw-r--r--   0 mark       (501) staff       (20)      364 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/type_defs/protocols.py
--rw-r--r--   0 mark       (501) staff       (20)     1209 2021-03-27 21:20:50.000000 troposphere-4.7.0/troposphere/utils.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.977900 troposphere-4.7.0/troposphere/validators/
--rw-r--r--   0 mark       (501) staff       (20)     6908 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     2162 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/acmpca.py
--rw-r--r--   0 mark       (501) staff       (20)      245 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/amazonmq.py
--rw-r--r--   0 mark       (501) staff       (20)     2294 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/apigateway.py
--rw-r--r--   0 mark       (501) staff       (20)     3080 2022-11-26 22:45:50.000000 troposphere-4.7.0/troposphere/validators/apigatewayv2.py
--rw-r--r--   0 mark       (501) staff       (20)     1255 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/appconfig.py
--rw-r--r--   0 mark       (501) staff       (20)      522 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/appmesh.py
--rw-r--r--   0 mark       (501) staff       (20)      360 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/appstream.py
--rw-r--r--   0 mark       (501) staff       (20)      351 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/appsync.py
--rw-r--r--   0 mark       (501) staff       (20)     1096 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/athena.py
--rw-r--r--   0 mark       (501) staff       (20)     5945 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/autoscaling.py
--rw-r--r--   0 mark       (501) staff       (20)     3500 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/autoscalingplans.py
--rw-r--r--   0 mark       (501) staff       (20)     5704 2023-02-27 00:20:46.000000 troposphere-4.7.0/troposphere/validators/awslambda.py
--rw-r--r--   0 mark       (501) staff       (20)     1062 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/backup.py
--rw-r--r--   0 mark       (501) staff       (20)     1810 2023-08-13 20:05:24.000000 troposphere-4.7.0/troposphere/validators/batch.py
--rw-r--r--   0 mark       (501) staff       (20)      939 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/cassandra.py
--rw-r--r--   0 mark       (501) staff       (20)      250 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/certificatemanager.py
--rw-r--r--   0 mark       (501) staff       (20)      739 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/chatbot.py
--rw-r--r--   0 mark       (501) staff       (20)     5576 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/cloudformation.py
--rw-r--r--   0 mark       (501) staff       (20)     6167 2023-08-13 20:05:24.000000 troposphere-4.7.0/troposphere/validators/cloudfront.py
--rw-r--r--   0 mark       (501) staff       (20)     2120 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/cloudwatch.py
--rw-r--r--   0 mark       (501) staff       (20)      338 2022-07-26 17:37:41.000000 troposphere-4.7.0/troposphere/validators/codeartifact.py
--rw-r--r--   0 mark       (501) staff       (20)     7349 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/codebuild.py
--rw-r--r--   0 mark       (501) staff       (20)      726 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/codecommit.py
--rw-r--r--   0 mark       (501) staff       (20)     1530 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/codedeploy.py
--rw-r--r--   0 mark       (501) staff       (20)      615 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/codestarconnections.py
--rw-r--r--   0 mark       (501) staff       (20)      614 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/cognito.py
--rw-r--r--   0 mark       (501) staff       (20)      796 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/config.py
--rw-r--r--   0 mark       (501) staff       (20)     1338 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/dlm.py
--rw-r--r--   0 mark       (501) staff       (20)      450 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/dms.py
--rw-r--r--   0 mark       (501) staff       (20)     3126 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/dynamodb.py
--rw-r--r--   0 mark       (501) staff       (20)    10155 2024-02-12 20:46:08.000000 troposphere-4.7.0/troposphere/validators/ec2.py
--rw-r--r--   0 mark       (501) staff       (20)      378 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/ecr.py
--rw-r--r--   0 mark       (501) staff       (20)     3670 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/ecs.py
--rw-r--r--   0 mark       (501) staff       (20)     1008 2023-08-13 20:05:24.000000 troposphere-4.7.0/troposphere/validators/efs.py
--rw-r--r--   0 mark       (501) staff       (20)     1533 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/eks.py
--rw-r--r--   0 mark       (501) staff       (20)     1931 2024-01-29 16:54:30.000000 troposphere-4.7.0/troposphere/validators/elasticache.py
--rw-r--r--   0 mark       (501) staff       (20)      697 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/elasticbeanstalk.py
--rw-r--r--   0 mark       (501) staff       (20)     1080 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/elasticloadbalancing.py
--rw-r--r--   0 mark       (501) staff       (20)     5271 2023-02-24 15:58:15.000000 troposphere-4.7.0/troposphere/validators/elasticloadbalancingv2.py
--rw-r--r--   0 mark       (501) staff       (20)     1822 2022-10-24 14:32:59.000000 troposphere-4.7.0/troposphere/validators/elasticsearch.py
--rw-r--r--   0 mark       (501) staff       (20)     6259 2023-08-13 20:37:09.000000 troposphere-4.7.0/troposphere/validators/emr.py
--rw-r--r--   0 mark       (501) staff       (20)     1744 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/firehose.py
--rw-r--r--   0 mark       (501) staff       (20)      266 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/fms.py
--rw-r--r--   0 mark       (501) staff       (20)     2977 2023-01-28 23:39:49.000000 troposphere-4.7.0/troposphere/validators/fsx.py
--rw-r--r--   0 mark       (501) staff       (20)     1331 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/globalaccelerator.py
--rw-r--r--   0 mark       (501) staff       (20)     1861 2024-01-15 20:08:25.000000 troposphere-4.7.0/troposphere/validators/glue.py
--rw-r--r--   0 mark       (501) staff       (20)      311 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/groundstation.py
--rw-r--r--   0 mark       (501) staff       (20)     2488 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/iam.py
--rw-r--r--   0 mark       (501) staff       (20)     1580 2022-07-29 04:58:27.000000 troposphere-4.7.0/troposphere/validators/imagebuilder.py
--rw-r--r--   0 mark       (501) staff       (20)      509 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/iot.py
--rw-r--r--   0 mark       (501) staff       (20)      394 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/iot1click.py
--rw-r--r--   0 mark       (501) staff       (20)      945 2023-08-13 20:05:24.000000 troposphere-4.7.0/troposphere/validators/iottwinmaker.py
--rw-r--r--   0 mark       (501) staff       (20)      520 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/kinesis.py
--rw-r--r--   0 mark       (501) staff       (20)      756 2022-12-09 19:28:46.000000 troposphere-4.7.0/troposphere/validators/kinesisanalyticsv2.py
--rw-r--r--   0 mark       (501) staff       (20)      802 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/kms.py
--rw-r--r--   0 mark       (501) staff       (20)      276 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/lex.py
--rw-r--r--   0 mark       (501) staff       (20)     1454 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/logs.py
--rw-r--r--   0 mark       (501) staff       (20)     1038 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/macie.py
--rw-r--r--   0 mark       (501) staff       (20)      441 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/mediastore.py
--rw-r--r--   0 mark       (501) staff       (20)      497 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/networkfirewall.py
--rw-r--r--   0 mark       (501) staff       (20)      674 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/opensearchservice.py
--rw-r--r--   0 mark       (501) staff       (20)     2080 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/opsworks.py
--rw-r--r--   0 mark       (501) staff       (20)      245 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/opsworkscm.py
--rw-r--r--   0 mark       (501) staff       (20)      481 2022-11-26 19:38:58.000000 troposphere-4.7.0/troposphere/validators/organizations.py
--rw-r--r--   0 mark       (501) staff       (20)    15707 2024-02-14 23:39:39.000000 troposphere-4.7.0/troposphere/validators/rds.py
--rw-r--r--   0 mark       (501) staff       (20)      759 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/rekognition.py
--rw-r--r--   0 mark       (501) staff       (20)     1219 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/resiliencehub.py
--rw-r--r--   0 mark       (501) staff       (20)      393 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/resourcegroups.py
--rw-r--r--   0 mark       (501) staff       (20)      828 2023-01-28 20:33:37.000000 troposphere-4.7.0/troposphere/validators/route53.py
--rw-r--r--   0 mark       (501) staff       (20)      434 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/route53resolver.py
--rw-r--r--   0 mark       (501) staff       (20)     3538 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/s3.py
--rw-r--r--   0 mark       (501) staff       (20)      858 2023-01-28 23:24:40.000000 troposphere-4.7.0/troposphere/validators/scheduler.py
--rw-r--r--   0 mark       (501) staff       (20)      934 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/secretsmanager.py
--rw-r--r--   0 mark       (501) staff       (20)      457 2023-10-22 17:53:55.000000 troposphere-4.7.0/troposphere/validators/servicecatalog.py
--rw-r--r--   0 mark       (501) staff       (20)      281 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/sns.py
--rw-r--r--   0 mark       (501) staff       (20)      732 2022-06-17 14:59:36.000000 troposphere-4.7.0/troposphere/validators/sqs.py
--rw-r--r--   0 mark       (501) staff       (20)     3091 2022-07-22 22:21:38.000000 troposphere-4.7.0/troposphere/validators/ssm.py
--rw-r--r--   0 mark       (501) staff       (20)      673 2024-03-06 21:41:19.000000 troposphere-4.7.0/troposphere/validators/synthetics.py
--rw-r--r--   0 mark       (501) staff       (20)      563 2023-10-22 17:53:55.000000 troposphere-4.7.0/troposphere/validators/transfer.py
--rw-r--r--   0 mark       (501) staff       (20)      264 2022-06-17 14:59:37.000000 troposphere-4.7.0/troposphere/validators/waf.py
--rw-r--r--   0 mark       (501) staff       (20)      264 2022-06-17 14:59:37.000000 troposphere-4.7.0/troposphere/validators/wafregional.py
--rw-r--r--   0 mark       (501) staff       (20)     4939 2023-08-13 20:05:24.000000 troposphere-4.7.0/troposphere/validators/wafv2.py
--rw-r--r--   0 mark       (501) staff       (20)     4962 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/verifiedpermissions.py
--rw-r--r--   0 mark       (501) staff       (20)      966 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/voiceid.py
--rw-r--r--   0 mark       (501) staff       (20)     9875 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/vpclattice.py
--rw-r--r--   0 mark       (501) staff       (20)     5660 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/waf.py
--rw-r--r--   0 mark       (501) staff       (20)     7671 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/wafregional.py
--rw-r--r--   0 mark       (501) staff       (20)    32847 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/wafv2.py
--rw-r--r--   0 mark       (501) staff       (20)     3317 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/wisdom.py
--rw-r--r--   0 mark       (501) staff       (20)     1710 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/workspaces.py
--rw-r--r--   0 mark       (501) staff       (20)     1448 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/workspacesthinclient.py
--rw-r--r--   0 mark       (501) staff       (20)     5440 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/workspacesweb.py
--rw-r--r--   0 mark       (501) staff       (20)     2442 2024-03-08 22:53:51.000000 troposphere-4.7.0/troposphere/xray.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-03-10 20:55:59.978296 troposphere-4.7.0/troposphere.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     9160 2024-03-10 20:55:59.000000 troposphere-4.7.0/troposphere.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)    13732 2024-03-10 20:55:59.000000 troposphere-4.7.0/troposphere.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2024-03-10 20:55:59.000000 troposphere-4.7.0/troposphere.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2021-03-27 20:52:43.000000 troposphere-4.7.0/troposphere.egg-info/not-zip-safe
--rw-r--r--   0 mark       (501) staff       (20)       39 2024-03-10 20:55:59.000000 troposphere-4.7.0/troposphere.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       12 2024-03-10 20:55:59.000000 troposphere-4.7.0/troposphere.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.614122 troposphere-4.8.0/
+-rw-r--r--   0 mark       (501) staff       (20)      563 2022-06-17 14:59:33.000000 troposphere-4.8.0/.gitignore
+-rw-r--r--   0 mark       (501) staff       (20)     1319 2017-04-14 00:59:43.000000 troposphere-4.8.0/LICENSE
+-rw-r--r--   0 mark       (501) staff       (20)      111 2019-05-06 00:16:28.000000 troposphere-4.8.0/MANIFEST.in
+-rw-r--r--   0 mark       (501) staff       (20)     9160 2024-04-29 19:32:15.613861 troposphere-4.8.0/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     7929 2022-06-17 14:59:33.000000 troposphere-4.8.0/README.rst
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.430379 troposphere-4.8.0/examples/
+-rw-r--r--   0 mark       (501) staff       (20)     5175 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/ApiGateway.py
+-rw-r--r--   0 mark       (501) staff       (20)     1061 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/ApplicationAutoScalingSample.py
+-rw-r--r--   0 mark       (501) staff       (20)     7076 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/ApplicationELB.py
+-rw-r--r--   0 mark       (501) staff       (20)     5440 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/ApplicationLB_FixedActions.py
+-rw-r--r--   0 mark       (501) staff       (20)     4339 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/AuroraServerlessRDS_SecretsManager.py
+-rw-r--r--   0 mark       (501) staff       (20)     8535 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/Autoscaling.py
+-rw-r--r--   0 mark       (501) staff       (20)     9383 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/AutoscalingHTTPRequests.py
+-rw-r--r--   0 mark       (501) staff       (20)     2883 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/Backup.py
+-rw-r--r--   0 mark       (501) staff       (20)     3607 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Batch.py
+-rw-r--r--   0 mark       (501) staff       (20)    11829 2022-08-08 22:11:46.000000 troposphere-4.8.0/examples/BatchEventSnsLambda.py
+-rw-r--r--   0 mark       (501) staff       (20)      508 2021-03-27 21:38:06.000000 troposphere-4.8.0/examples/CertificateManagerSample.py
+-rw-r--r--   0 mark       (501) staff       (20)      549 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/ClassExtensions.py
+-rw-r--r--   0 mark       (501) staff       (20)     3000 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/CloudFormation_Init_ConfigSet.py
+-rw-r--r--   0 mark       (501) staff       (20)     1833 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/CloudFront_Distribution_S3.py
+-rw-r--r--   0 mark       (501) staff       (20)     1558 2022-01-05 01:20:25.000000 troposphere-4.8.0/examples/CloudFront_StreamingDistribution_S3.py
+-rw-r--r--   0 mark       (501) staff       (20)     2915 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/CloudTrail.py
+-rw-r--r--   0 mark       (501) staff       (20)     1477 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/CloudWatchEventsSample.py
+-rw-r--r--   0 mark       (501) staff       (20)      773 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/CodeBuild.py
+-rw-r--r--   0 mark       (501) staff       (20)     2503 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/CodeDeploy.py
+-rw-r--r--   0 mark       (501) staff       (20)     3626 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/CodePipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)      990 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/CustomResource.py
+-rw-r--r--   0 mark       (501) staff       (20)     1544 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Dlm.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2298 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/DynamoDB_Table.py
+-rw-r--r--   0 mark       (501) staff       (20)     5293 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/DynamoDB_Table_With_GSI_And_NonKeyAttributes_Projection.py
+-rw-r--r--   0 mark       (501) staff       (20)     5031 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/DynamoDB_Table_With_GlobalSecondaryIndex.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2701 2021-04-24 21:53:41.000000 troposphere-4.8.0/examples/DynamoDB_Table_With_KinesisStreamSpecification.py
+-rw-r--r--   0 mark       (501) staff       (20)     6897 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/DynamoDB_Tables_OnDemand.py
+-rw-r--r--   0 mark       (501) staff       (20)     2064 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/EC2Conditions.py
+-rw-r--r--   0 mark       (501) staff       (20)     2299 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/EC2InstanceSample.py
+-rw-r--r--   0 mark       (501) staff       (20)     2710 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/EC2_Remove_Ephemeral_Drive.py
+-rw-r--r--   0 mark       (501) staff       (20)     1253 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/ECRSample.py
+-rw-r--r--   0 mark       (501) staff       (20)     8934 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/ECSCluster.py
+-rw-r--r--   0 mark       (501) staff       (20)     1272 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/ECSFargate.py
+-rw-r--r--   0 mark       (501) staff       (20)     4271 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/EFS.py
+-rw-r--r--   0 mark       (501) staff       (20)     4835 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/ELBSample.py
+-rw-r--r--   0 mark       (501) staff       (20)     8958 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/EMR_Cluster.py
+-rwxr-xr-x   0 mark       (501) staff       (20)    25606 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/ElastiCacheRedis.py
+-rw-r--r--   0 mark       (501) staff       (20)     5587 2021-07-04 20:54:52.000000 troposphere-4.8.0/examples/ElasticBeanstalk_Nodejs_Sample.py
+-rw-r--r--   0 mark       (501) staff       (20)     1596 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/ElasticsearchDomain.py
+-rw-r--r--   0 mark       (501) staff       (20)     2134 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Firehose_with_Redshift.py
+-rw-r--r--   0 mark       (501) staff       (20)     1413 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/IAM_Policies_SNS_Publish_To_SQS.py
+-rw-r--r--   0 mark       (501) staff       (20)      838 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/IAM_Roles_and_InstanceProfiles.py
+-rw-r--r--   0 mark       (501) staff       (20)     1919 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/IAM_Users_Groups_and_Policies.py
+-rw-r--r--   0 mark       (501) staff       (20)     1943 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/IAM_Users_snippet.py
+-rw-r--r--   0 mark       (501) staff       (20)     2670 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/IoTAnalytics.py
+-rw-r--r--   0 mark       (501) staff       (20)     1852 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/IoTSample.py
+-rw-r--r--   0 mark       (501) staff       (20)      441 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/Kinesis_Stream.py
+-rw-r--r--   0 mark       (501) staff       (20)     5327 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/Lambda.py
+-rw-r--r--   0 mark       (501) staff       (20)      829 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/Mediapackage.py
+-rw-r--r--   0 mark       (501) staff       (20)      317 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/Metadata.py
+-rw-r--r--   0 mark       (501) staff       (20)     1564 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/MskCluster.py
+-rw-r--r--   0 mark       (501) staff       (20)     3181 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/NatGateway.py
+-rw-r--r--   0 mark       (501) staff       (20)     5651 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/NetworkLB.py
+-rw-r--r--   0 mark       (501) staff       (20)     4834 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/OpenStack_AutoScaling.py
+-rw-r--r--   0 mark       (501) staff       (20)     1962 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/OpenStack_Server.py
+-rw-r--r--   0 mark       (501) staff       (20)     5280 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/OpsWorksSnippet.py
+-rw-r--r--   0 mark       (501) staff       (20)     1407 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/RDS_Snapshot_On_Delete.py
+-rw-r--r--   0 mark       (501) staff       (20)     5097 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/RDS_VPC.py
+-rw-r--r--   0 mark       (501) staff       (20)     1989 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/RDS_with_DBParameterGroup.py
+-rw-r--r--   0 mark       (501) staff       (20)     3514 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Redshift.py
+-rw-r--r--   0 mark       (501) staff       (20)     4876 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/RedshiftClusterInVpc.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     1722 2022-11-26 19:34:19.000000 troposphere-4.8.0/examples/RedshiftServerless.py
+-rw-r--r--   0 mark       (501) staff       (20)     1962 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/Route53_A.py
+-rw-r--r--   0 mark       (501) staff       (20)     1329 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/Route53_CNAME.py
+-rw-r--r--   0 mark       (501) staff       (20)     2491 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/Route53_RoundRobin.py
+-rw-r--r--   0 mark       (501) staff       (20)      815 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/S3_Bucket.py
+-rw-r--r--   0 mark       (501) staff       (20)     1081 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/S3_Bucket_With_AccelerateConfiguration.py
+-rw-r--r--   0 mark       (501) staff       (20)     2580 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/S3_Bucket_With_Versioning_And_Lifecycle_Rules.py
+-rw-r--r--   0 mark       (501) staff       (20)     1420 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/S3_Website_Bucket_With_Retain_On_Delete.py
+-rw-r--r--   0 mark       (501) staff       (20)     1530 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/SQSDLQ.py
+-rw-r--r--   0 mark       (501) staff       (20)     1021 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/SQSEncrypt.py
+-rw-r--r--   0 mark       (501) staff       (20)     2312 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/SQS_With_CloudWatch_Alarms.py
+-rw-r--r--   0 mark       (501) staff       (20)     2559 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/SSMExample.py
+-rw-r--r--   0 mark       (501) staff       (20)      550 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Secretsmanager.py
+-rw-r--r--   0 mark       (501) staff       (20)     1441 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Secretsmanager_Rds.py
+-rw-r--r--   0 mark       (501) staff       (20)     1946 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Serverless_Api_Backend.py
+-rw-r--r--   0 mark       (501) staff       (20)      814 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Serverless_Deployment_Preference.py
+-rw-r--r--   0 mark       (501) staff       (20)      969 2022-03-02 00:34:16.000000 troposphere-4.8.0/examples/Serverless_S3_Processor.py
+-rw-r--r--   0 mark       (501) staff       (20)     5077 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/VPC_EC2_Instance_With_Multiple_Dynamic_IPAddresses.py
+-rw-r--r--   0 mark       (501) staff       (20)     6446 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/VPC_With_VPN_Connection.py
+-rw-r--r--   0 mark       (501) staff       (20)    15713 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/VPC_single_instance_in_subnet.py
+-rw-r--r--   0 mark       (501) staff       (20)     1054 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/VpnEndpoint.py
+-rw-r--r--   0 mark       (501) staff       (20)     5454 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/WAF_Common_Attacks_Sample.py
+-rw-r--r--   0 mark       (501) staff       (20)     5462 2022-06-17 14:59:33.000000 troposphere-4.8.0/examples/WAF_Regional_Common_Attacks_Sample.py
+-rw-r--r--   0 mark       (501) staff       (20)     1511 2021-03-27 21:20:49.000000 troposphere-4.8.0/examples/WaitObject.py
+-rw-r--r--   0 mark       (501) staff       (20)      565 2023-12-21 21:43:55.000000 troposphere-4.8.0/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)      115 2019-05-06 00:16:28.000000 troposphere-4.8.0/requirements.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.431362 troposphere-4.8.0/scripts/
+-rwxr-xr-x   0 mark       (501) staff       (20)     6100 2022-07-22 22:21:38.000000 troposphere-4.8.0/scripts/cfn
+-rwxr-xr-x   0 mark       (501) staff       (20)    12048 2022-06-17 14:59:33.000000 troposphere-4.8.0/scripts/cfn2py
+-rw-r--r--   0 mark       (501) staff       (20)     1569 2024-04-29 19:32:15.614814 troposphere-4.8.0/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)       38 2021-03-27 20:52:28.000000 troposphere-4.8.0/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.463039 troposphere-4.8.0/tests/
+-rw-r--r--   0 mark       (501) staff       (20)     1945 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_apigateway.py
+-rw-r--r--   0 mark       (501) staff       (20)     2724 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_apigatewayv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     1680 2023-02-24 15:58:15.000000 troposphere-4.8.0/tests/test_appconfig.py
+-rw-r--r--   0 mark       (501) staff       (20)     1609 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_appsync.py
+-rw-r--r--   0 mark       (501) staff       (20)     4598 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_asg.py
+-rw-r--r--   0 mark       (501) staff       (20)     8412 2023-02-27 00:23:50.000000 troposphere-4.8.0/tests/test_awslambda.py
+-rw-r--r--   0 mark       (501) staff       (20)    20416 2023-11-10 16:04:26.000000 troposphere-4.8.0/tests/test_basic.py
+-rw-r--r--   0 mark       (501) staff       (20)     1072 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_cloudformation.py
+-rw-r--r--   0 mark       (501) staff       (20)      886 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_cloudfront.py
+-rw-r--r--   0 mark       (501) staff       (20)     1665 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_cloudwatch.py
+-rw-r--r--   0 mark       (501) staff       (20)     4112 2023-02-24 15:58:15.000000 troposphere-4.8.0/tests/test_codebuild.py
+-rw-r--r--   0 mark       (501) staff       (20)     1231 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_codecommit.py
+-rw-r--r--   0 mark       (501) staff       (20)      642 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_config.py
+-rw-r--r--   0 mark       (501) staff       (20)     2613 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_dict.py
+-rw-r--r--   0 mark       (501) staff       (20)      585 2023-02-24 15:58:15.000000 troposphere-4.8.0/tests/test_dlm.py
+-rw-r--r--   0 mark       (501) staff       (20)     4714 2023-08-13 20:05:24.000000 troposphere-4.8.0/tests/test_ec2.py
+-rw-r--r--   0 mark       (501) staff       (20)      308 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_ecr.py
+-rw-r--r--   0 mark       (501) staff       (20)     8500 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_ecs.py
+-rw-r--r--   0 mark       (501) staff       (20)     1988 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_efs.py
+-rw-r--r--   0 mark       (501) staff       (20)     1803 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_eks.py
+-rw-r--r--   0 mark       (501) staff       (20)     4712 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_elasticloadbalancerv2.py
+-rw-r--r--   0 mark       (501) staff       (20)    11735 2023-02-24 16:29:02.000000 troposphere-4.8.0/tests/test_emr.py
+-rw-r--r--   0 mark       (501) staff       (20)     1549 2022-01-17 22:13:33.000000 troposphere-4.8.0/tests/test_examples.py
+-rw-r--r--   0 mark       (501) staff       (20)     1773 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_examples_template_generator.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     1264 2023-10-25 14:19:18.000000 troposphere-4.8.0/tests/test_findinmap.py
+-rw-r--r--   0 mark       (501) staff       (20)      616 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_fsx.py
+-rw-r--r--   0 mark       (501) staff       (20)     1576 2023-12-06 22:15:23.000000 troposphere-4.8.0/tests/test_guardduty.py
+-rw-r--r--   0 mark       (501) staff       (20)     1876 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_int_type.py
+-rw-r--r--   0 mark       (501) staff       (20)      846 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_iot1click.py
+-rw-r--r--   0 mark       (501) staff       (20)      622 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_iottwinmaker.py
+-rw-r--r--   0 mark       (501) staff       (20)     2131 2022-10-24 14:32:59.000000 troposphere-4.8.0/tests/test_language_extensions.py
+-rw-r--r--   0 mark       (501) staff       (20)     2530 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_logs.py
+-rw-r--r--   0 mark       (501) staff       (20)      843 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_mappings.py
+-rw-r--r--   0 mark       (501) staff       (20)      612 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_networkfirewall.py
+-rw-r--r--   0 mark       (501) staff       (20)      809 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_opensearchservice.py
+-rw-r--r--   0 mark       (501) staff       (20)     1671 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_opsworks.py
+-rw-r--r--   0 mark       (501) staff       (20)     1323 2023-10-25 14:19:18.000000 troposphere-4.8.0/tests/test_parameters.py
+-rw-r--r--   0 mark       (501) staff       (20)     5150 2022-06-17 14:59:34.000000 troposphere-4.8.0/tests/test_policies.py
+-rw-r--r--   0 mark       (501) staff       (20)    14858 2024-02-14 23:42:50.000000 troposphere-4.8.0/tests/test_rds.py
+-rw-r--r--   0 mark       (501) staff       (20)     1336 2022-06-17 14:59:35.000000 troposphere-4.8.0/tests/test_resiliencehub.py
+-rw-r--r--   0 mark       (501) staff       (20)      409 2022-06-17 14:59:35.000000 troposphere-4.8.0/tests/test_route53.py
+-rw-r--r--   0 mark       (501) staff       (20)     2130 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_s3.py
+-rw-r--r--   0 mark       (501) staff       (20)      775 2023-01-28 23:24:40.000000 troposphere-4.8.0/tests/test_scheduler.py
+-rw-r--r--   0 mark       (501) staff       (20)    15112 2023-08-13 20:05:24.000000 troposphere-4.8.0/tests/test_serverless.py
+-rw-r--r--   0 mark       (501) staff       (20)      782 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_sqs.py
+-rw-r--r--   0 mark       (501) staff       (20)      527 2022-07-22 22:21:38.000000 troposphere-4.8.0/tests/test_ssm.py
+-rw-r--r--   0 mark       (501) staff       (20)      828 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_stepfunctions.py
+-rw-r--r--   0 mark       (501) staff       (20)     2653 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_tags.py
+-rw-r--r--   0 mark       (501) staff       (20)     6943 2023-10-26 21:02:29.000000 troposphere-4.8.0/tests/test_template.py
+-rw-r--r--   0 mark       (501) staff       (20)     4214 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_template_generator.py
+-rw-r--r--   0 mark       (501) staff       (20)     1795 2021-03-27 21:20:49.000000 troposphere-4.8.0/tests/test_userdata.py
+-rw-r--r--   0 mark       (501) staff       (20)     9703 2022-06-17 14:59:35.000000 troposphere-4.8.0/tests/test_validators.py
+-rw-r--r--   0 mark       (501) staff       (20)     4353 2022-06-17 14:59:35.000000 troposphere-4.8.0/tests/test_wafv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     2044 2022-06-17 14:59:35.000000 troposphere-4.8.0/tests/test_yaml.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.571317 troposphere-4.8.0/troposphere/
+-rw-r--r--   0 mark       (501) staff       (20)    37341 2024-04-29 19:28:39.000000 troposphere-4.8.0/troposphere/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     2053 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/accessanalyzer.py
+-rw-r--r--   0 mark       (501) staff       (20)    10858 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/acmpca.py
+-rw-r--r--   0 mark       (501) staff       (20)     4704 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/amazonmq.py
+-rw-r--r--   0 mark       (501) staff       (20)     5504 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/amplify.py
+-rw-r--r--   0 mark       (501) staff       (20)     8774 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/analytics.py
+-rw-r--r--   0 mark       (501) staff       (20)    17726 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/apigateway.py
+-rw-r--r--   0 mark       (501) staff       (20)    13938 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/apigatewayv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     5987 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/appconfig.py
+-rw-r--r--   0 mark       (501) staff       (20)    42057 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/appflow.py
+-rw-r--r--   0 mark       (501) staff       (20)     3408 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/appintegrations.py
+-rw-r--r--   0 mark       (501) staff       (20)     7355 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/applicationautoscaling.py
+-rw-r--r--   0 mark       (501) staff       (20)     8330 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/applicationinsights.py
+-rw-r--r--   0 mark       (501) staff       (20)    46906 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/appmesh.py
+-rw-r--r--   0 mark       (501) staff       (20)     9596 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/apprunner.py
+-rw-r--r--   0 mark       (501) staff       (20)    12585 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/appstream.py
+-rw-r--r--   0 mark       (501) staff       (20)    15117 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/appsync.py
+-rw-r--r--   0 mark       (501) staff       (20)     3201 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/aps.py
+-rw-r--r--   0 mark       (501) staff       (20)     1516 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/arczonalshift.py
+-rw-r--r--   0 mark       (501) staff       (20)     1610 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/ask.py
+-rw-r--r--   0 mark       (501) staff       (20)     5770 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/athena.py
+-rw-r--r--   0 mark       (501) staff       (20)     3045 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/auditmanager.py
+-rw-r--r--   0 mark       (501) staff       (20)    24067 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/autoscaling.py
+-rw-r--r--   0 mark       (501) staff       (20)     5587 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/autoscalingplans.py
+-rw-r--r--   0 mark       (501) staff       (20)    17344 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/awslambda.py
+-rw-r--r--   0 mark       (501) staff       (20)     3544 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/b2bi.py
+-rw-r--r--   0 mark       (501) staff       (20)    11634 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/backup.py
+-rw-r--r--   0 mark       (501) staff       (20)      711 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/backupgateway.py
+-rw-r--r--   0 mark       (501) staff       (20)    23154 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/batch.py
+-rw-r--r--   0 mark       (501) staff       (20)     2997 2024-04-29 19:03:28.000000 troposphere-4.8.0/troposphere/bcmdataexports.py
+-rw-r--r--   0 mark       (501) staff       (20)    16181 2024-04-29 19:03:28.000000 troposphere-4.8.0/troposphere/bedrock.py
+-rw-r--r--   0 mark       (501) staff       (20)     5549 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/billingconductor.py
+-rw-r--r--   0 mark       (501) staff       (20)     6713 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/budgets.py
+-rw-r--r--   0 mark       (501) staff       (20)     5681 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/cassandra.py
+-rw-r--r--   0 mark       (501) staff       (20)     2311 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/ce.py
+-rw-r--r--   0 mark       (501) staff       (20)     2028 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/certificatemanager.py
+-rw-r--r--   0 mark       (501) staff       (20)     1653 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/chatbot.py
+-rw-r--r--   0 mark       (501) staff       (20)    12676 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/cleanrooms.py
+-rw-r--r--   0 mark       (501) staff       (20)     2249 2024-04-29 19:03:28.000000 troposphere-4.8.0/troposphere/cleanroomsml.py
+-rw-r--r--   0 mark       (501) staff       (20)     1200 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/cloud9.py
+-rw-r--r--   0 mark       (501) staff       (20)    10879 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/cloudformation.py
+-rw-r--r--   0 mark       (501) staff       (20)    37095 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/cloudfront.py
+-rw-r--r--   0 mark       (501) staff       (20)     4985 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/cloudtrail.py
+-rw-r--r--   0 mark       (501) staff       (20)     8818 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/cloudwatch.py
+-rw-r--r--   0 mark       (501) staff       (20)     2812 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codeartifact.py
+-rw-r--r--   0 mark       (501) staff       (20)    12123 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codebuild.py
+-rw-r--r--   0 mark       (501) staff       (20)     1772 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codecommit.py
+-rw-r--r--   0 mark       (501) staff       (20)      625 2024-04-29 19:03:28.000000 troposphere-4.8.0/troposphere/codeconnections.py
+-rw-r--r--   0 mark       (501) staff       (20)    13982 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codedeploy.py
+-rw-r--r--   0 mark       (501) staff       (20)     1336 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codeguruprofiler.py
+-rw-r--r--   0 mark       (501) staff       (20)      725 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codegurureviewer.py
+-rw-r--r--   0 mark       (501) staff       (20)    10598 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codepipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)     1389 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/codestar.py
+-rw-r--r--   0 mark       (501) staff       (20)     1822 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codestarconnections.py
+-rw-r--r--   0 mark       (501) staff       (20)     1173 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/codestarnotifications.py
+-rw-r--r--   0 mark       (501) staff       (20)    25006 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/cognito.py
+-rw-r--r--   0 mark       (501) staff       (20)      803 2023-08-13 20:05:24.000000 troposphere-4.8.0/troposphere/compat.py
+-rw-r--r--   0 mark       (501) staff       (20)     5786 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/comprehend.py
+-rw-r--r--   0 mark       (501) staff       (20)    15661 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/config.py
+-rw-r--r--   0 mark       (501) staff       (20)    24550 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/connect.py
+-rw-r--r--   0 mark       (501) staff       (20)     3034 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/connectcampaigns.py
+-rw-r--r--   0 mark       (501) staff       (20)    43847 2023-10-26 21:12:57.000000 troposphere-4.8.0/troposphere/constants.py
+-rw-r--r--   0 mark       (501) staff       (20)     2132 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/controltower.py
+-rw-r--r--   0 mark       (501) staff       (20)      973 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/cur.py
+-rw-r--r--   0 mark       (501) staff       (20)    16498 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/customerprofiles.py
+-rw-r--r--   0 mark       (501) staff       (20)    22007 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/databrew.py
+-rw-r--r--   0 mark       (501) staff       (20)     2692 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/datapipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)    17089 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/datasync.py
+-rw-r--r--   0 mark       (501) staff       (20)    10063 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/datazone.py
+-rw-r--r--   0 mark       (501) staff       (20)     2113 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/dax.py
+-rw-r--r--   0 mark       (501) staff       (20)    11026 2024-04-29 19:03:28.000000 troposphere-4.8.0/troposphere/deadline.py
+-rw-r--r--   0 mark       (501) staff       (20)     1354 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/detective.py
+-rw-r--r--   0 mark       (501) staff       (20)     3286 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/devopsguru.py
+-rw-r--r--   0 mark       (501) staff       (20)     1626 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/directoryservice.py
+-rw-r--r--   0 mark       (501) staff       (20)    10001 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/dlm.py
+-rw-r--r--   0 mark       (501) staff       (20)    24459 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/dms.py
+-rw-r--r--   0 mark       (501) staff       (20)     3666 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/docdb.py
+-rw-r--r--   0 mark       (501) staff       (20)     1076 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/docdbelastic.py
+-rw-r--r--   0 mark       (501) staff       (20)    13375 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/dynamodb.py
+-rw-r--r--   0 mark       (501) staff       (20)   107011 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/ec2.py
+-rw-r--r--   0 mark       (501) staff       (20)     5929 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/ecr.py
+-rw-r--r--   0 mark       (501) staff       (20)    29731 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/ecs.py
+-rw-r--r--   0 mark       (501) staff       (20)     4954 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/efs.py
+-rw-r--r--   0 mark       (501) staff       (20)    11430 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/eks.py
+-rw-r--r--   0 mark       (501) staff       (20)    13111 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/elasticache.py
+-rw-r--r--   0 mark       (501) staff       (20)     5696 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/elasticbeanstalk.py
+-rw-r--r--   0 mark       (501) staff       (20)     4393 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/elasticloadbalancing.py
+-rw-r--r--   0 mark       (501) staff       (20)    16923 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/elasticloadbalancingv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     6672 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/elasticsearch.py
+-rw-r--r--   0 mark       (501) staff       (20)    19238 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/emr.py
+-rw-r--r--   0 mark       (501) staff       (20)     1495 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/emrcontainers.py
+-rw-r--r--   0 mark       (501) staff       (20)     6774 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/emrserverless.py
+-rw-r--r--   0 mark       (501) staff       (20)     8619 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/entityresolution.py
+-rw-r--r--   0 mark       (501) staff       (20)    16239 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/events.py
+-rw-r--r--   0 mark       (501) staff       (20)     1842 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/eventschemas.py
+-rw-r--r--   0 mark       (501) staff       (20)     8771 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/evidently.py
+-rw-r--r--   0 mark       (501) staff       (20)     1963 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/finspace.py
+-rw-r--r--   0 mark       (501) staff       (20)    25627 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/firehose.py
+-rw-r--r--   0 mark       (501) staff       (20)     4491 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/fis.py
+-rw-r--r--   0 mark       (501) staff       (20)     3508 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/fms.py
+-rw-r--r--   0 mark       (501) staff       (20)     2279 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/forecast.py
+-rw-r--r--   0 mark       (501) staff       (20)     6791 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/frauddetector.py
+-rw-r--r--   0 mark       (501) staff       (20)    15293 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/fsx.py
+-rw-r--r--   0 mark       (501) staff       (20)    18575 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/gamelift.py
+-rw-r--r--   0 mark       (501) staff       (20)     3968 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/globalaccelerator.py
+-rw-r--r--   0 mark       (501) staff       (20)    33072 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/glue.py
+-rw-r--r--   0 mark       (501) staff       (20)     3374 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/grafana.py
+-rw-r--r--   0 mark       (501) staff       (20)    18307 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/greengrass.py
+-rw-r--r--   0 mark       (501) staff       (20)    10421 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/greengrassv2.py
+-rw-r--r--   0 mark       (501) staff       (20)    10694 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/groundstation.py
+-rw-r--r--   0 mark       (501) staff       (20)     7073 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/guardduty.py
+-rw-r--r--   0 mark       (501) staff       (20)      575 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/healthimaging.py
+-rw-r--r--   0 mark       (501) staff       (20)     2499 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/healthlake.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.573524 troposphere-4.8.0/troposphere/helpers/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2017-01-20 05:47:11.000000 troposphere-4.8.0/troposphere/helpers/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     1382 2021-06-13 00:15:44.000000 troposphere-4.8.0/troposphere/helpers/userdata.py
+-rw-r--r--   0 mark       (501) staff       (20)     7747 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iam.py
+-rw-r--r--   0 mark       (501) staff       (20)     1227 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/identitystore.py
+-rw-r--r--   0 mark       (501) staff       (20)    20496 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/imagebuilder.py
+-rw-r--r--   0 mark       (501) staff       (20)     1446 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/inspector.py
+-rw-r--r--   0 mark       (501) staff       (20)     6843 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/inspectorv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     2667 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/internetmonitor.py
+-rw-r--r--   0 mark       (501) staff       (20)    44436 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/iot.py
+-rw-r--r--   0 mark       (501) staff       (20)     2101 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iot1click.py
+-rw-r--r--   0 mark       (501) staff       (20)    18061 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iotanalytics.py
+-rw-r--r--   0 mark       (501) staff       (20)     1511 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iotcoredeviceadvisor.py
+-rw-r--r--   0 mark       (501) staff       (20)    13364 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iotevents.py
+-rw-r--r--   0 mark       (501) staff       (20)      631 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iotfleethub.py
+-rw-r--r--   0 mark       (501) staff       (20)    11514 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/iotfleetwise.py
+-rw-r--r--   0 mark       (501) staff       (20)    12806 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iotsitewise.py
+-rw-r--r--   0 mark       (501) staff       (20)      946 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iotthingsgraph.py
+-rw-r--r--   0 mark       (501) staff       (20)     9082 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iottwinmaker.py
+-rw-r--r--   0 mark       (501) staff       (20)    15493 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/iotwireless.py
+-rw-r--r--   0 mark       (501) staff       (20)     5697 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/ivs.py
+-rw-r--r--   0 mark       (501) staff       (20)     2968 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/ivschat.py
+-rw-r--r--   0 mark       (501) staff       (20)     8853 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/kafkaconnect.py
+-rw-r--r--   0 mark       (501) staff       (20)    29327 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/kendra.py
+-rw-r--r--   0 mark       (501) staff       (20)     1020 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/kendraranking.py
+-rw-r--r--   0 mark       (501) staff       (20)     1771 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/kinesis.py
+-rw-r--r--   0 mark       (501) staff       (20)    19659 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/kinesisanalyticsv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     1133 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/kinesisvideo.py
+-rw-r--r--   0 mark       (501) staff       (20)     1915 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/kms.py
+-rw-r--r--   0 mark       (501) staff       (20)    10866 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/lakeformation.py
+-rw-r--r--   0 mark       (501) staff       (20)    34001 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/lex.py
+-rw-r--r--   0 mark       (501) staff       (20)     3834 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/licensemanager.py
+-rw-r--r--   0 mark       (501) staff       (20)    16575 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/lightsail.py
+-rw-r--r--   0 mark       (501) staff       (20)     4462 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/location.py
+-rw-r--r--   0 mark       (501) staff       (20)     6224 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/logs.py
+-rw-r--r--   0 mark       (501) staff       (20)     2834 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/lookoutequipment.py
+-rw-r--r--   0 mark       (501) staff       (20)     7958 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/lookoutmetrics.py
+-rw-r--r--   0 mark       (501) staff       (20)      498 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/lookoutvision.py
+-rw-r--r--   0 mark       (501) staff       (20)     3121 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/m2.py
+-rw-r--r--   0 mark       (501) staff       (20)     3472 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/macie.py
+-rw-r--r--   0 mark       (501) staff       (20)     4756 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/managedblockchain.py
+-rw-r--r--   0 mark       (501) staff       (20)    11226 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/mediaconnect.py
+-rw-r--r--   0 mark       (501) staff       (20)     2375 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/mediaconvert.py
+-rw-r--r--   0 mark       (501) staff       (20)    82677 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/medialive.py
+-rw-r--r--   0 mark       (501) staff       (20)    15907 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/mediapackage.py
+-rw-r--r--   0 mark       (501) staff       (20)     7207 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/mediapackagev2.py
+-rw-r--r--   0 mark       (501) staff       (20)     1963 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/mediastore.py
+-rw-r--r--   0 mark       (501) staff       (20)    10787 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/mediatailor.py
+-rw-r--r--   0 mark       (501) staff       (20)     3659 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/memorydb.py
+-rw-r--r--   0 mark       (501) staff       (20)    16296 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/msk.py
+-rw-r--r--   0 mark       (501) staff       (20)     2793 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/mwaa.py
+-rw-r--r--   0 mark       (501) staff       (20)     4431 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/neptune.py
+-rw-r--r--   0 mark       (501) staff       (20)     1600 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/neptunegraph.py
+-rw-r--r--   0 mark       (501) staff       (20)    16133 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/networkfirewall.py
+-rw-r--r--   0 mark       (501) staff       (20)    10773 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/networkmanager.py
+-rw-r--r--   0 mark       (501) staff       (20)     8804 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/nimblestudio.py
+-rw-r--r--   0 mark       (501) staff       (20)     1535 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/oam.py
+-rw-r--r--   0 mark       (501) staff       (20)     4565 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/omics.py
+-rw-r--r--   0 mark       (501) staff       (20)     3233 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/opensearchserverless.py
+-rw-r--r--   0 mark       (501) staff       (20)     9376 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/opensearchservice.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.574679 troposphere-4.8.0/troposphere/openstack/
+-rw-r--r--   0 mark       (501) staff       (20)       91 2021-03-27 15:02:50.000000 troposphere-4.8.0/troposphere/openstack/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     1798 2021-03-27 21:04:46.000000 troposphere-4.8.0/troposphere/openstack/heat.py
+-rw-r--r--   0 mark       (501) staff       (20)     8723 2023-08-13 20:37:09.000000 troposphere-4.8.0/troposphere/openstack/neutron.py
+-rw-r--r--   0 mark       (501) staff       (20)     5593 2022-06-17 14:59:35.000000 troposphere-4.8.0/troposphere/openstack/nova.py
+-rw-r--r--   0 mark       (501) staff       (20)    12555 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/opsworks.py
+-rw-r--r--   0 mark       (501) staff       (20)     1713 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/opsworkscm.py
+-rw-r--r--   0 mark       (501) staff       (20)     2193 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/organizations.py
+-rw-r--r--   0 mark       (501) staff       (20)     2754 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/osis.py
+-rw-r--r--   0 mark       (501) staff       (20)     2826 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/panorama.py
+-rw-r--r--   0 mark       (501) staff       (20)     1983 2024-04-29 19:03:28.000000 troposphere-4.8.0/troposphere/paymentcryptography.py
+-rw-r--r--   0 mark       (501) staff       (20)    16599 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/pcaconnectorad.py
+-rw-r--r--   0 mark       (501) staff       (20)     6121 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/personalize.py
+-rw-r--r--   0 mark       (501) staff       (20)    26184 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/pinpoint.py
+-rw-r--r--   0 mark       (501) staff       (20)     5976 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/pinpointemail.py
+-rw-r--r--   0 mark       (501) staff       (20)    23116 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/pipes.py
+-rw-r--r--   0 mark       (501) staff       (20)     2038 2022-06-17 14:59:35.000000 troposphere-4.8.0/troposphere/policies.py
+-rw-r--r--   0 mark       (501) staff       (20)     1804 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/proton.py
+-rw-r--r--   0 mark       (501) staff       (20)     1505 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/qldb.py
+-rw-r--r--   0 mark       (501) staff       (20)   265713 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/quicksight.py
+-rw-r--r--   0 mark       (501) staff       (20)     1152 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/ram.py
+-rw-r--r--   0 mark       (501) staff       (20)    19490 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/rds.py
+-rw-r--r--   0 mark       (501) staff       (20)    10165 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/redshift.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     5435 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/redshiftserverless.py
+-rw-r--r--   0 mark       (501) staff       (20)     3966 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/refactorspaces.py
+-rw-r--r--   0 mark       (501) staff       (20)     4387 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/rekognition.py
+-rw-r--r--   0 mark       (501) staff       (20)     3827 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/resiliencehub.py
+-rw-r--r--   0 mark       (501) staff       (20)     1863 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/resourceexplorer2.py
+-rw-r--r--   0 mark       (501) staff       (20)     2343 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/resourcegroups.py
+-rw-r--r--   0 mark       (501) staff       (20)     4196 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/robomaker.py
+-rw-r--r--   0 mark       (501) staff       (20)     2688 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/rolesanywhere.py
+-rw-r--r--   0 mark       (501) staff       (20)     8103 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/route53.py
+-rw-r--r--   0 mark       (501) staff       (20)     1463 2024-04-29 19:03:28.000000 troposphere-4.8.0/troposphere/route53profiles.py
+-rw-r--r--   0 mark       (501) staff       (20)     3233 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/route53recoverycontrol.py
+-rw-r--r--   0 mark       (501) staff       (20)     3654 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/route53recoveryreadiness.py
+-rw-r--r--   0 mark       (501) staff       (20)     6588 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/route53resolver.py
+-rw-r--r--   0 mark       (501) staff       (20)     2543 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/rum.py
+-rw-r--r--   0 mark       (501) staff       (20)    36935 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/s3.py
+-rw-r--r--   0 mark       (501) staff       (20)      932 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/s3express.py
+-rw-r--r--   0 mark       (501) staff       (20)     3223 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/s3objectlambda.py
+-rw-r--r--   0 mark       (501) staff       (20)     4439 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/s3outposts.py
+-rw-r--r--   0 mark       (501) staff       (20)    95319 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/sagemaker.py
+-rw-r--r--   0 mark       (501) staff       (20)     7106 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/scheduler.py
+-rw-r--r--   0 mark       (501) staff       (20)      475 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/sdb.py
+-rw-r--r--   0 mark       (501) staff       (20)     4391 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/secretsmanager.py
+-rw-r--r--   0 mark       (501) staff       (20)    15188 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/securityhub.py
+-rw-r--r--   0 mark       (501) staff       (20)     4554 2024-04-29 19:03:28.000000 troposphere-4.8.0/troposphere/securitylake.py
+-rw-r--r--   0 mark       (501) staff       (20)    27874 2024-04-25 15:54:48.000000 troposphere-4.8.0/troposphere/serverless.py
+-rw-r--r--   0 mark       (501) staff       (20)    11569 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/servicecatalog.py
+-rw-r--r--   0 mark       (501) staff       (20)     1886 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/servicecatalogappregistry.py
+-rw-r--r--   0 mark       (501) staff       (20)     4974 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/servicediscovery.py
+-rw-r--r--   0 mark       (501) staff       (20)    15107 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/ses.py
+-rw-r--r--   0 mark       (501) staff       (20)     2979 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/shield.py
+-rw-r--r--   0 mark       (501) staff       (20)     1441 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/signer.py
+-rw-r--r--   0 mark       (501) staff       (20)      985 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/simspaceweaver.py
+-rw-r--r--   0 mark       (501) staff       (20)     3082 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/sns.py
+-rw-r--r--   0 mark       (501) staff       (20)     2172 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/sqs.py
+-rw-r--r--   0 mark       (501) staff       (20)    14745 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/ssm.py
+-rw-r--r--   0 mark       (501) staff       (20)     4909 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/ssmcontacts.py
+-rw-r--r--   0 mark       (501) staff       (20)     5642 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/ssmincidents.py
+-rw-r--r--   0 mark       (501) staff       (20)     3272 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/sso.py
+-rw-r--r--   0 mark       (501) staff       (20)     4645 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/stepfunctions.py
+-rw-r--r--   0 mark       (501) staff       (20)     1605 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/supportapp.py
+-rw-r--r--   0 mark       (501) staff       (20)     4149 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/synthetics.py
+-rw-r--r--   0 mark       (501) staff       (20)     1110 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/systemsmanagersap.py
+-rw-r--r--   0 mark       (501) staff       (20)    17841 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/template_generator.py
+-rw-r--r--   0 mark       (501) staff       (20)     8965 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/timestream.py
+-rw-r--r--   0 mark       (501) staff       (20)    11970 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/transfer.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.575532 troposphere-4.8.0/troposphere/type_defs/
+-rw-r--r--   0 mark       (501) staff       (20)       24 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/type_defs/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)      156 2023-10-25 14:19:18.000000 troposphere-4.8.0/troposphere/type_defs/compat.py
+-rw-r--r--   0 mark       (501) staff       (20)      364 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/type_defs/protocols.py
+-rw-r--r--   0 mark       (501) staff       (20)     1209 2021-03-27 21:20:50.000000 troposphere-4.8.0/troposphere/utils.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.612686 troposphere-4.8.0/troposphere/validators/
+-rw-r--r--   0 mark       (501) staff       (20)     6908 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     2162 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/acmpca.py
+-rw-r--r--   0 mark       (501) staff       (20)      245 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/amazonmq.py
+-rw-r--r--   0 mark       (501) staff       (20)     2294 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/apigateway.py
+-rw-r--r--   0 mark       (501) staff       (20)     3080 2022-11-26 22:45:50.000000 troposphere-4.8.0/troposphere/validators/apigatewayv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     1255 2023-02-24 15:58:15.000000 troposphere-4.8.0/troposphere/validators/appconfig.py
+-rw-r--r--   0 mark       (501) staff       (20)      522 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/appmesh.py
+-rw-r--r--   0 mark       (501) staff       (20)      360 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/appstream.py
+-rw-r--r--   0 mark       (501) staff       (20)      351 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/appsync.py
+-rw-r--r--   0 mark       (501) staff       (20)     1096 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/athena.py
+-rw-r--r--   0 mark       (501) staff       (20)     5945 2023-02-24 15:58:15.000000 troposphere-4.8.0/troposphere/validators/autoscaling.py
+-rw-r--r--   0 mark       (501) staff       (20)     3500 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/autoscalingplans.py
+-rw-r--r--   0 mark       (501) staff       (20)     5704 2023-02-27 00:20:46.000000 troposphere-4.8.0/troposphere/validators/awslambda.py
+-rw-r--r--   0 mark       (501) staff       (20)     1062 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/backup.py
+-rw-r--r--   0 mark       (501) staff       (20)     1810 2023-08-13 20:05:24.000000 troposphere-4.8.0/troposphere/validators/batch.py
+-rw-r--r--   0 mark       (501) staff       (20)      939 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/cassandra.py
+-rw-r--r--   0 mark       (501) staff       (20)      250 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/certificatemanager.py
+-rw-r--r--   0 mark       (501) staff       (20)      739 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/chatbot.py
+-rw-r--r--   0 mark       (501) staff       (20)     5576 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/cloudformation.py
+-rw-r--r--   0 mark       (501) staff       (20)     6167 2023-08-13 20:05:24.000000 troposphere-4.8.0/troposphere/validators/cloudfront.py
+-rw-r--r--   0 mark       (501) staff       (20)     2120 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/cloudwatch.py
+-rw-r--r--   0 mark       (501) staff       (20)      338 2022-07-26 17:37:41.000000 troposphere-4.8.0/troposphere/validators/codeartifact.py
+-rw-r--r--   0 mark       (501) staff       (20)     7349 2023-02-24 15:58:15.000000 troposphere-4.8.0/troposphere/validators/codebuild.py
+-rw-r--r--   0 mark       (501) staff       (20)      726 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/codecommit.py
+-rw-r--r--   0 mark       (501) staff       (20)     1530 2023-02-24 15:58:15.000000 troposphere-4.8.0/troposphere/validators/codedeploy.py
+-rw-r--r--   0 mark       (501) staff       (20)      615 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/codestarconnections.py
+-rw-r--r--   0 mark       (501) staff       (20)      614 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/cognito.py
+-rw-r--r--   0 mark       (501) staff       (20)      796 2023-02-24 15:58:15.000000 troposphere-4.8.0/troposphere/validators/config.py
+-rw-r--r--   0 mark       (501) staff       (20)     1341 2024-04-25 15:54:48.000000 troposphere-4.8.0/troposphere/validators/dlm.py
+-rw-r--r--   0 mark       (501) staff       (20)      450 2023-02-24 15:58:15.000000 troposphere-4.8.0/troposphere/validators/dms.py
+-rw-r--r--   0 mark       (501) staff       (20)     3126 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/dynamodb.py
+-rw-r--r--   0 mark       (501) staff       (20)    10155 2024-02-12 20:46:08.000000 troposphere-4.8.0/troposphere/validators/ec2.py
+-rw-r--r--   0 mark       (501) staff       (20)      378 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/ecr.py
+-rw-r--r--   0 mark       (501) staff       (20)     3670 2023-02-24 15:58:15.000000 troposphere-4.8.0/troposphere/validators/ecs.py
+-rw-r--r--   0 mark       (501) staff       (20)     1008 2023-08-13 20:05:24.000000 troposphere-4.8.0/troposphere/validators/efs.py
+-rw-r--r--   0 mark       (501) staff       (20)     1533 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/eks.py
+-rw-r--r--   0 mark       (501) staff       (20)     1931 2024-01-29 16:54:30.000000 troposphere-4.8.0/troposphere/validators/elasticache.py
+-rw-r--r--   0 mark       (501) staff       (20)      697 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/elasticbeanstalk.py
+-rw-r--r--   0 mark       (501) staff       (20)     1080 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/elasticloadbalancing.py
+-rw-r--r--   0 mark       (501) staff       (20)     5271 2023-02-24 15:58:15.000000 troposphere-4.8.0/troposphere/validators/elasticloadbalancingv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     1822 2022-10-24 14:32:59.000000 troposphere-4.8.0/troposphere/validators/elasticsearch.py
+-rw-r--r--   0 mark       (501) staff       (20)     6259 2023-08-13 20:37:09.000000 troposphere-4.8.0/troposphere/validators/emr.py
+-rw-r--r--   0 mark       (501) staff       (20)     1744 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/firehose.py
+-rw-r--r--   0 mark       (501) staff       (20)      266 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/fms.py
+-rw-r--r--   0 mark       (501) staff       (20)     2977 2023-01-28 23:39:49.000000 troposphere-4.8.0/troposphere/validators/fsx.py
+-rw-r--r--   0 mark       (501) staff       (20)     1331 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/globalaccelerator.py
+-rw-r--r--   0 mark       (501) staff       (20)     1861 2024-01-15 20:08:25.000000 troposphere-4.8.0/troposphere/validators/glue.py
+-rw-r--r--   0 mark       (501) staff       (20)      311 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/groundstation.py
+-rw-r--r--   0 mark       (501) staff       (20)     2488 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/iam.py
+-rw-r--r--   0 mark       (501) staff       (20)     1580 2022-07-29 04:58:27.000000 troposphere-4.8.0/troposphere/validators/imagebuilder.py
+-rw-r--r--   0 mark       (501) staff       (20)      509 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/iot.py
+-rw-r--r--   0 mark       (501) staff       (20)      394 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/iot1click.py
+-rw-r--r--   0 mark       (501) staff       (20)      945 2023-08-13 20:05:24.000000 troposphere-4.8.0/troposphere/validators/iottwinmaker.py
+-rw-r--r--   0 mark       (501) staff       (20)      520 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/kinesis.py
+-rw-r--r--   0 mark       (501) staff       (20)      756 2022-12-09 19:28:46.000000 troposphere-4.8.0/troposphere/validators/kinesisanalyticsv2.py
+-rw-r--r--   0 mark       (501) staff       (20)      802 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/kms.py
+-rw-r--r--   0 mark       (501) staff       (20)      276 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/lex.py
+-rw-r--r--   0 mark       (501) staff       (20)     1454 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/logs.py
+-rw-r--r--   0 mark       (501) staff       (20)     1038 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/macie.py
+-rw-r--r--   0 mark       (501) staff       (20)      441 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/mediastore.py
+-rw-r--r--   0 mark       (501) staff       (20)      497 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/networkfirewall.py
+-rw-r--r--   0 mark       (501) staff       (20)      674 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/opensearchservice.py
+-rw-r--r--   0 mark       (501) staff       (20)     2080 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/opsworks.py
+-rw-r--r--   0 mark       (501) staff       (20)      245 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/opsworkscm.py
+-rw-r--r--   0 mark       (501) staff       (20)      481 2022-11-26 19:38:58.000000 troposphere-4.8.0/troposphere/validators/organizations.py
+-rw-r--r--   0 mark       (501) staff       (20)    15707 2024-02-14 23:39:39.000000 troposphere-4.8.0/troposphere/validators/rds.py
+-rw-r--r--   0 mark       (501) staff       (20)      759 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/rekognition.py
+-rw-r--r--   0 mark       (501) staff       (20)     1219 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/resiliencehub.py
+-rw-r--r--   0 mark       (501) staff       (20)      393 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/resourcegroups.py
+-rw-r--r--   0 mark       (501) staff       (20)      828 2023-01-28 20:33:37.000000 troposphere-4.8.0/troposphere/validators/route53.py
+-rw-r--r--   0 mark       (501) staff       (20)      434 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/route53resolver.py
+-rw-r--r--   0 mark       (501) staff       (20)     3538 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/s3.py
+-rw-r--r--   0 mark       (501) staff       (20)      858 2023-01-28 23:24:40.000000 troposphere-4.8.0/troposphere/validators/scheduler.py
+-rw-r--r--   0 mark       (501) staff       (20)      934 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/secretsmanager.py
+-rw-r--r--   0 mark       (501) staff       (20)      457 2023-10-22 17:53:55.000000 troposphere-4.8.0/troposphere/validators/servicecatalog.py
+-rw-r--r--   0 mark       (501) staff       (20)      281 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/sns.py
+-rw-r--r--   0 mark       (501) staff       (20)      732 2022-06-17 14:59:36.000000 troposphere-4.8.0/troposphere/validators/sqs.py
+-rw-r--r--   0 mark       (501) staff       (20)     3091 2022-07-22 22:21:38.000000 troposphere-4.8.0/troposphere/validators/ssm.py
+-rw-r--r--   0 mark       (501) staff       (20)      709 2024-04-25 15:54:48.000000 troposphere-4.8.0/troposphere/validators/synthetics.py
+-rw-r--r--   0 mark       (501) staff       (20)      563 2023-10-22 17:53:55.000000 troposphere-4.8.0/troposphere/validators/transfer.py
+-rw-r--r--   0 mark       (501) staff       (20)      264 2022-06-17 14:59:37.000000 troposphere-4.8.0/troposphere/validators/waf.py
+-rw-r--r--   0 mark       (501) staff       (20)      264 2022-06-17 14:59:37.000000 troposphere-4.8.0/troposphere/validators/wafregional.py
+-rw-r--r--   0 mark       (501) staff       (20)     4939 2023-08-13 20:05:24.000000 troposphere-4.8.0/troposphere/validators/wafv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     4930 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/verifiedpermissions.py
+-rw-r--r--   0 mark       (501) staff       (20)      966 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/voiceid.py
+-rw-r--r--   0 mark       (501) staff       (20)     9875 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/vpclattice.py
+-rw-r--r--   0 mark       (501) staff       (20)     5660 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/waf.py
+-rw-r--r--   0 mark       (501) staff       (20)     7671 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/wafregional.py
+-rw-r--r--   0 mark       (501) staff       (20)    32847 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/wafv2.py
+-rw-r--r--   0 mark       (501) staff       (20)     3317 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/wisdom.py
+-rw-r--r--   0 mark       (501) staff       (20)     1710 2024-04-29 18:22:39.000000 troposphere-4.8.0/troposphere/workspaces.py
+-rw-r--r--   0 mark       (501) staff       (20)     1448 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/workspacesthinclient.py
+-rw-r--r--   0 mark       (501) staff       (20)     5528 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/workspacesweb.py
+-rw-r--r--   0 mark       (501) staff       (20)     2442 2024-04-29 18:22:38.000000 troposphere-4.8.0/troposphere/xray.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-29 19:32:15.613107 troposphere-4.8.0/troposphere.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     9160 2024-04-29 19:32:15.000000 troposphere-4.8.0/troposphere.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)    13962 2024-04-29 19:32:15.000000 troposphere-4.8.0/troposphere.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2024-04-29 19:32:15.000000 troposphere-4.8.0/troposphere.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2021-03-27 20:52:43.000000 troposphere-4.8.0/troposphere.egg-info/not-zip-safe
+-rw-r--r--   0 mark       (501) staff       (20)       39 2024-04-29 19:32:15.000000 troposphere-4.8.0/troposphere.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       12 2024-04-29 19:32:15.000000 troposphere-4.8.0/troposphere.egg-info/top_level.txt
```

### Comparing `troposphere-4.7.0/.gitignore` & `troposphere-4.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/LICENSE` & `troposphere-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/PKG-INFO` & `troposphere-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troposphere
-Version: 4.7.0
+Version: 4.8.0
 Summary: AWS CloudFormation creation library
 Home-page: https://github.com/cloudtools/troposphere
 Author: Mark Peek
 Author-email: mark@peek.org
 License: New BSD license
 Project-URL: Changelog, https://github.com/cloudtools/troposphere/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/cloudtools/troposphere
```

### Comparing `troposphere-4.7.0/README.rst` & `troposphere-4.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ApiGateway.py` & `troposphere-4.8.0/examples/ApiGateway.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ApplicationAutoScalingSample.py` & `troposphere-4.8.0/examples/ApplicationAutoScalingSample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ApplicationELB.py` & `troposphere-4.8.0/examples/ApplicationELB.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ApplicationLB_FixedActions.py` & `troposphere-4.8.0/examples/ApplicationLB_FixedActions.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/AuroraServerlessRDS_SecretsManager.py` & `troposphere-4.8.0/examples/AuroraServerlessRDS_SecretsManager.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Autoscaling.py` & `troposphere-4.8.0/examples/Autoscaling.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/AutoscalingHTTPRequests.py` & `troposphere-4.8.0/examples/AutoscalingHTTPRequests.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Backup.py` & `troposphere-4.8.0/examples/Backup.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Batch.py` & `troposphere-4.8.0/examples/Batch.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/BatchEventSnsLambda.py` & `troposphere-4.8.0/examples/BatchEventSnsLambda.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ClassExtensions.py` & `troposphere-4.8.0/examples/ClassExtensions.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CloudFormation_Init_ConfigSet.py` & `troposphere-4.8.0/examples/CloudFormation_Init_ConfigSet.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CloudFront_Distribution_S3.py` & `troposphere-4.8.0/examples/CloudFront_Distribution_S3.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CloudFront_StreamingDistribution_S3.py` & `troposphere-4.8.0/examples/CloudFront_StreamingDistribution_S3.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CloudTrail.py` & `troposphere-4.8.0/examples/CloudTrail.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CloudWatchEventsSample.py` & `troposphere-4.8.0/examples/CloudWatchEventsSample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CodeBuild.py` & `troposphere-4.8.0/examples/CodeBuild.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CodeDeploy.py` & `troposphere-4.8.0/examples/CodeDeploy.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CodePipeline.py` & `troposphere-4.8.0/examples/CodePipeline.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/CustomResource.py` & `troposphere-4.8.0/examples/CustomResource.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Dlm.py` & `troposphere-4.8.0/examples/Dlm.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/DynamoDB_Table.py` & `troposphere-4.8.0/examples/DynamoDB_Table.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/DynamoDB_Table_With_GSI_And_NonKeyAttributes_Projection.py` & `troposphere-4.8.0/examples/DynamoDB_Table_With_GSI_And_NonKeyAttributes_Projection.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/DynamoDB_Table_With_GlobalSecondaryIndex.py` & `troposphere-4.8.0/examples/DynamoDB_Table_With_GlobalSecondaryIndex.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/DynamoDB_Table_With_KinesisStreamSpecification.py` & `troposphere-4.8.0/examples/DynamoDB_Table_With_KinesisStreamSpecification.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/DynamoDB_Tables_OnDemand.py` & `troposphere-4.8.0/examples/DynamoDB_Tables_OnDemand.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/EC2Conditions.py` & `troposphere-4.8.0/examples/EC2Conditions.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/EC2InstanceSample.py` & `troposphere-4.8.0/examples/EC2InstanceSample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/EC2_Remove_Ephemeral_Drive.py` & `troposphere-4.8.0/examples/EC2_Remove_Ephemeral_Drive.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ECRSample.py` & `troposphere-4.8.0/examples/ECRSample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ECSCluster.py` & `troposphere-4.8.0/examples/ECSCluster.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ECSFargate.py` & `troposphere-4.8.0/examples/ECSFargate.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/EFS.py` & `troposphere-4.8.0/examples/EFS.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ELBSample.py` & `troposphere-4.8.0/examples/ELBSample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/EMR_Cluster.py` & `troposphere-4.8.0/examples/EMR_Cluster.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ElastiCacheRedis.py` & `troposphere-4.8.0/examples/ElastiCacheRedis.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ElasticBeanstalk_Nodejs_Sample.py` & `troposphere-4.8.0/examples/ElasticBeanstalk_Nodejs_Sample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/ElasticsearchDomain.py` & `troposphere-4.8.0/examples/ElasticsearchDomain.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Firehose_with_Redshift.py` & `troposphere-4.8.0/examples/Firehose_with_Redshift.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/IAM_Policies_SNS_Publish_To_SQS.py` & `troposphere-4.8.0/examples/IAM_Policies_SNS_Publish_To_SQS.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/IAM_Roles_and_InstanceProfiles.py` & `troposphere-4.8.0/examples/IAM_Roles_and_InstanceProfiles.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/IAM_Users_Groups_and_Policies.py` & `troposphere-4.8.0/examples/IAM_Users_Groups_and_Policies.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/IAM_Users_snippet.py` & `troposphere-4.8.0/examples/IAM_Users_snippet.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/IoTAnalytics.py` & `troposphere-4.8.0/examples/IoTAnalytics.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/IoTSample.py` & `troposphere-4.8.0/examples/IoTSample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Lambda.py` & `troposphere-4.8.0/examples/Lambda.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Mediapackage.py` & `troposphere-4.8.0/examples/Mediapackage.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/MskCluster.py` & `troposphere-4.8.0/examples/MskCluster.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/NatGateway.py` & `troposphere-4.8.0/examples/NatGateway.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/NetworkLB.py` & `troposphere-4.8.0/examples/NetworkLB.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/OpenStack_AutoScaling.py` & `troposphere-4.8.0/examples/OpenStack_AutoScaling.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/OpenStack_Server.py` & `troposphere-4.8.0/examples/OpenStack_Server.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/OpsWorksSnippet.py` & `troposphere-4.8.0/examples/OpsWorksSnippet.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/RDS_Snapshot_On_Delete.py` & `troposphere-4.8.0/examples/RDS_Snapshot_On_Delete.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/RDS_VPC.py` & `troposphere-4.8.0/examples/RDS_VPC.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/RDS_with_DBParameterGroup.py` & `troposphere-4.8.0/examples/RDS_with_DBParameterGroup.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Redshift.py` & `troposphere-4.8.0/examples/Redshift.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/RedshiftClusterInVpc.py` & `troposphere-4.8.0/examples/RedshiftClusterInVpc.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/RedshiftServerless.py` & `troposphere-4.8.0/examples/RedshiftServerless.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Route53_A.py` & `troposphere-4.8.0/examples/Route53_A.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Route53_CNAME.py` & `troposphere-4.8.0/examples/Route53_CNAME.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Route53_RoundRobin.py` & `troposphere-4.8.0/examples/Route53_RoundRobin.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/S3_Bucket.py` & `troposphere-4.8.0/examples/S3_Bucket.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/S3_Bucket_With_AccelerateConfiguration.py` & `troposphere-4.8.0/examples/S3_Bucket_With_AccelerateConfiguration.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/S3_Bucket_With_Versioning_And_Lifecycle_Rules.py` & `troposphere-4.8.0/examples/S3_Bucket_With_Versioning_And_Lifecycle_Rules.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/S3_Website_Bucket_With_Retain_On_Delete.py` & `troposphere-4.8.0/examples/S3_Website_Bucket_With_Retain_On_Delete.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/SQSDLQ.py` & `troposphere-4.8.0/examples/SQSDLQ.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/SQSEncrypt.py` & `troposphere-4.8.0/examples/SQSEncrypt.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/SQS_With_CloudWatch_Alarms.py` & `troposphere-4.8.0/examples/SQS_With_CloudWatch_Alarms.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/SSMExample.py` & `troposphere-4.8.0/examples/SSMExample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Secretsmanager.py` & `troposphere-4.8.0/examples/Secretsmanager.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Secretsmanager_Rds.py` & `troposphere-4.8.0/examples/Secretsmanager_Rds.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Serverless_Api_Backend.py` & `troposphere-4.8.0/examples/Serverless_Api_Backend.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Serverless_Deployment_Preference.py` & `troposphere-4.8.0/examples/Serverless_Deployment_Preference.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/Serverless_S3_Processor.py` & `troposphere-4.8.0/examples/Serverless_S3_Processor.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/VPC_EC2_Instance_With_Multiple_Dynamic_IPAddresses.py` & `troposphere-4.8.0/examples/VPC_EC2_Instance_With_Multiple_Dynamic_IPAddresses.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/VPC_With_VPN_Connection.py` & `troposphere-4.8.0/examples/VPC_With_VPN_Connection.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/VPC_single_instance_in_subnet.py` & `troposphere-4.8.0/examples/VPC_single_instance_in_subnet.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/VpnEndpoint.py` & `troposphere-4.8.0/examples/VpnEndpoint.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/WAF_Common_Attacks_Sample.py` & `troposphere-4.8.0/examples/WAF_Common_Attacks_Sample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/WAF_Regional_Common_Attacks_Sample.py` & `troposphere-4.8.0/examples/WAF_Regional_Common_Attacks_Sample.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/examples/WaitObject.py` & `troposphere-4.8.0/examples/WaitObject.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/pyproject.toml` & `troposphere-4.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/scripts/cfn` & `troposphere-4.8.0/scripts/cfn`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/scripts/cfn2py` & `troposphere-4.8.0/scripts/cfn2py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/setup.cfg` & `troposphere-4.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_apigateway.py` & `troposphere-4.8.0/tests/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_apigatewayv2.py` & `troposphere-4.8.0/tests/test_apigatewayv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_appconfig.py` & `troposphere-4.8.0/tests/test_appconfig.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_appsync.py` & `troposphere-4.8.0/tests/test_appsync.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_asg.py` & `troposphere-4.8.0/tests/test_asg.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_awslambda.py` & `troposphere-4.8.0/tests/test_awslambda.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_basic.py` & `troposphere-4.8.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_cloudformation.py` & `troposphere-4.8.0/tests/test_cloudformation.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_cloudfront.py` & `troposphere-4.8.0/tests/test_cloudfront.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_cloudwatch.py` & `troposphere-4.8.0/tests/test_cloudwatch.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_codebuild.py` & `troposphere-4.8.0/tests/test_codebuild.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_codecommit.py` & `troposphere-4.8.0/tests/test_codecommit.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_config.py` & `troposphere-4.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_dict.py` & `troposphere-4.8.0/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_dlm.py` & `troposphere-4.8.0/tests/test_dlm.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_ec2.py` & `troposphere-4.8.0/tests/test_ec2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_ecs.py` & `troposphere-4.8.0/tests/test_ecs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_efs.py` & `troposphere-4.8.0/tests/test_efs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_eks.py` & `troposphere-4.8.0/tests/test_eks.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_elasticloadbalancerv2.py` & `troposphere-4.8.0/tests/test_elasticloadbalancerv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_emr.py` & `troposphere-4.8.0/tests/test_emr.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_examples.py` & `troposphere-4.8.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_examples_template_generator.py` & `troposphere-4.8.0/tests/test_examples_template_generator.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_findinmap.py` & `troposphere-4.8.0/tests/test_findinmap.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_fsx.py` & `troposphere-4.8.0/tests/test_fsx.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_guardduty.py` & `troposphere-4.8.0/tests/test_guardduty.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_int_type.py` & `troposphere-4.8.0/tests/test_int_type.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_iot1click.py` & `troposphere-4.8.0/tests/test_iot1click.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_iottwinmaker.py` & `troposphere-4.8.0/tests/test_iottwinmaker.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_language_extensions.py` & `troposphere-4.8.0/tests/test_language_extensions.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_logs.py` & `troposphere-4.8.0/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_mappings.py` & `troposphere-4.8.0/tests/test_mappings.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_networkfirewall.py` & `troposphere-4.8.0/tests/test_networkfirewall.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_opensearchservice.py` & `troposphere-4.8.0/tests/test_opensearchservice.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_opsworks.py` & `troposphere-4.8.0/tests/test_opsworks.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_parameters.py` & `troposphere-4.8.0/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_policies.py` & `troposphere-4.8.0/tests/test_policies.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_rds.py` & `troposphere-4.8.0/tests/test_rds.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_resiliencehub.py` & `troposphere-4.8.0/tests/test_resiliencehub.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_s3.py` & `troposphere-4.8.0/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_scheduler.py` & `troposphere-4.8.0/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_serverless.py` & `troposphere-4.8.0/tests/test_serverless.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_sqs.py` & `troposphere-4.8.0/tests/test_sqs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_ssm.py` & `troposphere-4.8.0/tests/test_ssm.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_stepfunctions.py` & `troposphere-4.8.0/tests/test_stepfunctions.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_tags.py` & `troposphere-4.8.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_template.py` & `troposphere-4.8.0/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_template_generator.py` & `troposphere-4.8.0/tests/test_template_generator.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_userdata.py` & `troposphere-4.8.0/tests/test_userdata.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_validators.py` & `troposphere-4.8.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_wafv2.py` & `troposphere-4.8.0/tests/test_wafv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/tests/test_yaml.py` & `troposphere-4.8.0/tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/__init__.py` & `troposphere-4.8.0/troposphere/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # We cannot `from .type_defs.compat import Final` here for now
     # https://github.com/microsoft/pyright/issues/4197
     if sys.version_info < (3, 8):
         from typing_extensions import Final
     else:
         from typing import Final
 
-__version__ = "4.7.0"
+__version__ = "4.8.0"
 
 # constants for DeletionPolicy and UpdateReplacePolicy
 Delete: Final = "Delete"
 Retain: Final = "Retain"
 RetainExceptOnCreate: Final = "RetainExceptOnCreate"
 Snapshot: Final = "Snapshot"
```

### Comparing `troposphere-4.7.0/troposphere/accessanalyzer.py` & `troposphere-4.8.0/troposphere/accessanalyzer.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/acmpca.py` & `troposphere-4.8.0/troposphere/acmpca.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/amazonmq.py` & `troposphere-4.8.0/troposphere/amazonmq.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/amplify.py` & `troposphere-4.8.0/troposphere/amplify.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,26 +123,14 @@
         "Framework": (str, False),
         "PullRequestEnvironmentName": (str, False),
         "Stage": (str, False),
         "Tags": (Tags, False),
     }
 
 
-class Certificate(AWSProperty):
-    """
-    `Certificate <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-amplify-domain-certificate.html>`__
-    """
-
-    props: PropsDictType = {
-        "CertificateArn": (str, False),
-        "CertificateType": (str, False),
-        "CertificateVerificationDNSRecord": (str, False),
-    }
-
-
 class CertificateSettings(AWSProperty):
     """
     `CertificateSettings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-amplify-domain-certificatesettings.html>`__
     """
 
     props: PropsDictType = {
         "CertificateType": (str, False),
@@ -168,14 +156,24 @@
 
     resource_type = "AWS::Amplify::Domain"
 
     props: PropsDictType = {
         "AppId": (str, True),
         "AutoSubDomainCreationPatterns": ([str], False),
         "AutoSubDomainIAMRole": (str, False),
-        "Certificate": (Certificate, False),
         "CertificateSettings": (CertificateSettings, False),
         "DomainName": (str, True),
         "EnableAutoSubDomain": (boolean, False),
         "SubDomainSettings": ([SubDomainSetting], True),
-        "UpdateStatus": (str, False),
+    }
+
+
+class Certificate(AWSProperty):
+    """
+    `Certificate <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-amplify-domain-certificate.html>`__
+    """
+
+    props: PropsDictType = {
+        "CertificateArn": (str, False),
+        "CertificateType": (str, False),
+        "CertificateVerificationDNSRecord": (str, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/analytics.py` & `troposphere-4.8.0/troposphere/analytics.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/apigateway.py` & `troposphere-4.8.0/troposphere/apigateway.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/apigatewayv2.py` & `troposphere-4.8.0/troposphere/apigatewayv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/appconfig.py` & `troposphere-4.8.0/troposphere/appconfig.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,27 +56,40 @@
         "RetrievalRoleArn": (str, False),
         "Tags": (Tags, False),
         "Type": (str, False),
         "Validators": ([Validators], False),
     }
 
 
+class DynamicExtensionParameters(AWSProperty):
+    """
+    `DynamicExtensionParameters <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-appconfig-deployment-dynamicextensionparameters.html>`__
+    """
+
+    props: PropsDictType = {
+        "ExtensionReference": (str, False),
+        "ParameterName": (str, False),
+        "ParameterValue": (str, False),
+    }
+
+
 class Deployment(AWSObject):
     """
     `Deployment <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-appconfig-deployment.html>`__
     """
 
     resource_type = "AWS::AppConfig::Deployment"
 
     props: PropsDictType = {
         "ApplicationId": (str, True),
         "ConfigurationProfileId": (str, True),
         "ConfigurationVersion": (str, True),
         "DeploymentStrategyId": (str, True),
         "Description": (str, False),
+        "DynamicExtensionParameters": ([DynamicExtensionParameters], False),
         "EnvironmentId": (str, True),
         "KmsKeyIdentifier": (str, False),
         "Tags": (Tags, False),
     }
 
 
 class DeploymentStrategy(AWSObject):
@@ -128,14 +141,15 @@
 class Parameter(AWSProperty):
     """
     `Parameter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-appconfig-extension-parameter.html>`__
     """
 
     props: PropsDictType = {
         "Description": (str, False),
+        "Dynamic": (boolean, False),
         "Required": (boolean, True),
     }
 
 
 class Extension(AWSObject):
     """
     `Extension <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-appconfig-extension.html>`__
```

### Comparing `troposphere-4.7.0/troposphere/appflow.py` & `troposphere-4.8.0/troposphere/appflow.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/appintegrations.py` & `troposphere-4.8.0/troposphere/appintegrations.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,52 @@
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, AWSProperty, PropsDictType, Tags
 
 
+class ExternalUrlConfig(AWSProperty):
+    """
+    `ExternalUrlConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-appintegrations-application-externalurlconfig.html>`__
+    """
+
+    props: PropsDictType = {
+        "AccessUrl": (str, True),
+        "ApprovedOrigins": ([str], False),
+    }
+
+
+class ApplicationSourceConfig(AWSProperty):
+    """
+    `ApplicationSourceConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-appintegrations-application-applicationsourceconfig.html>`__
+    """
+
+    props: PropsDictType = {
+        "ExternalUrlConfig": (ExternalUrlConfig, True),
+    }
+
+
+class Application(AWSObject):
+    """
+    `Application <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-appintegrations-application.html>`__
+    """
+
+    resource_type = "AWS::AppIntegrations::Application"
+
+    props: PropsDictType = {
+        "ApplicationSourceConfig": (ApplicationSourceConfig, True),
+        "Description": (str, True),
+        "Name": (str, True),
+        "Namespace": (str, False),
+        "Permissions": ([str], False),
+        "Tags": (Tags, False),
+    }
+
+
 class FileConfiguration(AWSProperty):
     """
     `FileConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-appintegrations-dataintegration-fileconfiguration.html>`__
     """
 
     props: PropsDictType = {
         "Filters": (dict, False),
```

### Comparing `troposphere-4.7.0/troposphere/applicationautoscaling.py` & `troposphere-4.8.0/troposphere/applicationautoscaling.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/applicationinsights.py` & `troposphere-4.8.0/troposphere/applicationinsights.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,14 +77,48 @@
         "LogGroupName": (str, False),
         "LogPath": (str, False),
         "LogType": (str, True),
         "PatternSet": (str, False),
     }
 
 
+class NetWeaverPrometheusExporter(AWSProperty):
+    """
+    `NetWeaverPrometheusExporter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-applicationinsights-application-netweaverprometheusexporter.html>`__
+    """
+
+    props: PropsDictType = {
+        "InstanceNumbers": ([str], True),
+        "PrometheusPort": (str, False),
+        "SAPSID": (str, True),
+    }
+
+
+class Process(AWSProperty):
+    """
+    `Process <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-applicationinsights-application-process.html>`__
+    """
+
+    props: PropsDictType = {
+        "AlarmMetrics": ([AlarmMetric], True),
+        "ProcessName": (str, True),
+    }
+
+
+class SQLServerPrometheusExporter(AWSProperty):
+    """
+    `SQLServerPrometheusExporter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-applicationinsights-application-sqlserverprometheusexporter.html>`__
+    """
+
+    props: PropsDictType = {
+        "PrometheusPort": (str, True),
+        "SQLSecretName": (str, True),
+    }
+
+
 class WindowsEvent(AWSProperty):
     """
     `WindowsEvent <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-applicationinsights-application-windowsevent.html>`__
     """
 
     props: PropsDictType = {
         "EventLevels": ([str], True),
@@ -102,26 +136,30 @@
     props: PropsDictType = {
         "AlarmMetrics": ([AlarmMetric], False),
         "Alarms": ([Alarm], False),
         "HAClusterPrometheusExporter": (HAClusterPrometheusExporter, False),
         "HANAPrometheusExporter": (HANAPrometheusExporter, False),
         "JMXPrometheusExporter": (JMXPrometheusExporter, False),
         "Logs": ([Log], False),
+        "NetWeaverPrometheusExporter": (NetWeaverPrometheusExporter, False),
+        "Processes": ([Process], False),
+        "SQLServerPrometheusExporter": (SQLServerPrometheusExporter, False),
         "WindowsEvents": ([WindowsEvent], False),
     }
 
 
 class SubComponentConfigurationDetails(AWSProperty):
     """
     `SubComponentConfigurationDetails <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-applicationinsights-application-subcomponentconfigurationdetails.html>`__
     """
 
     props: PropsDictType = {
         "AlarmMetrics": ([AlarmMetric], False),
         "Logs": ([Log], False),
+        "Processes": ([Process], False),
         "WindowsEvents": ([WindowsEvent], False),
     }
 
 
 class SubComponentTypeConfiguration(AWSProperty):
     """
     `SubComponentTypeConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-applicationinsights-application-subcomponenttypeconfiguration.html>`__
@@ -197,14 +235,15 @@
     """
     `Application <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-applicationinsights-application.html>`__
     """
 
     resource_type = "AWS::ApplicationInsights::Application"
 
     props: PropsDictType = {
+        "AttachMissingPermission": (boolean, False),
         "AutoConfigurationEnabled": (boolean, False),
         "CWEMonitorEnabled": (boolean, False),
         "ComponentMonitoringSettings": ([ComponentMonitoringSetting], False),
         "CustomComponents": ([CustomComponent], False),
         "GroupingType": (str, False),
         "LogPatternSets": ([LogPatternSet], False),
         "OpsCenterEnabled": (boolean, False),
```

### Comparing `troposphere-4.7.0/troposphere/appmesh.py` & `troposphere-4.8.0/troposphere/appmesh.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/apprunner.py` & `troposphere-4.8.0/troposphere/apprunner.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/appstream.py` & `troposphere-4.8.0/troposphere/appstream.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/appsync.py` & `troposphere-4.8.0/troposphere/appsync.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/aps.py` & `troposphere-4.8.0/troposphere/detective.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,49 +2,50 @@
 # All rights reserved.
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
-from . import AWSObject, AWSProperty, PropsDictType, Tags
+from . import AWSObject, PropsDictType, Tags
+from .validators import boolean
 
 
-class RuleGroupsNamespace(AWSObject):
+class Graph(AWSObject):
     """
-    `RuleGroupsNamespace <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-aps-rulegroupsnamespace.html>`__
+    `Graph <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-detective-graph.html>`__
     """
 
-    resource_type = "AWS::APS::RuleGroupsNamespace"
+    resource_type = "AWS::Detective::Graph"
 
     props: PropsDictType = {
-        "Data": (str, True),
-        "Name": (str, True),
+        "AutoEnableMembers": (boolean, False),
         "Tags": (Tags, False),
-        "Workspace": (str, True),
     }
 
 
-class LoggingConfiguration(AWSProperty):
+class MemberInvitation(AWSObject):
     """
-    `LoggingConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-aps-workspace-loggingconfiguration.html>`__
+    `MemberInvitation <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-detective-memberinvitation.html>`__
     """
 
+    resource_type = "AWS::Detective::MemberInvitation"
+
     props: PropsDictType = {
-        "LogGroupArn": (str, False),
+        "DisableEmailNotification": (boolean, False),
+        "GraphArn": (str, True),
+        "MemberEmailAddress": (str, True),
+        "MemberId": (str, True),
+        "Message": (str, False),
     }
 
 
-class Workspace(AWSObject):
+class OrganizationAdmin(AWSObject):
     """
-    `Workspace <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-aps-workspace.html>`__
+    `OrganizationAdmin <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-detective-organizationadmin.html>`__
     """
 
-    resource_type = "AWS::APS::Workspace"
+    resource_type = "AWS::Detective::OrganizationAdmin"
 
     props: PropsDictType = {
-        "AlertManagerDefinition": (str, False),
-        "Alias": (str, False),
-        "KmsKeyArn": (str, False),
-        "LoggingConfiguration": (LoggingConfiguration, False),
-        "Tags": (Tags, False),
+        "AccountId": (str, True),
     }
```

### Comparing `troposphere-4.7.0/troposphere/arczonalshift.py` & `troposphere-4.8.0/troposphere/arczonalshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     `ZonalAutoshiftConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-arczonalshift-zonalautoshiftconfiguration.html>`__
     """
 
     resource_type = "AWS::ARCZonalShift::ZonalAutoshiftConfiguration"
 
     props: PropsDictType = {
         "PracticeRunConfiguration": (PracticeRunConfiguration, False),
-        "ResourceIdentifier": (str, False),
+        "ResourceIdentifier": (str, True),
         "ZonalAutoshiftStatus": (str, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/ask.py` & `troposphere-4.8.0/troposphere/ask.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/athena.py` & `troposphere-4.8.0/troposphere/athena.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/auditmanager.py` & `troposphere-4.8.0/troposphere/auditmanager.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/autoscaling.py` & `troposphere-4.8.0/troposphere/autoscaling.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/autoscalingplans.py` & `troposphere-4.8.0/troposphere/autoscalingplans.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/awslambda.py` & `troposphere-4.8.0/troposphere/awslambda.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/b2bi.py` & `troposphere-4.8.0/troposphere/b2bi.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/backup.py` & `troposphere-4.8.0/troposphere/backup.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/backupgateway.py` & `troposphere-4.8.0/troposphere/backupgateway.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/batch.py` & `troposphere-4.8.0/troposphere/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,14 +440,15 @@
 
 class EksContainerSecurityContext(AWSProperty):
     """
     `EksContainerSecurityContext <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-batch-jobdefinition-ekscontainersecuritycontext.html>`__
     """
 
     props: PropsDictType = {
+        "AllowPrivilegeEscalation": (boolean, False),
         "Privileged": (boolean, False),
         "ReadOnlyRootFilesystem": (boolean, False),
         "RunAsGroup": (integer, False),
         "RunAsNonRoot": (boolean, False),
         "RunAsUser": (integer, False),
     }
 
@@ -523,14 +524,24 @@
         "EmptyDir": (EksEmptyDir, False),
         "HostPath": (EksHostPath, False),
         "Name": (str, True),
         "Secret": (EksSecret, False),
     }
 
 
+class ImagePullSecret(AWSProperty):
+    """
+    `ImagePullSecret <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-batch-jobdefinition-imagepullsecret.html>`__
+    """
+
+    props: PropsDictType = {
+        "Name": (str, True),
+    }
+
+
 class Metadata(AWSProperty):
     """
     `Metadata <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-batch-jobdefinition-podproperties-metadata.html>`__
     """
 
     props: PropsDictType = {
         "Labels": (dict, False),
@@ -542,14 +553,15 @@
     `PodProperties <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-batch-jobdefinition-podproperties.html>`__
     """
 
     props: PropsDictType = {
         "Containers": ([EksContainer], False),
         "DnsPolicy": (str, False),
         "HostNetwork": (boolean, False),
+        "ImagePullSecrets": ([ImagePullSecret], False),
         "InitContainers": ([EksContainer], False),
         "Metadata": (Metadata, False),
         "ServiceAccountName": (str, False),
         "ShareProcessNamespace": (boolean, False),
         "Volumes": ([EksVolume], False),
     }
 
@@ -654,24 +666,38 @@
 
     props: PropsDictType = {
         "ComputeEnvironment": (str, True),
         "Order": (integer, True),
     }
 
 
+class JobStateTimeLimitAction(AWSProperty):
+    """
+    `JobStateTimeLimitAction <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-batch-jobqueue-jobstatetimelimitaction.html>`__
+    """
+
+    props: PropsDictType = {
+        "Action": (str, True),
+        "MaxTimeSeconds": (integer, True),
+        "Reason": (str, True),
+        "State": (str, True),
+    }
+
+
 class JobQueue(AWSObject):
     """
     `JobQueue <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-batch-jobqueue.html>`__
     """
 
     resource_type = "AWS::Batch::JobQueue"
 
     props: PropsDictType = {
         "ComputeEnvironmentOrder": ([ComputeEnvironmentOrder], True),
         "JobQueueName": (str, False),
+        "JobStateTimeLimitActions": ([JobStateTimeLimitAction], False),
         "Priority": (integer, True),
         "SchedulingPolicyArn": (str, False),
         "State": (validate_queue_state, False),
         "Tags": (dict, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/billingconductor.py` & `troposphere-4.8.0/troposphere/billingconductor.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/budgets.py` & `troposphere-4.8.0/troposphere/budgets.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/cassandra.py` & `troposphere-4.8.0/troposphere/cassandra.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/ce.py` & `troposphere-4.8.0/troposphere/ce.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/certificatemanager.py` & `troposphere-4.8.0/troposphere/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/chatbot.py` & `troposphere-4.8.0/troposphere/chatbot.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/cleanrooms.py` & `troposphere-4.8.0/troposphere/cleanrooms.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, AWSProperty, PropsDictType, Tags
-from .validators import boolean, double
+from .validators import boolean, double, integer
 
 
 class AnalysisParameter(AWSProperty):
     """
     `AnalysisParameter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cleanrooms-analysistemplate-analysisparameter.html>`__
     """
 
@@ -151,22 +151,43 @@
         "JoinColumns": ([str], True),
         "JoinRequired": (str, False),
         "OutputConstraints": ([AggregationConstraint], True),
         "ScalarFunctions": ([str], True),
     }
 
 
+class DifferentialPrivacyColumn(AWSProperty):
+    """
+    `DifferentialPrivacyColumn <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cleanrooms-configuredtable-differentialprivacycolumn.html>`__
+    """
+
+    props: PropsDictType = {
+        "Name": (str, True),
+    }
+
+
+class DifferentialPrivacy(AWSProperty):
+    """
+    `DifferentialPrivacy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cleanrooms-configuredtable-differentialprivacy.html>`__
+    """
+
+    props: PropsDictType = {
+        "Columns": ([DifferentialPrivacyColumn], True),
+    }
+
+
 class AnalysisRuleCustom(AWSProperty):
     """
     `AnalysisRuleCustom <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cleanrooms-configuredtable-analysisrulecustom.html>`__
     """
 
     props: PropsDictType = {
         "AllowedAnalyses": ([str], True),
         "AllowedAnalysisProviders": ([str], False),
+        "DifferentialPrivacy": (DifferentialPrivacy, False),
     }
 
 
 class AnalysisRuleList(AWSProperty):
     """
     `AnalysisRuleList <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cleanrooms-configuredtable-analysisrulelist.html>`__
     """
@@ -335,14 +356,41 @@
         ),
         "PaymentConfiguration": (MembershipPaymentConfiguration, False),
         "QueryLogStatus": (str, True),
         "Tags": (Tags, False),
     }
 
 
+class Parameters(AWSProperty):
+    """
+    `Parameters <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cleanrooms-privacybudgettemplate-parameters.html>`__
+    """
+
+    props: PropsDictType = {
+        "Epsilon": (integer, True),
+        "UsersNoisePerQuery": (integer, True),
+    }
+
+
+class PrivacyBudgetTemplate(AWSObject):
+    """
+    `PrivacyBudgetTemplate <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-cleanrooms-privacybudgettemplate.html>`__
+    """
+
+    resource_type = "AWS::CleanRooms::PrivacyBudgetTemplate"
+
+    props: PropsDictType = {
+        "AutoRefresh": (str, True),
+        "MembershipIdentifier": (str, True),
+        "Parameters": (Parameters, True),
+        "PrivacyBudgetType": (str, True),
+        "Tags": (Tags, False),
+    }
+
+
 class AnalysisSchema(AWSProperty):
     """
     `AnalysisSchema <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cleanrooms-analysistemplate-analysisschema.html>`__
     """
 
     props: PropsDictType = {
         "ReferencedTables": ([str], True),
```

### Comparing `troposphere-4.7.0/troposphere/cloud9.py` & `troposphere-4.8.0/troposphere/cloud9.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/cloudformation.py` & `troposphere-4.8.0/troposphere/cloudformation.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/cloudfront.py` & `troposphere-4.8.0/troposphere/cloudfront.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/cloudtrail.py` & `troposphere-4.8.0/troposphere/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/cloudwatch.py` & `troposphere-4.8.0/troposphere/cloudwatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         "InsufficientDataActions": ([str], False),
         "MetricName": (str, False),
         "Metrics": ([MetricDataQuery], False),
         "Namespace": (str, False),
         "OKActions": ([str], False),
         "Period": (integer, False),
         "Statistic": (str, False),
+        "Tags": (Tags, False),
         "Threshold": (double, False),
         "ThresholdMetricId": (str, False),
         "TreatMissingData": (validate_treat_missing_data, False),
         "Unit": (str, False),
     }
 
     def validate(self):
@@ -122,14 +123,24 @@
 
     props: PropsDictType = {
         "ExcludedTimeRanges": ([Range], False),
         "MetricTimeZone": (str, False),
     }
 
 
+class MetricCharacteristics(AWSProperty):
+    """
+    `MetricCharacteristics <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cloudwatch-anomalydetector-metriccharacteristics.html>`__
+    """
+
+    props: PropsDictType = {
+        "PeriodicSpikes": (boolean, False),
+    }
+
+
 class MetricMathAnomalyDetector(AWSProperty):
     """
     `MetricMathAnomalyDetector <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cloudwatch-anomalydetector-metricmathanomalydetector.html>`__
     """
 
     props: PropsDictType = {
         "MetricDataQueries": ([MetricDataQuery], False),
@@ -138,14 +149,15 @@
 
 class SingleMetricAnomalyDetector(AWSProperty):
     """
     `SingleMetricAnomalyDetector <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cloudwatch-anomalydetector-singlemetricanomalydetector.html>`__
     """
 
     props: PropsDictType = {
+        "AccountId": (str, False),
         "Dimensions": ([MetricDimension], False),
         "MetricName": (str, False),
         "Namespace": (str, False),
         "Stat": (str, False),
     }
 
 
@@ -155,14 +167,15 @@
     """
 
     resource_type = "AWS::CloudWatch::AnomalyDetector"
 
     props: PropsDictType = {
         "Configuration": (Configuration, False),
         "Dimensions": ([MetricDimension], False),
+        "MetricCharacteristics": (MetricCharacteristics, False),
         "MetricMathAnomalyDetector": (MetricMathAnomalyDetector, False),
         "MetricName": (str, False),
         "Namespace": (str, False),
         "SingleMetricAnomalyDetector": (SingleMetricAnomalyDetector, False),
         "Stat": (str, False),
     }
 
@@ -181,14 +194,15 @@
         "ActionsSuppressorWaitPeriod": (integer, False),
         "AlarmActions": ([str], False),
         "AlarmDescription": (str, False),
         "AlarmName": (str, False),
         "AlarmRule": (str, True),
         "InsufficientDataActions": ([str], False),
         "OKActions": ([str], False),
+        "Tags": (Tags, False),
     }
 
 
 class Dashboard(AWSObject):
     """
     `Dashboard <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-cloudwatch-dashboard.html>`__
     """
```

### Comparing `troposphere-4.7.0/troposphere/codeartifact.py` & `troposphere-4.8.0/troposphere/eventschemas.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,42 +3,68 @@
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, PropsDictType, Tags
-from .validators.codeartifact import policytypes
+from .validators import boolean
 
 
-class Domain(AWSObject):
+class Discoverer(AWSObject):
     """
-    `Domain <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-codeartifact-domain.html>`__
+    `Discoverer <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eventschemas-discoverer.html>`__
     """
 
-    resource_type = "AWS::CodeArtifact::Domain"
+    resource_type = "AWS::EventSchemas::Discoverer"
 
     props: PropsDictType = {
-        "DomainName": (str, True),
-        "EncryptionKey": (str, False),
-        "PermissionsPolicyDocument": (policytypes, False),
+        "CrossAccount": (boolean, False),
+        "Description": (str, False),
+        "SourceArn": (str, True),
         "Tags": (Tags, False),
     }
 
 
-class Repository(AWSObject):
+class Registry(AWSObject):
+    """
+    `Registry <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eventschemas-registry.html>`__
+    """
+
+    resource_type = "AWS::EventSchemas::Registry"
+
+    props: PropsDictType = {
+        "Description": (str, False),
+        "RegistryName": (str, False),
+        "Tags": (Tags, False),
+    }
+
+
+class RegistryPolicy(AWSObject):
+    """
+    `RegistryPolicy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eventschemas-registrypolicy.html>`__
+    """
+
+    resource_type = "AWS::EventSchemas::RegistryPolicy"
+
+    props: PropsDictType = {
+        "Policy": (dict, True),
+        "RegistryName": (str, True),
+        "RevisionId": (str, False),
+    }
+
+
+class Schema(AWSObject):
     """
-    `Repository <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-codeartifact-repository.html>`__
+    `Schema <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eventschemas-schema.html>`__
     """
 
-    resource_type = "AWS::CodeArtifact::Repository"
+    resource_type = "AWS::EventSchemas::Schema"
 
     props: PropsDictType = {
+        "Content": (str, True),
         "Description": (str, False),
-        "DomainName": (str, True),
-        "DomainOwner": (str, False),
-        "ExternalConnections": ([str], False),
-        "PermissionsPolicyDocument": (policytypes, False),
-        "RepositoryName": (str, True),
+        "RegistryName": (str, True),
+        "SchemaName": (str, False),
         "Tags": (Tags, False),
-        "Upstreams": ([str], False),
+        "Type": (str, True),
     }
```

### Comparing `troposphere-4.7.0/troposphere/codebuild.py` & `troposphere-4.8.0/troposphere/codebuild.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/codecommit.py` & `troposphere-4.8.0/troposphere/codecommit.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/codedeploy.py` & `troposphere-4.8.0/troposphere/codedeploy.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/codeguruprofiler.py` & `troposphere-4.8.0/troposphere/codeguruprofiler.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/codegurureviewer.py` & `troposphere-4.8.0/troposphere/codegurureviewer.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/codepipeline.py` & `troposphere-4.8.0/troposphere/codepipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
         "InputArtifacts": ([InputArtifacts], False),
         "Name": (str, True),
         "Namespace": (str, False),
         "OutputArtifacts": ([OutputArtifacts], False),
         "Region": (str, False),
         "RoleArn": (str, False),
         "RunOrder": (integer, False),
+        "TimeoutInMinutes": (integer, False),
     }
 
 
 class Blockers(AWSProperty):
     """
     `Blockers <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-codepipeline-pipeline-stages-blockers.html>`__
     """
```

### Comparing `troposphere-4.7.0/troposphere/codestar.py` & `troposphere-4.8.0/troposphere/codestar.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/codestarconnections.py` & `troposphere-4.8.0/troposphere/codestarconnections.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,12 +47,14 @@
     """
 
     resource_type = "AWS::CodeStarConnections::SyncConfiguration"
 
     props: PropsDictType = {
         "Branch": (str, True),
         "ConfigFile": (str, True),
+        "PublishDeploymentStatus": (str, False),
         "RepositoryLinkId": (str, True),
         "ResourceName": (str, True),
         "RoleArn": (str, True),
         "SyncType": (str, True),
+        "TriggerResourceUpdateOn": (str, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/codestarnotifications.py` & `troposphere-4.8.0/troposphere/codestarnotifications.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/cognito.py` & `troposphere-4.8.0/troposphere/cognito.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/compat.py` & `troposphere-4.8.0/troposphere/compat.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/comprehend.py` & `troposphere-4.8.0/troposphere/comprehend.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/config.py` & `troposphere-4.8.0/troposphere/config.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/connect.py` & `troposphere-4.8.0/troposphere/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,24 +589,38 @@
 
     props: PropsDictType = {
         "InstanceId": (str, True),
         "Key": (str, True),
     }
 
 
+class Application(AWSProperty):
+    """
+    `Application <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-connect-securityprofile-application.html>`__
+    """
+
+    props: PropsDictType = {
+        "ApplicationPermissions": ([str], True),
+        "Namespace": (str, True),
+    }
+
+
 class SecurityProfile(AWSObject):
     """
     `SecurityProfile <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-connect-securityprofile.html>`__
     """
 
     resource_type = "AWS::Connect::SecurityProfile"
 
     props: PropsDictType = {
+        "AllowedAccessControlHierarchyGroupId": (str, False),
         "AllowedAccessControlTags": (Tags, False),
+        "Applications": ([Application], False),
         "Description": (str, False),
+        "HierarchyRestrictedResources": ([str], False),
         "InstanceArn": (str, True),
         "Permissions": ([str], False),
         "SecurityProfileName": (str, True),
         "TagRestrictedResources": ([str], False),
         "Tags": (Tags, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/connectcampaigns.py` & `troposphere-4.8.0/troposphere/connectcampaigns.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 class AnswerMachineDetectionConfig(AWSProperty):
     """
     `AnswerMachineDetectionConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-connectcampaigns-campaign-answermachinedetectionconfig.html>`__
     """
 
     props: PropsDictType = {
+        "AwaitAnswerMachinePrompt": (boolean, False),
         "EnableAnswerMachineDetection": (boolean, True),
     }
 
 
 class OutboundCallConfig(AWSProperty):
     """
     `OutboundCallConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-connectcampaigns-campaign-outboundcallconfig.html>`__
```

### Comparing `troposphere-4.7.0/troposphere/constants.py` & `troposphere-4.8.0/troposphere/constants.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/controltower.py` & `troposphere-4.8.0/troposphere/controltower.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/cur.py` & `troposphere-4.8.0/troposphere/cur.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/customerprofiles.py` & `troposphere-4.8.0/troposphere/customerprofiles.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/databrew.py` & `troposphere-4.8.0/troposphere/databrew.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/datapipeline.py` & `troposphere-4.8.0/troposphere/datapipeline.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/datasync.py` & `troposphere-4.8.0/troposphere/datasync.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,14 +399,49 @@
 
     props: PropsDictType = {
         "FilterType": (str, False),
         "Value": (str, False),
     }
 
 
+class ManifestConfigSourceS3(AWSProperty):
+    """
+    `ManifestConfigSourceS3 <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-manifestconfigsources3.html>`__
+    """
+
+    props: PropsDictType = {
+        "BucketAccessRoleArn": (str, False),
+        "ManifestObjectPath": (str, False),
+        "ManifestObjectVersionId": (str, False),
+        "S3BucketArn": (str, False),
+    }
+
+
+class Source(AWSProperty):
+    """
+    `Source <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-source.html>`__
+    """
+
+    props: PropsDictType = {
+        "S3": (ManifestConfigSourceS3, False),
+    }
+
+
+class ManifestConfig(AWSProperty):
+    """
+    `ManifestConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-manifestconfig.html>`__
+    """
+
+    props: PropsDictType = {
+        "Action": (str, False),
+        "Format": (str, False),
+        "Source": (Source, True),
+    }
+
+
 class Options(AWSProperty):
     """
     `Options <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-options.html>`__
     """
 
     props: PropsDictType = {
         "Atime": (str, False),
@@ -423,17 +458,17 @@
         "TaskQueueing": (str, False),
         "TransferMode": (str, False),
         "Uid": (str, False),
         "VerifyMode": (str, False),
     }
 
 
-class S3(AWSProperty):
+class TaskReportConfigDestinationS3(AWSProperty):
     """
-    `S3 <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-s3.html>`__
+    `TaskReportConfigDestinationS3 <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-taskreportconfigdestinations3.html>`__
     """
 
     props: PropsDictType = {
         "BucketAccessRoleArn": (str, False),
         "S3BucketArn": (str, False),
         "Subdirectory": (str, False),
     }
@@ -441,15 +476,15 @@
 
 class Destination(AWSProperty):
     """
     `Destination <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-destination.html>`__
     """
 
     props: PropsDictType = {
-        "S3": (S3, False),
+        "S3": (TaskReportConfigDestinationS3, False),
     }
 
 
 class Deleted(AWSProperty):
     """
     `Deleted <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-deleted.html>`__
     """
@@ -518,15 +553,16 @@
 
 class TaskSchedule(AWSProperty):
     """
     `TaskSchedule <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datasync-task-taskschedule.html>`__
     """
 
     props: PropsDictType = {
-        "ScheduleExpression": (str, True),
+        "ScheduleExpression": (str, False),
+        "Status": (str, False),
     }
 
 
 class Task(AWSObject):
     """
     `Task <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-datasync-task.html>`__
     """
@@ -534,14 +570,15 @@
     resource_type = "AWS::DataSync::Task"
 
     props: PropsDictType = {
         "CloudWatchLogGroupArn": (str, False),
         "DestinationLocationArn": (str, True),
         "Excludes": ([FilterRule], False),
         "Includes": ([FilterRule], False),
+        "ManifestConfig": (ManifestConfig, False),
         "Name": (str, False),
         "Options": (Options, False),
         "Schedule": (TaskSchedule, False),
         "SourceLocationArn": (str, True),
         "Tags": (Tags, False),
         "TaskReportConfig": (TaskReportConfig, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/datazone.py` & `troposphere-4.8.0/troposphere/datazone.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 class GlueRunConfigurationInput(AWSProperty):
     """
     `GlueRunConfigurationInput <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-datazone-datasource-gluerunconfigurationinput.html>`__
     """
 
     props: PropsDictType = {
+        "AutoImportDataQualityResult": (boolean, False),
         "DataAccessRole": (str, False),
         "RelationalFilterConfigurations": ([RelationalFilterConfiguration], True),
     }
 
 
 class RedshiftCredentialConfiguration(AWSProperty):
     """
```

### Comparing `troposphere-4.7.0/troposphere/dax.py` & `troposphere-4.8.0/troposphere/dax.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/detective.py` & `troposphere-4.8.0/troposphere/neptunegraph.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,50 +2,52 @@
 # All rights reserved.
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
-from . import AWSObject, PropsDictType, Tags
-from .validators import boolean
+from . import AWSObject, AWSProperty, PropsDictType, Tags
+from .validators import boolean, integer
 
 
-class Graph(AWSObject):
+class VectorSearchConfiguration(AWSProperty):
     """
-    `Graph <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-detective-graph.html>`__
+    `VectorSearchConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-neptunegraph-graph-vectorsearchconfiguration.html>`__
     """
 
-    resource_type = "AWS::Detective::Graph"
-
     props: PropsDictType = {
-        "AutoEnableMembers": (boolean, False),
-        "Tags": (Tags, False),
+        "VectorSearchDimension": (integer, True),
     }
 
 
-class MemberInvitation(AWSObject):
+class Graph(AWSObject):
     """
-    `MemberInvitation <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-detective-memberinvitation.html>`__
+    `Graph <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-neptunegraph-graph.html>`__
     """
 
-    resource_type = "AWS::Detective::MemberInvitation"
+    resource_type = "AWS::NeptuneGraph::Graph"
 
     props: PropsDictType = {
-        "DisableEmailNotification": (boolean, False),
-        "GraphArn": (str, True),
-        "MemberEmailAddress": (str, True),
-        "MemberId": (str, True),
-        "Message": (str, False),
+        "DeletionProtection": (boolean, False),
+        "GraphName": (str, False),
+        "ProvisionedMemory": (integer, True),
+        "PublicConnectivity": (boolean, False),
+        "ReplicaCount": (integer, False),
+        "Tags": (Tags, False),
+        "VectorSearchConfiguration": (VectorSearchConfiguration, False),
     }
 
 
-class OrganizationAdmin(AWSObject):
+class PrivateGraphEndpoint(AWSObject):
     """
-    `OrganizationAdmin <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-detective-organizationadmin.html>`__
+    `PrivateGraphEndpoint <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-neptunegraph-privategraphendpoint.html>`__
     """
 
-    resource_type = "AWS::Detective::OrganizationAdmin"
+    resource_type = "AWS::NeptuneGraph::PrivateGraphEndpoint"
 
     props: PropsDictType = {
-        "AccountId": (str, True),
+        "GraphIdentifier": (str, True),
+        "SecurityGroupIds": ([str], False),
+        "SubnetIds": ([str], False),
+        "VpcId": (str, True),
     }
```

### Comparing `troposphere-4.7.0/troposphere/devopsguru.py` & `troposphere-4.8.0/troposphere/devopsguru.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/directoryservice.py` & `troposphere-4.8.0/troposphere/directoryservice.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/dlm.py` & `troposphere-4.8.0/troposphere/dlm.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/dms.py` & `troposphere-4.8.0/troposphere/dms.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/docdb.py` & `troposphere-4.8.0/troposphere/docdb.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/docdbelastic.py` & `troposphere-4.8.0/troposphere/workspacesthinclient.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,31 +2,45 @@
 # All rights reserved.
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
-from . import AWSObject, PropsDictType, Tags
+from . import AWSObject, AWSProperty, PropsDictType, Tags
 from .validators import integer
 
 
-class Cluster(AWSObject):
+class MaintenanceWindow(AWSProperty):
     """
-    `Cluster <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-docdbelastic-cluster.html>`__
+    `MaintenanceWindow <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-workspacesthinclient-environment-maintenancewindow.html>`__
     """
 
-    resource_type = "AWS::DocDBElastic::Cluster"
+    props: PropsDictType = {
+        "ApplyTimeOf": (str, False),
+        "DaysOfTheWeek": ([str], False),
+        "EndTimeHour": (integer, False),
+        "EndTimeMinute": (integer, False),
+        "StartTimeHour": (integer, False),
+        "StartTimeMinute": (integer, False),
+        "Type": (str, True),
+    }
+
+
+class Environment(AWSObject):
+    """
+    `Environment <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-workspacesthinclient-environment.html>`__
+    """
+
+    resource_type = "AWS::WorkSpacesThinClient::Environment"
 
     props: PropsDictType = {
-        "AdminUserName": (str, True),
-        "AdminUserPassword": (str, False),
-        "AuthType": (str, True),
-        "ClusterName": (str, True),
-        "KmsKeyId": (str, False),
-        "PreferredMaintenanceWindow": (str, False),
-        "ShardCapacity": (integer, True),
-        "ShardCount": (integer, True),
-        "SubnetIds": ([str], False),
+        "DesiredSoftwareSetId": (str, False),
+        "DesktopArn": (str, True),
+        "DesktopEndpoint": (str, False),
+        "KmsKeyArn": (str, False),
+        "MaintenanceWindow": (MaintenanceWindow, False),
+        "Name": (str, False),
+        "SoftwareSetUpdateMode": (str, False),
+        "SoftwareSetUpdateSchedule": (str, False),
         "Tags": (Tags, False),
-        "VpcSecurityGroupIds": ([str], False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/dynamodb.py` & `troposphere-4.8.0/troposphere/dynamodb.py`

 * *Files 9% similar despite different names*

```diff
@@ -189,39 +189,62 @@
     """
 
     props: PropsDictType = {
         "KMSMasterKeyId": (str, True),
     }
 
 
+class ResourcePolicy(AWSProperty):
+    """
+    `ResourcePolicy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-dynamodb-table-resourcepolicy.html>`__
+    """
+
+    props: PropsDictType = {
+        "PolicyDocument": (dict, True),
+    }
+
+
+class ReplicaStreamSpecification(AWSProperty):
+    """
+    `ReplicaStreamSpecification <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-dynamodb-globaltable-replicastreamspecification.html>`__
+    """
+
+    props: PropsDictType = {
+        "ResourcePolicy": (ResourcePolicy, True),
+    }
+
+
 class ReplicaSpecification(AWSProperty):
     """
     `ReplicaSpecification <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-dynamodb-globaltable-replicaspecification.html>`__
     """
 
     props: PropsDictType = {
         "ContributorInsightsSpecification": (ContributorInsightsSpecification, False),
         "DeletionProtectionEnabled": (boolean, False),
         "GlobalSecondaryIndexes": ([ReplicaGlobalSecondaryIndexSpecification], False),
         "KinesisStreamSpecification": (KinesisStreamSpecification, False),
         "PointInTimeRecoverySpecification": (PointInTimeRecoverySpecification, False),
         "ReadProvisionedThroughputSettings": (ReadProvisionedThroughputSettings, False),
         "Region": (str, True),
+        "ReplicaStreamSpecification": (ReplicaStreamSpecification, False),
+        "ResourcePolicy": (ResourcePolicy, False),
         "SSESpecification": (ReplicaSSESpecification, False),
         "TableClass": (str, False),
         "Tags": (Tags, False),
     }
 
 
 class StreamSpecification(AWSProperty):
     """
     `StreamSpecification <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-dynamodb-table-streamspecification.html>`__
     """
 
     props: PropsDictType = {
+        "ResourcePolicy": (ResourcePolicy, False),
         "StreamViewType": (str, True),
     }
 
 
 class TimeToLiveSpecification(AWSProperty):
     """
     `TimeToLiveSpecification <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-dynamodb-table-timetolivespecification.html>`__
@@ -356,14 +379,15 @@
         "GlobalSecondaryIndexes": ([GlobalSecondaryIndex], False),
         "ImportSourceSpecification": (ImportSourceSpecification, False),
         "KeySchema": ([KeySchema], True),
         "KinesisStreamSpecification": (KinesisStreamSpecification, False),
         "LocalSecondaryIndexes": ([LocalSecondaryIndex], False),
         "PointInTimeRecoverySpecification": (PointInTimeRecoverySpecification, False),
         "ProvisionedThroughput": (ProvisionedThroughput, False),
+        "ResourcePolicy": (ResourcePolicy, False),
         "SSESpecification": (SSESpecification, False),
         "StreamSpecification": (StreamSpecification, False),
         "TableClass": (table_class_validator, False),
         "TableName": (str, False),
         "Tags": (Tags, False),
         "TimeToLiveSpecification": (TimeToLiveSpecification, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/ec2.py` & `troposphere-4.8.0/troposphere/ec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,16 @@
     """
     `CustomerGateway <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ec2-customergateway.html>`__
     """
 
     resource_type = "AWS::EC2::CustomerGateway"
 
     props: PropsDictType = {
-        "BgpAsn": (integer, True),
+        "BgpAsn": (integer, False),
+        "CertificateArn": (str, False),
         "DeviceName": (str, False),
         "IpAddress": (str, True),
         "Tags": (validate_tags_or_list, False),
         "Type": (str, True),
     }
 
 
@@ -293,14 +294,15 @@
     """
 
     resource_type = "AWS::EC2::DHCPOptions"
 
     props: PropsDictType = {
         "DomainName": (str, False),
         "DomainNameServers": ([str], False),
+        "Ipv6AddressPreferredLeaseTime": (integer, False),
         "NetbiosNameServers": ([str], False),
         "NetbiosNodeType": (integer, False),
         "NtpServers": ([str], False),
         "Tags": (validate_tags_or_list, False),
     }
 
 
@@ -879,15 +881,15 @@
         "VolumeSize": (integer, False),
         "VolumeType": (str, False),
     }
 
 
 class BlockDeviceMapping(AWSProperty):
     """
-    `BlockDeviceMapping <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-blockdev-mapping.html>`__
+    `BlockDeviceMapping <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-blockdevicemapping.html>`__
     """
 
     props: PropsDictType = {
         "DeviceName": (str, True),
         "Ebs": (EBSBlockDevice, False),
         "NoDevice": (dict, False),
         "VirtualName": (str, False),
@@ -998,15 +1000,15 @@
         "Primary": (boolean, False),
         "PrivateIpAddress": (str, True),
     }
 
 
 class NetworkInterfaceProperty(AWSProperty):
     """
-    `NetworkInterfaceProperty <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-network-iface-embedded.html>`__
+    `NetworkInterfaceProperty <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-networkinterface.html>`__
     """
 
     props: PropsDictType = {
         "AssociateCarrierIpAddress": (boolean, False),
         "AssociatePublicIpAddress": (boolean, False),
         "DeleteOnTermination": (boolean, False),
         "Description": (str, False),
@@ -1032,37 +1034,37 @@
         "EnableResourceNameDnsARecord": (boolean, False),
         "HostnameType": (str, False),
     }
 
 
 class AssociationParameters(AWSProperty):
     """
-    `AssociationParameters <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-ssmassociations-associationparameters.html>`__
+    `AssociationParameters <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-associationparameter.html>`__
     """
 
     props: PropsDictType = {
         "Key": (str, True),
         "Value": ([str], True),
     }
 
 
 class SsmAssociations(AWSProperty):
     """
-    `SsmAssociations <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-ssmassociations.html>`__
+    `SsmAssociations <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-ssmassociation.html>`__
     """
 
     props: PropsDictType = {
         "AssociationParameters": ([AssociationParameters], False),
         "DocumentName": (str, True),
     }
 
 
 class Instance(AWSObject):
     """
-    `Instance <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance.html>`__
+    `Instance <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ec2-instance.html>`__
     """
 
     resource_type = "AWS::EC2::Instance"
 
     props: PropsDictType = {
         "AdditionalInfo": (str, False),
         "Affinity": (str, False),
@@ -1378,15 +1380,14 @@
 class MaintenanceOptions(AWSProperty):
     """
     `MaintenanceOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-launchtemplate-maintenanceoptions.html>`__
     """
 
     props: PropsDictType = {
         "AutoRecovery": (str, False),
-        "RebootMigration": (str, False),
     }
 
 
 class MetadataOptions(AWSProperty):
     """
     `MetadataOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-launchtemplate-metadataoptions.html>`__
     """
@@ -1997,15 +1998,15 @@
         "Tags": (validate_tags_or_list, False),
         "VpcId": (str, True),
     }
 
 
 class SecurityGroup(AWSObject):
     """
-    `SecurityGroup <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-security-group.html>`__
+    `SecurityGroup <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ec2-securitygroup.html>`__
     """
 
     resource_type = "AWS::EC2::SecurityGroup"
 
     props: PropsDictType = {
         "GroupDescription": (str, True),
         "GroupName": (str, False),
@@ -2346,14 +2347,15 @@
 
     props: PropsDictType = {
         "AssignIpv6AddressOnCreation": (boolean, False),
         "AvailabilityZone": (str, False),
         "AvailabilityZoneId": (str, False),
         "CidrBlock": (str, False),
         "EnableDns64": (boolean, False),
+        "EnableLniAtDeviceIndex": (integer, False),
         "Ipv4IpamPoolId": (str, False),
         "Ipv4NetmaskLength": (integer, False),
         "Ipv6CidrBlock": (str, False),
         "Ipv6CidrBlocks": ([str], False),
         "Ipv6IpamPoolId": (str, False),
         "Ipv6Native": (boolean, False),
         "Ipv6NetmaskLength": (integer, False),
@@ -3193,15 +3195,15 @@
         "VolumeSize": (integer, False),
         "VolumeType": (str, False),
     }
 
 
 class Egress(AWSProperty):
     """
-    `Egress <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-security-group-rule.html>`__
+    `Egress <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-securitygroup-egress.html>`__
     """
 
     props: PropsDictType = {
         "CidrIp": (str, False),
         "CidrIpv6": (str, False),
         "Description": (str, False),
         "DestinationPrefixListId": (str, False),
@@ -3210,15 +3212,15 @@
         "IpProtocol": (str, True),
         "ToPort": (integer, False),
     }
 
 
 class Ingress(AWSProperty):
     """
-    `Ingress <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-security-group-rule.html>`__
+    `Ingress <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-securitygroup-ingress.html>`__
     """
 
     props: PropsDictType = {
         "CidrIp": (str, False),
         "CidrIpv6": (str, False),
         "Description": (str, False),
         "FromPort": (integer, False),
@@ -3229,45 +3231,37 @@
         "SourceSecurityGroupOwnerId": (str, False),
         "ToPort": (integer, False),
     }
 
 
 class MountPoint(AWSProperty):
     """
-    `MountPoint <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-mount-point.html>`__
+    `MountPoint <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-volume.html>`__
     """
 
     props: PropsDictType = {
         "Device": (str, True),
         "VolumeId": (str, True),
     }
 
 
-class NoDevice(AWSProperty):
-    """
-    `NoDevice <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-nodevice.html>`__
-    """
-
-    props: PropsDictType = {}
-
-
 class PeeringAttachmentStatus(AWSProperty):
     """
     `PeeringAttachmentStatus <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-transitgatewaypeeringattachment-peeringattachmentstatus.html>`__
     """
 
     props: PropsDictType = {
         "Code": (str, False),
         "Message": (str, False),
     }
 
 
 class SecurityGroupRule(AWSProperty):
     """
-    `SecurityGroupRule <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-security-group-rule.html>`__
+    `SecurityGroupRule <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-securitygroup-ingress.html>`__
     """
 
     props: PropsDictType = {
         "CidrIp": (str, False),
         "CidrIpv6": (str, False),
         "Description": (str, False),
         "DestinationPrefixListId": (str, False),
@@ -3296,14 +3290,14 @@
         "RouteOrigin": (str, False),
         "State": (str, False),
     }
 
 
 class VolumeProperty(AWSProperty):
     """
-    `VolumeProperty <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-mount-point.html>`__
+    `VolumeProperty <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance-volume.html>`__
     """
 
     props: PropsDictType = {
         "Device": (str, True),
         "VolumeId": (str, True),
     }
```

### Comparing `troposphere-4.7.0/troposphere/ecr.py` & `troposphere-4.8.0/troposphere/ecr.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     props: PropsDictType = {
         "ReplicationConfiguration": (ReplicationConfigurationProperty, True),
     }
 
 
 class EncryptionConfiguration(AWSProperty):
     """
-    `EncryptionConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecr-repository-encryptionconfiguration.html>`__
+    `EncryptionConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecr-repositorycreationtemplate-encryptionconfiguration.html>`__
     """
 
     props: PropsDictType = {
         "EncryptionType": (str, True),
         "KmsKey": (str, False),
     }
 
@@ -167,7 +167,26 @@
         "ImageScanningConfiguration": (ImageScanningConfiguration, False),
         "ImageTagMutability": (str, False),
         "LifecyclePolicy": (LifecyclePolicy, False),
         "RepositoryName": (str, False),
         "RepositoryPolicyText": (policytypes, False),
         "Tags": (Tags, False),
     }
+
+
+class RepositoryCreationTemplate(AWSObject):
+    """
+    `RepositoryCreationTemplate <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ecr-repositorycreationtemplate.html>`__
+    """
+
+    resource_type = "AWS::ECR::RepositoryCreationTemplate"
+
+    props: PropsDictType = {
+        "AppliedFor": ([str], True),
+        "Description": (str, False),
+        "EncryptionConfiguration": (EncryptionConfiguration, False),
+        "ImageTagMutability": (str, False),
+        "LifecyclePolicy": (str, False),
+        "Prefix": (str, True),
+        "RepositoryPolicy": (str, False),
+        "ResourceTags": (Tags, False),
+    }
```

### Comparing `troposphere-4.7.0/troposphere/ecs.py` & `troposphere-4.8.0/troposphere/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -818,14 +818,37 @@
         "FilesystemId": (str, True),
         "RootDirectory": (str, False),
         "TransitEncryption": (ecs_efs_encryption_status, False),
         "TransitEncryptionPort": (validate_transit_encryption_port, False),
     }
 
 
+class FSxAuthorizationConfig(AWSProperty):
+    """
+    `FSxAuthorizationConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecs-taskdefinition-fsxauthorizationconfig.html>`__
+    """
+
+    props: PropsDictType = {
+        "CredentialsParameter": (str, True),
+        "Domain": (str, True),
+    }
+
+
+class FSxWindowsFileServerVolumeConfiguration(AWSProperty):
+    """
+    `FSxWindowsFileServerVolumeConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecs-taskdefinition-fsxwindowsfileservervolumeconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "AuthorizationConfig": (FSxAuthorizationConfig, False),
+        "FileSystemId": (str, True),
+        "RootDirectory": (str, True),
+    }
+
+
 class Host(AWSProperty):
     """
     `Host <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecs-taskdefinition-hostvolumeproperties.html>`__
     """
 
     props: PropsDictType = {
         "SourcePath": (str, False),
@@ -837,14 +860,18 @@
     `Volume <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ecs-taskdefinition-volume.html>`__
     """
 
     props: PropsDictType = {
         "ConfiguredAtLaunch": (boolean, False),
         "DockerVolumeConfiguration": (DockerVolumeConfiguration, False),
         "EFSVolumeConfiguration": (EFSVolumeConfiguration, False),
+        "FSxWindowsFileServerVolumeConfiguration": (
+            FSxWindowsFileServerVolumeConfiguration,
+            False,
+        ),
         "Host": (Host, False),
         "Name": (str, False),
     }
 
 
 class TaskDefinition(AWSObject):
     """
```

### Comparing `troposphere-4.7.0/troposphere/efs.py` & `troposphere-4.8.0/troposphere/efs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/eks.py` & `troposphere-4.8.0/troposphere/eks.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/elasticache.py` & `troposphere-4.8.0/troposphere/elasticache.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,26 +265,28 @@
 
 class DataStorage(AWSProperty):
     """
     `DataStorage <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-elasticache-serverlesscache-datastorage.html>`__
     """
 
     props: PropsDictType = {
-        "Maximum": (integer, True),
+        "Maximum": (integer, False),
+        "Minimum": (integer, False),
         "Unit": (str, True),
     }
 
 
 class ECPUPerSecond(AWSProperty):
     """
     `ECPUPerSecond <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-elasticache-serverlesscache-ecpupersecond.html>`__
     """
 
     props: PropsDictType = {
-        "Maximum": (integer, True),
+        "Maximum": (integer, False),
+        "Minimum": (integer, False),
     }
 
 
 class CacheUsageLimits(AWSProperty):
     """
     `CacheUsageLimits <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-elasticache-serverlesscache-cacheusagelimits.html>`__
     """
```

### Comparing `troposphere-4.7.0/troposphere/elasticbeanstalk.py` & `troposphere-4.8.0/troposphere/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/elasticloadbalancing.py` & `troposphere-4.8.0/troposphere/elasticloadbalancing.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/elasticloadbalancingv2.py` & `troposphere-4.8.0/troposphere/elasticloadbalancingv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/elasticsearch.py` & `troposphere-4.8.0/troposphere/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/emr.py` & `troposphere-4.8.0/troposphere/emr.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/emrcontainers.py` & `troposphere-4.8.0/troposphere/emrcontainers.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/emrserverless.py` & `troposphere-4.8.0/troposphere/emrserverless.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/entityresolution.py` & `troposphere-4.8.0/troposphere/entityresolution.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 class IdMappingWorkflowInputSource(AWSProperty):
     """
     `IdMappingWorkflowInputSource <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-entityresolution-idmappingworkflow-idmappingworkflowinputsource.html>`__
     """
 
     props: PropsDictType = {
         "InputSourceARN": (str, True),
-        "SchemaArn": (str, True),
+        "SchemaArn": (str, False),
+        "Type": (str, False),
     }
 
 
 class IdMappingWorkflowOutputSource(AWSProperty):
     """
     `IdMappingWorkflowOutputSource <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-entityresolution-idmappingworkflow-idmappingworkflowoutputsource.html>`__
     """
@@ -72,21 +73,75 @@
 
     resource_type = "AWS::EntityResolution::IdMappingWorkflow"
 
     props: PropsDictType = {
         "Description": (str, False),
         "IdMappingTechniques": (IdMappingTechniques, True),
         "InputSourceConfig": ([IdMappingWorkflowInputSource], True),
-        "OutputSourceConfig": ([IdMappingWorkflowOutputSource], True),
+        "OutputSourceConfig": ([IdMappingWorkflowOutputSource], False),
         "RoleArn": (str, True),
         "Tags": (Tags, False),
         "WorkflowName": (str, True),
     }
 
 
+class NamespaceProviderProperties(AWSProperty):
+    """
+    `NamespaceProviderProperties <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-entityresolution-idnamespace-namespaceproviderproperties.html>`__
+    """
+
+    props: PropsDictType = {
+        "ProviderConfiguration": (dict, False),
+        "ProviderServiceArn": (str, True),
+    }
+
+
+class IdNamespaceIdMappingWorkflowProperties(AWSProperty):
+    """
+    `IdNamespaceIdMappingWorkflowProperties <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-entityresolution-idnamespace-idnamespaceidmappingworkflowproperties.html>`__
+    """
+
+    props: PropsDictType = {
+        "IdMappingType": (str, True),
+        "ProviderProperties": (NamespaceProviderProperties, False),
+    }
+
+
+class IdNamespaceInputSource(AWSProperty):
+    """
+    `IdNamespaceInputSource <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-entityresolution-idnamespace-idnamespaceinputsource.html>`__
+    """
+
+    props: PropsDictType = {
+        "InputSourceARN": (str, True),
+        "SchemaName": (str, False),
+    }
+
+
+class IdNamespace(AWSObject):
+    """
+    `IdNamespace <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-entityresolution-idnamespace.html>`__
+    """
+
+    resource_type = "AWS::EntityResolution::IdNamespace"
+
+    props: PropsDictType = {
+        "Description": (str, False),
+        "IdMappingWorkflowProperties": (
+            [IdNamespaceIdMappingWorkflowProperties],
+            False,
+        ),
+        "IdNamespaceName": (str, True),
+        "InputSourceConfig": ([IdNamespaceInputSource], False),
+        "RoleArn": (str, False),
+        "Tags": (Tags, False),
+        "Type": (str, True),
+    }
+
+
 class InputSource(AWSProperty):
     """
     `InputSource <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-entityresolution-matchingworkflow-inputsource.html>`__
     """
 
     props: PropsDictType = {
         "ApplyNormalization": (boolean, False),
@@ -167,14 +222,31 @@
         "ResolutionTechniques": (ResolutionTechniques, True),
         "RoleArn": (str, True),
         "Tags": (Tags, False),
         "WorkflowName": (str, True),
     }
 
 
+class PolicyStatement(AWSObject):
+    """
+    `PolicyStatement <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-entityresolution-policystatement.html>`__
+    """
+
+    resource_type = "AWS::EntityResolution::PolicyStatement"
+
+    props: PropsDictType = {
+        "Action": ([str], False),
+        "Arn": (str, True),
+        "Condition": (str, False),
+        "Effect": (str, False),
+        "Principal": ([str], False),
+        "StatementId": (str, True),
+    }
+
+
 class SchemaInputAttribute(AWSProperty):
     """
     `SchemaInputAttribute <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-entityresolution-schemamapping-schemainputattribute.html>`__
     """
 
     props: PropsDictType = {
         "FieldName": (str, True),
```

### Comparing `troposphere-4.7.0/troposphere/events.py` & `troposphere-4.8.0/troposphere/events.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/eventschemas.py` & `troposphere-4.8.0/troposphere/inspector.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,68 +3,49 @@
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, PropsDictType, Tags
-from .validators import boolean
+from .validators import integer
 
 
-class Discoverer(AWSObject):
+class AssessmentTarget(AWSObject):
     """
-    `Discoverer <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eventschemas-discoverer.html>`__
+    `AssessmentTarget <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-inspector-assessmenttarget.html>`__
     """
 
-    resource_type = "AWS::EventSchemas::Discoverer"
+    resource_type = "AWS::Inspector::AssessmentTarget"
 
     props: PropsDictType = {
-        "CrossAccount": (boolean, False),
-        "Description": (str, False),
-        "SourceArn": (str, True),
-        "Tags": (Tags, False),
+        "AssessmentTargetName": (str, False),
+        "ResourceGroupArn": (str, False),
     }
 
 
-class Registry(AWSObject):
+class AssessmentTemplate(AWSObject):
     """
-    `Registry <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eventschemas-registry.html>`__
+    `AssessmentTemplate <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-inspector-assessmenttemplate.html>`__
     """
 
-    resource_type = "AWS::EventSchemas::Registry"
+    resource_type = "AWS::Inspector::AssessmentTemplate"
 
     props: PropsDictType = {
-        "Description": (str, False),
-        "RegistryName": (str, False),
-        "Tags": (Tags, False),
+        "AssessmentTargetArn": (str, True),
+        "AssessmentTemplateName": (str, False),
+        "DurationInSeconds": (integer, True),
+        "RulesPackageArns": ([str], True),
+        "UserAttributesForFindings": (Tags, False),
     }
 
 
-class RegistryPolicy(AWSObject):
+class ResourceGroup(AWSObject):
     """
-    `RegistryPolicy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eventschemas-registrypolicy.html>`__
+    `ResourceGroup <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-inspector-resourcegroup.html>`__
     """
 
-    resource_type = "AWS::EventSchemas::RegistryPolicy"
+    resource_type = "AWS::Inspector::ResourceGroup"
 
     props: PropsDictType = {
-        "Policy": (dict, True),
-        "RegistryName": (str, True),
-        "RevisionId": (str, False),
-    }
-
-
-class Schema(AWSObject):
-    """
-    `Schema <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eventschemas-schema.html>`__
-    """
-
-    resource_type = "AWS::EventSchemas::Schema"
-
-    props: PropsDictType = {
-        "Content": (str, True),
-        "Description": (str, False),
-        "RegistryName": (str, True),
-        "SchemaName": (str, False),
-        "Tags": (Tags, False),
-        "Type": (str, True),
+        "ResourceGroupTags": (Tags, True),
     }
```

### Comparing `troposphere-4.7.0/troposphere/evidently.py` & `troposphere-4.8.0/troposphere/evidently.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/finspace.py` & `troposphere-4.8.0/troposphere/finspace.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/firehose.py` & `troposphere-4.8.0/troposphere/firehose.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/fis.py` & `troposphere-4.8.0/troposphere/fis.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/fms.py` & `troposphere-4.8.0/troposphere/fms.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/forecast.py` & `troposphere-4.8.0/troposphere/forecast.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/frauddetector.py` & `troposphere-4.8.0/troposphere/frauddetector.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/fsx.py` & `troposphere-4.8.0/troposphere/fsx.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/gamelift.py` & `troposphere-4.8.0/troposphere/gamelift.py`

 * *Files 20% similar despite different names*

```diff
@@ -61,14 +61,123 @@
         "OperatingSystem": (str, False),
         "ServerSdkVersion": (str, False),
         "StorageLocation": (StorageLocation, False),
         "Version": (str, False),
     }
 
 
+class ContainerDependency(AWSProperty):
+    """
+    `ContainerDependency <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-containergroupdefinition-containerdependency.html>`__
+    """
+
+    props: PropsDictType = {
+        "Condition": (str, True),
+        "ContainerName": (str, True),
+    }
+
+
+class ContainerEnvironment(AWSProperty):
+    """
+    `ContainerEnvironment <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-containergroupdefinition-containerenvironment.html>`__
+    """
+
+    props: PropsDictType = {
+        "Name": (str, True),
+        "Value": (str, True),
+    }
+
+
+class ContainerHealthCheck(AWSProperty):
+    """
+    `ContainerHealthCheck <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-containergroupdefinition-containerhealthcheck.html>`__
+    """
+
+    props: PropsDictType = {
+        "Command": ([str], True),
+        "Interval": (integer, False),
+        "Retries": (integer, False),
+        "StartPeriod": (integer, False),
+        "Timeout": (integer, False),
+    }
+
+
+class MemoryLimits(AWSProperty):
+    """
+    `MemoryLimits <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-containergroupdefinition-memorylimits.html>`__
+    """
+
+    props: PropsDictType = {
+        "HardLimit": (integer, False),
+        "SoftLimit": (integer, False),
+    }
+
+
+class ContainerPortRange(AWSProperty):
+    """
+    `ContainerPortRange <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-containergroupdefinition-containerportrange.html>`__
+    """
+
+    props: PropsDictType = {
+        "FromPort": (integer, True),
+        "Protocol": (str, True),
+        "ToPort": (integer, True),
+    }
+
+
+class PortConfiguration(AWSProperty):
+    """
+    `PortConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-containergroupdefinition-portconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "ContainerPortRanges": ([ContainerPortRange], True),
+    }
+
+
+class ContainerDefinition(AWSProperty):
+    """
+    `ContainerDefinition <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-containergroupdefinition-containerdefinition.html>`__
+    """
+
+    props: PropsDictType = {
+        "Command": ([str], False),
+        "ContainerName": (str, True),
+        "Cpu": (integer, False),
+        "DependsOn": ([ContainerDependency], False),
+        "EntryPoint": ([str], False),
+        "Environment": ([ContainerEnvironment], False),
+        "Essential": (boolean, False),
+        "HealthCheck": (ContainerHealthCheck, False),
+        "ImageUri": (str, True),
+        "MemoryLimits": (MemoryLimits, False),
+        "PortConfiguration": (PortConfiguration, False),
+        "ResolvedImageDigest": (str, False),
+        "WorkingDirectory": (str, False),
+    }
+
+
+class ContainerGroupDefinition(AWSObject):
+    """
+    `ContainerGroupDefinition <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-gamelift-containergroupdefinition.html>`__
+    """
+
+    resource_type = "AWS::GameLift::ContainerGroupDefinition"
+
+    props: PropsDictType = {
+        "ContainerDefinitions": ([ContainerDefinition], True),
+        "Name": (str, True),
+        "OperatingSystem": (str, True),
+        "SchedulingStrategy": (str, False),
+        "Tags": (Tags, False),
+        "TotalCpuLimit": (integer, True),
+        "TotalMemoryLimit": (integer, True),
+    }
+
+
 class AnywhereConfiguration(AWSProperty):
     """
     `AnywhereConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-fleet-anywhereconfiguration.html>`__
     """
 
     props: PropsDictType = {
         "Cost": (str, True),
@@ -81,14 +190,48 @@
     """
 
     props: PropsDictType = {
         "CertificateType": (str, True),
     }
 
 
+class ConnectionPortRange(AWSProperty):
+    """
+    `ConnectionPortRange <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-fleet-connectionportrange.html>`__
+    """
+
+    props: PropsDictType = {
+        "FromPort": (integer, True),
+        "ToPort": (integer, True),
+    }
+
+
+class ContainerGroupsPerInstance(AWSProperty):
+    """
+    `ContainerGroupsPerInstance <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-fleet-containergroupsperinstance.html>`__
+    """
+
+    props: PropsDictType = {
+        "DesiredReplicaContainerGroupsPerInstance": (integer, False),
+        "MaxReplicaContainerGroupsPerInstance": (integer, False),
+    }
+
+
+class ContainerGroupsConfiguration(AWSProperty):
+    """
+    `ContainerGroupsConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-fleet-containergroupsconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "ConnectionPortRange": (ConnectionPortRange, True),
+        "ContainerGroupDefinitionNames": ([str], True),
+        "ContainerGroupsPerInstance": (ContainerGroupsPerInstance, False),
+    }
+
+
 class IpPermission(AWSProperty):
     """
     `IpPermission <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-gamelift-fleet-ippermission.html>`__
     """
 
     props: PropsDictType = {
         "FromPort": (integer, True),
@@ -196,14 +339,15 @@
 
     props: PropsDictType = {
         "AnywhereConfiguration": (AnywhereConfiguration, False),
         "ApplyCapacity": (str, False),
         "BuildId": (str, False),
         "CertificateConfiguration": (CertificateConfiguration, False),
         "ComputeType": (str, False),
+        "ContainerGroupsConfiguration": (ContainerGroupsConfiguration, False),
         "Description": (str, False),
         "DesiredEC2Instances": (integer, False),
         "EC2InboundPermissions": ([IpPermission], False),
         "EC2InstanceType": (str, False),
         "FleetType": (str, False),
         "InstanceRoleARN": (str, False),
         "InstanceRoleCredentialsProvider": (str, False),
```

### Comparing `troposphere-4.7.0/troposphere/globalaccelerator.py` & `troposphere-4.8.0/troposphere/globalaccelerator.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,40 @@
         "IpAddressType": (accelerator_ipaddresstype, False),
         "IpAddresses": ([str], False),
         "Name": (str, True),
         "Tags": (Tags, False),
     }
 
 
+class Resource(AWSProperty):
+    """
+    `Resource <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-globalaccelerator-crossaccountattachment-resource.html>`__
+    """
+
+    props: PropsDictType = {
+        "EndpointId": (str, True),
+        "Region": (str, False),
+    }
+
+
+class CrossAccountAttachment(AWSObject):
+    """
+    `CrossAccountAttachment <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-globalaccelerator-crossaccountattachment.html>`__
+    """
+
+    resource_type = "AWS::GlobalAccelerator::CrossAccountAttachment"
+
+    props: PropsDictType = {
+        "Name": (str, True),
+        "Principals": ([str], False),
+        "Resources": ([Resource], False),
+        "Tags": (Tags, False),
+    }
+
+
 class EndpointConfiguration(AWSProperty):
     """
     `EndpointConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-globalaccelerator-endpointgroup-endpointconfiguration.html>`__
     """
 
     props: PropsDictType = {
         "AttachmentArn": (str, False),
```

### Comparing `troposphere-4.7.0/troposphere/glue.py` & `troposphere-4.8.0/troposphere/glue.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,25 @@
 
     props: PropsDictType = {
         "CatalogId": (str, True),
         "ConnectionInput": (ConnectionInput, True),
     }
 
 
+class LakeFormationConfiguration(AWSProperty):
+    """
+    `LakeFormationConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-glue-crawler-lakeformationconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "AccountId": (str, False),
+        "UseLakeFormationCredentials": (boolean, False),
+    }
+
+
 class RecrawlPolicy(AWSProperty):
     """
     `RecrawlPolicy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-glue-crawler-recrawlpolicy.html>`__
     """
 
     props: PropsDictType = {
         "RecrawlBehavior": (str, False),
@@ -271,14 +282,15 @@
 
     props: PropsDictType = {
         "Classifiers": ([str], False),
         "Configuration": (str, False),
         "CrawlerSecurityConfiguration": (str, False),
         "DatabaseName": (str, False),
         "Description": (str, False),
+        "LakeFormationConfiguration": (LakeFormationConfiguration, False),
         "Name": (str, False),
         "RecrawlPolicy": (RecrawlPolicy, False),
         "Role": (str, True),
         "Schedule": (Schedule, False),
         "SchemaChangePolicy": (SchemaChangePolicy, False),
         "TablePrefix": (str, False),
         "Tags": (dict, False),
```

### Comparing `troposphere-4.7.0/troposphere/grafana.py` & `troposphere-4.8.0/troposphere/grafana.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/greengrass.py` & `troposphere-4.8.0/troposphere/greengrass.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/greengrassv2.py` & `troposphere-4.8.0/troposphere/greengrassv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/groundstation.py` & `troposphere-4.8.0/troposphere/groundstation.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/guardduty.py` & `troposphere-4.8.0/troposphere/guardduty.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/healthimaging.py` & `troposphere-4.8.0/troposphere/healthimaging.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/healthlake.py` & `troposphere-4.8.0/troposphere/healthlake.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/helpers/userdata.py` & `troposphere-4.8.0/troposphere/helpers/userdata.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iam.py` & `troposphere-4.8.0/troposphere/iam.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/identitystore.py` & `troposphere-4.8.0/troposphere/identitystore.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/imagebuilder.py` & `troposphere-4.8.0/troposphere/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/inspector.py` & `troposphere-4.8.0/troposphere/kinesisvideo.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,46 +6,37 @@
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, PropsDictType, Tags
 from .validators import integer
 
 
-class AssessmentTarget(AWSObject):
+class SignalingChannel(AWSObject):
     """
-    `AssessmentTarget <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-inspector-assessmenttarget.html>`__
+    `SignalingChannel <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-kinesisvideo-signalingchannel.html>`__
     """
 
-    resource_type = "AWS::Inspector::AssessmentTarget"
+    resource_type = "AWS::KinesisVideo::SignalingChannel"
 
     props: PropsDictType = {
-        "AssessmentTargetName": (str, False),
-        "ResourceGroupArn": (str, False),
+        "MessageTtlSeconds": (integer, False),
+        "Name": (str, False),
+        "Tags": (Tags, False),
+        "Type": (str, False),
     }
 
 
-class AssessmentTemplate(AWSObject):
+class Stream(AWSObject):
     """
-    `AssessmentTemplate <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-inspector-assessmenttemplate.html>`__
+    `Stream <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-kinesisvideo-stream.html>`__
     """
 
-    resource_type = "AWS::Inspector::AssessmentTemplate"
+    resource_type = "AWS::KinesisVideo::Stream"
 
     props: PropsDictType = {
-        "AssessmentTargetArn": (str, True),
-        "AssessmentTemplateName": (str, False),
-        "DurationInSeconds": (integer, True),
-        "RulesPackageArns": ([str], True),
-        "UserAttributesForFindings": (Tags, False),
-    }
-
-
-class ResourceGroup(AWSObject):
-    """
-    `ResourceGroup <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-inspector-resourcegroup.html>`__
-    """
-
-    resource_type = "AWS::Inspector::ResourceGroup"
-
-    props: PropsDictType = {
-        "ResourceGroupTags": (Tags, True),
+        "DataRetentionInHours": (integer, False),
+        "DeviceName": (str, False),
+        "KmsKeyId": (str, False),
+        "MediaType": (str, False),
+        "Name": (str, False),
+        "Tags": (Tags, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/inspectorv2.py` & `troposphere-4.8.0/troposphere/inspectorv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/internetmonitor.py` & `troposphere-4.8.0/troposphere/internetmonitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, AWSProperty, PropsDictType, Tags
-from .validators import double, integer
+from .validators import boolean, double, integer
 
 
 class LocalHealthEventsConfig(AWSProperty):
     """
     `LocalHealthEventsConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-internetmonitor-monitor-localhealtheventsconfig.html>`__
     """
 
@@ -62,15 +62,17 @@
     `Monitor <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-internetmonitor-monitor.html>`__
     """
 
     resource_type = "AWS::InternetMonitor::Monitor"
 
     props: PropsDictType = {
         "HealthEventsConfig": (HealthEventsConfig, False),
+        "IncludeLinkedAccounts": (boolean, False),
         "InternetMeasurementsLogDelivery": (InternetMeasurementsLogDelivery, False),
+        "LinkedAccountId": (str, False),
         "MaxCityNetworksToMonitor": (integer, False),
         "MonitorName": (str, True),
         "Resources": ([str], False),
         "ResourcesToAdd": ([str], False),
         "ResourcesToRemove": ([str], False),
         "Status": (str, False),
         "Tags": (Tags, False),
```

### Comparing `troposphere-4.7.0/troposphere/iot.py` & `troposphere-4.8.0/troposphere/iot.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iot1click.py` & `troposphere-4.8.0/troposphere/iot1click.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iotanalytics.py` & `troposphere-4.8.0/troposphere/iotanalytics.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iotcoredeviceadvisor.py` & `troposphere-4.8.0/troposphere/iotcoredeviceadvisor.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iotevents.py` & `troposphere-4.8.0/troposphere/iotevents.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iotfleethub.py` & `troposphere-4.8.0/troposphere/iotfleethub.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iotfleetwise.py` & `troposphere-4.8.0/troposphere/iotfleetwise.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iotsitewise.py` & `troposphere-4.8.0/troposphere/iotsitewise.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,22 +357,33 @@
     """
 
     props: PropsDictType = {
         "CoreDeviceThingName": (str, True),
     }
 
 
+class SiemensIE(AWSProperty):
+    """
+    `SiemensIE <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-iotsitewise-gateway-siemensie.html>`__
+    """
+
+    props: PropsDictType = {
+        "IotCoreThingName": (str, True),
+    }
+
+
 class GatewayPlatform(AWSProperty):
     """
     `GatewayPlatform <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-iotsitewise-gateway-gatewayplatform.html>`__
     """
 
     props: PropsDictType = {
         "Greengrass": (Greengrass, False),
         "GreengrassV2": (GreengrassV2, False),
+        "SiemensIE": (SiemensIE, False),
     }
 
 
 class Gateway(AWSObject):
     """
     `Gateway <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-iotsitewise-gateway.html>`__
     """
```

### Comparing `troposphere-4.7.0/troposphere/iotthingsgraph.py` & `troposphere-4.8.0/troposphere/iotthingsgraph.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iottwinmaker.py` & `troposphere-4.8.0/troposphere/iottwinmaker.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/iotwireless.py` & `troposphere-4.8.0/troposphere/iotwireless.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/ivs.py` & `troposphere-4.8.0/troposphere/aps.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,128 +3,116 @@
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, AWSProperty, PropsDictType, Tags
-from .validators import boolean, integer
 
 
-class Channel(AWSObject):
+class RuleGroupsNamespace(AWSObject):
     """
-    `Channel <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ivs-channel.html>`__
+    `RuleGroupsNamespace <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-aps-rulegroupsnamespace.html>`__
     """
 
-    resource_type = "AWS::IVS::Channel"
+    resource_type = "AWS::APS::RuleGroupsNamespace"
 
     props: PropsDictType = {
-        "Authorized": (boolean, False),
-        "InsecureIngest": (boolean, False),
-        "LatencyMode": (str, False),
-        "Name": (str, False),
-        "Preset": (str, False),
-        "RecordingConfigurationArn": (str, False),
+        "Data": (str, True),
+        "Name": (str, True),
         "Tags": (Tags, False),
-        "Type": (str, False),
+        "Workspace": (str, True),
     }
 
 
-class PlaybackKeyPair(AWSObject):
+class AmpConfiguration(AWSProperty):
     """
-    `PlaybackKeyPair <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ivs-playbackkeypair.html>`__
+    `AmpConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-aps-scraper-ampconfiguration.html>`__
     """
 
-    resource_type = "AWS::IVS::PlaybackKeyPair"
-
     props: PropsDictType = {
-        "Name": (str, False),
-        "PublicKeyMaterial": (str, False),
-        "Tags": (Tags, False),
+        "WorkspaceArn": (str, True),
     }
 
 
-class S3DestinationConfiguration(AWSProperty):
+class Destination(AWSProperty):
     """
-    `S3DestinationConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ivs-recordingconfiguration-s3destinationconfiguration.html>`__
+    `Destination <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-aps-scraper-destination.html>`__
     """
 
     props: PropsDictType = {
-        "BucketName": (str, True),
+        "AmpConfiguration": (AmpConfiguration, True),
     }
 
 
-class DestinationConfiguration(AWSProperty):
+class ScrapeConfiguration(AWSProperty):
     """
-    `DestinationConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ivs-recordingconfiguration-destinationconfiguration.html>`__
+    `ScrapeConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-aps-scraper-scrapeconfiguration.html>`__
     """
 
     props: PropsDictType = {
-        "S3": (S3DestinationConfiguration, False),
+        "ConfigurationBlob": (str, True),
     }
 
 
-class RenditionConfiguration(AWSProperty):
+class EksConfiguration(AWSProperty):
     """
-    `RenditionConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ivs-recordingconfiguration-renditionconfiguration.html>`__
+    `EksConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-aps-scraper-eksconfiguration.html>`__
     """
 
     props: PropsDictType = {
-        "RenditionSelection": (str, False),
-        "Renditions": ([str], False),
+        "ClusterArn": (str, True),
+        "SecurityGroupIds": ([str], False),
+        "SubnetIds": ([str], True),
     }
 
 
-class ThumbnailConfiguration(AWSProperty):
+class Source(AWSProperty):
     """
-    `ThumbnailConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ivs-recordingconfiguration-thumbnailconfiguration.html>`__
+    `Source <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-aps-scraper-source.html>`__
     """
 
     props: PropsDictType = {
-        "RecordingMode": (str, False),
-        "Resolution": (str, False),
-        "Storage": ([str], False),
-        "TargetIntervalSeconds": (integer, False),
+        "EksConfiguration": (EksConfiguration, True),
     }
 
 
-class RecordingConfiguration(AWSObject):
+class Scraper(AWSObject):
     """
-    `RecordingConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ivs-recordingconfiguration.html>`__
+    `Scraper <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-aps-scraper.html>`__
     """
 
-    resource_type = "AWS::IVS::RecordingConfiguration"
+    resource_type = "AWS::APS::Scraper"
 
     props: PropsDictType = {
-        "DestinationConfiguration": (DestinationConfiguration, True),
-        "Name": (str, False),
-        "RecordingReconnectWindowSeconds": (integer, False),
-        "RenditionConfiguration": (RenditionConfiguration, False),
+        "Alias": (str, False),
+        "Destination": (Destination, True),
+        "ScrapeConfiguration": (ScrapeConfiguration, True),
+        "Source": (Source, True),
         "Tags": (Tags, False),
-        "ThumbnailConfiguration": (ThumbnailConfiguration, False),
     }
 
 
-class Stage(AWSObject):
+class LoggingConfiguration(AWSProperty):
     """
-    `Stage <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ivs-stage.html>`__
+    `LoggingConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-aps-workspace-loggingconfiguration.html>`__
     """
 
-    resource_type = "AWS::IVS::Stage"
-
     props: PropsDictType = {
-        "Name": (str, False),
-        "Tags": (Tags, False),
+        "LogGroupArn": (str, False),
     }
 
 
-class StreamKey(AWSObject):
+class Workspace(AWSObject):
     """
-    `StreamKey <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ivs-streamkey.html>`__
+    `Workspace <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-aps-workspace.html>`__
     """
 
-    resource_type = "AWS::IVS::StreamKey"
+    resource_type = "AWS::APS::Workspace"
 
     props: PropsDictType = {
-        "ChannelArn": (str, True),
+        "AlertManagerDefinition": (str, False),
+        "Alias": (str, False),
+        "KmsKeyArn": (str, False),
+        "LoggingConfiguration": (LoggingConfiguration, False),
         "Tags": (Tags, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/ivschat.py` & `troposphere-4.8.0/troposphere/ivschat.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/kafkaconnect.py` & `troposphere-4.8.0/troposphere/kafkaconnect.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All rights reserved.
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
-from . import AWSObject, AWSProperty, PropsDictType
+from . import AWSObject, AWSProperty, PropsDictType, Tags
 from .validators import boolean, integer
 
 
 class ScaleInPolicy(AWSProperty):
     """
     `ScaleInPolicy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-connector-scaleinpolicy.html>`__
     """
@@ -170,38 +170,38 @@
     """
 
     props: PropsDictType = {
         "WorkerLogDelivery": (WorkerLogDelivery, True),
     }
 
 
-class CustomPlugin(AWSProperty):
+class CustomPluginProperty(AWSProperty):
     """
-    `CustomPlugin <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-connector-customplugin.html>`__
+    `CustomPluginProperty <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-connector-customplugin.html>`__
     """
 
     props: PropsDictType = {
         "CustomPluginArn": (str, True),
         "Revision": (integer, True),
     }
 
 
 class Plugin(AWSProperty):
     """
     `Plugin <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-connector-plugin.html>`__
     """
 
     props: PropsDictType = {
-        "CustomPlugin": (CustomPlugin, True),
+        "CustomPlugin": (CustomPluginProperty, True),
     }
 
 
-class WorkerConfiguration(AWSProperty):
+class WorkerConfigurationProperty(AWSProperty):
     """
-    `WorkerConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-connector-workerconfiguration.html>`__
+    `WorkerConfigurationProperty <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-connector-workerconfiguration.html>`__
     """
 
     props: PropsDictType = {
         "Revision": (integer, True),
         "WorkerConfigurationArn": (str, True),
     }
 
@@ -221,9 +221,74 @@
         "KafkaCluster": (KafkaCluster, True),
         "KafkaClusterClientAuthentication": (KafkaClusterClientAuthentication, True),
         "KafkaClusterEncryptionInTransit": (KafkaClusterEncryptionInTransit, True),
         "KafkaConnectVersion": (str, True),
         "LogDelivery": (LogDelivery, False),
         "Plugins": ([Plugin], True),
         "ServiceExecutionRoleArn": (str, True),
-        "WorkerConfiguration": (WorkerConfiguration, False),
+        "Tags": (Tags, False),
+        "WorkerConfiguration": (WorkerConfigurationProperty, False),
+    }
+
+
+class S3Location(AWSProperty):
+    """
+    `S3Location <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-customplugin-s3location.html>`__
+    """
+
+    props: PropsDictType = {
+        "BucketArn": (str, True),
+        "FileKey": (str, True),
+        "ObjectVersion": (str, False),
+    }
+
+
+class CustomPluginLocation(AWSProperty):
+    """
+    `CustomPluginLocation <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-customplugin-custompluginlocation.html>`__
+    """
+
+    props: PropsDictType = {
+        "S3Location": (S3Location, True),
+    }
+
+
+class CustomPlugin(AWSObject):
+    """
+    `CustomPlugin <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-kafkaconnect-customplugin.html>`__
+    """
+
+    resource_type = "AWS::KafkaConnect::CustomPlugin"
+
+    props: PropsDictType = {
+        "ContentType": (str, True),
+        "Description": (str, False),
+        "Location": (CustomPluginLocation, True),
+        "Name": (str, True),
+        "Tags": (Tags, False),
+    }
+
+
+class WorkerConfiguration(AWSObject):
+    """
+    `WorkerConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-kafkaconnect-workerconfiguration.html>`__
+    """
+
+    resource_type = "AWS::KafkaConnect::WorkerConfiguration"
+
+    props: PropsDictType = {
+        "Description": (str, False),
+        "Name": (str, True),
+        "PropertiesFileContent": (str, True),
+        "Tags": (Tags, False),
+    }
+
+
+class CustomPluginFileDescription(AWSProperty):
+    """
+    `CustomPluginFileDescription <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-kafkaconnect-customplugin-custompluginfiledescription.html>`__
+    """
+
+    props: PropsDictType = {
+        "FileMd5": (str, False),
+        "FileSize": (integer, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/kendra.py` & `troposphere-4.8.0/troposphere/kendra.py`

 * *Files 0% similar despite different names*

```diff
@@ -697,14 +697,15 @@
 
     resource_type = "AWS::Kendra::Faq"
 
     props: PropsDictType = {
         "Description": (str, False),
         "FileFormat": (str, False),
         "IndexId": (str, True),
+        "LanguageCode": (str, False),
         "Name": (str, True),
         "RoleArn": (str, True),
         "S3Path": (S3Path, True),
         "Tags": (Tags, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/kendraranking.py` & `troposphere-4.8.0/troposphere/kendraranking.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/kinesis.py` & `troposphere-4.8.0/troposphere/kinesis.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/kinesisanalyticsv2.py` & `troposphere-4.8.0/troposphere/kinesisanalyticsv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/kinesisvideo.py` & `troposphere-4.8.0/troposphere/systemsmanagersap.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,41 +2,38 @@
 # All rights reserved.
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
-from . import AWSObject, PropsDictType, Tags
-from .validators import integer
+from . import AWSObject, AWSProperty, PropsDictType, Tags
 
 
-class SignalingChannel(AWSObject):
+class Credential(AWSProperty):
     """
-    `SignalingChannel <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-kinesisvideo-signalingchannel.html>`__
+    `Credential <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-systemsmanagersap-application-credential.html>`__
     """
 
-    resource_type = "AWS::KinesisVideo::SignalingChannel"
-
     props: PropsDictType = {
-        "MessageTtlSeconds": (integer, False),
-        "Name": (str, False),
-        "Tags": (Tags, False),
-        "Type": (str, False),
+        "CredentialType": (str, False),
+        "DatabaseName": (str, False),
+        "SecretId": (str, False),
     }
 
 
-class Stream(AWSObject):
+class Application(AWSObject):
     """
-    `Stream <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-kinesisvideo-stream.html>`__
+    `Application <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-systemsmanagersap-application.html>`__
     """
 
-    resource_type = "AWS::KinesisVideo::Stream"
+    resource_type = "AWS::SystemsManagerSAP::Application"
 
     props: PropsDictType = {
-        "DataRetentionInHours": (integer, False),
-        "DeviceName": (str, False),
-        "KmsKeyId": (str, False),
-        "MediaType": (str, False),
-        "Name": (str, False),
+        "ApplicationId": (str, True),
+        "ApplicationType": (str, True),
+        "Credentials": ([Credential], False),
+        "Instances": ([str], False),
+        "SapInstanceNumber": (str, False),
+        "Sid": (str, False),
         "Tags": (Tags, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/kms.py` & `troposphere-4.8.0/troposphere/kms.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         "Enabled": (boolean, False),
         "KeyPolicy": (policytypes, False),
         "KeySpec": (str, False),
         "KeyUsage": (key_usage_type, False),
         "MultiRegion": (boolean, False),
         "Origin": (str, False),
         "PendingWindowInDays": (validate_pending_window_in_days, False),
+        "RotationPeriodInDays": (integer, False),
         "Tags": (validate_tags_or_list, False),
     }
 
 
 class ReplicaKey(AWSObject):
     """
     `ReplicaKey <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-kms-replicakey.html>`__
```

### Comparing `troposphere-4.7.0/troposphere/lakeformation.py` & `troposphere-4.8.0/troposphere/lakeformation.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/lex.py` & `troposphere-4.8.0/troposphere/lex.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/licensemanager.py` & `troposphere-4.8.0/troposphere/licensemanager.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/lightsail.py` & `troposphere-4.8.0/troposphere/lightsail.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/location.py` & `troposphere-4.8.0/troposphere/location.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/logs.py` & `troposphere-4.8.0/troposphere/logs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/lookoutequipment.py` & `troposphere-4.8.0/troposphere/lookoutequipment.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/lookoutmetrics.py` & `troposphere-4.8.0/troposphere/lookoutmetrics.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/m2.py` & `troposphere-4.8.0/troposphere/m2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/macie.py` & `troposphere-4.8.0/troposphere/macie.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/managedblockchain.py` & `troposphere-4.8.0/troposphere/managedblockchain.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/mediaconnect.py` & `troposphere-4.8.0/troposphere/mediaconnect.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/mediaconvert.py` & `troposphere-4.8.0/troposphere/mediaconvert.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/medialive.py` & `troposphere-4.8.0/troposphere/medialive.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,20 +242,22 @@
 
 class AudioDescription(AWSProperty):
     """
     `AudioDescription <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-audiodescription.html>`__
     """
 
     props: PropsDictType = {
+        "AudioDashRoles": ([str], False),
         "AudioNormalizationSettings": (AudioNormalizationSettings, False),
         "AudioSelectorName": (str, False),
         "AudioType": (str, False),
         "AudioTypeControl": (str, False),
         "AudioWatermarkingSettings": (AudioWatermarkSettings, False),
         "CodecSettings": (AudioCodecSettings, False),
+        "DvbDashAccessibility": (str, False),
         "LanguageCode": (str, False),
         "LanguageCodeControl": (str, False),
         "Name": (str, False),
         "RemixSettings": (RemixSettings, False),
         "StreamName": (str, False),
     }
 
@@ -541,16 +543,18 @@
 class CaptionDescription(AWSProperty):
     """
     `CaptionDescription <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-captiondescription.html>`__
     """
 
     props: PropsDictType = {
         "Accessibility": (str, False),
+        "CaptionDashRoles": ([str], False),
         "CaptionSelectorName": (str, False),
         "DestinationSettings": (CaptionDestinationSettings, False),
+        "DvbDashAccessibility": (str, False),
         "LanguageCode": (str, False),
         "LanguageDescription": (str, False),
         "Name": (str, False),
     }
 
 
 class ColorCorrection(AWSProperty):
@@ -805,14 +809,24 @@
     props: PropsDictType = {
         "ContainerSettings": (ArchiveContainerSettings, False),
         "Extension": (str, False),
         "NameModifier": (str, False),
     }
 
 
+class CmafIngestOutputSettings(AWSProperty):
+    """
+    `CmafIngestOutputSettings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-cmafingestoutputsettings.html>`__
+    """
+
+    props: PropsDictType = {
+        "NameModifier": (str, False),
+    }
+
+
 class FrameCaptureOutputSettings(AWSProperty):
     """
     `FrameCaptureOutputSettings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-framecaptureoutputsettings.html>`__
     """
 
     props: PropsDictType = {
         "NameModifier": (str, False),
@@ -1007,14 +1021,15 @@
 class OutputSettings(AWSProperty):
     """
     `OutputSettings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-outputsettings.html>`__
     """
 
     props: PropsDictType = {
         "ArchiveOutputSettings": (ArchiveOutputSettings, False),
+        "CmafIngestOutputSettings": (CmafIngestOutputSettings, False),
         "FrameCaptureOutputSettings": (FrameCaptureOutputSettings, False),
         "HlsOutputSettings": (HlsOutputSettings, False),
         "MediaPackageOutputSettings": (MediaPackageOutputSettings, False),
         "MsSmoothOutputSettings": (MsSmoothOutputSettings, False),
         "MultiplexOutputSettings": (MultiplexOutputSettings, False),
         "RtmpOutputSettings": (RtmpOutputSettings, False),
         "UdpOutputSettings": (UdpOutputSettings, False),
@@ -1063,14 +1078,29 @@
     props: PropsDictType = {
         "ArchiveCdnSettings": (ArchiveCdnSettings, False),
         "Destination": (OutputLocationRef, False),
         "RolloverInterval": (integer, False),
     }
 
 
+class CmafIngestGroupSettings(AWSProperty):
+    """
+    `CmafIngestGroupSettings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-cmafingestgroupsettings.html>`__
+    """
+
+    props: PropsDictType = {
+        "Destination": (OutputLocationRef, False),
+        "NielsenId3Behavior": (str, False),
+        "Scte35Type": (str, False),
+        "SegmentLength": (integer, False),
+        "SegmentLengthUnits": (str, False),
+        "SendDelayMs": (integer, False),
+    }
+
+
 class FrameCaptureS3Settings(AWSProperty):
     """
     `FrameCaptureS3Settings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-framecaptures3settings.html>`__
     """
 
     props: PropsDictType = {
         "CannedAcl": (str, False),
@@ -1342,14 +1372,15 @@
 class OutputGroupSettings(AWSProperty):
     """
     `OutputGroupSettings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-outputgroupsettings.html>`__
     """
 
     props: PropsDictType = {
         "ArchiveGroupSettings": (ArchiveGroupSettings, False),
+        "CmafIngestGroupSettings": (CmafIngestGroupSettings, False),
         "FrameCaptureGroupSettings": (FrameCaptureGroupSettings, False),
         "HlsGroupSettings": (HlsGroupSettings, False),
         "MediaPackageGroupSettings": (MediaPackageGroupSettings, False),
         "MsSmoothGroupSettings": (MsSmoothGroupSettings, False),
         "MultiplexGroupSettings": (MultiplexGroupSettings, False),
         "RtmpGroupSettings": (RtmpGroupSettings, False),
         "UdpGroupSettings": (UdpGroupSettings, False),
@@ -1585,25 +1616,31 @@
         "GopClosedCadence": (integer, False),
         "GopSize": (double, False),
         "GopSizeUnits": (str, False),
         "Level": (str, False),
         "LookAheadRateControl": (str, False),
         "MaxBitrate": (integer, False),
         "MinIInterval": (integer, False),
+        "MvOverPictureBoundaries": (str, False),
+        "MvTemporalPredictor": (str, False),
         "ParDenominator": (integer, False),
         "ParNumerator": (integer, False),
         "Profile": (str, False),
         "QvbrQualityLevel": (integer, False),
         "RateControlMode": (str, False),
         "ScanType": (str, False),
         "SceneChangeDetect": (str, False),
         "Slices": (integer, False),
         "Tier": (str, False),
+        "TileHeight": (integer, False),
+        "TilePadding": (str, False),
+        "TileWidth": (integer, False),
         "TimecodeBurninSettings": (TimecodeBurninSettings, False),
         "TimecodeInsertion": (str, False),
+        "TreeblockSize": (str, False),
     }
 
 
 class Mpeg2FilterSettings(AWSProperty):
     """
     `Mpeg2FilterSettings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-medialive-channel-mpeg2filtersettings.html>`__
     """
```

### Comparing `troposphere-4.7.0/troposphere/mediapackage.py` & `troposphere-4.8.0/troposphere/mediapackage.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/mediapackagev2.py` & `troposphere-4.8.0/troposphere/mediapackagev2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/mediastore.py` & `troposphere-4.8.0/troposphere/mediastore.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/mediatailor.py` & `troposphere-4.8.0/troposphere/mediatailor.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     """
     `Channel <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mediatailor-channel.html>`__
     """
 
     resource_type = "AWS::MediaTailor::Channel"
 
     props: PropsDictType = {
+        "Audiences": ([str], False),
         "ChannelName": (str, True),
         "FillerSlate": (SlateSource, False),
         "LogConfiguration": (LogConfigurationForChannel, False),
         "Outputs": ([RequestOutputItem], True),
         "PlaybackMode": (str, True),
         "Tags": (Tags, False),
         "Tier": (str, False),
```

### Comparing `troposphere-4.7.0/troposphere/memorydb.py` & `troposphere-4.8.0/troposphere/memorydb.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/msk.py` & `troposphere-4.8.0/troposphere/msk.py`

 * *Files 3% similar despite different names*

```diff
@@ -463,23 +463,34 @@
         "ConsumerGroupsToExclude": ([str], False),
         "ConsumerGroupsToReplicate": ([str], True),
         "DetectAndCopyNewConsumerGroups": (boolean, False),
         "SynchroniseConsumerGroupOffsets": (boolean, False),
     }
 
 
+class ReplicationStartingPosition(AWSProperty):
+    """
+    `ReplicationStartingPosition <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-msk-replicator-replicationstartingposition.html>`__
+    """
+
+    props: PropsDictType = {
+        "Type": (str, False),
+    }
+
+
 class TopicReplication(AWSProperty):
     """
     `TopicReplication <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-msk-replicator-topicreplication.html>`__
     """
 
     props: PropsDictType = {
         "CopyAccessControlListsForTopics": (boolean, False),
         "CopyTopicConfigurations": (boolean, False),
         "DetectAndCopyNewTopics": (boolean, False),
+        "StartingPosition": (ReplicationStartingPosition, False),
         "TopicsToExclude": ([str], False),
         "TopicsToReplicate": ([str], True),
     }
 
 
 class ReplicationInfo(AWSProperty):
     """
```

### Comparing `troposphere-4.7.0/troposphere/mwaa.py` & `troposphere-4.8.0/troposphere/mwaa.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/neptune.py` & `troposphere-4.8.0/troposphere/neptune.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/neptunegraph.py` & `troposphere-4.8.0/troposphere/signer.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,51 +3,49 @@
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, AWSProperty, PropsDictType, Tags
-from .validators import boolean, integer
+from .validators import integer
 
 
-class VectorSearchConfiguration(AWSProperty):
+class ProfilePermission(AWSObject):
     """
-    `VectorSearchConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-neptunegraph-graph-vectorsearchconfiguration.html>`__
+    `ProfilePermission <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-signer-profilepermission.html>`__
     """
 
+    resource_type = "AWS::Signer::ProfilePermission"
+
     props: PropsDictType = {
-        "VectorSearchDimension": (integer, True),
+        "Action": (str, True),
+        "Principal": (str, True),
+        "ProfileName": (str, True),
+        "ProfileVersion": (str, False),
+        "StatementId": (str, True),
     }
 
 
-class Graph(AWSObject):
+class SignatureValidityPeriod(AWSProperty):
     """
-    `Graph <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-neptunegraph-graph.html>`__
+    `SignatureValidityPeriod <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-signer-signingprofile-signaturevalidityperiod.html>`__
     """
 
-    resource_type = "AWS::NeptuneGraph::Graph"
-
     props: PropsDictType = {
-        "DeletionProtection": (boolean, False),
-        "GraphName": (str, False),
-        "ProvisionedMemory": (integer, True),
-        "PublicConnectivity": (boolean, False),
-        "ReplicaCount": (integer, False),
-        "Tags": (Tags, False),
-        "VectorSearchConfiguration": (VectorSearchConfiguration, False),
+        "Type": (str, False),
+        "Value": (integer, False),
     }
 
 
-class PrivateGraphEndpoint(AWSObject):
+class SigningProfile(AWSObject):
     """
-    `PrivateGraphEndpoint <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-neptunegraph-privategraphendpoint.html>`__
+    `SigningProfile <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-signer-signingprofile.html>`__
     """
 
-    resource_type = "AWS::NeptuneGraph::PrivateGraphEndpoint"
+    resource_type = "AWS::Signer::SigningProfile"
 
     props: PropsDictType = {
-        "GraphIdentifier": (str, True),
-        "SecurityGroupIds": ([str], False),
-        "SubnetIds": ([str], False),
-        "VpcId": (str, True),
+        "PlatformId": (str, True),
+        "SignatureValidityPeriod": (SignatureValidityPeriod, False),
+        "Tags": (Tags, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/networkfirewall.py` & `troposphere-4.8.0/troposphere/networkfirewall.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/networkmanager.py` & `troposphere-4.8.0/troposphere/networkmanager.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/nimblestudio.py` & `troposphere-4.8.0/troposphere/nimblestudio.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/oam.py` & `troposphere-4.8.0/troposphere/s3express.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,34 +5,32 @@
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, PropsDictType
 
 
-class Link(AWSObject):
+class BucketPolicy(AWSObject):
     """
-    `Link <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-oam-link.html>`__
+    `BucketPolicy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-s3express-bucketpolicy.html>`__
     """
 
-    resource_type = "AWS::Oam::Link"
+    resource_type = "AWS::S3Express::BucketPolicy"
 
     props: PropsDictType = {
-        "LabelTemplate": (str, False),
-        "ResourceTypes": ([str], True),
-        "SinkIdentifier": (str, True),
-        "Tags": (dict, False),
+        "Bucket": (str, True),
+        "PolicyDocument": (dict, True),
     }
 
 
-class Sink(AWSObject):
+class DirectoryBucket(AWSObject):
     """
-    `Sink <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-oam-sink.html>`__
+    `DirectoryBucket <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-s3express-directorybucket.html>`__
     """
 
-    resource_type = "AWS::Oam::Sink"
+    resource_type = "AWS::S3Express::DirectoryBucket"
 
     props: PropsDictType = {
-        "Name": (str, True),
-        "Policy": (dict, False),
-        "Tags": (dict, False),
+        "BucketName": (str, False),
+        "DataRedundancy": (str, True),
+        "LocationName": (str, True),
     }
```

### Comparing `troposphere-4.7.0/troposphere/omics.py` & `troposphere-4.8.0/troposphere/omics.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/opensearchserverless.py` & `troposphere-4.8.0/troposphere/opensearchserverless.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/opensearchservice.py` & `troposphere-4.8.0/troposphere/opensearchservice.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/openstack/heat.py` & `troposphere-4.8.0/troposphere/openstack/heat.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/openstack/neutron.py` & `troposphere-4.8.0/troposphere/openstack/neutron.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/openstack/nova.py` & `troposphere-4.8.0/troposphere/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/opsworks.py` & `troposphere-4.8.0/troposphere/opsworks.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/opsworkscm.py` & `troposphere-4.8.0/troposphere/opsworkscm.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/organizations.py` & `troposphere-4.8.0/troposphere/organizations.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/osis.py` & `troposphere-4.8.0/troposphere/osis.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/panorama.py` & `troposphere-4.8.0/troposphere/panorama.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/pcaconnectorad.py` & `troposphere-4.8.0/troposphere/pcaconnectorad.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/personalize.py` & `troposphere-4.8.0/troposphere/personalize.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/pinpoint.py` & `troposphere-4.8.0/troposphere/pinpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,14 +492,15 @@
 
     props: PropsDictType = {
         "ApplicationId": (str, True),
         "ConfigurationSet": (str, False),
         "Enabled": (boolean, False),
         "FromAddress": (str, True),
         "Identity": (str, True),
+        "OrchestrationSendingRoleArn": (str, False),
         "RoleArn": (str, False),
     }
 
 
 class EmailTemplate(AWSObject):
     """
     `EmailTemplate <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-pinpoint-emailtemplate.html>`__
```

### Comparing `troposphere-4.7.0/troposphere/pinpointemail.py` & `troposphere-4.8.0/troposphere/pinpointemail.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/pipes.py` & `troposphere-4.8.0/troposphere/pipes.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/policies.py` & `troposphere-4.8.0/troposphere/policies.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/proton.py` & `troposphere-4.8.0/troposphere/proton.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/qldb.py` & `troposphere-4.8.0/troposphere/qldb.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/quicksight.py` & `troposphere-4.8.0/troposphere/quicksight.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,22 +453,314 @@
     props: PropsDictType = {
         "CustomFilterConfiguration": (CustomFilterConfiguration, False),
         "CustomFilterListConfiguration": (CustomFilterListConfiguration, False),
         "FilterListConfiguration": (FilterListConfiguration, False),
     }
 
 
+class FontSize(AWSProperty):
+    """
+    `FontSize <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-fontsize.html>`__
+    """
+
+    props: PropsDictType = {
+        "Relative": (str, False),
+    }
+
+
+class FontWeight(AWSProperty):
+    """
+    `FontWeight <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-fontweight.html>`__
+    """
+
+    props: PropsDictType = {
+        "Name": (str, False),
+    }
+
+
+class FontConfiguration(AWSProperty):
+    """
+    `FontConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-fontconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "FontColor": (str, False),
+        "FontDecoration": (str, False),
+        "FontSize": (FontSize, False),
+        "FontStyle": (str, False),
+        "FontWeight": (FontWeight, False),
+    }
+
+
+class LabelOptions(AWSProperty):
+    """
+    `LabelOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-labeloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "CustomLabel": (str, False),
+        "FontConfiguration": (FontConfiguration, False),
+        "Visibility": (str, False),
+    }
+
+
+class SheetControlInfoIconLabelOptions(AWSProperty):
+    """
+    `SheetControlInfoIconLabelOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-sheetcontrolinfoiconlabeloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "InfoIconText": (str, False),
+        "Visibility": (str, False),
+    }
+
+
+class DateTimePickerControlDisplayOptions(AWSProperty):
+    """
+    `DateTimePickerControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-datetimepickercontroldisplayoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DateTimeFormat": (str, False),
+        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
+        "TitleOptions": (LabelOptions, False),
+    }
+
+
+class DefaultDateTimePickerControlOptions(AWSProperty):
+    """
+    `DefaultDateTimePickerControlOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaultdatetimepickercontroloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DisplayOptions": (DateTimePickerControlDisplayOptions, False),
+        "Type": (str, False),
+    }
+
+
+class ListControlSelectAllOptions(AWSProperty):
+    """
+    `ListControlSelectAllOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-listcontrolselectalloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "Visibility": (str, False),
+    }
+
+
+class DropDownControlDisplayOptions(AWSProperty):
+    """
+    `DropDownControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-dropdowncontroldisplayoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
+        "SelectAllOptions": (ListControlSelectAllOptions, False),
+        "TitleOptions": (LabelOptions, False),
+    }
+
+
+class FilterSelectableValues(AWSProperty):
+    """
+    `FilterSelectableValues <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filterselectablevalues.html>`__
+    """
+
+    props: PropsDictType = {
+        "Values": ([str], False),
+    }
+
+
+class DefaultFilterDropDownControlOptions(AWSProperty):
+    """
+    `DefaultFilterDropDownControlOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaultfilterdropdowncontroloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DisplayOptions": (DropDownControlDisplayOptions, False),
+        "SelectableValues": (FilterSelectableValues, False),
+        "Type": (str, False),
+    }
+
+
+class ListControlSearchOptions(AWSProperty):
+    """
+    `ListControlSearchOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-listcontrolsearchoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "Visibility": (str, False),
+    }
+
+
+class ListControlDisplayOptions(AWSProperty):
+    """
+    `ListControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-listcontroldisplayoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
+        "SearchOptions": (ListControlSearchOptions, False),
+        "SelectAllOptions": (ListControlSelectAllOptions, False),
+        "TitleOptions": (LabelOptions, False),
+    }
+
+
+class DefaultFilterListControlOptions(AWSProperty):
+    """
+    `DefaultFilterListControlOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaultfilterlistcontroloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DisplayOptions": (ListControlDisplayOptions, False),
+        "SelectableValues": (FilterSelectableValues, False),
+        "Type": (str, False),
+    }
+
+
+class RelativeDateTimeControlDisplayOptions(AWSProperty):
+    """
+    `RelativeDateTimeControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-relativedatetimecontroldisplayoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DateTimeFormat": (str, False),
+        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
+        "TitleOptions": (LabelOptions, False),
+    }
+
+
+class DefaultRelativeDateTimeControlOptions(AWSProperty):
+    """
+    `DefaultRelativeDateTimeControlOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaultrelativedatetimecontroloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DisplayOptions": (RelativeDateTimeControlDisplayOptions, False),
+    }
+
+
+class SliderControlDisplayOptions(AWSProperty):
+    """
+    `SliderControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-slidercontroldisplayoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
+        "TitleOptions": (LabelOptions, False),
+    }
+
+
+class DefaultSliderControlOptions(AWSProperty):
+    """
+    `DefaultSliderControlOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaultslidercontroloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DisplayOptions": (SliderControlDisplayOptions, False),
+        "MaximumValue": (double, True),
+        "MinimumValue": (double, True),
+        "StepSize": (double, True),
+        "Type": (str, False),
+    }
+
+
+class TextControlPlaceholderOptions(AWSProperty):
+    """
+    `TextControlPlaceholderOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-textcontrolplaceholderoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "Visibility": (str, False),
+    }
+
+
+class TextAreaControlDisplayOptions(AWSProperty):
+    """
+    `TextAreaControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-textareacontroldisplayoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
+        "PlaceholderOptions": (TextControlPlaceholderOptions, False),
+        "TitleOptions": (LabelOptions, False),
+    }
+
+
+class DefaultTextAreaControlOptions(AWSProperty):
+    """
+    `DefaultTextAreaControlOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaulttextareacontroloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "Delimiter": (str, False),
+        "DisplayOptions": (TextAreaControlDisplayOptions, False),
+    }
+
+
+class TextFieldControlDisplayOptions(AWSProperty):
+    """
+    `TextFieldControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-textfieldcontroldisplayoptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
+        "PlaceholderOptions": (TextControlPlaceholderOptions, False),
+        "TitleOptions": (LabelOptions, False),
+    }
+
+
+class DefaultTextFieldControlOptions(AWSProperty):
+    """
+    `DefaultTextFieldControlOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaulttextfieldcontroloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DisplayOptions": (TextFieldControlDisplayOptions, False),
+    }
+
+
+class DefaultFilterControlOptions(AWSProperty):
+    """
+    `DefaultFilterControlOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaultfiltercontroloptions.html>`__
+    """
+
+    props: PropsDictType = {
+        "DefaultDateTimePickerOptions": (DefaultDateTimePickerControlOptions, False),
+        "DefaultDropdownOptions": (DefaultFilterDropDownControlOptions, False),
+        "DefaultListOptions": (DefaultFilterListControlOptions, False),
+        "DefaultRelativeDateTimeOptions": (
+            DefaultRelativeDateTimeControlOptions,
+            False,
+        ),
+        "DefaultSliderOptions": (DefaultSliderControlOptions, False),
+        "DefaultTextAreaOptions": (DefaultTextAreaControlOptions, False),
+        "DefaultTextFieldOptions": (DefaultTextFieldControlOptions, False),
+    }
+
+
+class DefaultFilterControlConfiguration(AWSProperty):
+    """
+    `DefaultFilterControlConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-defaultfiltercontrolconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "ControlOptions": (DefaultFilterControlOptions, True),
+        "Title": (str, True),
+    }
+
+
 class CategoryFilter(AWSProperty):
     """
     `CategoryFilter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-categoryfilter.html>`__
     """
 
     props: PropsDictType = {
         "Column": (ColumnIdentifier, True),
         "Configuration": (CategoryFilterConfiguration, True),
+        "DefaultFilterControlConfiguration": (DefaultFilterControlConfiguration, False),
         "FilterId": (str, True),
     }
 
 
 class AttributeAggregationFunction(AWSProperty):
     """
     `AttributeAggregationFunction <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-attributeaggregationfunction.html>`__
@@ -518,14 +810,15 @@
     """
     `NumericEqualityFilter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-numericequalityfilter.html>`__
     """
 
     props: PropsDictType = {
         "AggregationFunction": (AggregationFunction, False),
         "Column": (ColumnIdentifier, True),
+        "DefaultFilterControlConfiguration": (DefaultFilterControlConfiguration, False),
         "FilterId": (str, True),
         "MatchOperator": (str, True),
         "NullOption": (str, True),
         "ParameterName": (str, False),
         "SelectAllOptions": (str, False),
         "Value": (double, False),
     }
@@ -546,14 +839,15 @@
     """
     `NumericRangeFilter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-numericrangefilter.html>`__
     """
 
     props: PropsDictType = {
         "AggregationFunction": (AggregationFunction, False),
         "Column": (ColumnIdentifier, True),
+        "DefaultFilterControlConfiguration": (DefaultFilterControlConfiguration, False),
         "FilterId": (str, True),
         "IncludeMaximum": (boolean, False),
         "IncludeMinimum": (boolean, False),
         "NullOption": (str, True),
         "RangeMaximum": (NumericRangeFilterValue, False),
         "RangeMinimum": (NumericRangeFilterValue, False),
         "SelectAllOptions": (str, False),
@@ -587,14 +881,15 @@
     """
     `RelativeDatesFilter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-relativedatesfilter.html>`__
     """
 
     props: PropsDictType = {
         "AnchorDateConfiguration": (AnchorDateConfiguration, True),
         "Column": (ColumnIdentifier, True),
+        "DefaultFilterControlConfiguration": (DefaultFilterControlConfiguration, False),
         "ExcludePeriodConfiguration": (ExcludePeriodConfiguration, False),
         "FilterId": (str, True),
         "MinimumGranularity": (str, False),
         "NullOption": (str, True),
         "ParameterName": (str, False),
         "RelativeDateType": (str, True),
         "RelativeDateValue": (double, False),
@@ -616,14 +911,15 @@
 class TimeEqualityFilter(AWSProperty):
     """
     `TimeEqualityFilter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-timeequalityfilter.html>`__
     """
 
     props: PropsDictType = {
         "Column": (ColumnIdentifier, True),
+        "DefaultFilterControlConfiguration": (DefaultFilterControlConfiguration, False),
         "FilterId": (str, True),
         "ParameterName": (str, False),
         "RollingDate": (RollingDateConfiguration, False),
         "TimeGranularity": (str, False),
         "Value": (str, False),
     }
 
@@ -643,14 +939,15 @@
 class TimeRangeFilter(AWSProperty):
     """
     `TimeRangeFilter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-timerangefilter.html>`__
     """
 
     props: PropsDictType = {
         "Column": (ColumnIdentifier, True),
+        "DefaultFilterControlConfiguration": (DefaultFilterControlConfiguration, False),
         "ExcludePeriodConfiguration": (ExcludePeriodConfiguration, False),
         "FilterId": (str, True),
         "IncludeMaximum": (boolean, False),
         "IncludeMinimum": (boolean, False),
         "NullOption": (str, True),
         "RangeMaximumValue": (TimeRangeFilterValue, False),
         "RangeMinimumValue": (TimeRangeFilterValue, False),
@@ -674,14 +971,15 @@
     """
     `TopBottomFilter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-topbottomfilter.html>`__
     """
 
     props: PropsDictType = {
         "AggregationSortConfigurations": ([AggregationSortConfiguration], True),
         "Column": (ColumnIdentifier, True),
+        "DefaultFilterControlConfiguration": (DefaultFilterControlConfiguration, False),
         "FilterId": (str, True),
         "Limit": (double, False),
         "ParameterName": (str, False),
         "TimeGranularity": (str, False),
     }
 
 
@@ -925,97 +1223,14 @@
         "DateTimeParameterDeclaration": (DateTimeParameterDeclaration, False),
         "DecimalParameterDeclaration": (DecimalParameterDeclaration, False),
         "IntegerParameterDeclaration": (IntegerParameterDeclaration, False),
         "StringParameterDeclaration": (StringParameterDeclaration, False),
     }
 
 
-class FontSize(AWSProperty):
-    """
-    `FontSize <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-fontsize.html>`__
-    """
-
-    props: PropsDictType = {
-        "Relative": (str, False),
-    }
-
-
-class FontWeight(AWSProperty):
-    """
-    `FontWeight <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-fontweight.html>`__
-    """
-
-    props: PropsDictType = {
-        "Name": (str, False),
-    }
-
-
-class FontConfiguration(AWSProperty):
-    """
-    `FontConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-fontconfiguration.html>`__
-    """
-
-    props: PropsDictType = {
-        "FontColor": (str, False),
-        "FontDecoration": (str, False),
-        "FontSize": (FontSize, False),
-        "FontStyle": (str, False),
-        "FontWeight": (FontWeight, False),
-    }
-
-
-class LabelOptions(AWSProperty):
-    """
-    `LabelOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-labeloptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "CustomLabel": (str, False),
-        "FontConfiguration": (FontConfiguration, False),
-        "Visibility": (str, False),
-    }
-
-
-class SheetControlInfoIconLabelOptions(AWSProperty):
-    """
-    `SheetControlInfoIconLabelOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-sheetcontrolinfoiconlabeloptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "InfoIconText": (str, False),
-        "Visibility": (str, False),
-    }
-
-
-class DateTimePickerControlDisplayOptions(AWSProperty):
-    """
-    `DateTimePickerControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-datetimepickercontroldisplayoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "DateTimeFormat": (str, False),
-        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
-        "TitleOptions": (LabelOptions, False),
-    }
-
-
-class FilterDateTimePickerControl(AWSProperty):
-    """
-    `FilterDateTimePickerControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filterdatetimepickercontrol.html>`__
-    """
-
-    props: PropsDictType = {
-        "DisplayOptions": (DateTimePickerControlDisplayOptions, False),
-        "FilterControlId": (str, True),
-        "SourceFilterId": (str, True),
-        "Title": (str, True),
-        "Type": (str, False),
-    }
-
-
 class CascadingControlSource(AWSProperty):
     """
     `CascadingControlSource <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-cascadingcontrolsource.html>`__
     """
 
     props: PropsDictType = {
         "ColumnToMatch": (ColumnIdentifier, False),
@@ -1029,43 +1244,37 @@
     """
 
     props: PropsDictType = {
         "SourceControls": ([CascadingControlSource], False),
     }
 
 
-class ListControlSelectAllOptions(AWSProperty):
+class FilterCrossSheetControl(AWSProperty):
     """
-    `ListControlSelectAllOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-listcontrolselectalloptions.html>`__
+    `FilterCrossSheetControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filtercrosssheetcontrol.html>`__
     """
 
     props: PropsDictType = {
-        "Visibility": (str, False),
-    }
-
-
-class DropDownControlDisplayOptions(AWSProperty):
-    """
-    `DropDownControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-dropdowncontroldisplayoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
-        "SelectAllOptions": (ListControlSelectAllOptions, False),
-        "TitleOptions": (LabelOptions, False),
+        "CascadingControlConfiguration": (CascadingControlConfiguration, False),
+        "FilterControlId": (str, True),
+        "SourceFilterId": (str, True),
     }
 
 
-class FilterSelectableValues(AWSProperty):
+class FilterDateTimePickerControl(AWSProperty):
     """
-    `FilterSelectableValues <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filterselectablevalues.html>`__
+    `FilterDateTimePickerControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filterdatetimepickercontrol.html>`__
     """
 
     props: PropsDictType = {
-        "Values": ([str], False),
+        "DisplayOptions": (DateTimePickerControlDisplayOptions, False),
+        "FilterControlId": (str, True),
+        "SourceFilterId": (str, True),
+        "Title": (str, True),
+        "Type": (str, False),
     }
 
 
 class FilterDropDownControl(AWSProperty):
     """
     `FilterDropDownControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filterdropdowncontrol.html>`__
     """
@@ -1077,37 +1286,14 @@
         "SelectableValues": (FilterSelectableValues, False),
         "SourceFilterId": (str, True),
         "Title": (str, True),
         "Type": (str, False),
     }
 
 
-class ListControlSearchOptions(AWSProperty):
-    """
-    `ListControlSearchOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-listcontrolsearchoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "Visibility": (str, False),
-    }
-
-
-class ListControlDisplayOptions(AWSProperty):
-    """
-    `ListControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-listcontroldisplayoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
-        "SearchOptions": (ListControlSearchOptions, False),
-        "SelectAllOptions": (ListControlSelectAllOptions, False),
-        "TitleOptions": (LabelOptions, False),
-    }
-
-
 class FilterListControl(AWSProperty):
     """
     `FilterListControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filterlistcontrol.html>`__
     """
 
     props: PropsDictType = {
         "CascadingControlConfiguration": (CascadingControlConfiguration, False),
@@ -1116,50 +1302,27 @@
         "SelectableValues": (FilterSelectableValues, False),
         "SourceFilterId": (str, True),
         "Title": (str, True),
         "Type": (str, False),
     }
 
 
-class RelativeDateTimeControlDisplayOptions(AWSProperty):
-    """
-    `RelativeDateTimeControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-relativedatetimecontroldisplayoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "DateTimeFormat": (str, False),
-        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
-        "TitleOptions": (LabelOptions, False),
-    }
-
-
 class FilterRelativeDateTimeControl(AWSProperty):
     """
     `FilterRelativeDateTimeControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filterrelativedatetimecontrol.html>`__
     """
 
     props: PropsDictType = {
         "DisplayOptions": (RelativeDateTimeControlDisplayOptions, False),
         "FilterControlId": (str, True),
         "SourceFilterId": (str, True),
         "Title": (str, True),
     }
 
 
-class SliderControlDisplayOptions(AWSProperty):
-    """
-    `SliderControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-slidercontroldisplayoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
-        "TitleOptions": (LabelOptions, False),
-    }
-
-
 class FilterSliderControl(AWSProperty):
     """
     `FilterSliderControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filterslidercontrol.html>`__
     """
 
     props: PropsDictType = {
         "DisplayOptions": (SliderControlDisplayOptions, False),
@@ -1169,62 +1332,28 @@
         "SourceFilterId": (str, True),
         "StepSize": (double, True),
         "Title": (str, True),
         "Type": (str, False),
     }
 
 
-class TextControlPlaceholderOptions(AWSProperty):
-    """
-    `TextControlPlaceholderOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-textcontrolplaceholderoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "Visibility": (str, False),
-    }
-
-
-class TextAreaControlDisplayOptions(AWSProperty):
-    """
-    `TextAreaControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-textareacontroldisplayoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
-        "PlaceholderOptions": (TextControlPlaceholderOptions, False),
-        "TitleOptions": (LabelOptions, False),
-    }
-
-
 class FilterTextAreaControl(AWSProperty):
     """
     `FilterTextAreaControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filtertextareacontrol.html>`__
     """
 
     props: PropsDictType = {
         "Delimiter": (str, False),
         "DisplayOptions": (TextAreaControlDisplayOptions, False),
         "FilterControlId": (str, True),
         "SourceFilterId": (str, True),
         "Title": (str, True),
     }
 
 
-class TextFieldControlDisplayOptions(AWSProperty):
-    """
-    `TextFieldControlDisplayOptions <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-textfieldcontroldisplayoptions.html>`__
-    """
-
-    props: PropsDictType = {
-        "InfoIconLabelOptions": (SheetControlInfoIconLabelOptions, False),
-        "PlaceholderOptions": (TextControlPlaceholderOptions, False),
-        "TitleOptions": (LabelOptions, False),
-    }
-
-
 class FilterTextFieldControl(AWSProperty):
     """
     `FilterTextFieldControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filtertextfieldcontrol.html>`__
     """
 
     props: PropsDictType = {
         "DisplayOptions": (TextFieldControlDisplayOptions, False),
@@ -1236,14 +1365,15 @@
 
 class FilterControl(AWSProperty):
     """
     `FilterControl <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-quicksight-template-filtercontrol.html>`__
     """
 
     props: PropsDictType = {
+        "CrossSheet": (FilterCrossSheetControl, False),
         "DateTimePicker": (FilterDateTimePickerControl, False),
         "Dropdown": (FilterDropDownControl, False),
         "List": (FilterListControl, False),
         "RelativeDateTime": (FilterRelativeDateTimeControl, False),
         "Slider": (FilterSliderControl, False),
         "TextArea": (FilterTextAreaControl, False),
         "TextField": (FilterTextFieldControl, False),
```

### Comparing `troposphere-4.7.0/troposphere/ram.py` & `troposphere-4.8.0/troposphere/ram.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/rds.py` & `troposphere-4.8.0/troposphere/rds.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,26 @@
     """
     `CustomDBEngineVersion <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-rds-customdbengineversion.html>`__
     """
 
     resource_type = "AWS::RDS::CustomDBEngineVersion"
 
     props: PropsDictType = {
-        "DatabaseInstallationFilesS3BucketName": (str, True),
+        "DatabaseInstallationFilesS3BucketName": (str, False),
         "DatabaseInstallationFilesS3Prefix": (str, False),
         "Description": (str, False),
         "Engine": (str, True),
         "EngineVersion": (str, True),
+        "ImageId": (str, False),
         "KMSKeyId": (str, False),
         "Manifest": (str, False),
+        "SourceCustomDbEngineVersionIdentifier": (str, False),
         "Status": (str, False),
         "Tags": (Tags, False),
+        "UseAwsProvidedLatestImage": (boolean, False),
     }
 
 
 class DBClusterRole(AWSProperty):
     """
     `DBClusterRole <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-rds-dbcluster-dbclusterrole.html>`__
     """
@@ -228,14 +231,15 @@
     resource_type = "AWS::RDS::DBInstance"
 
     props: PropsDictType = {
         "AllocatedStorage": (validate_str_or_int, False),
         "AllowMajorVersionUpgrade": (boolean, False),
         "AssociatedRoles": ([DBInstanceRole], False),
         "AutoMinorVersionUpgrade": (boolean, False),
+        "AutomaticBackupReplicationKmsKeyId": (str, False),
         "AutomaticBackupReplicationRegion": (str, False),
         "AvailabilityZone": (str, False),
         "BackupRetentionPeriod": (validate_backup_retention_period, False),
         "CACertificateIdentifier": (str, False),
         "CertificateDetails": (CertificateDetails, False),
         "CertificateRotationRestart": (boolean, False),
         "CharacterSetName": (str, False),
@@ -508,14 +512,16 @@
     `Integration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-rds-integration.html>`__
     """
 
     resource_type = "AWS::RDS::Integration"
 
     props: PropsDictType = {
         "AdditionalEncryptionContext": (dict, False),
+        "DataFilter": (str, False),
+        "Description": (str, False),
         "IntegrationName": (str, False),
         "KMSKeyId": (str, False),
         "SourceArn": (str, True),
         "Tags": (Tags, False),
         "TargetArn": (str, True),
     }
```

### Comparing `troposphere-4.7.0/troposphere/redshift.py` & `troposphere-4.8.0/troposphere/redshift.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/redshiftserverless.py` & `troposphere-4.8.0/troposphere/redshiftserverless.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,26 @@
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, AWSProperty, PropsDictType, Tags
 from .validators import boolean, integer
 
 
+class SnapshotCopyConfiguration(AWSProperty):
+    """
+    `SnapshotCopyConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-redshiftserverless-namespace-snapshotcopyconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "DestinationKmsKeyId": (str, False),
+        "DestinationRegion": (str, True),
+        "SnapshotRetentionPeriod": (integer, False),
+    }
+
+
 class Namespace(AWSObject):
     """
     `Namespace <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-redshiftserverless-namespace.html>`__
     """
 
     resource_type = "AWS::RedshiftServerless::Namespace"
 
@@ -28,14 +40,15 @@
         "IamRoles": ([str], False),
         "KmsKeyId": (str, False),
         "LogExports": ([str], False),
         "ManageAdminPassword": (boolean, False),
         "NamespaceName": (str, True),
         "NamespaceResourcePolicy": (dict, False),
         "RedshiftIdcApplicationArn": (str, False),
+        "SnapshotCopyConfigurations": ([SnapshotCopyConfiguration], False),
         "Tags": (Tags, False),
     }
 
 
 class ConfigParameter(AWSProperty):
     """
     `ConfigParameter <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-redshiftserverless-workgroup-configparameter.html>`__
```

### Comparing `troposphere-4.7.0/troposphere/refactorspaces.py` & `troposphere-4.8.0/troposphere/refactorspaces.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/rekognition.py` & `troposphere-4.8.0/troposphere/rekognition.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/resiliencehub.py` & `troposphere-4.8.0/troposphere/resiliencehub.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,14 +93,27 @@
 
     props: PropsDictType = {
         "RpoInSecs": (integer, True),
         "RtoInSecs": (integer, True),
     }
 
 
+class PolicyMap(AWSProperty):
+    """
+    `PolicyMap <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-resiliencehub-resiliencypolicy-policymap.html>`__
+    """
+
+    props: PropsDictType = {
+        "AZ": (FailurePolicy, True),
+        "Hardware": (FailurePolicy, True),
+        "Region": (FailurePolicy, False),
+        "Software": (FailurePolicy, True),
+    }
+
+
 class ResiliencyPolicy(AWSObject):
     """
     `ResiliencyPolicy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-resiliencehub-resiliencypolicy.html>`__
     """
 
     resource_type = "AWS::ResilienceHub::ResiliencyPolicy"
```

### Comparing `troposphere-4.7.0/troposphere/resourceexplorer2.py` & `troposphere-4.8.0/troposphere/resourceexplorer2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/resourcegroups.py` & `troposphere-4.8.0/troposphere/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/robomaker.py` & `troposphere-4.8.0/troposphere/robomaker.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/rolesanywhere.py` & `troposphere-4.8.0/troposphere/rolesanywhere.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/route53.py` & `troposphere-4.8.0/troposphere/route53.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/route53recoverycontrol.py` & `troposphere-4.8.0/troposphere/route53recoverycontrol.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/route53recoveryreadiness.py` & `troposphere-4.8.0/troposphere/route53recoveryreadiness.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/route53resolver.py` & `troposphere-4.8.0/troposphere/route53resolver.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/rum.py` & `troposphere-4.8.0/troposphere/rum.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/s3.py` & `troposphere-4.8.0/troposphere/s3.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/s3express.py` & `troposphere-4.8.0/troposphere/simspaceweaver.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 # All rights reserved.
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
-from . import AWSObject, PropsDictType
+from . import AWSObject, AWSProperty, PropsDictType
 
 
-class BucketPolicy(AWSObject):
+class S3Location(AWSProperty):
     """
-    `BucketPolicy <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-s3express-bucketpolicy.html>`__
+    `S3Location <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-simspaceweaver-simulation-s3location.html>`__
     """
 
-    resource_type = "AWS::S3Express::BucketPolicy"
-
     props: PropsDictType = {
-        "Bucket": (str, True),
-        "PolicyDocument": (dict, True),
+        "BucketName": (str, True),
+        "ObjectKey": (str, True),
     }
 
 
-class DirectoryBucket(AWSObject):
+class Simulation(AWSObject):
     """
-    `DirectoryBucket <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-s3express-directorybucket.html>`__
+    `Simulation <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-simspaceweaver-simulation.html>`__
     """
 
-    resource_type = "AWS::S3Express::DirectoryBucket"
+    resource_type = "AWS::SimSpaceWeaver::Simulation"
 
     props: PropsDictType = {
-        "BucketName": (str, False),
-        "DataRedundancy": (str, True),
-        "LocationName": (str, True),
+        "MaximumDuration": (str, False),
+        "Name": (str, True),
+        "RoleArn": (str, True),
+        "SchemaS3Location": (S3Location, False),
+        "SnapshotS3Location": (S3Location, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/s3objectlambda.py` & `troposphere-4.8.0/troposphere/s3objectlambda.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/s3outposts.py` & `troposphere-4.8.0/troposphere/s3outposts.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/sagemaker.py` & `troposphere-4.8.0/troposphere/sagemaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,24 @@
         "ContainerEnvironmentVariables": (
             [CustomImageContainerEnvironmentVariable],
             False,
         ),
     }
 
 
+class CodeEditorAppImageConfig(AWSProperty):
+    """
+    `CodeEditorAppImageConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-sagemaker-appimageconfig-codeeditorappimageconfig.html>`__
+    """
+
+    props: PropsDictType = {
+        "ContainerConfig": (ContainerConfig, False),
+    }
+
+
 class JupyterLabAppImageConfig(AWSProperty):
     """
     `JupyterLabAppImageConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-sagemaker-appimageconfig-jupyterlabappimageconfig.html>`__
     """
 
     props: PropsDictType = {
         "ContainerConfig": (ContainerConfig, False),
@@ -114,14 +124,15 @@
     `AppImageConfig <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-sagemaker-appimageconfig.html>`__
     """
 
     resource_type = "AWS::SageMaker::AppImageConfig"
 
     props: PropsDictType = {
         "AppImageConfigName": (str, True),
+        "CodeEditorAppImageConfig": (CodeEditorAppImageConfig, False),
         "JupyterLabAppImageConfig": (JupyterLabAppImageConfig, False),
         "KernelGatewayImageConfig": (KernelGatewayImageConfig, False),
         "Tags": (Tags, False),
     }
 
 
 class GitConfig(AWSProperty):
@@ -517,14 +528,15 @@
 
 class CodeEditorAppSettings(AWSProperty):
     """
     `CodeEditorAppSettings <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-sagemaker-userprofile-codeeditorappsettings.html>`__
     """
 
     props: PropsDictType = {
+        "CustomImages": ([CustomImage], False),
         "DefaultResourceSpec": (ResourceSpec, False),
         "LifecycleConfigArns": ([str], False),
     }
 
 
 class EFSFileSystemConfig(AWSProperty):
     """
```

### Comparing `troposphere-4.7.0/troposphere/scheduler.py` & `troposphere-4.8.0/troposphere/scheduler.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/secretsmanager.py` & `troposphere-4.8.0/troposphere/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/serverless.py` & `troposphere-4.8.0/troposphere/serverless.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,14 +567,15 @@
     props: PropsDictType = {
         "Stream": (str, True),
         "StartingPosition": (starting_position_validator, True),
         "BatchSize": (positive_integer, False),
         "BisectBatchOnFunctionError": (bool, False),
         "DestinationConfig": (DestinationConfig, False),
         "Enabled": (bool, False),
+        "FilterCriteria": (FilterCriteria, False),
         "MaximumBatchingWindowInSeconds": (positive_integer, False),
         "MaximumRecordAgeInSeconds": (integer_range(60, 604800), False),
         "MaximumRetryAttempts": (positive_integer, False),
         "ParallelizationFactor": (integer_range(1, 10), False),
     }
 
 
@@ -765,15 +766,15 @@
         "Broker": (str, True),
         "DynamicPolicyName": (bool, False),
         "Enabled": (bool, False),
         "FilterCriteria": (FilterCriteria, False),
         "MaximumBatchingWindowInSeconds": (integer, False),
         "Queues": ([str], True),
         "SecretsManagerKmsKeyId": (str, False),
-        "SourceAccessConfigurations": ([str], True),
+        "SourceAccessConfigurations": ([SourceAccessConfiguration], True),
     }
 
 
 class DocumentDBEvent(AWSObject):
     resource_type = "DocumentDB"
 
     props: PropsDictType = {
```

### Comparing `troposphere-4.7.0/troposphere/servicecatalog.py` & `troposphere-4.8.0/troposphere/servicecatalog.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/servicecatalogappregistry.py` & `troposphere-4.8.0/troposphere/servicecatalogappregistry.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/servicediscovery.py` & `troposphere-4.8.0/troposphere/servicediscovery.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/ses.py` & `troposphere-4.8.0/troposphere/ses.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/shield.py` & `troposphere-4.8.0/troposphere/shield.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/signer.py` & `troposphere-4.8.0/troposphere/route53profiles.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-# Copyright (c) 2012-2022, Mark Peek <mark@peek.org>
+# Copyright (c) 2012-2024, Mark Peek <mark@peek.org>
 # All rights reserved.
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
-from . import AWSObject, AWSProperty, PropsDictType, Tags
-from .validators import integer
+from . import AWSObject, PropsDictType, Tags
 
 
-class ProfilePermission(AWSObject):
+class Profile(AWSObject):
     """
-    `ProfilePermission <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-signer-profilepermission.html>`__
+    `Profile <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-route53profiles-profile.html>`__
     """
 
-    resource_type = "AWS::Signer::ProfilePermission"
+    resource_type = "AWS::Route53Profiles::Profile"
 
     props: PropsDictType = {
-        "Action": (str, True),
-        "Principal": (str, True),
-        "ProfileName": (str, True),
-        "ProfileVersion": (str, False),
-        "StatementId": (str, True),
+        "Name": (str, True),
+        "Tags": (Tags, False),
     }
 
 
-class SignatureValidityPeriod(AWSProperty):
+class ProfileAssociation(AWSObject):
     """
-    `SignatureValidityPeriod <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-signer-signingprofile-signaturevalidityperiod.html>`__
+    `ProfileAssociation <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-route53profiles-profileassociation.html>`__
     """
 
+    resource_type = "AWS::Route53Profiles::ProfileAssociation"
+
     props: PropsDictType = {
-        "Type": (str, False),
-        "Value": (integer, False),
+        "Arn": (str, False),
+        "Name": (str, True),
+        "ProfileId": (str, True),
+        "ResourceId": (str, True),
+        "Tags": (Tags, False),
     }
 
 
-class SigningProfile(AWSObject):
+class ProfileResourceAssociation(AWSObject):
     """
-    `SigningProfile <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-signer-signingprofile.html>`__
+    `ProfileResourceAssociation <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-route53profiles-profileresourceassociation.html>`__
     """
 
-    resource_type = "AWS::Signer::SigningProfile"
+    resource_type = "AWS::Route53Profiles::ProfileResourceAssociation"
 
     props: PropsDictType = {
-        "PlatformId": (str, True),
-        "SignatureValidityPeriod": (SignatureValidityPeriod, False),
-        "Tags": (Tags, False),
+        "Name": (str, True),
+        "ProfileId": (str, True),
+        "ResourceArn": (str, True),
+        "ResourceProperties": (str, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/sns.py` & `troposphere-4.8.0/troposphere/sns.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/sqs.py` & `troposphere-4.8.0/troposphere/sqs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/ssm.py` & `troposphere-4.8.0/troposphere/ssm.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/ssmcontacts.py` & `troposphere-4.8.0/troposphere/ssmcontacts.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/ssmincidents.py` & `troposphere-4.8.0/troposphere/ssmincidents.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/sso.py` & `troposphere-4.8.0/troposphere/sso.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/stepfunctions.py` & `troposphere-4.8.0/troposphere/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/supportapp.py` & `troposphere-4.8.0/troposphere/supportapp.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/synthetics.py` & `troposphere-4.8.0/troposphere/synthetics.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/template_generator.py` & `troposphere-4.8.0/troposphere/template_generator.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/timestream.py` & `troposphere-4.8.0/troposphere/timestream.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # See LICENSE file for full license.
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, AWSProperty, PropsDictType, Tags
-from .validators import boolean
+from .validators import boolean, integer
 
 
 class Database(AWSObject):
     """
     `Database <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-timestream-database.html>`__
     """
 
@@ -33,14 +33,50 @@
         "BucketName": (str, True),
         "EncryptionOption": (str, True),
         "KmsKeyId": (str, False),
         "ObjectKeyPrefix": (str, False),
     }
 
 
+class LogDeliveryConfiguration(AWSProperty):
+    """
+    `LogDeliveryConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-timestream-influxdbinstance-logdeliveryconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "S3Configuration": (S3Configuration, True),
+    }
+
+
+class InfluxDBInstance(AWSObject):
+    """
+    `InfluxDBInstance <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-timestream-influxdbinstance.html>`__
+    """
+
+    resource_type = "AWS::Timestream::InfluxDBInstance"
+
+    props: PropsDictType = {
+        "AllocatedStorage": (integer, False),
+        "Bucket": (str, False),
+        "DbInstanceType": (str, False),
+        "DbParameterGroupIdentifier": (str, False),
+        "DbStorageType": (str, False),
+        "DeploymentType": (str, False),
+        "LogDeliveryConfiguration": (LogDeliveryConfiguration, False),
+        "Name": (str, False),
+        "Organization": (str, False),
+        "Password": (str, False),
+        "PubliclyAccessible": (boolean, False),
+        "Tags": (Tags, False),
+        "Username": (str, False),
+        "VpcSecurityGroupIds": ([str], False),
+        "VpcSubnetIds": ([str], False),
+    }
+
+
 class ErrorReportConfiguration(AWSProperty):
     """
     `ErrorReportConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-timestream-scheduledquery-errorreportconfiguration.html>`__
     """
 
     props: PropsDictType = {
         "S3Configuration": (S3Configuration, True),
```

### Comparing `troposphere-4.7.0/troposphere/transfer.py` & `troposphere-4.8.0/troposphere/transfer.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/utils.py` & `troposphere-4.8.0/troposphere/utils.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/__init__.py` & `troposphere-4.8.0/troposphere/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/acmpca.py` & `troposphere-4.8.0/troposphere/validators/acmpca.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/apigateway.py` & `troposphere-4.8.0/troposphere/validators/apigateway.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/apigatewayv2.py` & `troposphere-4.8.0/troposphere/validators/apigatewayv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/appconfig.py` & `troposphere-4.8.0/troposphere/validators/appconfig.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/appmesh.py` & `troposphere-4.8.0/troposphere/validators/appmesh.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/athena.py` & `troposphere-4.8.0/troposphere/validators/athena.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/autoscaling.py` & `troposphere-4.8.0/troposphere/validators/autoscaling.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/autoscalingplans.py` & `troposphere-4.8.0/troposphere/validators/autoscalingplans.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/awslambda.py` & `troposphere-4.8.0/troposphere/validators/awslambda.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/backup.py` & `troposphere-4.8.0/troposphere/validators/backup.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/batch.py` & `troposphere-4.8.0/troposphere/validators/batch.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/cassandra.py` & `troposphere-4.8.0/troposphere/validators/cassandra.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/chatbot.py` & `troposphere-4.8.0/troposphere/validators/chatbot.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/cloudformation.py` & `troposphere-4.8.0/troposphere/validators/cloudformation.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/cloudfront.py` & `troposphere-4.8.0/troposphere/validators/cloudfront.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/cloudwatch.py` & `troposphere-4.8.0/troposphere/validators/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/codebuild.py` & `troposphere-4.8.0/troposphere/validators/codebuild.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/codecommit.py` & `troposphere-4.8.0/troposphere/validators/codecommit.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/codedeploy.py` & `troposphere-4.8.0/troposphere/validators/codedeploy.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/codestarconnections.py` & `troposphere-4.8.0/troposphere/validators/codestarconnections.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/cognito.py` & `troposphere-4.8.0/troposphere/validators/cognito.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/config.py` & `troposphere-4.8.0/troposphere/validators/config.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/dlm.py` & `troposphere-4.8.0/troposphere/validators/dlm.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def validate_interval(interval):
     """
     Interval validation rule.
     Property: CreateRule.Interval
     """
 
-    VALID_INTERVALS = (2, 3, 4, 6, 8, 12, 24)
+    VALID_INTERVALS = (1, 2, 3, 4, 6, 8, 12, 24)
 
     if interval not in VALID_INTERVALS:
         raise ValueError(
             "Interval must be one of : %s"
             % ", ".join([str(i) for i in VALID_INTERVALS])
         )
     return interval
```

### Comparing `troposphere-4.7.0/troposphere/validators/dynamodb.py` & `troposphere-4.8.0/troposphere/validators/dynamodb.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/ec2.py` & `troposphere-4.8.0/troposphere/validators/ec2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/ecs.py` & `troposphere-4.8.0/troposphere/validators/ecs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/efs.py` & `troposphere-4.8.0/troposphere/validators/efs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/eks.py` & `troposphere-4.8.0/troposphere/validators/eks.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/elasticache.py` & `troposphere-4.8.0/troposphere/validators/elasticache.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/elasticbeanstalk.py` & `troposphere-4.8.0/troposphere/validators/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/elasticloadbalancing.py` & `troposphere-4.8.0/troposphere/validators/elasticloadbalancing.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/elasticloadbalancingv2.py` & `troposphere-4.8.0/troposphere/validators/elasticloadbalancingv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/elasticsearch.py` & `troposphere-4.8.0/troposphere/validators/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/emr.py` & `troposphere-4.8.0/troposphere/validators/emr.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/firehose.py` & `troposphere-4.8.0/troposphere/validators/firehose.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/fsx.py` & `troposphere-4.8.0/troposphere/validators/fsx.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/globalaccelerator.py` & `troposphere-4.8.0/troposphere/validators/globalaccelerator.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/glue.py` & `troposphere-4.8.0/troposphere/validators/glue.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/iam.py` & `troposphere-4.8.0/troposphere/validators/iam.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/imagebuilder.py` & `troposphere-4.8.0/troposphere/validators/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/iottwinmaker.py` & `troposphere-4.8.0/troposphere/validators/iottwinmaker.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/kinesis.py` & `troposphere-4.8.0/troposphere/validators/kinesis.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/kinesisanalyticsv2.py` & `troposphere-4.8.0/troposphere/validators/kinesisanalyticsv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/kms.py` & `troposphere-4.8.0/troposphere/validators/kms.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/logs.py` & `troposphere-4.8.0/troposphere/validators/logs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/macie.py` & `troposphere-4.8.0/troposphere/validators/macie.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/opensearchservice.py` & `troposphere-4.8.0/troposphere/validators/opensearchservice.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/opsworks.py` & `troposphere-4.8.0/troposphere/validators/opsworks.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/rds.py` & `troposphere-4.8.0/troposphere/validators/rds.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/rekognition.py` & `troposphere-4.8.0/troposphere/validators/rekognition.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/resiliencehub.py` & `troposphere-4.8.0/troposphere/validators/resiliencehub.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/route53.py` & `troposphere-4.8.0/troposphere/validators/route53.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/s3.py` & `troposphere-4.8.0/troposphere/validators/s3.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/scheduler.py` & `troposphere-4.8.0/troposphere/validators/scheduler.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/secretsmanager.py` & `troposphere-4.8.0/troposphere/validators/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/sqs.py` & `troposphere-4.8.0/troposphere/validators/sqs.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/ssm.py` & `troposphere-4.8.0/troposphere/validators/ssm.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/transfer.py` & `troposphere-4.8.0/troposphere/validators/transfer.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/validators/wafv2.py` & `troposphere-4.8.0/troposphere/validators/wafv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/verifiedpermissions.py` & `troposphere-4.8.0/troposphere/verifiedpermissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,32 @@
 #
 # *** Do not modify - this file is autogenerated ***
 
 
 from . import AWSObject, AWSProperty, PropsDictType
 
 
+class CognitoGroupConfiguration(AWSProperty):
+    """
+    `CognitoGroupConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-verifiedpermissions-identitysource-cognitogroupconfiguration.html>`__
+    """
+
+    props: PropsDictType = {
+        "GroupEntityType": (str, True),
+    }
+
+
 class CognitoUserPoolConfiguration(AWSProperty):
     """
     `CognitoUserPoolConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-verifiedpermissions-identitysource-cognitouserpoolconfiguration.html>`__
     """
 
     props: PropsDictType = {
         "ClientIds": ([str], False),
+        "GroupConfiguration": (CognitoGroupConfiguration, False),
         "UserPoolArn": (str, True),
     }
 
 
 class IdentitySourceConfiguration(AWSProperty):
     """
     `IdentitySourceConfiguration <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-verifiedpermissions-identitysource-identitysourceconfiguration.html>`__
@@ -144,20 +155,7 @@
     resource_type = "AWS::VerifiedPermissions::PolicyTemplate"
 
     props: PropsDictType = {
         "Description": (str, False),
         "PolicyStoreId": (str, True),
         "Statement": (str, True),
     }
-
-
-class IdentitySourceDetails(AWSProperty):
-    """
-    `IdentitySourceDetails <http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-verifiedpermissions-identitysource-identitysourcedetails.html>`__
-    """
-
-    props: PropsDictType = {
-        "ClientIds": ([str], False),
-        "DiscoveryUrl": (str, False),
-        "OpenIdIssuer": (str, False),
-        "UserPoolArn": (str, False),
-    }
```

### Comparing `troposphere-4.7.0/troposphere/voiceid.py` & `troposphere-4.8.0/troposphere/voiceid.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/vpclattice.py` & `troposphere-4.8.0/troposphere/vpclattice.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/waf.py` & `troposphere-4.8.0/troposphere/waf.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/wafregional.py` & `troposphere-4.8.0/troposphere/wafregional.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/wafv2.py` & `troposphere-4.8.0/troposphere/wafv2.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/wisdom.py` & `troposphere-4.8.0/troposphere/wisdom.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/workspaces.py` & `troposphere-4.8.0/troposphere/workspaces.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere/workspacesweb.py` & `troposphere-4.8.0/troposphere/workspacesweb.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,17 @@
 
     props: PropsDictType = {
         "AdditionalEncryptionContext": (dict, False),
         "AuthenticationType": (str, False),
         "BrowserSettingsArn": (str, False),
         "CustomerManagedKey": (str, False),
         "DisplayName": (str, False),
+        "InstanceType": (str, False),
         "IpAccessSettingsArn": (str, False),
+        "MaxConcurrentSessions": (double, False),
         "NetworkSettingsArn": (str, False),
         "Tags": (Tags, False),
         "TrustStoreArn": (str, False),
         "UserAccessLoggingSettingsArn": (str, False),
         "UserSettingsArn": (str, False),
     }
```

### Comparing `troposphere-4.7.0/troposphere/xray.py` & `troposphere-4.8.0/troposphere/xray.py`

 * *Files identical despite different names*

### Comparing `troposphere-4.7.0/troposphere.egg-info/PKG-INFO` & `troposphere-4.8.0/troposphere.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troposphere
-Version: 4.7.0
+Version: 4.8.0
 Summary: AWS CloudFormation creation library
 Home-page: https://github.com/cloudtools/troposphere
 Author: Mark Peek
 Author-email: mark@peek.org
 License: New BSD license
 Project-URL: Changelog, https://github.com/cloudtools/troposphere/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/cloudtools/troposphere
```

### Comparing `troposphere-4.7.0/troposphere.egg-info/SOURCES.txt` & `troposphere-4.8.0/troposphere.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -172,29 +172,33 @@
 troposphere/autoscaling.py
 troposphere/autoscalingplans.py
 troposphere/awslambda.py
 troposphere/b2bi.py
 troposphere/backup.py
 troposphere/backupgateway.py
 troposphere/batch.py
+troposphere/bcmdataexports.py
+troposphere/bedrock.py
 troposphere/billingconductor.py
 troposphere/budgets.py
 troposphere/cassandra.py
 troposphere/ce.py
 troposphere/certificatemanager.py
 troposphere/chatbot.py
 troposphere/cleanrooms.py
+troposphere/cleanroomsml.py
 troposphere/cloud9.py
 troposphere/cloudformation.py
 troposphere/cloudfront.py
 troposphere/cloudtrail.py
 troposphere/cloudwatch.py
 troposphere/codeartifact.py
 troposphere/codebuild.py
 troposphere/codecommit.py
+troposphere/codeconnections.py
 troposphere/codedeploy.py
 troposphere/codeguruprofiler.py
 troposphere/codegurureviewer.py
 troposphere/codepipeline.py
 troposphere/codestar.py
 troposphere/codestarconnections.py
 troposphere/codestarnotifications.py
@@ -209,14 +213,15 @@
 troposphere/cur.py
 troposphere/customerprofiles.py
 troposphere/databrew.py
 troposphere/datapipeline.py
 troposphere/datasync.py
 troposphere/datazone.py
 troposphere/dax.py
+troposphere/deadline.py
 troposphere/detective.py
 troposphere/devopsguru.py
 troposphere/directoryservice.py
 troposphere/dlm.py
 troposphere/dms.py
 troposphere/docdb.py
 troposphere/docdbelastic.py
@@ -313,14 +318,15 @@
 troposphere/opensearchserverless.py
 troposphere/opensearchservice.py
 troposphere/opsworks.py
 troposphere/opsworkscm.py
 troposphere/organizations.py
 troposphere/osis.py
 troposphere/panorama.py
+troposphere/paymentcryptography.py
 troposphere/pcaconnectorad.py
 troposphere/personalize.py
 troposphere/pinpoint.py
 troposphere/pinpointemail.py
 troposphere/pipes.py
 troposphere/policies.py
 troposphere/proton.py
@@ -334,27 +340,29 @@
 troposphere/rekognition.py
 troposphere/resiliencehub.py
 troposphere/resourceexplorer2.py
 troposphere/resourcegroups.py
 troposphere/robomaker.py
 troposphere/rolesanywhere.py
 troposphere/route53.py
+troposphere/route53profiles.py
 troposphere/route53recoverycontrol.py
 troposphere/route53recoveryreadiness.py
 troposphere/route53resolver.py
 troposphere/rum.py
 troposphere/s3.py
 troposphere/s3express.py
 troposphere/s3objectlambda.py
 troposphere/s3outposts.py
 troposphere/sagemaker.py
 troposphere/scheduler.py
 troposphere/sdb.py
 troposphere/secretsmanager.py
 troposphere/securityhub.py
+troposphere/securitylake.py
 troposphere/serverless.py
 troposphere/servicecatalog.py
 troposphere/servicecatalogappregistry.py
 troposphere/servicediscovery.py
 troposphere/ses.py
 troposphere/shield.py
 troposphere/signer.py
```

