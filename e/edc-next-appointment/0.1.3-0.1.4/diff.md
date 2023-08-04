# Comparing `tmp/edc-next-appointment-0.1.3.tar.gz` & `tmp/edc-next-appointment-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-next-appointment-0.1.3.tar", last modified: Tue Aug  1 05:11:37 2023, max compression
+gzip compressed data, was "edc-next-appointment-0.1.4.tar", last modified: Fri Aug  4 04:07:13 2023, max compression
```

## Comparing `edc-next-appointment-0.1.3.tar` & `edc-next-appointment-0.1.4.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.682360 edc-next-appointment-0.1.3/
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.672717 edc-next-appointment-0.1.3/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.676073 edc-next-appointment-0.1.3/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     3121 2023-07-27 12:18:27.000000 edc-next-appointment-0.1.3/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2023-07-24 19:09:02.000000 edc-next-appointment-0.1.3/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      126 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-08-01 05:11:37.682454 edc-next-appointment-0.1.3/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1600 2023-07-27 01:53:02.000000 edc-next-appointment-0.1.3/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.677398 edc-next-appointment-0.1.3/edc_next_appointment/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      184 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/choices.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.678558 edc-next-appointment-0.1.3/edc_next_appointment/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      143 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/form_validators/form_validator_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      309 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/form_validators/next_appointment_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2153 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/edc_next_appointment/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      550 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.678868 edc-next-appointment-0.1.3/edc_next_appointment/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     2898 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1789 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1771 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4541 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/modelform_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.679117 edc-next-appointment-0.1.3/edc_next_appointment/models/
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      224 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/models/list_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.679381 edc-next-appointment-0.1.3/edc_next_appointment/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.680560 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1019 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.680824 edc-next-appointment-0.1.3/edc_next_appointment/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1972 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/tests/test_next_appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)      214 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      760 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.678126 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-08-01 05:11:37.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2074 2023-08-01 05:11:37.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 05:11:37.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-25 13:58:46.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2023-08-01 05:11:37.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.682228 edc-next-appointment-0.1.3/next_appointment_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1051 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      191 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      444 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/consents.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2154 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      292 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)      694 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/views.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2051 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/visit_schedules.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1786 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2083 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1238 2023-08-01 05:11:37.682765 edc-next-appointment-0.1.3/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.161712 edc-next-appointment-0.1.4/
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.151275 edc-next-appointment-0.1.4/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.155000 edc-next-appointment-0.1.4/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1927 2023-08-04 04:07:05.000000 edc-next-appointment-0.1.4/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     3121 2023-07-27 12:18:27.000000 edc-next-appointment-0.1.4/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2023-07-24 19:09:02.000000 edc-next-appointment-0.1.4/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      126 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2480 2023-08-04 04:07:13.161801 edc-next-appointment-0.1.4/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1600 2023-07-27 01:53:02.000000 edc-next-appointment-0.1.4/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.156444 edc-next-appointment-0.1.4/edc_next_appointment/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      184 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/choices.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.157703 edc-next-appointment-0.1.4/edc_next_appointment/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      143 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/form_validators/form_validator_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      309 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/form_validators/next_appointment_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-08-04 04:07:05.000000 edc-next-appointment-0.1.4/edc_next_appointment/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      550 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.158151 edc-next-appointment-0.1.4/edc_next_appointment/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2898 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      407 2023-08-04 04:07:05.000000 edc-next-appointment-0.1.4/edc_next_appointment/migrations/0002_infosources_extra_value.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1789 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1771 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4541 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/modelform_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.158411 edc-next-appointment-0.1.4/edc_next_appointment/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      224 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/models/list_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.158661 edc-next-appointment-0.1.4/edc_next_appointment/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.159650 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1019 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.160042 edc-next-appointment-0.1.4/edc_next_appointment/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1972 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/edc_next_appointment/tests/tests/test_next_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      214 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      760 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.4/edc_next_appointment/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.157266 edc-next-appointment-0.1.4/edc_next_appointment.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2480 2023-08-04 04:07:13.000000 edc-next-appointment-0.1.4/edc_next_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2138 2023-08-04 04:07:13.000000 edc-next-appointment-0.1.4/edc_next_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-04 04:07:13.000000 edc-next-appointment-0.1.4/edc_next_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-25 13:58:46.000000 edc-next-appointment-0.1.4/edc_next_appointment.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2023-08-04 04:07:13.000000 edc-next-appointment-0.1.4/edc_next_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:07:13.161587 edc-next-appointment-0.1.4/next_appointment_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1051 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      191 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      444 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2154 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      292 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      694 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/views.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2051 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/next_appointment_app/visit_schedules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1747 2023-08-04 04:07:05.000000 edc-next-appointment-0.1.4/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2083 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.4/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1198 2023-08-04 04:07:13.162091 edc-next-appointment-0.1.4/setup.cfg
```

### Comparing `edc-next-appointment-0.1.3/.github/workflows/build.yml` & `edc-next-appointment-0.1.4/.github/workflows/build.yml`

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

### Comparing `edc-next-appointment-0.1.3/.gitignore` & `edc-next-appointment-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/.pre-commit-config.yaml` & `edc-next-appointment-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/LICENSE` & `edc-next-appointment-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/PKG-INFO` & `edc-next-appointment-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: edc-next-appointment
-Version: 0.1.3
+Version: 0.1.4
 Summary: Base classes for managing next appointment CRF at each timepoint in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-next-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc appointment,scheduling,CRF,clinicedc,clinical trials
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
 
 edc-next-appointment
