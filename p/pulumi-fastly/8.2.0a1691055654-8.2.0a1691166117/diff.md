# Comparing `tmp/pulumi_fastly-8.2.0a1691055654.tar.gz` & `tmp/pulumi_fastly-8.2.0a1691166117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.2.0a1691055654.tar", last modified: Thu Aug  3 09:46:18 2023, max compression
+gzip compressed data, was "pulumi_fastly-8.2.0a1691166117.tar", last modified: Fri Aug  4 16:26:23 2023, max compression
```

## Comparing `pulumi_fastly-8.2.0a1691055654.tar` & `pulumi_fastly-8.2.0a1691166117.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:46:18.606748 pulumi_fastly-8.2.0a1691055654/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-03 09:46:18.606748 pulumi_fastly-8.2.0a1691055654/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:46:18.602748 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   509912 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:46:18.606748 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)   454355 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    96684 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    35186 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:46:18.606748 pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:46:18.606748 pulumi_fastly-8.2.0a1691055654/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-03 09:46:18.000000 pulumi_fastly-8.2.0a1691055654/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:26:23.023555 pulumi_fastly-8.2.0a1691166117/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-04 16:26:23.023555 pulumi_fastly-8.2.0a1691166117/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:26:23.019555 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   508584 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:26:23.023555 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)   454421 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96684 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35186 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:26:23.023555 pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-04 16:26:23.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-04 16:26:23.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:26:23.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:26:23.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-04 16:26:23.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 16:26:23.000000 pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:26:23.023555 pulumi_fastly-8.2.0a1691166117/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-04 16:26:22.000000 pulumi_fastly-8.2.0a1691166117/setup.py
```

### Comparing `pulumi_fastly-8.2.0a1691055654/PKG-INFO` & `pulumi_fastly-8.2.0a1691166117/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.2.0a1691055654
+Version: 8.2.0a1691166117
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-8.2.0a1691055654/README.md` & `pulumi_fastly-8.2.0a1691166117/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/__init__.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .configstore import *
 from .configstore_entries import *
+from .get_configstores import *
 from .get_datacenters import *
 from .get_dictionaries import *
 from .get_fastly_ip_ranges import *
+from .get_kvstores import *
 from .get_package_hash import *
 from .get_services import *
 from .get_tls_activation import *
 from .get_tls_activation_ids import *
 from .get_tls_certificate import *
 from .get_tls_certificate_ids import *
 from .get_tls_configuration import *
