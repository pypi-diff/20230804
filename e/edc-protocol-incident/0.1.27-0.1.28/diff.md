# Comparing `tmp/edc-protocol-incident-0.1.27.tar.gz` & `tmp/edc-protocol-incident-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-protocol-incident-0.1.27.tar", last modified: Tue Aug  1 05:20:53 2023, max compression
+gzip compressed data, was "edc-protocol-incident-0.1.28.tar", last modified: Fri Aug  4 04:11:56 2023, max compression
```

## Comparing `edc-protocol-incident-0.1.27.tar` & `edc-protocol-incident-0.1.28.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.318661 edc-protocol-incident-0.1.27/
--rw-r--r--   0 erikvw     (501) staff       (20)      123 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.27/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.302201 edc-protocol-incident-0.1.27/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.305986 edc-protocol-incident-0.1.27/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.27/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.27/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.27/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.27/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-09-09 17:06:27.000000 edc-protocol-incident-0.1.27/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.27/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-08-01 05:20:53.318770 edc-protocol-incident-0.1.27/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1232 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.27/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.308262 edc-protocol-incident-0.1.27/edc_protocol_incident/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1331 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.309568 edc-protocol-incident-0.1.27/edc_protocol_incident/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2592 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/admin/protocol_deviation_violation_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      475 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/admin/protocol_incident_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      244 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      892 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1637 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      358 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.310372 edc-protocol-incident-0.1.27/edc_protocol_incident/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      182 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/form_validators/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1554 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/form_validators/protocol_incident_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.310824 edc-protocol-incident-0.1.27/edc_protocol_incident/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      135 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      992 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/forms/protocol_deviation_violation_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      794 2022-10-04 02:54:16.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/forms/protocol_incident_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1552 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.314581 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    31949 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    73009 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2355 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0002_auto_20210911_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1181 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0003_auto_20211104_1456.py
--rw-r--r--   0 erikvw     (501) staff       (20)      719 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26979 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2621 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1455 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0007_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1086 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1217 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0009_auto_20220826_0258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1091 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0010_auto_20220826_0322.py
--rw-r--r--   0 erikvw     (501) staff       (20)      783 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0011_auto_20220826_0406.py
--rw-r--r--   0 erikvw     (501) staff       (20)      867 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0012_auto_20220913_2139.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2207 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0013_auto_20220927_0349.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1380 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0014_auto_20220927_0400.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0015_auto_20220927_0401.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1890 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      690 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-07-10 15:04:28.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0018_alter_protocoldeviationviolation_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.314998 edc-protocol-incident-0.1.27/edc_protocol_incident/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      170 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4116 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3943 2023-07-20 03:10:12.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3887 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/modeladmin_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.315979 edc-protocol-incident-0.1.27/edc_protocol_incident/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      773 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/models/list_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1018 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/models/protocol_deviation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)      946 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/models/protocol_incident.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.316206 edc-protocol-incident-0.1.27/edc_protocol_incident/pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/pdf_reports/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.316927 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.318133 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1895 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.318520 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5901 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/tests/test_protocol_incident.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9323 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/tests/test_protocol_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1638 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      220 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.27/edc_protocol_incident/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:20:53.309071 edc-protocol-incident-0.1.27/edc_protocol_incident.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-08-01 05:20:53.000000 edc-protocol-incident-0.1.27/edc_protocol_incident.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     4062 2023-08-01 05:20:53.000000 edc-protocol-incident-0.1.27/edc_protocol_incident.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 05:20:53.000000 edc-protocol-incident-0.1.27/edc_protocol_incident.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-27 01:17:18.000000 edc-protocol-incident-0.1.27/edc_protocol_incident.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2023-08-01 05:20:53.000000 edc-protocol-incident-0.1.27/edc_protocol_incident.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1788 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.27/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1187 2023-08-01 05:20:46.000000 edc-protocol-incident-0.1.27/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1241 2023-08-01 05:20:53.319070 edc-protocol-incident-0.1.27/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.351256 edc-protocol-incident-0.1.28/
+-rw-r--r--   0 erikvw     (501) staff       (20)      123 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.28/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.334643 edc-protocol-incident-0.1.28/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.338596 edc-protocol-incident-0.1.28/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1927 2023-08-04 04:11:48.000000 edc-protocol-incident-0.1.28/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.28/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.28/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.28/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.28/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-09-09 17:06:27.000000 edc-protocol-incident-0.1.28/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.28/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2117 2023-08-04 04:11:56.351360 edc-protocol-incident-0.1.28/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1232 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.28/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.340666 edc-protocol-incident-0.1.28/edc_protocol_incident/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1331 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.341813 edc-protocol-incident-0.1.28/edc_protocol_incident/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2592 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/admin/protocol_deviation_violation_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      475 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/admin/protocol_incident_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      244 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      892 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1637 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      358 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.342642 edc-protocol-incident-0.1.28/edc_protocol_incident/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      182 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/form_validators/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1554 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/form_validators/protocol_incident_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.343059 edc-protocol-incident-0.1.28/edc_protocol_incident/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      135 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      992 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/forms/protocol_deviation_violation_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      794 2022-10-04 02:54:16.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/forms/protocol_incident_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1552 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.346657 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    31949 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    73009 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2355 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0002_auto_20210911_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1181 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0003_auto_20211104_1456.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      719 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26979 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2621 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1455 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0007_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1086 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1217 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0009_auto_20220826_0258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1091 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0010_auto_20220826_0322.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      783 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0011_auto_20220826_0406.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      867 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0012_auto_20220913_2139.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2207 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0013_auto_20220927_0349.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1380 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0014_auto_20220927_0400.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0015_auto_20220927_0401.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1890 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      690 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-07-10 15:04:28.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0018_alter_protocoldeviationviolation_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      848 2023-08-04 04:11:48.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0019_actionsrequired_extra_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.347019 edc-protocol-incident-0.1.28/edc_protocol_incident/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      170 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4116 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3943 2023-07-20 03:10:12.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3887 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/modeladmin_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.347756 edc-protocol-incident-0.1.28/edc_protocol_incident/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      773 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/models/list_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1018 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/models/protocol_deviation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      946 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/models/protocol_incident.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.347944 edc-protocol-incident-0.1.28/edc_protocol_incident/pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/pdf_reports/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.348602 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.349804 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1895 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.351088 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5901 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/tests/test_protocol_incident.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9323 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/tests/test_protocol_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1638 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      220 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.28/edc_protocol_incident/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:11:56.341407 edc-protocol-incident-0.1.28/edc_protocol_incident.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2117 2023-08-04 04:11:56.000000 edc-protocol-incident-0.1.28/edc_protocol_incident.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     4140 2023-08-04 04:11:56.000000 edc-protocol-incident-0.1.28/edc_protocol_incident.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-04 04:11:56.000000 edc-protocol-incident-0.1.28/edc_protocol_incident.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-27 01:17:18.000000 edc-protocol-incident-0.1.28/edc_protocol_incident.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2023-08-04 04:11:56.000000 edc-protocol-incident-0.1.28/edc_protocol_incident.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1749 2023-08-04 04:11:48.000000 edc-protocol-incident-0.1.28/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1187 2023-08-01 05:20:46.000000 edc-protocol-incident-0.1.28/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1201 2023-08-04 04:11:56.351668 edc-protocol-incident-0.1.28/setup.cfg
```

### Comparing `edc-protocol-incident-0.1.27/.github/workflows/build.yml` & `edc-protocol-incident-0.1.28/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,16 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.10', '3.11']
+        python-version: ['3.11']
         django-version: ['4.1', '4.2', 'dev']
