# Comparing `tmp/aws_obp_1-0.0.3.tar.gz` & `tmp/aws_obp_1-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_obp_1-0.0.3.tar", last modified: Thu Jul 27 17:04:01 2023, max compression
+gzip compressed data, was "aws_obp_1-0.1.0.tar", last modified: Fri Aug  4 05:06:47 2023, max compression
```

## Comparing `aws_obp_1-0.0.3.tar` & `aws_obp_1-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 17:04:01.818030 aws_obp_1-0.0.3/
--rw-rw-rw-   0        0        0      368 2023-07-27 17:04:01.817031 aws_obp_1-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 05:16:17.000000 aws_obp_1-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 17:04:01.804845 aws_obp_1-0.0.3/aws_obp_1/
--rw-rw-rw-   0        0        0     6263 2023-07-27 16:59:10.000000 aws_obp_1-0.0.3/aws_obp_1/__init__.py
--rw-rw-rw-   0        0        0     6203 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/auto_scaling.py
--rw-rw-rw-   0        0        0     5991 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/ec2.py
--rw-rw-rw-   0        0        0     2478 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/lambda_fn.py
--rw-rw-rw-   0        0        0    13805 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/lb.py
--rw-rw-rw-   0        0        0     1831 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/rds.py
--rw-rw-rw-   0        0        0     4895 2023-07-27 16:59:10.000000 aws_obp_1-0.0.3/aws_obp_1/s3.py
--rw-rw-rw-   0        0        0     8969 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 17:04:01.815030 aws_obp_1-0.0.3/aws_obp_1.egg-info/
--rw-rw-rw-   0        0        0      368 2023-07-27 17:04:01.000000 aws_obp_1-0.0.3/aws_obp_1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-27 17:04:01.000000 aws_obp_1-0.0.3/aws_obp_1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 17:04:01.000000 aws_obp_1-0.0.3/aws_obp_1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 17:04:01.000000 aws_obp_1-0.0.3/aws_obp_1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      549 2023-07-27 16:59:10.000000 aws_obp_1-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 17:04:01.819030 aws_obp_1-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:47.092528 aws_obp_1-0.1.0/
+-rw-rw-rw-   0        0        0      368 2023-08-04 05:06:47.089530 aws_obp_1-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 05:16:17.000000 aws_obp_1-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:47.069557 aws_obp_1-0.1.0/aws_obp_1/
+-rw-rw-rw-   0        0        0     8872 2023-08-04 05:04:41.000000 aws_obp_1-0.1.0/aws_obp_1/__init__.py
+-rw-rw-rw-   0        0        0     6287 2023-08-03 16:43:38.000000 aws_obp_1-0.1.0/aws_obp_1/auto_scaling.py
+-rw-rw-rw-   0        0        0     6075 2023-08-03 16:43:38.000000 aws_obp_1-0.1.0/aws_obp_1/ec2.py
+-rw-rw-rw-   0        0        0     2506 2023-08-03 16:43:38.000000 aws_obp_1-0.1.0/aws_obp_1/lambda_fn.py
+-rw-rw-rw-   0        0        0    13945 2023-08-03 16:43:38.000000 aws_obp_1-0.1.0/aws_obp_1/lb.py
+-rw-rw-rw-   0        0        0     1859 2023-08-03 16:43:38.000000 aws_obp_1-0.1.0/aws_obp_1/rds.py
+-rw-rw-rw-   0        0        0     4951 2023-08-03 16:43:38.000000 aws_obp_1-0.1.0/aws_obp_1/s3.py
+-rw-rw-rw-   0        0        0     9249 2023-08-03 16:43:38.000000 aws_obp_1-0.1.0/aws_obp_1/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:47.085675 aws_obp_1-0.1.0/aws_obp_1.egg-info/
+-rw-rw-rw-   0        0        0      368 2023-08-04 05:06:46.000000 aws_obp_1-0.1.0/aws_obp_1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-08-04 05:06:46.000000 aws_obp_1-0.1.0/aws_obp_1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 05:06:46.000000 aws_obp_1-0.1.0/aws_obp_1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 05:06:46.000000 aws_obp_1-0.1.0/aws_obp_1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 05:06:46.000000 aws_obp_1-0.1.0/aws_obp_1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      596 2023-08-04 05:06:09.000000 aws_obp_1-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 05:06:47.092528 aws_obp_1-0.1.0/setup.cfg
```

### Comparing `aws_obp_1-0.0.3/aws_obp_1/__init__.py` & `aws_obp_1-0.1.0/aws_obp_1/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,97 @@
+import datetime
+
+import boto3
+import pytz
 from boto3 import session
 import logging
 
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Klera DevOps'
-__version__ = '0.0.3'
+__version__ = '0.1.0'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
-            self.session = session.Session(
-                aws_access_key_id=kwargs['aws_access_key_id'],
-                aws_secret_access_key=kwargs['aws_secret_access_key'],
-            )
+            if 'iam_role_to_assume' in kwargs.keys():
+                self.iam_role_to_assume = kwargs['iam_role_to_assume']
+                self.sts_client = boto3.client(
+                    'sts',
+                    aws_access_key_id=kwargs['aws_access_key_id'],
+                    aws_secret_access_key=kwargs['aws_secret_access_key'],
+                )
+                self.creds = self.sts_client.assume_role(
+                    RoleArn=self.iam_role_to_assume,
+                    RoleSessionName='RecommenderSession',
+                    DurationSeconds=3600
+                )
+                self.session = session.Session(
+                    aws_access_key_id=self.creds['Credentials']['AccessKeyId'],
+                    aws_secret_access_key=self.creds['Credentials']['SecretAccessKey'],
+                    aws_session_token=self.creds['Credentials']['SessionToken']
+                )
+            else:
+                self.session = session.Session(
+                    aws_access_key_id=kwargs['aws_access_key_id'],
+                    aws_secret_access_key=kwargs['aws_secret_access_key'],
+                )
         elif 'profile_name' in kwargs.keys():
             self.session = session.Session(profile_name=kwargs['profile_name'])
