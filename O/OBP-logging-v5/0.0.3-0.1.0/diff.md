# Comparing `tmp/OBP_logging_v5-0.0.3.tar.gz` & `tmp/OBP_logging_v5-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_logging_v5-0.0.3.tar", last modified: Thu Feb  2 13:04:56 2023, max compression
+gzip compressed data, was "OBP_logging_v5-0.1.0.tar", last modified: Fri Aug  4 07:29:44 2023, max compression
```

## Comparing `OBP_logging_v5-0.0.3.tar` & `OBP_logging_v5-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-02 13:04:56.232705 OBP_logging_v5-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-02-02 13:04:56.201450 OBP_logging_v5-0.0.3/OBP_logging_v5/
--rw-rw-rw-   0        0        0     3669 2023-02-02 13:02:12.000000 OBP_logging_v5-0.0.3/OBP_logging_v5/__init__.py
--rw-rw-rw-   0        0        0     4286 2023-01-25 05:47:41.000000 OBP_logging_v5-0.0.3/OBP_logging_v5/cloudwatch.py
--rw-rw-rw-   0        0        0     2131 2023-02-01 10:06:17.000000 OBP_logging_v5-0.0.3/OBP_logging_v5/ec2.py
--rw-rw-rw-   0        0        0     7485 2023-02-01 05:35:22.000000 OBP_logging_v5-0.0.3/OBP_logging_v5/rds.py
--rw-rw-rw-   0        0        0     4616 2023-02-01 10:05:04.000000 OBP_logging_v5-0.0.3/OBP_logging_v5/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:04:56.232705 OBP_logging_v5-0.0.3/OBP_logging_v5.egg-info/
--rw-rw-rw-   0        0        0      373 2023-02-02 13:04:56.000000 OBP_logging_v5-0.0.3/OBP_logging_v5.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-02-02 13:04:56.000000 OBP_logging_v5-0.0.3/OBP_logging_v5.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-02 13:04:56.000000 OBP_logging_v5-0.0.3/OBP_logging_v5.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-02-02 13:04:56.000000 OBP_logging_v5-0.0.3/OBP_logging_v5.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      373 2023-02-02 13:04:56.232705 OBP_logging_v5-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-25 05:47:41.000000 OBP_logging_v5-0.0.3/README.md
--rw-rw-rw-   0        0        0      554 2023-02-02 13:02:22.000000 OBP_logging_v5-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-02 13:04:56.232705 OBP_logging_v5-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 07:29:44.298233 OBP_logging_v5-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-08-04 07:29:44.256281 OBP_logging_v5-0.1.0/OBP_logging_v5/
+-rw-rw-rw-   0        0        0     6276 2023-08-04 07:23:27.000000 OBP_logging_v5-0.1.0/OBP_logging_v5/__init__.py
+-rw-rw-rw-   0        0        0     4342 2023-08-04 07:23:27.000000 OBP_logging_v5-0.1.0/OBP_logging_v5/cloudwatch.py
+-rw-rw-rw-   0        0        0     2159 2023-08-04 07:23:27.000000 OBP_logging_v5-0.1.0/OBP_logging_v5/ec2.py
+-rw-rw-rw-   0        0        0     7597 2023-08-04 07:23:27.000000 OBP_logging_v5-0.1.0/OBP_logging_v5/rds.py
+-rw-rw-rw-   0        0        0     4756 2023-08-04 07:26:29.000000 OBP_logging_v5-0.1.0/OBP_logging_v5/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:29:44.291934 OBP_logging_v5-0.1.0/OBP_logging_v5.egg-info/
+-rw-rw-rw-   0        0        0      373 2023-08-04 07:29:44.000000 OBP_logging_v5-0.1.0/OBP_logging_v5.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-08-04 07:29:44.000000 OBP_logging_v5-0.1.0/OBP_logging_v5.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:29:44.000000 OBP_logging_v5-0.1.0/OBP_logging_v5.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 07:29:44.000000 OBP_logging_v5-0.1.0/OBP_logging_v5.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-04 07:29:44.000000 OBP_logging_v5-0.1.0/OBP_logging_v5.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      373 2023-08-04 07:29:44.296733 OBP_logging_v5-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-25 05:47:41.000000 OBP_logging_v5-0.1.0/README.md
+-rw-rw-rw-   0        0        0      603 2023-08-04 07:19:13.000000 OBP_logging_v5-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:29:44.299258 OBP_logging_v5-0.1.0/setup.cfg
```

### Comparing `OBP_logging_v5-0.0.3/OBP_logging_v5/cloudwatch.py` & `OBP_logging_v5-0.1.0/OBP_logging_v5/cloudwatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # checks the compliance for cloudwatch-log-group-encrypted
 def log_group_encrypted(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside cloudwatch :: log_group_encrypted()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.18'
     compliance_type = 'Cloudwatch log group encrypted'
     description = 'Checks if a log group in Amazon CloudWatch Logs is encrypted with an AWS Key Management Service (' \
@@ -68,14 +69,15 @@
 # compliance check for cloudwatch log group retention period
 def log_group_retention_period_check(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside cloudwatch :: log_group_retention_period_check()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.22'
     compliance_type = 'Cloudwatch log group retention period check'
     description = 'Checks if Amazon CloudWatch LogGroup retention period is set to specific number of days (<=30)'
```

### Comparing `OBP_logging_v5-0.0.3/OBP_logging_v5/ec2.py` & `OBP_logging_v5-0.1.0/OBP_logging_v5/ec2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def ec2_instance_no_public_ip(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_instance_no_public_ip()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.32'
     compliance_type = 'Ec2 Instance No Public Ip'
     description = 'Checks whether Amazon Elastic Compute Cloud (Amazon EC2) instances have a public IP association. ' \
```

### Comparing `OBP_logging_v5-0.0.3/OBP_logging_v5/rds.py` & `OBP_logging_v5-0.1.0/OBP_logging_v5/rds.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # checks compliance for rds logging enabled
 def rds_logging_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside rds :: rds_logging_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.77'
     compliance_type = 'RDS Logging Enabled'
     description = 'Checks that respective logs of Amazon Relational Database Service (Amazon RDS) are enabled'
@@ -65,14 +66,15 @@
 def rds_cluster_deletion_protection_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside rds :: rds_cluster_deletion_protection_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id5.13'
     compliance_type = 'Rds Cluster Deletion Protection Enabled'
     description = 'Checks if an Amazon Relational Database Service (Amazon RDS) cluster has deletion protection enabled'
@@ -114,14 +116,15 @@
 def rds_cluster_multi_az_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :param kwargs:
     :return:
     """
     logger.info(" ---Inside rds :: rds_cluster_multi_az_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id5.14'
     compliance_type = 'Rds Cluster Multi Az Enabled'
     description = 'Checks if an Amazon Relational Database Service (Amazon RDS) cluster has Multi-AZ replication ' \
@@ -163,14 +166,15 @@
 # checks compliance for RdsInstanceIamAuthenticationEnabled
 def rds_instance_iam_authentication_enabled(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside rds :: rds_instance_iam_authentication_enabled()--- ")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id5.15'
     compliance_type = 'Rds Instance Iam Authentication Enabled'
     description = "Checks if an Amazon Relational Database Service (Amazon RDS) instance has AWS Identity and Access " \
```

### Comparing `OBP_logging_v5-0.0.3/OBP_logging_v5/utils.py` & `OBP_logging_v5-0.1.0/OBP_logging_v5/utils.py`

 * *Files 6% similar despite different names*

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
 def list_log_groups(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_log_groups()--- ")
+    self.refresh_session()
 
     log_groups = {}
 
     for region in regions:
         # Connect to the cloudwatch log service
         client = self.session.client('logs', region_name=region)
         marker = ''
@@ -71,14 +73,15 @@
 def list_rds_instances(self, regions: list) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_rds_instances()--- ")
+    self.refresh_session()
     rds_list = {}
 
     for region in regions:
         client = self.session.client('rds', region_name=region)
         marker = ''
         while True:
             if marker == '':
@@ -103,14 +106,15 @@
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
@@ -136,14 +140,15 @@
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
```

### Comparing `OBP_logging_v5-0.0.3/pyproject.toml` & `OBP_logging_v5-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "OBP_logging_v5"
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
+
 
 #[project.urls]
 #"Homepage" = ""
 #"Bug Tracker" = ""
```