-        exclude:
-          - python-version: '3.10'
-            django-version: 'dev'
     services:
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
```

### Comparing `edc-protocol-incident-0.1.27/.gitignore` & `edc-protocol-incident-0.1.28/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/.pre-commit-config.yaml` & `edc-protocol-incident-0.1.28/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/LICENSE` & `edc-protocol-incident-0.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/PKG-INFO` & `edc-protocol-incident-0.1.28/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: edc-protocol-incident
-Version: 0.1.27
+Version: 0.1.28
 Summary: Classes for protocol incident (violations/deviations) in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-protocol-incident
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc protocol incident violations deviations,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
 
 edc-protocol-incident
```

### Comparing `edc-protocol-incident-0.1.27/README.rst` & `edc-protocol-incident-0.1.28/README.rst`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/action_items.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/admin/protocol_deviation_violation_admin.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/admin/protocol_deviation_violation_admin.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/auth_objects.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/auths.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/auths.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/form_validators/mixins.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/form_validators/mixins.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/form_validators/protocol_incident_form_validator.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/form_validators/protocol_incident_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/forms/protocol_deviation_violation_form.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/forms/protocol_deviation_violation_form.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/forms/protocol_incident_form.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/forms/protocol_incident_form.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/list_data.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0001_initial.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0002_auto_20210911_2036.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0002_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0003_auto_20211104_1456.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0003_auto_20211104_1456.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0007_auto_20220704_1841.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0007_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0009_auto_20220826_0258.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0009_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0010_auto_20220826_0322.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0010_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0011_auto_20220826_0406.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0011_auto_20220826_0406.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0012_auto_20220913_2139.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0012_auto_20220913_2139.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0013_auto_20220927_0349.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0013_auto_20220927_0349.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0014_auto_20220927_0400.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0014_auto_20220927_0400.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0015_auto_20220927_0401.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0015_auto_20220927_0401.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/migrations/0018_alter_protocoldeviationviolation_options_and_more.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/migrations/0018_alter_protocoldeviationviolation_options_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/modeladmin_mixins.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/models/list_models.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/models/list_models.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/models/protocol_deviation_violation.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/models/protocol_deviation_violation.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/models/protocol_incident.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/models/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/tests/action_items.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/tests/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-rsa-local-private.pem` & `edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem` & `edc-protocol-incident-0.1.28/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/tests/holidays.csv` & `edc-protocol-incident-0.1.28/edc_protocol_incident/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/tests/tests/test_protocol_incident.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/tests/tests/test_protocol_incident.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/tests/tests/test_protocol_violation.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/tests/tests/test_protocol_violation.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident/tests/visit_schedule.py` & `edc-protocol-incident-0.1.28/edc_protocol_incident/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident.egg-info/PKG-INFO` & `edc-protocol-incident-0.1.28/edc_protocol_incident.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: edc-protocol-incident
-Version: 0.1.27
+Version: 0.1.28
 Summary: Classes for protocol incident (violations/deviations) in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-protocol-incident
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc protocol incident violations deviations,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
 
 edc-protocol-incident
```