```

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
 @pulumi.input_type
 class ServiceComputeBackendArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
                  name: pulumi.Input[str],
                  between_bytes_timeout: Optional[pulumi.Input[int]] = None,
                  connect_timeout: Optional[pulumi.Input[int]] = None,
-                 error_threshold: Optional[pulumi.Input[int]] = None,
                  first_byte_timeout: Optional[pulumi.Input[int]] = None,
                  healthcheck: Optional[pulumi.Input[str]] = None,
                  keepalive_time: Optional[pulumi.Input[int]] = None,
                  max_conn: Optional[pulumi.Input[int]] = None,
                  max_tls_version: Optional[pulumi.Input[str]] = None,
                  min_tls_version: Optional[pulumi.Input[str]] = None,
                  override_host: Optional[pulumi.Input[str]] = None,
@@ -207,15 +206,14 @@
                  use_ssl: Optional[pulumi.Input[bool]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] address: An IPv4, hostname, or IPv6 address for the Backend
         :param pulumi.Input[str] name: Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[int] between_bytes_timeout: How long to wait between bytes in milliseconds. Default `10000`
         :param pulumi.Input[int] connect_timeout: How long to wait for a timeout in milliseconds. Default `1000`
-        :param pulumi.Input[int] error_threshold: Number of errors to allow before the Backend is marked as down. Default `0`
         :param pulumi.Input[int] first_byte_timeout: How long to wait for the first bytes in milliseconds. Default `15000`
         :param pulumi.Input[str] healthcheck: Name of a defined `healthcheck` to assign to this backend
         :param pulumi.Input[int] keepalive_time: How long in seconds to keep a persistent connection to the backend between requests.
         :param pulumi.Input[int] max_conn: Maximum number of connections for this Backend. Default `200`
         :param pulumi.Input[str] max_tls_version: Maximum allowed TLS version on SSL connections to this backend.
         :param pulumi.Input[str] min_tls_version: Minimum allowed TLS version on SSL connections to this backend.
         :param pulumi.Input[str] override_host: The hostname to override the Host header
@@ -233,16 +231,14 @@
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         if between_bytes_timeout is not None:
             pulumi.set(__self__, "between_bytes_timeout", between_bytes_timeout)
         if connect_timeout is not None:
             pulumi.set(__self__, "connect_timeout", connect_timeout)
-        if error_threshold is not None:
-            pulumi.set(__self__, "error_threshold", error_threshold)
         if first_byte_timeout is not None:
             pulumi.set(__self__, "first_byte_timeout", first_byte_timeout)
         if healthcheck is not None:
             pulumi.set(__self__, "healthcheck", healthcheck)
         if keepalive_time is not None:
             pulumi.set(__self__, "keepalive_time", keepalive_time)
         if max_conn is not None:
@@ -321,26 +317,14 @@
         return pulumi.get(self, "connect_timeout")
 
     @connect_timeout.setter
     def connect_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "connect_timeout", value)
 
     @property
-    @pulumi.getter(name="errorThreshold")
-    def error_threshold(self) -> Optional[pulumi.Input[int]]:
-        """
-        Number of errors to allow before the Backend is marked as down. Default `0`
-        """
-        return pulumi.get(self, "error_threshold")
-
-    @error_threshold.setter
-    def error_threshold(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "error_threshold", value)
-
-    @property
     @pulumi.getter(name="firstByteTimeout")
     def first_byte_timeout(self) -> Optional[pulumi.Input[int]]:
         """
         How long to wait for the first bytes in milliseconds. Default `15000`
         """
         return pulumi.get(self, "first_byte_timeout")
 
@@ -4387,15 +4371,14 @@
 class ServiceVclBackendArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
                  name: pulumi.Input[str],
                  auto_loadbalance: Optional[pulumi.Input[bool]] = None,
                  between_bytes_timeout: Optional[pulumi.Input[int]] = None,
                  connect_timeout: Optional[pulumi.Input[int]] = None,
-                 error_threshold: Optional[pulumi.Input[int]] = None,
                  first_byte_timeout: Optional[pulumi.Input[int]] = None,
                  healthcheck: Optional[pulumi.Input[str]] = None,
                  keepalive_time: Optional[pulumi.Input[int]] = None,
                  max_conn: Optional[pulumi.Input[int]] = None,
                  max_tls_version: Optional[pulumi.Input[str]] = None,
                  min_tls_version: Optional[pulumi.Input[str]] = None,
                  override_host: Optional[pulumi.Input[str]] = None,
@@ -4413,15 +4396,14 @@
                  weight: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] address: An IPv4, hostname, or IPv6 address for the Backend
         :param pulumi.Input[str] name: Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[bool] auto_loadbalance: Denotes if this Backend should be included in the pool of backends that requests are load balanced against. Default `false`
         :param pulumi.Input[int] between_bytes_timeout: How long to wait between bytes in milliseconds. Default `10000`
         :param pulumi.Input[int] connect_timeout: How long to wait for a timeout in milliseconds. Default `1000`
-        :param pulumi.Input[int] error_threshold: Number of errors to allow before the Backend is marked as down. Default `0`
         :param pulumi.Input[int] first_byte_timeout: How long to wait for the first bytes in milliseconds. Default `15000`
         :param pulumi.Input[str] healthcheck: Name of a defined `healthcheck` to assign to this backend
         :param pulumi.Input[int] keepalive_time: How long in seconds to keep a persistent connection to the backend between requests.
         :param pulumi.Input[int] max_conn: Maximum number of connections for this Backend. Default `200`
         :param pulumi.Input[str] max_tls_version: Maximum allowed TLS version on SSL connections to this backend.
         :param pulumi.Input[str] min_tls_version: Minimum allowed TLS version on SSL connections to this backend.
         :param pulumi.Input[str] override_host: The hostname to override the Host header
@@ -4442,16 +4424,14 @@
         pulumi.set(__self__, "name", name)
         if auto_loadbalance is not None:
             pulumi.set(__self__, "auto_loadbalance", auto_loadbalance)
         if between_bytes_timeout is not None:
             pulumi.set(__self__, "between_bytes_timeout", between_bytes_timeout)
         if connect_timeout is not None:
             pulumi.set(__self__, "connect_timeout", connect_timeout)
-        if error_threshold is not None:
-            pulumi.set(__self__, "error_threshold", error_threshold)
         if first_byte_timeout is not None:
             pulumi.set(__self__, "first_byte_timeout", first_byte_timeout)
         if healthcheck is not None:
             pulumi.set(__self__, "healthcheck", healthcheck)
         if keepalive_time is not None:
             pulumi.set(__self__, "keepalive_time", keepalive_time)
         if max_conn is not None:
@@ -4544,26 +4524,14 @@
         return pulumi.get(self, "connect_timeout")
 
     @connect_timeout.setter
     def connect_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "connect_timeout", value)
 
     @property
-    @pulumi.getter(name="errorThreshold")
-    def error_threshold(self) -> Optional[pulumi.Input[int]]:
-        """
-        Number of errors to allow before the Backend is marked as down. Default `0`
-        """
-        return pulumi.get(self, "error_threshold")
-
-    @error_threshold.setter
-    def error_threshold(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "error_threshold", value)
-
-    @property
     @pulumi.getter(name="firstByteTimeout")
     def first_byte_timeout(self) -> Optional[pulumi.Input[int]]:
         """
         How long to wait for the first bytes in milliseconds. Default `15000`
         """
         return pulumi.get(self, "first_byte_timeout")
 
@@ -11236,15 +11204,15 @@
         :param pulumi.Input[bool] bypass_busy_wait: Disable collapsed forwarding, so you don't wait for other objects to origin
         :param pulumi.Input[str] default_host: Sets the host header
         :param pulumi.Input[bool] force_miss: Force a cache miss for the request. If specified, can be `true` or `false`
         :param pulumi.Input[bool] force_ssl: Forces the request to use SSL (Redirects a non-SSL request to SSL)
         :param pulumi.Input[bool] geo_headers: Injects Fastly-Geo-Country, Fastly-Geo-City, and Fastly-Geo-Region into the request headers
         :param pulumi.Input[str] hash_keys: Comma separated list of varnish request object fields that should be in the hash key
         :param pulumi.Input[int] max_stale_age: How old an object is allowed to be to serve `stale-if-error` or `stale-while-revalidate`, in seconds
-        :param pulumi.Input[str] request_condition: Name of already defined `condition` to determine if this request setting should be applied
+        :param pulumi.Input[str] request_condition: Name of already defined `condition` to determine if this request setting should be applied (should be unique across multiple instances of `request_setting`)
         :param pulumi.Input[bool] timer_support: Injects the X-Timer info into the request for viewing origin fetch durations
         :param pulumi.Input[str] xff: X-Forwarded-For, should be `clear`, `leave`, `append`, `append_all`, or `overwrite`. Default `append`
         """
         pulumi.set(__self__, "name", name)
         if action is not None:
             pulumi.set(__self__, "action", action)
         if bypass_busy_wait is not None:
@@ -11382,15 +11350,15 @@
     def max_stale_age(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_stale_age", value)
 
     @property
     @pulumi.getter(name="requestCondition")
     def request_condition(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of already defined `condition` to determine if this request setting should be applied
+        Name of already defined `condition` to determine if this request setting should be applied (should be unique across multiple instances of `request_setting`)
         """
         return pulumi.get(self, "request_condition")
 
     @request_condition.setter
     def request_condition(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "request_condition", value)
```

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/configstore.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_services.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/outputs.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,18 @@
     'ServiceVclSnippet',
     'ServiceVclVcl',
     'ServiceVclWaf',
     'ServiceWafConfigurationRule',
     'ServiceWafConfigurationRuleExclusion',
     'TlsSubscriptionManagedDnsChallenge',
     'TlsSubscriptionManagedHttpChallenge',