+        elif 'iam_role_to_assume' in kwargs.keys():
+            self.iam_role_to_assume = kwargs['iam_role_to_assume']
+            self.sts_client = boto3.client('sts')
+            self.creds = self.sts_client.assume_role(
+                RoleArn=kwargs['iam_role_to_assume'],
+                RoleSessionName='RecommenderSession',
+                DurationSeconds=3600
+            )
+            self.session = session.Session(
+                aws_access_key_id=self.creds['Credentials']['AccessKeyId'],
+                aws_secret_access_key=self.creds['Credentials']['SecretAccessKey'],
+                aws_session_token=self.creds['Credentials']['SessionToken']
+            )
 
     from .utils import get_regions, list_rds_clusters, list_ec2_instances, list_eni, list_security_groups, \
         list_lambda_functions, list_elbv2, list_auto_scaling_groups, list_as_launch_configs, list_elb
     from .rds import rds_cluster_iam_authentication_enabled
     from .ec2 import ec2_token_hop_limit_check, ec2_security_group_attached_to_eni, ec2_instance_role_assigned
     from .s3 import alarm_s3_bucket_policy_change, s3_lifecycle_policy_check
     from .lambda_fn import lambda_function_settings_check
     from .lb import alb_http_drop_invalid_header_enabled, alb_waf_enabled, elbv2_multiple_az, \
         elbv2_acm_certificate_required, clb_multiple_az
     from .auto_scaling import auto_scaling_multiple_az, auto_scaling_launch_config_requires_imdsv2, \
         auto_scaling_launch_config_hop_limit
 
+    # refresh session
+    def refresh_session(self):
+        try:
+            self.sts_client
+        except AttributeError:
+            logger.info('No need to refresh the session!')
+            return
+        remaining_duration_seconds = (
+                self.creds['Credentials']['Expiration'] - datetime.datetime.now(pytz.utc)).total_seconds()
+
+        if remaining_duration_seconds < 900:
+            self.creds = self.sts_client.assume_role(
+                RoleArn=self.iam_role_to_assume,
+                RoleSessionName='RecommenderSession',
+                DurationSeconds=3600
+            )
+            self.session = session.Session(
+                aws_access_key_id=self.creds['Credentials']['AccessKeyId'],
+                aws_secret_access_key=self.creds['Credentials']['SecretAccessKey'],
+                aws_session_token=self.creds['Credentials']['SessionToken']
+            )
+
     def get_compliance(self) -> list:
         """
         :return:
         """
         regions = self.get_regions()
 
         compliance = []
