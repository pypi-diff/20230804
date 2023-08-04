# Comparing `tmp/edc-rx-0.1.8.tar.gz` & `tmp/edc-rx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-rx-0.1.8.tar", last modified: Tue Aug  1 05:30:14 2023, max compression
+gzip compressed data, was "edc-rx-0.1.9.tar", last modified: Fri Aug  4 04:17:45 2023, max compression
```

## Comparing `edc-rx-0.1.8.tar` & `edc-rx-0.1.9.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.360447 edc-rx-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.351813 edc-rx-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.355169 edc-rx-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 15:54:44.000000 edc-rx-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-24 15:54:44.000000 edc-rx-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-08-01 05:30:14.360540 edc-rx-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.8/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.356082 edc-rx-0.1.8/edc_rx/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.357295 edc-rx-0.1.8/edc_rx/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.8/edc_rx/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.8/edc_rx/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.357886 edc-rx-0.1.8/edc_rx/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1610 2023-08-01 05:30:07.000000 edc-rx-0.1.8/edc_rx/model_mixins/drug_refill_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.8/edc_rx/model_mixins/drug_supply_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.8/edc_rx/model_mixins/treatment_pay_methods.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.358404 edc-rx-0.1.8/edc_rx/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1237 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      723 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.358769 edc-rx-0.1.8/edc_rx/modelform_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/modelform_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2047 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.358912 edc-rx-0.1.8/edc_rx/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.8/edc_rx/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.360070 edc-rx-0.1.8/edc_rx/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.360309 edc-rx-0.1.8/edc_rx/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.8/edc_rx/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4204 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/tests/tests/test_utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      757 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.356927 edc-rx-0.1.8/edc_rx.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-08-01 05:30:14.000000 edc-rx-0.1.8/edc_rx.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1335 2023-08-01 05:30:14.000000 edc-rx-0.1.8/edc_rx.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 05:30:14.000000 edc-rx-0.1.8/edc_rx.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.8/edc_rx.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-08-01 05:30:14.000000 edc-rx-0.1.8/edc_rx.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 15:54:44.000000 edc-rx-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-08-01 05:30:14.360826 edc-rx-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.566882 edc-rx-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.558284 edc-rx-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.561585 edc-rx-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1927 2023-08-04 04:17:38.000000 edc-rx-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-24 15:54:44.000000 edc-rx-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1436 2023-08-04 04:17:45.566970 edc-rx-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.9/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.562330 edc-rx-0.1.9/edc_rx/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.563570 edc-rx-0.1.9/edc_rx/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.9/edc_rx/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2023-08-04 04:17:38.000000 edc-rx-0.1.9/edc_rx/migrations/0002_rxmodificationreasons_extra_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.9/edc_rx/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.564279 edc-rx-0.1.9/edc_rx/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1610 2023-08-01 05:30:07.000000 edc-rx-0.1.9/edc_rx/model_mixins/drug_refill_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.9/edc_rx/model_mixins/drug_supply_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.9/edc_rx/model_mixins/treatment_pay_methods.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.564859 edc-rx-0.1.9/edc_rx/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1237 2023-07-12 23:50:53.000000 edc-rx-0.1.9/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      723 2023-07-12 23:50:53.000000 edc-rx-0.1.9/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.565213 edc-rx-0.1.9/edc_rx/modelform_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/modelform_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2047 2023-07-12 23:50:53.000000 edc-rx-0.1.9/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.565358 edc-rx-0.1.9/edc_rx/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.9/edc_rx/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.566521 edc-rx-0.1.9/edc_rx/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.566758 edc-rx-0.1.9/edc_rx/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.9/edc_rx/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4204 2023-07-12 23:50:53.000000 edc-rx-0.1.9/edc_rx/tests/tests/test_utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.9/edc_rx/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      757 2023-07-12 23:50:53.000000 edc-rx-0.1.9/edc_rx/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-04 04:17:45.563109 edc-rx-0.1.9/edc_rx.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1436 2023-08-04 04:17:45.000000 edc-rx-0.1.9/edc_rx.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1404 2023-08-04 04:17:45.000000 edc-rx-0.1.9/edc_rx.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-04 04:17:45.000000 edc-rx-0.1.9/edc_rx.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.9/edc_rx.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-08-04 04:17:45.000000 edc-rx-0.1.9/edc_rx.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1719 2023-08-04 04:17:38.000000 edc-rx-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1126 2023-08-04 04:17:45.567249 edc-rx-0.1.9/setup.cfg
```

### Comparing `edc-rx-0.1.8/.github/workflows/build.yml` & `edc-rx-0.1.9/.github/workflows/build.yml`

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

### Comparing `edc-rx-0.1.8/.gitignore` & `edc-rx-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/.pre-commit-config.yaml` & `edc-rx-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/LICENSE` & `edc-rx-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/PKG-INFO` & `edc-rx-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Medications refill and supply model/form mixins for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
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
```

### Comparing `edc-rx-0.1.8/README.rst` & `edc-rx-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/migrations/0001_initial.py` & `edc-rx-0.1.9/edc_rx/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/model_mixins/drug_refill_model_mixin.py` & `edc-rx-0.1.9/edc_rx/model_mixins/drug_refill_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/model_mixins/drug_supply_model_mixin.py` & `edc-rx-0.1.9/edc_rx/model_mixins/drug_supply_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/model_mixins/treatment_pay_methods.py` & `edc-rx-0.1.9/edc_rx/model_mixins/treatment_pay_methods.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py` & `edc-rx-0.1.9/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py` & `edc-rx-0.1.9/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py` & `edc-rx-0.1.9/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-local-private.pem` & `edc-rx-0.1.9/edc_rx/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-restricted-private.pem` & `edc-rx-0.1.9/edc_rx/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/tests/tests/test_utils.py` & `edc-rx-0.1.9/edc_rx/tests/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx/utils.py` & `edc-rx-0.1.9/edc_rx/utils.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/edc_rx.egg-info/PKG-INFO` & `edc-rx-0.1.9/edc_rx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Medications refill and supply model/form mixins for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
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
```

### Comparing `edc-rx-0.1.8/edc_rx.egg-info/SOURCES.txt` & `edc-rx-0.1.9/edc_rx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 edc_rx/utils.py
 edc_rx.egg-info/PKG-INFO
 edc_rx.egg-info/SOURCES.txt
 edc_rx.egg-info/dependency_links.txt
 edc_rx.egg-info/not-zip-safe
 edc_rx.egg-info/top_level.txt
 edc_rx/migrations/0001_initial.py
+edc_rx/migrations/0002_rxmodificationreasons_extra_value_and_more.py
 edc_rx/migrations/__init__.py
 edc_rx/model_mixins/__init__.py
 edc_rx/model_mixins/drug_refill_model_mixin.py
 edc_rx/model_mixins/drug_supply_model_mixin.py
 edc_rx/model_mixins/treatment_pay_methods.py
 edc_rx/modeladmin_mixins/__init__.py
 edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
```

### Comparing `edc-rx-0.1.8/pyproject.toml` & `edc-rx-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

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

### Comparing `edc-rx-0.1.8/runtests.py` & `edc-rx-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.8/setup.cfg` & `edc-rx-0.1.9/setup.cfg`

 * *Files 9% similar despite different names*

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

