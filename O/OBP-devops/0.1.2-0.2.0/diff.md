# Comparing `tmp/OBP_devops-0.1.2.tar.gz` & `tmp/OBP_devops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_devops-0.1.2.tar", last modified: Thu Jul 27 17:49:33 2023, max compression
+gzip compressed data, was "OBP_devops-0.2.0.tar", last modified: Fri Aug  4 06:02:26 2023, max compression
```

## Comparing `OBP_devops-0.1.2.tar` & `OBP_devops-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 17:49:33.961032 OBP_devops-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-27 17:49:33.940811 OBP_devops-0.1.2/OBP_devops/
--rw-rw-rw-   0        0        0     7208 2023-07-27 17:49:00.000000 OBP_devops-0.1.2/OBP_devops/__init__.py
--rw-rw-rw-   0        0        0     2600 2023-01-27 06:22:26.000000 OBP_devops-0.1.2/OBP_devops/cloudformation.py
--rw-rw-rw-   0        0        0     9072 2023-01-27 06:22:26.000000 OBP_devops-0.1.2/OBP_devops/codebuild.py
--rw-rw-rw-   0        0        0     2632 2023-05-31 12:31:36.000000 OBP_devops-0.1.2/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py
--rw-rw-rw-   0        0        0     3016 2023-05-31 12:31:35.000000 OBP_devops-0.1.2/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py
--rw-rw-rw-   0        0        0     2480 2023-05-31 12:31:35.000000 OBP_devops-0.1.2/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py
--rw-rw-rw-   0        0        0     2365 2023-01-27 05:16:17.000000 OBP_devops-0.1.2/OBP_devops/codepipeline.py
--rw-rw-rw-   0        0        0     4336 2023-01-27 06:22:27.000000 OBP_devops-0.1.2/OBP_devops/ecr.py
--rw-rw-rw-   0        0        0     1906 2023-05-31 12:31:36.000000 OBP_devops-0.1.2/OBP_devops/ecr_private_tag_immutability_enabled.py
--rw-rw-rw-   0        0        0     1849 2023-05-31 12:31:36.000000 OBP_devops-0.1.2/OBP_devops/ecs_container_insights_enabled.py
--rw-rw-rw-   0        0        0     1926 2023-07-20 07:08:22.000000 OBP_devops-0.1.2/OBP_devops/ecs_containers_non_privileged.py
--rw-rw-rw-   0        0        0     2000 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_containers_read_only_access.py
--rw-rw-rw-   0        0        0     2058 2023-05-31 12:31:35.000000 OBP_devops-0.1.2/OBP_devops/ecs_fargate_latest_platform_version.py
--rw-rw-rw-   0        0        0     1951 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_task_definition_memory_hard_limit.py
--rw-rw-rw-   0        0        0     2060 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_task_definition_nonroot_user.py
--rw-rw-rw-   0        0        0     1957 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_task_definition_pid_mode_check.py
--rw-rw-rw-   0        0        0     2156 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_task_definition_user_for_host_mode_check.py
--rw-rw-rw-   0        0        0     4711 2023-01-27 06:22:27.000000 OBP_devops-0.1.2/OBP_devops/eks.py
--rw-rw-rw-   0        0        0     3326 2023-01-30 07:27:29.000000 OBP_devops-0.1.2/OBP_devops/elastic_beanstalk.py
--rw-rw-rw-   0        0        0     6477 2023-05-31 12:13:47.000000 OBP_devops-0.1.2/OBP_devops/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 17:49:33.955032 OBP_devops-0.1.2/OBP_devops.egg-info/
--rw-rw-rw-   0        0        0      369 2023-07-27 17:49:33.000000 OBP_devops-0.1.2/OBP_devops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-07-27 17:49:33.000000 OBP_devops-0.1.2/OBP_devops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 17:49:33.000000 OBP_devops-0.1.2/OBP_devops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 17:49:33.000000 OBP_devops-0.1.2/OBP_devops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-07-27 17:49:33.960030 OBP_devops-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_devops-0.1.2/README.md
--rw-rw-rw-   0        0        0      550 2023-07-27 17:49:00.000000 OBP_devops-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 17:49:33.962030 OBP_devops-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 06:02:26.499070 OBP_devops-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-08-04 06:02:26.425970 OBP_devops-0.2.0/OBP_devops/
+-rw-rw-rw-   0        0        0     9792 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/__init__.py
+-rw-rw-rw-   0        0        0     2628 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/cloudformation.py
+-rw-rw-rw-   0        0        0     9184 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/codebuild.py
+-rw-rw-rw-   0        0        0     2660 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py
+-rw-rw-rw-   0        0        0     3044 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py
+-rw-rw-rw-   0        0        0     2508 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py
+-rw-rw-rw-   0        0        0     2393 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/codepipeline.py
+-rw-rw-rw-   0        0        0     4392 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecr.py
+-rw-rw-rw-   0        0        0     1934 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecr_private_tag_immutability_enabled.py
+-rw-rw-rw-   0        0        0     1877 2023-08-04 05:58:04.000000 OBP_devops-0.2.0/OBP_devops/ecs_container_insights_enabled.py
+-rw-rw-rw-   0        0        0     1954 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecs_containers_non_privileged.py
+-rw-rw-rw-   0        0        0     2028 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecs_containers_read_only_access.py
+-rw-rw-rw-   0        0        0     2086 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecs_fargate_latest_platform_version.py
+-rw-rw-rw-   0        0        0     1979 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecs_task_definition_memory_hard_limit.py
+-rw-rw-rw-   0        0        0     2088 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecs_task_definition_nonroot_user.py
+-rw-rw-rw-   0        0        0     1985 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecs_task_definition_pid_mode_check.py
+-rw-rw-rw-   0        0        0     2184 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/ecs_task_definition_user_for_host_mode_check.py
+-rw-rw-rw-   0        0        0     4767 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/eks.py
+-rw-rw-rw-   0        0        0     3382 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/elastic_beanstalk.py
+-rw-rw-rw-   0        0        0     6673 2023-08-04 05:58:03.000000 OBP_devops-0.2.0/OBP_devops/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:02:26.488929 OBP_devops-0.2.0/OBP_devops.egg-info/
+-rw-rw-rw-   0        0        0      369 2023-08-04 06:02:26.000000 OBP_devops-0.2.0/OBP_devops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2023-08-04 06:02:26.000000 OBP_devops-0.2.0/OBP_devops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 06:02:26.000000 OBP_devops-0.2.0/OBP_devops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 06:02:26.000000 OBP_devops-0.2.0/OBP_devops.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 06:02:26.000000 OBP_devops-0.2.0/OBP_devops.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-08-04 06:02:26.497027 OBP_devops-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_devops-0.2.0/README.md
+-rw-rw-rw-   0        0        0      597 2023-08-04 05:58:04.000000 OBP_devops-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 06:02:26.499070 OBP_devops-0.2.0/setup.cfg
```

### Comparing `OBP_devops-0.1.2/OBP_devops/cloudformation.py` & `OBP_devops-0.2.0/OBP_devops/cloudformation.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def stack_notification_check(self, regions: list) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside cloudformation :: stack_notification_check()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.1'
     compliance_type = "Cloudformation stack notification check"
     description = "Checks whether your CloudFormation stacks are sending event notifications to an SNS topic"