+    'GetConfigstoresStoreResult',
     'GetDatacentersPopResult',
     'GetDictionariesDictionaryResult',
+    'GetKvstoresStoreResult',
     'GetServicesDetailResult',
     'GetTlsConfigurationDnsRecordResult',
     'GetWafRulesRuleResult',
 ]
 
 @pulumi.output_type
 class ServiceACLEntriesEntry(dict):
@@ -171,16 +173,14 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "betweenBytesTimeout":
             suggest = "between_bytes_timeout"
         elif key == "connectTimeout":
             suggest = "connect_timeout"
-        elif key == "errorThreshold":
-            suggest = "error_threshold"
         elif key == "firstByteTimeout":
             suggest = "first_byte_timeout"
         elif key == "keepaliveTime":
             suggest = "keepalive_time"
         elif key == "maxConn":
             suggest = "max_conn"
         elif key == "maxTlsVersion":
@@ -218,15 +218,14 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  address: str,
                  name: str,
                  between_bytes_timeout: Optional[int] = None,
                  connect_timeout: Optional[int] = None,
-                 error_threshold: Optional[int] = None,
                  first_byte_timeout: Optional[int] = None,
                  healthcheck: Optional[str] = None,
                  keepalive_time: Optional[int] = None,
                  max_conn: Optional[int] = None,
                  max_tls_version: Optional[str] = None,
                  min_tls_version: Optional[str] = None,
                  override_host: Optional[str] = None,