```

### Comparing `aws_obp_1-0.0.3/aws_obp_1/auto_scaling.py` & `aws_obp_1-0.1.0/aws_obp_1/auto_scaling.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def auto_scaling_multiple_az(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside auto_scaling :: auto_scaling_multiple_az()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id85.4'
     compliance_type = 'Auto Scaling Multiple AZ'
     description = "Checks if the Auto Scaling group spans multiple Availability Zones. The rule is NON_COMPLIANT " \
@@ -62,14 +63,15 @@
 def auto_scaling_launch_config_requires_imdsv2(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside auto_scaling :: auto_scaling_launch_config_requires_imdsv2()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id85.3'
     compliance_type = 'Auto Scaling Launch Configuration Requires IMDSV2'
     description = "Checks whether only IMDSv2 is enabled. This rule is NON_COMPLIANT if the " \
@@ -120,14 +122,15 @@
 def auto_scaling_launch_config_hop_limit(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside auto_scaling :: auto_scaling_launch_config_hop_limit--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id85.2'
     compliance_type = 'Auto Scaling Launch Configuration Hop Limit'
     description = "Checks the number of network hops that the metadata token can travel. This rule is NON_COMPLIANT " \
```

### Comparing `aws_obp_1-0.0.3/aws_obp_1/ec2.py` & `aws_obp_1-0.1.0/aws_obp_1/ec2.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def ec2_token_hop_limit_check(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_token_hop_limit_check--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id45.2'
     compliance_type = 'EC2 Token hop limit check'
     description = "Checks if an Amazon Elastic Compute Cloud (EC2) instance metadata has a specified token hop limit " \
@@ -69,14 +70,15 @@
 def ec2_security_group_attached_to_eni(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_security_group_attached_to_eni()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id18.2'
     compliance_type = 'EC2 Security Group Attached to ENI'
     description = "Checks if non-default security groups are attached to Elastic network interfaces (ENIs). The rule " \
@@ -128,14 +130,15 @@
 def ec2_instance_role_assigned(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_instance_role_assigned--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id26.1'
     compliance_type = 'EC2 Instance Role Assigned'
     description = "Checks if an Amazon Elastic Compute Cloud (EC2) instance has role assigned"
```

### Comparing `aws_obp_1-0.0.3/aws_obp_1/lambda_fn.py` & `aws_obp_1-0.1.0/aws_obp_1/lambda_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def lambda_function_settings_check(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside lambda_fn :: lambda_function_settings_check()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id93.1'
     compliance_type = 'Lambda function settings check'
     description = "Checks if the AWS Lambda function settings for runtime, role, timeout, and memory size match " \
```

### Comparing `aws_obp_1-0.0.3/aws_obp_1/lb.py` & `aws_obp_1-0.1.0/aws_obp_1/lb.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 def alb_http_drop_invalid_header_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside lb :: alb_http_drop_invalid_header_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.4'
     compliance_type = 'ALB HTTP drop invalid header enabled'
     description = "Checks if rule evaluates AWS Application Load Balancers (ALB) to ensure they are configured to " \
@@ -71,14 +72,15 @@
 def alb_waf_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside lb :: alb_waf_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.6'
     compliance_type = 'ALB WAF Enabled'
     description = "Checks if Web Application Firewall (WAF) is enabled on Application Load Balancers (ALBs). " \
@@ -136,14 +138,15 @@
 def elbv2_multiple_az(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside lb :: elbv2_multiple_az()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id30.4'
     compliance_type = 'ELBV2 Multiple AZ'
     description = "Checks if an Elastic Load Balancer V2 (Application, Network, or Gateway Load Balancer) has " \
@@ -187,14 +190,15 @@
 def elbv2_acm_certificate_required(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside lb :: elbv2_acm_certificate_required()---  ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.51'
     compliance_type = 'ELBV2 ACM Certificate Required'
     description = "Checks if Application Load Balancers and Network Load Balancers have listeners that are " \
@@ -268,14 +272,15 @@
 def clb_multiple_az(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside lb :: clb_multiple_az()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id56.3'
     compliance_type = 'CLB Multiple AZ'
     description = "Checks if a Classic Load Balancer spans multiple Availability Zones (AZs). The rule is " \
```

### Comparing `aws_obp_1-0.0.3/aws_obp_1/rds.py` & `aws_obp_1-0.1.0/aws_obp_1/rds.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def rds_cluster_iam_authentication_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside rds :: rds_cluster_iam_authentication_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id95.1'
     compliance_type = 'Rds Cluster Iam Authentication Enabled'
     description = "Checks if an Amazon RDS Cluster has AWS Identity and Access Management (IAM) authentication enabled"
```

### Comparing `aws_obp_1-0.0.3/aws_obp_1/s3.py` & `aws_obp_1-0.1.0/aws_obp_1/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # Checks compliance for Alarm s3 bucket policy change
 def alarm_s3_bucket_policy_change(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside s3 :: alarm_s3_bucket_policy_change()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id25.17'
     compliance_type = 'Alarm S3 Bucket Policy Change'
     description = "Ensure there is an Amazon CloudWatch alarm created and configured in your AWS account " \
@@ -65,14 +66,15 @@
 # Checks compliance for s3 lifecycle policy check
 def s3_lifecycle_policy_check(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside s3 :: s3_lifecycle_policy_check()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id65.2'
     compliance_type = 'S3 lifecycle policy check'
     description = "Checks if a lifecycle rule is configured for an Amazon Simple Storage Service (Amazon S3) bucket. " \
```

### Comparing `aws_obp_1-0.0.3/aws_obp_1/utils.py` & `aws_obp_1-0.1.0/aws_obp_1/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def get_regions(self):
     logger.info(" ---Inside utils :: get_regions()--- ")
+    self.refresh_session()
     """Summary
 
     Returns:
         TYPE: Description
     """
 
     client = self.session.client('ec2', region_name='us-east-1')
@@ -34,14 +35,15 @@
 def list_rds_clusters(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_rds_clusters()--- ")
+    self.refresh_session()
 
     cluster_lst = {}
 
     for region in regions:
         client = self.session.client('rds', region_name=region)
         marker = ''
         while True:
@@ -67,14 +69,15 @@
 def list_ec2_instances(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_ec2_instances()--- ")
+    self.refresh_session()
 
     instances = {}
 
     for region in regions:
         client = self.session.client('ec2', region_name=region)
         marker = ''
         while True:
@@ -100,14 +103,15 @@
 def list_security_groups(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_security_groups()--- ")
+    self.refresh_session()
 
     sg_lst = {}
 
     for region in regions:
         client = self.session.client('ec2', region_name=region)
         marker = ''
         while True:
@@ -132,14 +136,15 @@
 # return the list of ENI
 def list_eni(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
+    self.refresh_session()
     logger.info(" ---Inside utils :: list_eni()--- ")
 
     eni_lst = {}
 
     for region in regions:
         client = self.session.client('ec2', region_name=region)
         marker = ''
@@ -165,14 +170,15 @@
 # returns the list of lambda functions
 def list_lambda_functions(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
+    self.refresh_session()
     logger.info(" ---Inside utils :: list_lambda_functions()--- ")
 
     lambda_list = {}
 
     for region in regions:
         client = self.session.client('lambda', region_name=region)
         marker = ''
@@ -197,14 +203,15 @@
 # returns the list Elastic load balancers
 def list_elbv2(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
+    self.refresh_session()
     logger.info(" ---Inside utils :: list_elbv2()--- ")
 
     elb_lst = {}
 
     for region in regions:
         client = self.session.client('elbv2', region_name=region)
         marker = ''
@@ -230,14 +237,15 @@
 # returns the list of auto scaling groups
 def list_auto_scaling_groups(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
+    self.refresh_session()
     logger.info(" ---Inside utils :: list_auto_scaling_groups()--- ")
 
     asg_lst = {}
 
     for region in regions:
         client = self.session.client('autoscaling', region_name=region)
         marker = ''
@@ -264,14 +272,15 @@
 # returns the list of auto scaling launch configs
 def list_as_launch_configs(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
+    self.refresh_session()
     logger.info(" ---Inside utils :: list_as_launch_configs()--- ")
 
     launch_configs = {}
 
     for region in regions:
         client = self.session.client('autoscaling', region_name=region)
         marker = ''
@@ -297,14 +306,15 @@
 # returns the list Elastic load balancers
 def list_elb(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
+    self.refresh_session()
     logger.info(" ---Inside utils :: list_elb()--- ")
 
     elb_lst = {}
 
     for region in regions:
         client = self.session.client('elb', region_name=region)
         marker = ''
```

### Comparing `aws_obp_1-0.0.3/pyproject.toml` & `aws_obp_1-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_obp_1"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
   { name="ravish.sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "boto3",
+    "pytz"
+]
 
 #[project.urls]
 #"Homepage" = ""
 #"Bug Tracker" = ""
```