```

### Comparing `OBP_devops-0.1.2/OBP_devops/codebuild.py` & `OBP_devops-0.2.0/OBP_devops/codebuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Checks if an AWS CodeBuild project has encryption enabled for all of its artifacts
 def project_artifact_encryption_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside codebuild :: project_artifact_encryption_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id30.1'
     compliance_type = "Codebuild project artifact encryption enabled"
     description = "Checks if an AWS CodeBuild project has encryption enabled for all of its artifacts"
@@ -77,14 +78,15 @@
 # Checks if an AWS CodeBuild project environment has privileged mode enabled
 def project_environment_privileged_check(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside codebuild :: project_environment_privileged_check()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id30.2'
     compliance_type = "Codebuild project privileged check"
     description = "Checks if an AWS CodeBuild project environment has privileged mode enabled. The rule is " \
@@ -137,14 +139,15 @@
 # Checks if an AWS CodeBuild project environment has at least one log option enabled
 def project_logging_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside codebuild :: project_logging_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id29.1'
     compliance_type = "Codebuild project logging enabled"
     description = "Checks if an AWS CodeBuild project environment has at least one log option enabled. The rule is " \
@@ -204,14 +207,15 @@
 # Checks if an AWS CodeBuild project configured with Amazon S3 Logs has encryption enabled for its logs
 def project_s3_logs_encrypted(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside codebuild :: project_s3_logs_encrypted()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.2'
     compliance_type = "CodeBuild project s3 logs encrypted"
     description = "Checks if an AWS CodeBuild project configured with Amazon S3 Logs has encryption enabled for its " \
```

### Comparing `OBP_devops-0.1.2/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py` & `OBP_devops-0.2.0/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def codedeploy_auto_rollback_monitor_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: codedeploy_auto_rollback_monitor_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.3'
     compliance_type = "codedeploy_auto_rollback_monitor_enabled"
     description = "Checks if the deployment group is configured with automatic deployment rollback and deployment " \
```

### Comparing `OBP_devops-0.1.2/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py` & `OBP_devops-0.2.0/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def codedeploy_ec2_minimum_healthy_hosts_configured(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: codedeploy_ec2_minimum_healthy_hosts_configured()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.4'
     compliance_type = "codedeploy_ec2_minimum_healthy_hosts_configured"
     description = "Checks if the deployment group for EC2/On-Premises Compute Platform is configured with a minimum healthy hosts fleet percentage or host count is greater than or equal to the input threshold. Default:: (minimumHealthyHostsFleetPercent=66) and (minimumHealthyHostsHostCount=1)"
```

### Comparing `OBP_devops-0.1.2/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py` & `OBP_devops-0.2.0/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def codedeploy_lambda_allatonce_traffic_shift_disabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: codedeploy_lambda_allatonce_traffic_shift_disabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.5'
     compliance_type = "codedeploy_lambda_allatonce_traffic_shift_disabled"
     description = "Checks if the deployment group for Lambda Compute Platform is not using the default deployment configuration."
```

### Comparing `OBP_devops-0.1.2/OBP_devops/codepipeline.py` & `OBP_devops-0.2.0/OBP_devops/codepipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 def codepipeline_deployment_count_check(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside codepipeline :: codepipeline_deployment_count_check()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.6'
     compliance_type = "CodePipeline deployment count check"
     description = "Checks whether the first deployment stage of the AWS Codepipeline performs more than one deployment"
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecr.py` & `OBP_devops-0.2.0/OBP_devops/ecr.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 def ecr_private_image_scanning_enabled(self, **kwargs) -> dict:
     """
     :param repo_lst:
     :param self:
     :return:
     """
     logger.info(" ---Inside ecr :: ecr_private_image_scanning_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id30.3'
     compliance_type = "ECR Private Image Scanning Enabled"
     description = "Checks if a private Amazon Elastic Container Registry (ECR) repository has image scanning enabled"
@@ -69,14 +70,15 @@
 def ecr_private_lifecycle_policy_configured(self, **kwargs) -> dict:
     """
     :param self:
     :param repo_lst:
     :return:
     """
     logger.info(" ---Inside ecr :: ecr_private_lifecycle_policy_configured()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.8'
     compliance_type = "ECR Private lifecycle policy configured"
     description = "Checks if a private Amazon Elastic Container Registry (ECR) repository has at least one lifecycle " \
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecr_private_tag_immutability_enabled.py` & `OBP_devops-0.2.0/OBP_devops/ecr_private_tag_immutability_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def ecr_private_tag_immutability_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecr_private_tag_immutability_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id44.9'
     compliance_type = "ecr_private_tag_immutability_enabled"
     description = "Checks if a private Amazon Elastic Container Registry (ECR) repository has tag immutability enabled."
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecs_container_insights_enabled.py` & `OBP_devops-0.2.0/OBP_devops/ecs_container_insights_enabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def ecs_container_insights_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_container_insights_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.1'
     compliance_type = "ecs_container_insights_enabled"
     description = "Checks if Amazon Elastic Container Service clusters have container insights enabled."
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecs_containers_non_privileged.py` & `OBP_devops-0.2.0/OBP_devops/ecs_containers_non_privileged.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def ecs_containers_non_privileged(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_containers_non_privileged()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.2'
     compliance_type = "ecs_containers_non_privileged"
     description = "Checks if the privileged parameter in the container definition of ECSTaskDefinitions is set to ‘true’. "
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecs_containers_read_only_access.py` & `OBP_devops-0.2.0/OBP_devops/ecs_containers_read_only_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def ecs_containers_read_only_access(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_containers_read_only_access()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.3'
     compliance_type = "ecs_containers_read_only_access"
     description = "Checks if Amazon Elastic Container Service (Amazon ECS) Containers only have read-only access to " \
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecs_fargate_latest_platform_version.py` & `OBP_devops-0.2.0/OBP_devops/ecs_fargate_latest_platform_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def ecs_fargate_latest_platform_version(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_fargate_latest_platform_version()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.4'
     compliance_type = "ecs_fargate_latest_platform_version"
     description = "Checks if Amazon Elastic Container Service (ECS) Fargate Services is running on the latest Fargate platform version."
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecs_task_definition_memory_hard_limit.py` & `OBP_devops-0.2.0/OBP_devops/ecs_task_definition_memory_hard_limit.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def ecs_task_definition_memory_hard_limit(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_task_definition_memory_hard_limit()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.6'
     compliance_type = "ecs_task_definition_memory_hard_limit"
     description = "Checks if ECS task definitions have a set memory limit for its container definitions. "
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecs_task_definition_nonroot_user.py` & `OBP_devops-0.2.0/OBP_devops/ecs_task_definition_nonroot_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def ecs_task_definition_nonroot_user(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_taskdefinition_nonroot_user()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.7'
     compliance_type = "ecs_task_definition_nonroot_user"
     description = "Checks if Amazon Elastic Container Service (Amazon ECS) Containers only have read-only access to its root filesystems. . "
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecs_task_definition_pid_mode_check.py` & `OBP_devops-0.2.0/OBP_devops/ecs_task_definition_pid_mode_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def ecs_task_definition_pid_mode_check(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_task_definition_pid_mode_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.8'
     compliance_type = "ecs_task_definition_pid_mode_check"
     description = "Checks if ECSTaskDefinitions are configured to share a host’s process namespace with its Amazon " \
```

### Comparing `OBP_devops-0.1.2/OBP_devops/ecs_task_definition_user_for_host_mode_check.py` & `OBP_devops-0.2.0/OBP_devops/ecs_task_definition_user_for_host_mode_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def ecs_task_definition_user_for_host_mode_check(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP DevOps :: ecs_task_definition_user_for_host_mode_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.38'
     compliance_type = "ecs_task_definition_user_for_host_mode_check"
     description = "Checks if an Amazon ECS task definition with host networking mode has 'privileged' or 'user' container definitions. . "
```

### Comparing `OBP_devops-0.1.2/OBP_devops/eks.py` & `OBP_devops-0.2.0/OBP_devops/eks.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     """
     :param exception:
     :param self:
     :param eks_lst:
     :return:
     """
     logger.info(" ---Inside eks :: eks_secrets_encrypted()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.14'
     compliance_type = "EKS secrets encrypted"
     description = "Checks if Amazon Elastic Kubernetes Service clusters are configured to have Kubernetes secrets " \
@@ -81,14 +82,15 @@
 def eks_endpoint_no_public_access(self, **kwargs) -> dict:
     """
     :param self:
     :param eks_lst:
     :return:
     """
     logger.info(" ---Inside eks :: eks_endpoint_no_public_access()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id7.13'
     compliance_type = "EKS endpoint no public access"
     description = "Checks whether Amazon Elastic Kubernetes Service (Amazon EKS) endpoint is not publicly accessible"
```

### Comparing `OBP_devops-0.1.2/OBP_devops/elastic_beanstalk.py` & `OBP_devops-0.2.0/OBP_devops/elastic_beanstalk.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def enhanced_health_reporting_enabled(self, environments: dict) -> dict:
     """
     :param self:
     :param environments:
     :return:
     """
     logger.info(" ---Inside elastic_beanstalk :: enhanced_health_reporting_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.13'
     compliance_type = "Beanstalk Enhanced Health Reporting Enabled"
     description = "Checks if an AWS Elastic Beanstalk environment is configured for enhanced health reporting. The " \
@@ -48,14 +49,15 @@
 def managed_updates_enabled(self, environments: dict) -> dict:
     """
     :param self:
     :param environments:
     :return:
     """
     logger.info(" ---Inside elastic_beanstalk :: managed_updates_enabled()---")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.41'
     compliance_type = 'Elastic Beanstalk managed updates enabled'
     description = 'Checks if managed platform updates in an AWS Elastic Beanstalk environment is enabled'
```

### Comparing `OBP_devops-0.1.2/OBP_devops/utils.py` & `OBP_devops-0.2.0/OBP_devops/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns the list of regions
 def get_regions(self):
     logger.info(" ---Inside utils :: get_regions()--- ")
+    self.refresh_session()
     """Summary
 
     Returns:
         TYPE: Description
     """
 
     client = self.session.client('ec2', region_name='us-east-1')
@@ -36,14 +37,15 @@
 def list_elastic_beanstalk_envs(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_elastic_beanstalk_envs()---")
+    self.refresh_session()
 
     environments = {}
 
     for region in regions:
         try:
             client = self.session.client('elasticbeanstalk', region_name=region)
             marker = ''
@@ -73,14 +75,15 @@
 def list_eks_clusters(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_eks_clusters()--- ")
+    self.refresh_session()
 
     clusters_lst = {}
 
     for region in regions:
         client = self.session.client('eks', region_name=region)
         marker = ''
         while True:
@@ -106,14 +109,15 @@
 def list_ecr_repositories(self, regions: list) -> dict:
     """
     :param self:
     :param region:
     :return:
     """
     logger.info(" ---Inside utils :: list_ecr_repositories()--- ")
+    self.refresh_session()
 
     repos = {}
 
     for region in regions:
         client = self.session.client('ecr', region_name=region)
         marker = ''
         while True:
@@ -139,14 +143,15 @@
 def list_codebuild_projects(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_codebuild_project()--- ")
+    self.refresh_session()
 
     project_lst = {}
 
     for region in regions:
         client = self.session.client('codebuild', region_name=region)
         marker = ''
         while True:
@@ -172,14 +177,15 @@
 def list_code_pipelines(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_code_pipelines()--- ")
+    self.refresh_session()
 
     pipelines = {}
 
     for region in regions:
         try:
             client = self.session.client('codepipeline', region_name=region)
             marker = ''
@@ -208,14 +214,15 @@
 def list_task_definitions(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_task_definitions()--- ")
+    self.refresh_session()
 
     task_definitions = {}
 
     for region in regions:
         client = self.session.client('ecs', region_name=region)
         response = client.list_task_definitions()
```

### Comparing `OBP_devops-0.1.2/OBP_devops.egg-info/SOURCES.txt` & `OBP_devops-0.2.0/OBP_devops.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 OBP_devops/ecs_task_definition_user_for_host_mode_check.py
 OBP_devops/eks.py
 OBP_devops/elastic_beanstalk.py
 OBP_devops/utils.py
 OBP_devops.egg-info/PKG-INFO
 OBP_devops.egg-info/SOURCES.txt
 OBP_devops.egg-info/dependency_links.txt
+OBP_devops.egg-info/requires.txt
 OBP_devops.egg-info/top_level.txt
```