```

### Comparing `edc-next-appointment-0.1.3/README.rst` & `edc-next-appointment-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/form_validators/form_validator_mixins.py` & `edc-next-appointment-0.1.4/edc_next_appointment/form_validators/form_validator_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/form_validators.py` & `edc-next-appointment-0.1.4/edc_next_appointment/form_validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     @property
     def health_facility(self) -> HealthFacility | None:
         if not self._health_facility:
             if self.cleaned_data.get("health_facility"):
                 self._health_facility = self.cleaned_data.get("health_facility")
             else:
                 raise self.raise_validation_error(
-                    {"health_facility": "This field is required."}
+                    {"health_facility": "This field is required."}, INVALID_ERROR
                 )
         return self._health_facility
 
     def validate_date_is_on_clinic_day(self):
         if appt_date := self.cleaned_data.get("appt_date"):
             if not self.health_facility.clinic_days:
                 if appt_date.isoweekday() > 5:
```

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/list_data.py` & `edc-next-appointment-0.1.4/edc_next_appointment/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/migrations/0001_initial.py` & `edc-next-appointment-0.1.4/edc_next_appointment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/model_mixins.py` & `edc-next-appointment-0.1.4/edc_next_appointment/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/modeladmin_mixins.py` & `edc-next-appointment-0.1.4/edc_next_appointment/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/modelform_mixins.py` & `edc-next-appointment-0.1.4/edc_next_appointment/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-local-private.pem` & `edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem` & `edc-next-appointment-0.1.4/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/tests/holidays.csv` & `edc-next-appointment-0.1.4/edc_next_appointment/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/tests/tests/test_next_appointment.py` & `edc-next-appointment-0.1.4/edc_next_appointment/tests/tests/test_next_appointment.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment/utils.py` & `edc-next-appointment-0.1.4/edc_next_appointment/utils.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment.egg-info/PKG-INFO` & `edc-next-appointment-0.1.4/edc_next_appointment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: edc-next-appointment
-Version: 0.1.3
+Version: 0.1.4
 Summary: Base classes for managing next appointment CRF at each timepoint in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-next-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc appointment,scheduling,CRF,clinicedc,clinical trials
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
 
 edc-next-appointment
```

### Comparing `edc-next-appointment-0.1.3/edc_next_appointment.egg-info/SOURCES.txt` & `edc-next-appointment-0.1.4/edc_next_appointment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 edc_next_appointment.egg-info/dependency_links.txt
 edc_next_appointment.egg-info/not-zip-safe
 edc_next_appointment.egg-info/top_level.txt
 edc_next_appointment/form_validators/__init__.py
 edc_next_appointment/form_validators/form_validator_mixins.py
 edc_next_appointment/form_validators/next_appointment_form_validator.py
 edc_next_appointment/migrations/0001_initial.py
+edc_next_appointment/migrations/0002_infosources_extra_value.py
 edc_next_appointment/migrations/__init__.py
 edc_next_appointment/models/__init__.py
 edc_next_appointment/models/list_models.py
 edc_next_appointment/tests/__init__.py
 edc_next_appointment/tests/holidays.csv
 edc_next_appointment/tests/etc/user-aes-local.key
 edc_next_appointment/tests/etc/user-aes-restricted.key
```

### Comparing `edc-next-appointment-0.1.3/next_appointment_app/admin.py` & `edc-next-appointment-0.1.4/next_appointment_app/admin.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/next_appointment_app/models.py` & `edc-next-appointment-0.1.4/next_appointment_app/models.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/next_appointment_app/urls.py` & `edc-next-appointment-0.1.4/next_appointment_app/urls.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/next_appointment_app/visit_schedules.py` & `edc-next-appointment-0.1.4/next_appointment_app/visit_schedules.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/pyproject.toml` & `edc-next-appointment-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

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

### Comparing `edc-next-appointment-0.1.3/runtests.py` & `edc-next-appointment-0.1.4/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.3/setup.cfg` & `edc-next-appointment-0.1.4/setup.cfg`

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