@@ -242,15 +241,14 @@
                  use_ssl: Optional[bool] = None,
                  weight: Optional[int] = None):
         """
         :param str address: An IPv4, hostname, or IPv6 address for the Backend
         :param str name: Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
         :param int between_bytes_timeout: How long to wait between bytes in milliseconds. Default `10000`
         :param int connect_timeout: How long to wait for a timeout in milliseconds. Default `1000`
-        :param int error_threshold: Number of errors to allow before the Backend is marked as down. Default `0`
         :param int first_byte_timeout: How long to wait for the first bytes in milliseconds. Default `15000`
         :param str healthcheck: Name of a defined `healthcheck` to assign to this backend
         :param int keepalive_time: How long in seconds to keep a persistent connection to the backend between requests.
         :param int max_conn: Maximum number of connections for this Backend. Default `200`
         :param str max_tls_version: Maximum allowed TLS version on SSL connections to this backend.
         :param str min_tls_version: Minimum allowed TLS version on SSL connections to this backend.
         :param str override_host: The hostname to override the Host header
@@ -268,16 +266,14 @@
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         if between_bytes_timeout is not None:
             pulumi.set(__self__, "between_bytes_timeout", between_bytes_timeout)
         if connect_timeout is not None:
             pulumi.set(__self__, "connect_timeout", connect_timeout)
-        if error_threshold is not None:
-            pulumi.set(__self__, "error_threshold", error_threshold)
         if first_byte_timeout is not None:
             pulumi.set(__self__, "first_byte_timeout", first_byte_timeout)
         if healthcheck is not None:
             pulumi.set(__self__, "healthcheck", healthcheck)
         if keepalive_time is not None:
             pulumi.set(__self__, "keepalive_time", keepalive_time)
         if max_conn is not None:
@@ -340,22 +336,14 @@
     def connect_timeout(self) -> Optional[int]:
         """
         How long to wait for a timeout in milliseconds. Default `1000`
         """
         return pulumi.get(self, "connect_timeout")
 
     @property
-    @pulumi.getter(name="errorThreshold")
-    def error_threshold(self) -> Optional[int]:
-        """
-        Number of errors to allow before the Backend is marked as down. Default `0`
-        """
-        return pulumi.get(self, "error_threshold")
-
-    @property
     @pulumi.getter(name="firstByteTimeout")
     def first_byte_timeout(self) -> Optional[int]:
         """
         How long to wait for the first bytes in milliseconds. Default `15000`
         """
         return pulumi.get(self, "first_byte_timeout")
 
@@ -3977,16 +3965,14 @@
         suggest = None
         if key == "autoLoadbalance":
             suggest = "auto_loadbalance"
         elif key == "betweenBytesTimeout":
             suggest = "between_bytes_timeout"
         elif key == "connectTimeout":
             suggest = "connect_timeout"
-        elif key == "errorThreshold":
-            suggest = "error_threshold"
         elif key == "firstByteTimeout":
             suggest = "first_byte_timeout"
         elif key == "keepaliveTime":
             suggest = "keepalive_time"
         elif key == "maxConn":
             suggest = "max_conn"
         elif key == "maxTlsVersion":
@@ -4027,15 +4013,14 @@
 
     def __init__(__self__, *,
                  address: str,
                  name: str,
                  auto_loadbalance: Optional[bool] = None,
                  between_bytes_timeout: Optional[int] = None,
                  connect_timeout: Optional[int] = None,
-                 error_threshold: Optional[int] = None,
                  first_byte_timeout: Optional[int] = None,
                  healthcheck: Optional[str] = None,
                  keepalive_time: Optional[int] = None,
                  max_conn: Optional[int] = None,
                  max_tls_version: Optional[str] = None,
                  min_tls_version: Optional[str] = None,
                  override_host: Optional[str] = None,
@@ -4053,15 +4038,14 @@
                  weight: Optional[int] = None):
         """
         :param str address: An IPv4, hostname, or IPv6 address for the Backend
         :param str name: Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
         :param bool auto_loadbalance: Denotes if this Backend should be included in the pool of backends that requests are load balanced against. Default `false`
         :param int between_bytes_timeout: How long to wait between bytes in milliseconds. Default `10000`
         :param int connect_timeout: How long to wait for a timeout in milliseconds. Default `1000`
