# Comparing `tmp/OBP_reliability_pillar-0.1.4.tar.gz` & `tmp/OBP_reliability_pillar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_reliability_pillar-0.1.4.tar", last modified: Thu Jul 27 18:55:09 2023, max compression
+gzip compressed data, was "OBP_reliability_pillar-0.2.0.tar", last modified: Fri Aug  4 05:48:26 2023, max compression
```

## Comparing `OBP_reliability_pillar-0.1.4.tar` & `OBP_reliability_pillar-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:09.266029 OBP_reliability_pillar-0.1.4/
--rw-rw-rw-   0        0        0        0 2022-11-24 06:08:48.000000 OBP_reliability_pillar-0.1.4/LICENCE
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:07.769669 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/
--rw-rw-rw-   0        0        0     4908 2023-07-27 18:54:35.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:07.919405 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/auto_scaling/
--rw-rw-rw-   0        0        0      197 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/auto_scaling/__init__.py
--rw-rw-rw-   0        0        0     2101 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
--rw-rw-rw-   0        0        0      607 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/auto_scaling/compliance.py
--rw-rw-rw-   0        0        0     2223 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.003388 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/cloudwatch/
--rw-rw-rw-   0        0        0      193 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/cloudwatch/__init__.py
--rw-rw-rw-   0        0        0     3134 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/cloudwatch/alarm_action_check.py
--rw-rw-rw-   0        0        0      485 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/cloudwatch/compliance.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.128178 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/
--rw-rw-rw-   0        0        0      187 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      667 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/compliance.py
--rw-rw-rw-   0        0        0     2565 2023-07-17 18:59:49.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py
--rw-rw-rw-   0        0        0     2106 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py
--rw-rw-rw-   0        0        0      557 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.236742 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/ec2/
--rw-rw-rw-   0        0        0      177 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/ec2/__init__.py
--rw-rw-rw-   0        0        0      709 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/ec2/compliance.py
--rw-rw-rw-   0        0        0     2233 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py
--rw-rw-rw-   0        0        0     2257 2023-05-31 08:17:16.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/ec2/instance_in_vpc.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.319979 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_beanstalk/
--rw-rw-rw-   0        0        0      205 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_beanstalk/__init__.py
--rw-rw-rw-   0        0        0      508 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_beanstalk/compliance.py
--rw-rw-rw-   0        0        0     2339 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.462083 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/
--rw-rw-rw-   0        0        0      177 2023-01-27 09:44:59.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/__init__.py
--rw-rw-rw-   0        0        0      737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/compliance.py
--rw-rw-rw-   0        0        0     1829 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py
--rw-rw-rw-   0        0        0     1994 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py
--rw-rw-rw-   0        0        0     1700 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.555221 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_search/
--rw-rw-rw-   0        0        0      197 2023-01-27 11:52:50.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_search/__init__.py
--rw-rw-rw-   0        0        0      432 2023-05-31 11:40:25.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_search/compliance.py
--rw-rw-rw-   0        0        0     1940 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.629489 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/guard_duty/
--rw-rw-rw-   0        0        0      207 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/guard_duty/__init__.py
--rw-rw-rw-   0        0        0      430 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/guard_duty/compliance.py
--rw-rw-rw-   0        0        0     1965 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.769620 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/
--rw-rw-rw-   0        0        0      181 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/__init__.py
--rw-rw-rw-   0        0        0      648 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/compliance.py
--rw-rw-rw-   0        0        0     1932 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py
--rw-rw-rw-   0        0        0     1737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py
--rw-rw-rw-   0        0        0      844 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:08.993080 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/
--rw-rw-rw-   0        0        0      360 2023-06-06 07:06:27.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/__init__.py
--rw-rw-rw-   0        0        0     2126 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/compliance.py
--rw-rw-rw-   0        0        0     1558 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
--rw-rw-rw-   0        0        0     2319 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_backup_enabled.py
--rw-rw-rw-   0        0        0     2126 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py
--rw-rw-rw-   0        0        0     1479 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py
--rw-rw-rw-   0        0        0     1375 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:09.073718 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/redshift/
--rw-rw-rw-   0        0        0      283 2023-07-27 18:54:35.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/redshift/__init__.py
--rw-rw-rw-   0        0        0     1738 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/redshift/compliance.py
--rw-rw-rw-   0        0        0     1383 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/redshift/redshift_backup_enabled.py
--rw-rw-rw-   0        0        0     1710 2023-05-31 08:41:05.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:09.244885 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/
--rw-rw-rw-   0        0        0      297 2023-06-06 07:10:52.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/compliance.py
--rw-rw-rw-   0        0        0     1825 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py
--rw-rw-rw-   0        0        0     1796 2023-05-31 09:39:39.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py
--rw-rw-rw-   0        0        0     1932 2023-07-18 05:30:32.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:09.256962 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/security_hub/
--rw-rw-rw-   0        0        0     1586 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/security_hub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:55:07.794472 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar.egg-info/
--rw-rw-rw-   0        0        0     1114 2023-07-27 18:55:07.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2023-07-27 18:55:07.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 18:55:07.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-27 18:55:07.000000 OBP_reliability_pillar-0.1.4/OBP_reliability_pillar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1114 2023-07-27 18:55:09.264580 OBP_reliability_pillar-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      755 2022-12-19 13:35:30.000000 OBP_reliability_pillar-0.1.4/README.md
--rw-rw-rw-   0        0        0      498 2023-07-27 18:54:35.000000 OBP_reliability_pillar-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 18:55:09.266385 OBP_reliability_pillar-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:26.201206 OBP_reliability_pillar-0.2.0/
+-rw-rw-rw-   0        0        0        0 2022-11-24 06:08:48.000000 OBP_reliability_pillar-0.2.0/LICENCE
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.536769 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/
+-rw-rw-rw-   0        0        0     7511 2023-08-04 05:48:01.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.599275 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/auto_scaling/
+-rw-rw-rw-   0        0        0      197 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/auto_scaling/__init__.py
+-rw-rw-rw-   0        0        0     2129 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
+-rw-rw-rw-   0        0        0      607 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/auto_scaling/compliance.py
+-rw-rw-rw-   0        0        0     2251 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.637232 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/cloudwatch/
+-rw-rw-rw-   0        0        0      193 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/cloudwatch/__init__.py
+-rw-rw-rw-   0        0        0     3162 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/cloudwatch/alarm_action_check.py
+-rw-rw-rw-   0        0        0      485 2023-08-04 05:33:09.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/cloudwatch/compliance.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.683989 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/
+-rw-rw-rw-   0        0        0      187 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      667 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/compliance.py
+-rw-rw-rw-   0        0        0     2593 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py
+-rw-rw-rw-   0        0        0     2134 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py
+-rw-rw-rw-   0        0        0      557 2023-08-04 05:43:24.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.753029 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/ec2/
+-rw-rw-rw-   0        0        0      177 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/ec2/__init__.py
+-rw-rw-rw-   0        0        0      730 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/ec2/compliance.py
+-rw-rw-rw-   0        0        0     2261 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     2285 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/ec2/instance_in_vpc.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.784271 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_beanstalk/
+-rw-rw-rw-   0        0        0      205 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_beanstalk/__init__.py
+-rw-rw-rw-   0        0        0      531 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_beanstalk/compliance.py
+-rw-rw-rw-   0        0        0     2367 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.853350 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/
+-rw-rw-rw-   0        0        0      177 2023-01-27 09:44:59.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/compliance.py
+-rw-rw-rw-   0        0        0     1857 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py
+-rw-rw-rw-   0        0        0     2024 2023-08-04 05:33:09.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py
+-rw-rw-rw-   0        0        0     1756 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.888504 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_search/
+-rw-rw-rw-   0        0        0      197 2023-01-27 11:52:50.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_search/__init__.py
+-rw-rw-rw-   0        0        0      434 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_search/compliance.py
+-rw-rw-rw-   0        0        0     1946 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.938356 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/guard_duty/
+-rw-rw-rw-   0        0        0      207 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/guard_duty/__init__.py
+-rw-rw-rw-   0        0        0      432 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/guard_duty/compliance.py
+-rw-rw-rw-   0        0        0     1997 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:26.001361 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/
+-rw-rw-rw-   0        0        0      181 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-08-04 05:33:09.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/compliance.py
+-rw-rw-rw-   0        0        0     1960 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py
+-rw-rw-rw-   0        0        0     1765 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py
+-rw-rw-rw-   0        0        0      844 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:26.085731 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/
+-rw-rw-rw-   0        0        0      360 2023-06-06 07:06:27.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/__init__.py
+-rw-rw-rw-   0        0        0     2172 2023-08-04 05:33:09.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/compliance.py
+-rw-rw-rw-   0        0        0     1586 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
+-rw-rw-rw-   0        0        0     2319 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_backup_enabled.py
+-rw-rw-rw-   0        0        0     2154 2023-08-04 05:33:09.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     1507 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py
+-rw-rw-rw-   0        0        0     1403 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:26.138147 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/redshift/
+-rw-rw-rw-   0        0        0      283 2023-07-27 18:54:35.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/redshift/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-08-04 05:33:09.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/redshift/compliance.py
+-rw-rw-rw-   0        0        0     1411 2023-08-04 05:33:09.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/redshift/redshift_backup_enabled.py
+-rw-rw-rw-   0        0        0     1738 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:26.185026 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/
+-rw-rw-rw-   0        0        0      297 2023-06-06 07:10:52.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/compliance.py
+-rw-rw-rw-   0        0        0     1853 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py
+-rw-rw-rw-   0        0        0     1824 2023-08-04 05:33:10.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py
+-rw-rw-rw-   0        0        0     1960 2023-08-04 05:33:09.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:26.201206 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/security_hub/
+-rw-rw-rw-   0        0        0     1586 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/security_hub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:48:25.536769 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar.egg-info/
+-rw-rw-rw-   0        0        0     1114 2023-08-04 05:48:25.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3124 2023-08-04 05:48:25.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 05:48:25.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 05:48:25.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-04 05:48:25.000000 OBP_reliability_pillar-0.2.0/OBP_reliability_pillar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1114 2023-08-04 05:48:26.201206 OBP_reliability_pillar-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2022-12-19 13:35:30.000000 OBP_reliability_pillar-0.2.0/README.md
+-rw-rw-rw-   0        0        0      543 2023-08-04 05:21:57.000000 OBP_reliability_pillar-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 05:48:26.201206 OBP_reliability_pillar-0.2.0/setup.cfg
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 def asg_elb_healthcheck_required(self) -> dict:
     """
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

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/auto_scaling/compliance.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/auto_scaling/compliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from OBP_reliability_pillar.auto_scaling.asg_elb_healthcheck_required import *
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks autoscaling compliance
-def auto_scaling_compliance(self, regions) -> dict:
+def auto_scaling_compliance(self, regions) -> list:
     logger.info(" ---Inside auto_scaling_compliance()")
     response = [
         launch_config_public_ip_disabled(self, regions),
         # Already covered in monitoring module, hence commenting here
         # asg_elb_healthcheck_required(self)
     ]
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def launch_config_public_ip_disabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside autoscaling :: launch_config_public_ip_disabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.12'
     compliance_type = "Launch configuration public ip disabled"
     description = "Checks if public ip is disabled in launch configuration or not"
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/cloudwatch/alarm_action_check.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/cloudwatch/alarm_action_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def alarm_action_check(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside cloudwatch :: alarm_action_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.17'
     compliance_type = "Cloudwatch Alarm check"
     description = "Checks whether CloudWatch alarms have at least one alarm action, one INSUFFICIENT_DATA action, or one OK action enabled."
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/compliance.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def dynamodb_autoscaling_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside dynamodb :: dynamodb_autoscaling_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.25'
     compliance_type = "Dynamodb autoscaling enabled"
     description = "Checks if Auto Scaling or On-Demand is enabled on your DynamoDB tables"
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def dynamodb_pitr_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside dynamodb :: dynamodb_pitr_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id5.5'
     compliance_type = "Dynamodb pitr enabled"
     description = "Checks that point in time recovery (PITR) is enabled for Amazon DynamoDB tables"
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/dynamodb/utils.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/ec2/compliance.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/ec2/compliance.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns consolidated dynamodb compliance
 def ec2_compliance(self, regions) -> list:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_compliance()")
 
     response = [
         # Already covered in monitoring module, hence commenting here
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # checks compliance.py for ec2 instance detailed monitoring enabled
 def ec2_instance_detailed_monitoring_enabled(self) -> dict:
     """
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

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/ec2/instance_in_vpc.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/ec2/instance_in_vpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def instance_in_vpc(self, regions: list) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 : instance_in_vpc()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.67'
     compliance_type = "EC2 instance In VPC"
     description = "Checks if your EC2 instances belong to a virtual private cloud (VPC)"
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def enhanced_health_reporting_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_beanstalk :: enhanced_health_reporting_enabled()")
+    self.refresh_session()
 
     # regions = self.session.get_available_regions('elasticbeanstalk')
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.13'
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/compliance.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def cross_zone_load_balancing_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_load_balancer :: cross_zone_load_balancing_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.47'
     compliance_type = "Cross Zone Load Balancing Enabled"
     description = "Checks if cross zone load balancing is enabled or not"
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def elb_deletion_protection_enabled(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_load_balancer :: elb_deletion_protection_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.48'
     compliance_type = "ELB Deletion Protection Enabled"
     description = "Checks whether an Elastic Load Balancer has deletion protection enabled"
@@ -52,8 +53,8 @@
         'failReason': failReason,
         'resource_type': resource_type,
         'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
         'Description': description,
         'Risk Level': risk_level
-    }
+    }
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_load_balancer/utils.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_load_balancer/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns the list of load balancers
 def list_elb_v2(self, region: str) -> list:
     logger.info(" ---Inside list_elb()")