### Comparing `edc-protocol-incident-0.1.27/edc_protocol_incident.egg-info/SOURCES.txt` & `edc-protocol-incident-0.1.28/edc_protocol_incident.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 edc_protocol_incident/migrations/0012_auto_20220913_2139.py
 edc_protocol_incident/migrations/0013_auto_20220927_0349.py
 edc_protocol_incident/migrations/0014_auto_20220927_0400.py
 edc_protocol_incident/migrations/0015_auto_20220927_0401.py
 edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py
 edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
 edc_protocol_incident/migrations/0018_alter_protocoldeviationviolation_options_and_more.py
+edc_protocol_incident/migrations/0019_actionsrequired_extra_value_and_more.py
 edc_protocol_incident/migrations/__init__.py
 edc_protocol_incident/model_mixins/__init__.py
 edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py
 edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py
 edc_protocol_incident/models/__init__.py
 edc_protocol_incident/models/list_models.py
 edc_protocol_incident/models/protocol_deviation_violation.py
```

### Comparing `edc-protocol-incident-0.1.27/pyproject.toml` & `edc-protocol-incident-0.1.28/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,23 +32,21 @@
   "if TYPE_CHECKING:",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{310}-dj{41,42},
     py{311}-dj{41,42,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.10: py310
     3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
     4.1: dj41
     4.2: dj42, lint
     dev: djdev
```

### Comparing `edc-protocol-incident-0.1.27/runtests.py` & `edc-protocol-incident-0.1.28/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.27/setup.cfg` & `edc-protocol-incident-0.1.28/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.10
+python_requires = >=3.11
 zip_safe = False
 include_package_data = True
 packages = find:
 
 [options.packages.find]
 exclude = 
 	examples*
```