-        :param int error_threshold: Number of errors to allow before the Backend is marked as down. Default `0`
         :param int first_byte_timeout: How long to wait for the first bytes in milliseconds. Default `15000`
         :param str healthcheck: Name of a defined `healthcheck` to assign to this backend
         :param int keepalive_time: How long in seconds to keep a persistent connection to the backend between requests.
         :param int max_conn: Maximum number of connections for this Backend. Default `200`
         :param str max_tls_version: Maximum allowed TLS version on SSL connections to this backend.
         :param str min_tls_version: Minimum allowed TLS version on SSL connections to this backend.
         :param str override_host: The hostname to override the Host header
@@ -4082,16 +4066,14 @@
         pulumi.set(__self__, "name", name)
         if auto_loadbalance is not None:
             pulumi.set(__self__, "auto_loadbalance", auto_loadbalance)
         if between_bytes_timeout is not None:
             pulumi.set(__self__, "between_bytes_timeout", between_bytes_timeout)
         if connect_timeout is not None:
             pulumi.set(__self__, "connect_timeout", connect_timeout)
-        if error_threshold is not None:
-            pulumi.set(__self__, "error_threshold", error_threshold)
         if first_byte_timeout is not None:
             pulumi.set(__self__, "first_byte_timeout", first_byte_timeout)
         if healthcheck is not None:
             pulumi.set(__self__, "healthcheck", healthcheck)
         if keepalive_time is not None:
             pulumi.set(__self__, "keepalive_time", keepalive_time)
         if max_conn is not None:
@@ -4164,22 +4146,14 @@
     def connect_timeout(self) -> Optional[int]:
         """
         How long to wait for a timeout in milliseconds. Default `1000`
         """
         return pulumi.get(self, "connect_timeout")
 
     @property
-    @pulumi.getter(name="errorThreshold")
-    def error_threshold(self) -> Optional[int]:
-        """
-        Number of errors to allow before the Backend is marked as down. Default `0`
-        """
-        return pulumi.get(self, "error_threshold")
-
-    @property
     @pulumi.getter(name="firstByteTimeout")
     def first_byte_timeout(self) -> Optional[int]:
         """
         How long to wait for the first bytes in milliseconds. Default `15000`
         """
         return pulumi.get(self, "first_byte_timeout")
 