+    self.refresh_session()
     res = []
     client = self.session.client('elbv2', region_name=region)
 
     marker = ''
     while True:
         if marker == '' or marker is None:
             response = client.describe_load_balancers()
@@ -33,14 +34,15 @@
             break
 
     return res
 
 
 def list_elb(self, region: str) -> list:
     logger.info(" ---Inside list_elb()")
+    self.refresh_session()
     res = []
     client = self.session.client('elb', region_name=region)
 
     marker = ''
     while True:
         if marker == '' or marker is None:
             response = client.describe_load_balancers()
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def elastic_search_in_vpc_only(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside elastic_search :: elastic_search_in_vpc_only()")
+    self.refresh_session()
 
     result = True
     failReason = ""
     offenders = []
     control_id = 'Id3.43'
     compliance_type = "Elastic search in vpc"
     description = "Checks if Elasticsearch domains are in Amazon Virtual Private Cloud (Amazon VPC)"
@@ -42,15 +43,14 @@
                 except KeyError:
                     result = False
                     failReason = "Elastic search domain does not reside in a vpc"
                     offenders.append(domain['DomainName'])
 
         except ClientError as e:
             logger.error("Something wrong with the region {}: {}".format(region, e))
-    print('dheeraj')
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from botocore.exceptions import ClientError
 
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+
 # check the compliance for guard duty enabled
 def guard_duty_enabled(self) -> dict:
     """
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
@@ -57,8 +59,8 @@
         'failReason': failReason,
         'resource_type': resource_type,
         'ControlId': control_id,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
         'Description': description,
         'Risk Level': risk_level
-    }
+    }
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/compliance.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/compliance.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from OBP_reliability_pillar.lambdafn.lambda_inside_vpc import lambda_inside_vpc
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks aws lambda compliance
-def lambda_compliance(self, regions) -> dict:
+def lambda_compliance(self, regions) -> list:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside lambdafn :: lambda_compliance()")
     response = [
         # Already covered in monitoring module, hence commenting here
         # lambda_dlq_check(self),
         lambda_inside_vpc(self, regions),
     ]
 
-    return response
+    return response
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 def lambda_dlq_check(self) -> dict:
     """
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

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def lambda_inside_vpc(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside lambda :: lambda_inside_vpc()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.72'
     compliance_type = "Lambda DLQ check"
     description = "Checks whether an AWS Lambda function is configured with a dead-letter queue."
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/lambdafn/utils.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/lambdafn/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns the list of lambda functions
-def list_lambda_functions(client) -> dict:
+def list_lambda_functions(client) -> list:
     """
     :param client:
     :param self:
     :return:
     """
     logger.info(" ---Inside lambdafn.utils :: list_lambda_functions")
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/compliance.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/compliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # list rds instances
 def list_rds_instances(self, regions) -> dict:
     """
+    :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_rds_instances()--- ")
+    self.refresh_session()
     rds_instance_lst = {}
 
     for region in regions:
         client = self.session.client('rds', region_name=region)
         marker = ''
         while True:
             if marker == '':
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def rds_automatic_minor_version_upgrade_enabled(self, rds_instances: dict) -> dict:
     """
     :param rds_instances:
     :param self:
     :return dict: AWS RDS automatic minor version enabled compliance.py
     """
     logger.info(" ---Inside rds :: rds_automatic_minor_version_upgrade_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id5.12'
     compliance_type = "RDS instance automatic minor version upgrade enabled"
     description = "Checks if automatic minor version upgrade is enabled for RDS instances."
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_backup_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def rds_enhanced_monitoring_enabled(self) -> dict:
     """
 
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

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def rds_instance_deletion_protection_enabled(self, rds_instances: dict) -> dict:
     """
     :param self:
     :param rds_instances:
     :return:
     """
     logger.info(" ---Inside rds :: rds_instance_deletion_protection_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.76'
     compliance_type = "RDS instance deletion protection enabled"
     description = "Checks if deletion protection is enabled for RDS instances."
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # checks compliance.py for rds automatic minor version enabled
 def rds_multi_az_support_enabled(self, rds_instances: dict) -> dict:
     """
     :param self:
     :param rds_instances:
     """
     logger.info(" ---Inside rds :: rds_multi_az_support_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.78'
     compliance_type = "RDS multi az support enabled"
     description = "Checks if multi az support is enabled for RDS instances."
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/redshift/compliance.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/redshift/compliance.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def list_redshift_clusters(self, regions) -> dict:
     """
     :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside redshift :: list_redshift_clusters()--- ")
+    self.refresh_session()
     redshift_clusters = {}
 
     for region in regions:
         client = self.session.client('redshift', region_name=region)
         marker = ''
         while True:
             if marker == '' or marker is None:
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/redshift/redshift_backup_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/redshift/redshift_backup_enabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def redshift_backup_enabled(self, redshift_clusters) -> dict:
     """
     :param redshift_clusters:
     :param self:
     :return:
     """
     logger.info(" ---Inside redshift :: redshift_backup_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.80'
     compliance_type = "Redshift Backup Enabled"
     description = "Checks if backup is enabled on redshift cluster or not"
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def redshift_cluster_maintenance_settings_check(self, redshift_clusters) -> dict:
     """
     :param redshift_clusters:
     :param self:
     :return:
     """
     logger.info(" ---Inside redshift :: redshift_cluster_maintenance_settings_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.83'
     compliance_type = "Redshift cluster maintenance settings check"
     description = "Checks whether Amazon Redshift clusters have the specified maintenance settings"
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/compliance.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/compliance.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 #     list s3 buckets
 def list_s3_buckets(self) -> list:
     """
     :return:
     """
     logger.info(" ---Inside utils :: list_s3_buckets")
+    self.refresh_session()
 
     buckets = []
 
     client = self.session.client('s3')
     response = client.list_buckets()
 
     return response['Buckets']
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def s3_bucket_default_lock_enabled(self, buckets) -> dict:
     """
     :param buckets:
     :param self:
     :return:
     """
     logger.info(" ---Inside s3 :: s3_bucket_default_lock_enabled")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.88'
     compliance_type = "S3 bucket default lock enabled"
     description = "Checks whether Amazon S3 bucket has lock enabled, by default"
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def s3_bucket_replication_enabled(self, buckets):
     """
     :param buckets:
     :param self:
     :return dict: details of s3 bucket replication enabled compliance.py
     """
     logger.info(" ---Inside s3 :: s3_bucket_replication_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.91'
     compliance_type = "S3 bucket replication enabled"
     description = "Checks if bucket replication is enabled in s3 buckets."
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     """
 
     :param buckets:
     :param self:
     :return dict: details of s3 bucket versioning enabled compliance.py
     """
     logger.info(" ---Inside s3 :: s3_bucket_versioning_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.20'
     compliance_type = "S3 bucket versioning enabled"
     description = "Checks if bucket versioning is enabled in s3 buckets."
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar/security_hub/__init__.py` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar/security_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar.egg-info/PKG-INFO` & `OBP_reliability_pillar-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP-reliability-pillar
-Version: 0.1.4
+Name: OBP_reliability_pillar
+Version: 0.2.0
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `OBP_reliability_pillar-0.1.4/OBP_reliability_pillar.egg-info/SOURCES.txt` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENCE
 README.md
 pyproject.toml
 OBP_reliability_pillar/__init__.py
 OBP_reliability_pillar.egg-info/PKG-INFO
 OBP_reliability_pillar.egg-info/SOURCES.txt
 OBP_reliability_pillar.egg-info/dependency_links.txt
+OBP_reliability_pillar.egg-info/requires.txt
 OBP_reliability_pillar.egg-info/top_level.txt
 OBP_reliability_pillar/auto_scaling/__init__.py
 OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
 OBP_reliability_pillar/auto_scaling/compliance.py
 OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
 OBP_reliability_pillar/cloudwatch/__init__.py
 OBP_reliability_pillar/cloudwatch/alarm_action_check.py
```

### Comparing `OBP_reliability_pillar-0.1.4/PKG-INFO` & `OBP_reliability_pillar-0.2.0/OBP_reliability_pillar.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP_reliability_pillar
-Version: 0.1.4
+Name: OBP-reliability-pillar
+Version: 0.2.0
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `OBP_reliability_pillar-0.1.4/README.md` & `OBP_reliability_pillar-0.2.0/README.md`

 * *Files identical despite different names*

