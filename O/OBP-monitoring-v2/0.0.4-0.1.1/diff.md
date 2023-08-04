# Comparing `tmp/OBP_monitoring_v2-0.0.4.tar.gz` & `tmp/OBP_monitoring_v2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_monitoring_v2-0.0.4.tar", last modified: Thu Jul 27 17:15:26 2023, max compression
+gzip compressed data, was "OBP_monitoring_v2-0.1.1.tar", last modified: Fri Aug  4 07:18:37 2023, max compression
```

## Comparing `OBP_monitoring_v2-0.0.4.tar` & `OBP_monitoring_v2-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 17:15:26.756410 OBP_monitoring_v2-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-27 17:15:26.738415 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/
--rw-rw-rw-   0        0        0     1782 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/__init__.py
--rw-rw-rw-   0        0        0     2133 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/asg_elb_healthcheck_required.py
--rw-rw-rw-   0        0        0     2265 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py
--rw-rw-rw-   0        0        0     1999 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/guard_duty_enabled.py
--rw-rw-rw-   0        0        0     2384 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/lambda_concurrency_check.py
--rw-rw-rw-   0        0        0     1950 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/lambda_dlq_check.py
--rw-rw-rw-   0        0        0     2158 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py
--rw-rw-rw-   0        0        0     2079 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/s3_event_notifications_enabled.py
--rw-rw-rw-   0        0        0     1627 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 17:15:26.752415 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/
--rw-rw-rw-   0        0        0      376 2023-07-27 17:15:26.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-07-27 17:15:26.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 17:15:26.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-27 17:15:26.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      376 2023-07-27 17:15:26.755412 OBP_monitoring_v2-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_monitoring_v2-0.0.4/README.md
--rw-rw-rw-   0        0        0      557 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 17:15:26.756410 OBP_monitoring_v2-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 07:18:37.534961 OBP_monitoring_v2-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-08-04 07:18:37.495502 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/
+-rw-rw-rw-   0        0        0     4389 2023-08-04 07:17:54.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-08-04 06:05:38.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/asg_elb_healthcheck_required.py
+-rw-rw-rw-   0        0        0     2293 2023-08-04 06:05:38.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     2027 2023-08-04 06:05:38.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/guard_duty_enabled.py
+-rw-rw-rw-   0        0        0     2412 2023-08-04 06:05:38.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/lambda_concurrency_check.py
+-rw-rw-rw-   0        0        0     1978 2023-08-04 06:05:38.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/lambda_dlq_check.py
+-rw-rw-rw-   0        0        0     2186 2023-08-04 06:05:38.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     2107 2023-08-04 06:05:38.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/s3_event_notifications_enabled.py
+-rw-rw-rw-   0        0        0     1655 2023-08-04 06:05:38.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:18:37.527792 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-08-04 07:18:37.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-08-04 07:18:37.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:18:37.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 07:18:37.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-04 07:18:37.000000 OBP_monitoring_v2-0.1.1/OBP_monitoring_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      376 2023-08-04 07:18:37.532043 OBP_monitoring_v2-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_monitoring_v2-0.1.1/README.md
+-rw-rw-rw-   0        0        0      604 2023-08-04 07:17:54.000000 OBP_monitoring_v2-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:18:37.535460 OBP_monitoring_v2-0.1.1/setup.cfg
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/asg_elb_healthcheck_required.py` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/asg_elb_healthcheck_required.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def asg_elb_healthcheck_required(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return dict:
     """
     logger.info(" ---Inside autoscaling :: asg_elb_healthcheck_required()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.11'
     compliance_type = "AutoScaling Group ELB health check required"
     description = "Checks if ELB health check is enabled on autoscaling group"
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def ec2_instance_detailed_monitoring_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_instance_detailed_monitoring_enabled")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.30'
     compliance_type = "EC2 instance detailed monitoring enabled"
     description = "Checks if detailed monitoring is enabled for EC2 instances."
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/guard_duty_enabled.py` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/guard_duty_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def guard_duty_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside guard_duty :: guard_duty_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.55'
     compliance_type = "Guard Duty Enabled"
     description = "Checks if Amazon GuardDuty is enabled in your AWS account and region"
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/lambda_concurrency_check.py` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/lambda_concurrency_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def lambda_concurrency_check(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP Monitoring :: lambda_concurrency_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.70'
     compliance_type = "lambda-concurrency-check"
     description = "Checks whether the AWS Lambda function is configured with function-level concurrent execution limit."
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/lambda_dlq_check.py` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/lambda_dlq_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def lambda_dlq_check(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside lambdafn :: lambda_dlq_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id13.1'
     compliance_type = "Lambda DLQ check"
     description = "Checks whether an AWS Lambda function is configured with a dead-letter queue."
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     """
 
     :param regions:
     :param self:
     :return dict: rds enhanced monitoring enabled compliance.py details
     """
     logger.info(" ---Inside rds :: rds_enhanced_monitoring_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.74'
     compliance_type = "RDS instance enhanced monitoring enabled"
     description = "Checks if enhanced monitoring is enabled for RDS instances."
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/s3_event_notifications_enabled.py` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/s3_event_notifications_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def s3_event_notifications_enabled(self):
     """
 
     :param self:
     :return dict:
     """
     logger.info(" ---Inside OBP MMonitoring :: s3_event_notificationsenabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id11.1'
     compliance_type = "S3 event notifications enabled"
     description = "Checks if Amazon S3 Events Notifications are enabled on an S3 bucket."
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/utils.py` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2/utils.py`

 * *Files 2% similar despite different names*

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
```

### Comparing `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/SOURCES.txt` & `OBP_monitoring_v2-0.1.1/OBP_monitoring_v2.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 OBP_monitoring_v2/lambda_dlq_check.py
 OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py
 OBP_monitoring_v2/s3_event_notifications_enabled.py
 OBP_monitoring_v2/utils.py
 OBP_monitoring_v2.egg-info/PKG-INFO
 OBP_monitoring_v2.egg-info/SOURCES.txt
 OBP_monitoring_v2.egg-info/dependency_links.txt
+OBP_monitoring_v2.egg-info/requires.txt
 OBP_monitoring_v2.egg-info/top_level.txt
```

### Comparing `OBP_monitoring_v2-0.0.4/pyproject.toml` & `OBP_monitoring_v2-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "OBP_monitoring_v2"
-version = "0.0.4"
+version = "0.1.1"
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