@@ -10146,15 +10120,15 @@
         :param bool bypass_busy_wait: Disable collapsed forwarding, so you don't wait for other objects to origin
         :param str default_host: Sets the host header
         :param bool force_miss: Force a cache miss for the request. If specified, can be `true` or `false`
         :param bool force_ssl: Forces the request to use SSL (Redirects a non-SSL request to SSL)
         :param bool geo_headers: Injects Fastly-Geo-Country, Fastly-Geo-City, and Fastly-Geo-Region into the request headers
         :param str hash_keys: Comma separated list of varnish request object fields that should be in the hash key
         :param int max_stale_age: How old an object is allowed to be to serve `stale-if-error` or `stale-while-revalidate`, in seconds
-        :param str request_condition: Name of already defined `condition` to determine if this request setting should be applied
+        :param str request_condition: Name of already defined `condition` to determine if this request setting should be applied (should be unique across multiple instances of `request_setting`)
         :param bool timer_support: Injects the X-Timer info into the request for viewing origin fetch durations
         :param str xff: X-Forwarded-For, should be `clear`, `leave`, `append`, `append_all`, or `overwrite`. Default `append`
         """
         pulumi.set(__self__, "name", name)
         if action is not None:
             pulumi.set(__self__, "action", action)
         if bypass_busy_wait is not None:
@@ -10253,15 +10227,15 @@
         """
         return pulumi.get(self, "max_stale_age")
 
     @property
     @pulumi.getter(name="requestCondition")
     def request_condition(self) -> Optional[str]:
         """
-        Name of already defined `condition` to determine if this request setting should be applied
+        Name of already defined `condition` to determine if this request setting should be applied (should be unique across multiple instances of `request_setting`)
         """
         return pulumi.get(self, "request_condition")
 
     @property
     @pulumi.getter(name="timerSupport")
     def timer_support(self) -> Optional[bool]:
         """
@@ -10823,14 +10797,39 @@
         """
         A list with the value(s) to which the DNS record should point.
         """
         return pulumi.get(self, "record_values")
 
 
 @pulumi.output_type
+class GetConfigstoresStoreResult(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 name: str):
+        """
+        :param str id: The ID of this resource.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The ID of this resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+
+@pulumi.output_type
 class GetDatacentersPopResult(dict):
     def __init__(__self__, *,
                  code: str,
                  group: str,
                  name: str,
                  shield: str):
         pulumi.set(__self__, "code", code)
@@ -10888,14 +10887,39 @@
     @property
     @pulumi.getter(name="writeOnly")
     def write_only(self) -> bool:
         return pulumi.get(self, "write_only")
 
 
 @pulumi.output_type
+class GetKvstoresStoreResult(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 name: str):
+        """
+        :param str id: The ID of this resource.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The ID of this resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+
+@pulumi.output_type
 class GetServicesDetailResult(dict):
     def __init__(__self__, *,
                  comment: str,
                  created_at: str,
                  customer_id: str,
                  id: str,
                  name: str,
```

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/provider.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly/user.py` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-fastly
-Version: 8.2.0a1691055654
+Version: 8.2.0a1691166117
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-8.2.0a1691055654/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.2.0a1691166117/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 README.md
 setup.py
 pulumi_fastly/__init__.py
 pulumi_fastly/_inputs.py
 pulumi_fastly/_utilities.py
 pulumi_fastly/configstore.py
 pulumi_fastly/configstore_entries.py
+pulumi_fastly/get_configstores.py
 pulumi_fastly/get_datacenters.py
 pulumi_fastly/get_dictionaries.py
 pulumi_fastly/get_fastly_ip_ranges.py
+pulumi_fastly/get_kvstores.py
 pulumi_fastly/get_package_hash.py
 pulumi_fastly/get_services.py
 pulumi_fastly/get_tls_activation.py
 pulumi_fastly/get_tls_activation_ids.py
 pulumi_fastly/get_tls_certificate.py
 pulumi_fastly/get_tls_certificate_ids.py
 pulumi_fastly/get_tls_configuration.py
```

### Comparing `pulumi_fastly-8.2.0a1691055654/setup.py` & `pulumi_fastly-8.2.0a1691166117/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "8.2.0a1691055654"
-PLUGIN_VERSION = "8.2.0-alpha.1691055654+0cf364a6"
+VERSION = "8.2.0a1691166117"
+PLUGIN_VERSION = "8.2.0-alpha.1691166117+78b1d13d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'fastly', PLUGIN_VERSION])
         except OSError as error:
```

