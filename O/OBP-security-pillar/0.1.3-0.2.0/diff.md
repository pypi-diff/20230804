# Comparing `tmp/OBP_security_pillar-0.1.3.tar.gz` & `tmp/OBP_security_pillar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_security_pillar-0.1.3.tar", last modified: Thu Jul 27 16:47:54 2023, max compression
+gzip compressed data, was "OBP_security_pillar-0.2.0.tar", last modified: Fri Aug  4 05:35:35 2023, max compression
```

## Comparing `OBP_security_pillar-0.1.3.tar` & `OBP_security_pillar-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.808684 OBP_security_pillar-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.365058 OBP_security_pillar-0.1.3/OBP_security_pillar/
--rw-rw-rw-   0        0        0     4065 2023-07-27 16:47:33.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.408467 OBP_security_pillar-0.1.3/OBP_security_pillar/auto_scaling/
--rw-rw-rw-   0        0        0      475 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/auto_scaling/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-01-27 08:23:40.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.456988 OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/
--rw-rw-rw-   0        0        0      724 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/__init__.py
--rw-rw-rw-   0        0        0     2509 2023-01-27 08:24:11.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py
--rw-rw-rw-   0        0        0     3124 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/driver.py
--rw-rw-rw-   0        0        0     1251 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/compliance.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.483314 OBP_security_pillar-0.1.3/OBP_security_pillar/dynamodb/
--rw-rw-rw-   0        0        0      493 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/dynamodb/__init__.py
--rw-rw-rw-   0        0        0     2863 2023-01-27 08:24:38.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.638033 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/
--rw-rw-rw-   0        0        0     2214 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/Incoming_ssh_disabled.py
--rw-rw-rw-   0        0        0     2852 2023-05-25 10:19:42.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/__init__.py
--rw-rw-rw-   0        0        0     3275 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py
--rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py
--rw-rw-rw-   0        0        0     2105 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_encrypted_volume.py
--rw-rw-rw-   0        0        0     1540 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_imdsv2_check.py
--rw-rw-rw-   0        0        0     3047 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py
--rw-rw-rw-   0        0        0     1431 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py
--rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_profile_attached.py
--rw-rw-rw-   0        0        0     2088 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_volume_inuse_check.py
--rw-rw-rw-   0        0        0     2223 2023-01-27 08:28:22.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/instance_in_vpc.py
--rw-rw-rw-   0        0        0     2348 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py
--rw-rw-rw-   0        0        0     2793 2023-01-27 08:43:11.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/elb_logging_enabled.py
--rw-rw-rw-   0        0        0     2268 2023-01-27 08:43:27.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/elb_tls_https_listeners_only.py
--rw-rw-rw-   0        0        0     1969 2023-01-27 08:44:03.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/guard_duty_enabled.py
--rw-rw-rw-   0        0        0     2387 2023-01-27 08:44:27.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/lambda_inside_vpc.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.709479 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/
--rw-rw-rw-   0        0        0     2835 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/__init__.py
--rw-rw-rw-   0        0        0     1554 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
--rw-rw-rw-   0        0        0     1379 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_instance_public_access_check.py
--rw-rw-rw-   0        0        0     1392 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_snapshot_encrypted.py
--rw-rw-rw-   0        0        0     1901 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py
--rw-rw-rw-   0        0        0     1401 2023-05-25 09:14:26.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_storage_encrypted.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.805753 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/
--rw-rw-rw-   0        0        0     1706 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_logging_enabled.py
--rw-rw-rw-   0        0        0     2145 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py
--rw-rw-rw-   0        0        0     2147 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py
--rw-rw-rw-   0        0        0     1391 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py
--rw-rw-rw-   0        0        0     2260 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py
--rw-rw-rw-   0        0        0     1954 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py
--rw-rw-rw-   0        0        0     1817 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_default_encryption_kms.py
--rw-rw-rw-   0        0        0     1761 2023-01-04 11:06:48.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/security_hub_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.376236 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/
--rw-rw-rw-   0        0        0      797 2023-07-27 16:47:54.000000 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2223 2023-07-27 16:47:54.000000 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 16:47:54.000000 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-27 16:47:54.000000 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      797 2023-07-27 16:47:54.807685 OBP_security_pillar-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 OBP_security_pillar-0.1.3/README.md
--rw-rw-rw-   0        0        0      495 2023-07-27 16:47:33.000000 OBP_security_pillar-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 16:47:54.808684 OBP_security_pillar-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.723555 OBP_security_pillar-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:34.900074 OBP_security_pillar-0.2.0/OBP_security_pillar/
+-rw-rw-rw-   0        0        0     6554 2023-08-04 05:34:43.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:34.968993 OBP_security_pillar-0.2.0/OBP_security_pillar/auto_scaling/
+-rw-rw-rw-   0        0        0      475 2023-05-25 10:12:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/auto_scaling/__init__.py
+-rw-rw-rw-   0        0        0     2217 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.042582 OBP_security_pillar-0.2.0/OBP_security_pillar/cloudtrail/
+-rw-rw-rw-   0        0        0      724 2023-05-25 10:12:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/cloudtrail/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py
+-rw-rw-rw-   0        0        0     3152 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/cloudtrail/driver.py
+-rw-rw-rw-   0        0        0     1251 2023-01-27 07:29:08.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/compliance.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.093449 OBP_security_pillar-0.2.0/OBP_security_pillar/dynamodb/
+-rw-rw-rw-   0        0        0      493 2023-05-25 10:12:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0     2891 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.408810 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/
+-rw-rw-rw-   0        0        0     2242 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/Incoming_ssh_disabled.py
+-rw-rw-rw-   0        0        0     2852 2023-05-25 10:19:42.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/__init__.py
+-rw-rw-rw-   0        0        0     3303 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py
+-rw-rw-rw-   0        0        0     1547 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py
+-rw-rw-rw-   0        0        0     2133 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_encrypted_volume.py
+-rw-rw-rw-   0        0        0     1568 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_imdsv2_check.py
+-rw-rw-rw-   0        0        0     3075 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py
+-rw-rw-rw-   0        0        0     1459 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py
+-rw-rw-rw-   0        0        0     1547 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_instance_profile_attached.py
+-rw-rw-rw-   0        0        0     2116 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_volume_inuse_check.py
+-rw-rw-rw-   0        0        0     2251 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/instance_in_vpc.py
+-rw-rw-rw-   0        0        0     2376 2023-08-04 05:24:27.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py
+-rw-rw-rw-   0        0        0     2849 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/elb_logging_enabled.py
+-rw-rw-rw-   0        0        0     2296 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/elb_tls_https_listeners_only.py
+-rw-rw-rw-   0        0        0     1997 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/guard_duty_enabled.py
+-rw-rw-rw-   0        0        0     2443 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/lambda_inside_vpc.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.551007 OBP_security_pillar-0.2.0/OBP_security_pillar/rds/
+-rw-rw-rw-   0        0        0     2835 2023-05-25 09:38:15.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/rds/__init__.py
+-rw-rw-rw-   0        0        0     1582 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
+-rw-rw-rw-   0        0        0     1407 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_instance_public_access_check.py
+-rw-rw-rw-   0        0        0     1420 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_snapshot_encrypted.py
+-rw-rw-rw-   0        0        0     1929 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py
+-rw-rw-rw-   0        0        0     1429 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_storage_encrypted.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.723555 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/
+-rw-rw-rw-   0        0        0     1706 2023-05-25 10:12:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/__init__.py
+-rw-rw-rw-   0        0        0     1673 2023-08-04 05:18:08.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_logging_enabled.py
+-rw-rw-rw-   0        0        0     2173 2023-08-04 05:18:08.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py
+-rw-rw-rw-   0        0        0     2175 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py
+-rw-rw-rw-   0        0        0     1419 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py
+-rw-rw-rw-   0        0        0     2288 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py
+-rw-rw-rw-   0        0        0     1982 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py
+-rw-rw-rw-   0        0        0     1845 2023-08-04 05:18:07.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_default_encryption_kms.py
+-rw-rw-rw-   0        0        0     1761 2023-01-04 11:06:48.000000 OBP_security_pillar-0.2.0/OBP_security_pillar/security_hub_enabled.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:34.920372 OBP_security_pillar-0.2.0/OBP_security_pillar.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-08-04 05:35:34.000000 OBP_security_pillar-0.2.0/OBP_security_pillar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2265 2023-08-04 05:35:34.000000 OBP_security_pillar-0.2.0/OBP_security_pillar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 05:35:34.000000 OBP_security_pillar-0.2.0/OBP_security_pillar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 05:35:34.000000 OBP_security_pillar-0.2.0/OBP_security_pillar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-04 05:35:34.000000 OBP_security_pillar-0.2.0/OBP_security_pillar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2023-08-04 05:35:35.723555 OBP_security_pillar-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 OBP_security_pillar-0.2.0/README.md
+-rw-rw-rw-   0        0        0      540 2023-08-04 05:18:08.000000 OBP_security_pillar-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 05:35:35.731605 OBP_security_pillar-0.2.0/setup.cfg
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 def launch_config_public_ip_disabled(self) -> dict:
     """
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

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/__init__.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 def cloudtrail_cloudwatch_logs_enabled(self) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside cloudtrail :: cloudtrail_cloudwatch_logs_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.1'
 
     compliance_type = "cloud-trail cloudwatch logs enabled"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/driver.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/cloudtrail/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 def driver(self) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside cloudtrail :: driver()")
+    self.refresh_session()
 
     compliance_result = {
         "cloud-trail cloudwatch logs enabled": Compliance(
             'cloud-trail cloudwatch logs enabled',
             'Checks whether AWS CloudTrail trails are configured to send logs to Amazon CloudWatch logs',
             'CloudTrail'
         )
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/compliance.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 def dynamodb_table_encrypted_kms(self) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside dynamodb :: dynamodb_table_encrypted_kms()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.27'
     compliance_type = "Dynamodb Table Encrypted KMS"
     description = "Checks if Amazon DynamoDB table is encrypted with AWS Key Management Service (KMS)"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/Incoming_ssh_disabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/Incoming_ssh_disabled.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # Ensure no security groups allow ingress from 0.0.0.0/0 to port 22
 def incoming_ssh_disabled(self, regions):
     logger.info(" ---Inside incoming_ssh_disabled()")
+    self.refresh_session()
     """Summary
 
     Returns:
         TYPE: Description
     """
     result = True
     failReason = ""
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/__init__.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def ebs_snapshot_public_restorable_check(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ebs_snapshot_public_restorable_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.29'
 
     compliance_type = "EBS snapshot public restorable check"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def ec2_ebs_encryption_by_default(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_ebs_encryption_by_default()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.4'
     compliance_type = "EC2 EBS Encryption by default"
     description = "Check that Amazon Elastic Block Store (EBS) encryption is enabled by default"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_encrypted_volume.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_encrypted_volume.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # checks the compliance for the ec2 volume in use check
 def ec2_encrypted_volume(self) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_encrypted_volume()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = ''
 
     compliance_type = "Attached Ec2 volume are encrypted"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_imdsv2_check.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_imdsv2_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def ec2_imdsv2_check(self, ec2_instances) -> dict:
     """
     :param ec2_instances:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_imdsv2_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id5.7'
 
     compliance_type = "EC2 IMDS v2 Enabled"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def ec2_instance_managed_by_ssm(self, ec2_instances) -> dict:
     """
     :param ec2_instances:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_instance_managed_by_ssm()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.31'
 
     compliance_type = "EC2 instance managed by ssm"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def ec2_instance_multiple_eni_check(self, ec2_instances) -> dict:
     """
     :param ec2_instances:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_instance_multiple_eni_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id18.1'
 
     compliance_type = "Ec2 Instance multiple eni check"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_profile_attached.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_instance_profile_attached.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def ec2_instance_profile_attached(self, ec2_instances) -> dict:
     """
     :param ec2_instances:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_instance_profile_attached()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.33'
 
     compliance_type = "Ec2 instance profile attached"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_volume_inuse_check.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/ec2_volume_inuse_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def ec2_volume_inuse_check(self, regions) -> dict:
     """
     :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_volume_inuse_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.37'
 
     compliance_type = "Ec2 volume in use"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/instance_in_vpc.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/instance_in_vpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 def instance_in_vpc(self) -> dict:
     """
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
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # Ensure VPC flow logging is enabled in all VPCs (Scored)
 def vpc_logging_enabled(self, regions) -> dict:
     logger.info(" ---Inside vpc_logging_enabled()--- ")
+    self.refresh_session()
     """Summary
 
     Returns:
         TYPE: Description
     """
     result = True
     failReason = ""
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/elb_logging_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/elb_logging_enabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # returns the list of elastic load balancers
 def list_elb(self, region: str) -> list:
     logger.info(" ---Inside utils :: list_elb()---")
+    self.refresh_session()
     """Summary
 
     Returns:
         TYPE: list
     """
 
     elb_lst = []
@@ -42,14 +43,15 @@
 
 def elb_logging_enabled(self) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside ensure_elb_access_logging_enabled")
+    self.refresh_session()
 
     result = True
     failReason = ""
     offenders = []
     control_id = 'Id3.49'
 
     compliance_type = "ELB logging enabled"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/elb_tls_https_listeners_only.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/elb_tls_https_listeners_only.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # Ensure that your Amazon Classic Load Balancer listeners are using a secure protocol (HTTPS or SSL)
 def elb_tls_https_listeners_only(self) -> dict:
     logger.info(" ---Inside elb_tls_https_listeners_only()")
+    self.refresh_session()
     """Summary
 
     Returns:
         TYPE: dict
     """
 
     result = True
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/guard_duty_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/guard_duty_enabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
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
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/lambda_inside_vpc.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/lambda_inside_vpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def list_lambda_functions(client) -> dict:
     """
     :param client:
     :param self:
     :return:
     """
     logger.info(" ---Inside lambdafn.utils :: list_lambda_functions")
+    self.refresh_session()
 
     function_lst = []
 
     marker = ''
     while True:
         if marker == '' or marker is None:
             response = client.list_functions()
@@ -41,14 +42,15 @@
 # checks the compliance for lambda-inside-vpc
 def lambda_inside_vpc(self) -> dict:
     """
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
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/__init__.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def rds_automatic_minor_version_upgrade_enabled(self, rds_instances) -> dict:
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
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_instance_public_access_check.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_instance_public_access_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def rds_instance_public_access_check(self, rds_instances) -> dict:
     """
     :param rds_instances:
     :param self:
     :return:
     """
     logger.info(" ---Inside rds :: rds_instance_public_access_check()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.10'
 
     compliance_type = "RDS instance public access check"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_snapshot_encrypted.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_snapshot_encrypted.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def rds_snapshot_encrypted(self, rds_snapshots) -> dict:
     """
     :param rds_snapshots:
     :param self:
     :return:
     """
     logger.info(" ---Inside rds :: rds_snapshot_encrypted()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.79'
 
     compliance_type = "RDS snapshot encrypted"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def rds_snapshots_public_prohibited(self, rds_snapshots) -> dict:
     """
     :param rds_snapshots:
     :param self:
     :return:
     """
     logger.info(" ---Inside rds :: rds_snapshots_public_prohibited")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.11'
 
     compliance_type = "RDS snapshot public prohibited"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_storage_encrypted.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/rds/rds_storage_encrypted.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def rds_storage_encrypted(self, rds_instances) -> dict:
     """
     :param rds_instances:
     :param self:
     :return dict:
     """
     logger.info(" ---Inside rds :: rds_storage_encrypted()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.12'
 
     compliance_type = "RDS Storage Encrypted"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/__init__.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_logging_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_logging_enabled.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     """
 
     :param buckets:
     :param self:
     :return dict:
     """
     logger.info(" ---Inside s3 :: s3_bucket_logging_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.16'
     compliance_type = "S3 bucket logging enabled"
     description = "Checks whether logging is enabled for your S3 buckets"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def s3_bucket_public_read_prohibited(self, buckets):
     logger.info(" ---Inside s3 :: s3_bucket_public_read_prohibited()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.17'
     compliance_type = "S3 bucket public read prohibited"
     description = "Checks whether public read is prohibited for your S3 buckets"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def s3_bucket_public_write_prohibited(self, buckets):
     logger.info(" ---Inside s3 :: s3_bucket_public_write_prohibited()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.18'
     compliance_type = "S3 bucket public write prohibited"
     description = "Checks whether public write is prohibited for your S3 buckets"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def s3_bucket_server_side_encryption_enabled(self, buckets):
     logger.info(" ---Inside s3 :: s3_bucket_server_side_encryption_enabled()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id1.19'
     compliance_type = "S3 bucket server side encryption enabled"
     description = "Checks whether server side encryption is enabled for your S3 buckets"
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def s3_bucket_ssl_requests_only(self, buckets):
     logger.info(" ---Inside s3 :: s3_bucket_ssl_requests_only()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.92'
     compliance_type = "S3 bucket SSL requests only"
     description = "Checks whether S3 buckets have policies that require requests to use Secure Socket Layer (SSL)."
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py`

 * *Files 5% similar despite different names*

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

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_default_encryption_kms.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/s3/s3_default_encryption_kms.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def s3_default_encryption_kms(self, buckets):
     logger.info(" ---Inside s3 :: s3_default_encryption_kms()")
+    self.refresh_session()
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.93'
     compliance_type = "S3 bucket default encryption KMS"
     description = "Checks whether S3 buckets are encrypted with AWS Key Management Service(AWS KMS)."
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar/security_hub_enabled.py` & `OBP_security_pillar-0.2.0/OBP_security_pillar/security_hub_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/PKG-INFO` & `OBP_security_pillar-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP-security-pillar
-Version: 0.1.3
+Name: OBP_security_pillar
+Version: 0.2.0
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/SOURCES.txt` & `OBP_security_pillar-0.2.0/OBP_security_pillar.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 OBP_security_pillar/elb_tls_https_listeners_only.py
 OBP_security_pillar/guard_duty_enabled.py
 OBP_security_pillar/lambda_inside_vpc.py
 OBP_security_pillar/security_hub_enabled.py
 OBP_security_pillar.egg-info/PKG-INFO
 OBP_security_pillar.egg-info/SOURCES.txt
 OBP_security_pillar.egg-info/dependency_links.txt
+OBP_security_pillar.egg-info/requires.txt
 OBP_security_pillar.egg-info/top_level.txt
 OBP_security_pillar/auto_scaling/__init__.py
 OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py
 OBP_security_pillar/cloudtrail/__init__.py
 OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py
 OBP_security_pillar/cloudtrail/driver.py
 OBP_security_pillar/dynamodb/__init__.py
```

### Comparing `OBP_security_pillar-0.1.3/PKG-INFO` & `OBP_security_pillar-0.2.0/OBP_security_pillar.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP_security_pillar
-Version: 0.1.3
+Name: OBP-security-pillar
+Version: 0.2.0
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

