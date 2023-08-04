# Comparing `tmp/onqlave-python-dev-0.0.2.tar.gz` & `tmp/onqlave-python-dev-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onqlave-python-dev-0.0.2.tar", last modified: Thu Aug  3 06:07:21 2023, max compression
+gzip compressed data, was "onqlave-python-dev-0.1.0.tar", last modified: Fri Aug  4 06:45:26 2023, max compression
```

## Comparing `onqlave-python-dev-0.0.2.tar` & `onqlave-python-dev-0.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.955350 onqlave-python-dev-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-08-03 06:07:21.955350 onqlave-python-dev-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.935349 onqlave-python-dev-0.0.2/onqlave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.939349 onqlave-python-dev-0.0.2/onqlave/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/connection/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.939349 onqlave-python-dev-0.0.2/onqlave/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.939349 onqlave-python-dev-0.0.2/onqlave/contracts/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/contracts/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/contracts/requests/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.939349 onqlave-python-dev-0.0.2/onqlave/contracts/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/contracts/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/contracts/responses/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.939349 onqlave-python-dev-0.0.2/onqlave/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/credentials/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.943349 onqlave-python-dev-0.0.2/onqlave/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/encryption/encrypted_stream_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/encryption/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/encryption/plain_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.943349 onqlave-python-dev-0.0.2/onqlave/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/errors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.943349 onqlave-python-dev-0.0.2/onqlave/keymanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.947349 onqlave-python-dev-0.0.2/onqlave/keymanager/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/factories/aes_gcm_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/factories/xchacha20_poly1305_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/id_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/key_manager_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.947349 onqlave-python-dev-0.0.2/onqlave/keymanager/keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/keys/aes_gcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/keys/xchacha_20_poly_1350.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.947349 onqlave-python-dev-0.0.2/onqlave/keymanager/onqlave_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/onqlave_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/onqlave_types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.947349 onqlave-python-dev-0.0.2/onqlave/keymanager/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/operations/aes_128_gcm_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/operations/aes_256_gcm_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.951349 onqlave-python-dev-0.0.2/onqlave/keymanager/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/primitives/aes_gcm_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/keymanager/random_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.951349 onqlave-python-dev-0.0.2/onqlave/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.951349 onqlave-python-dev-0.0.2/onqlave/messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/messages/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.951349 onqlave-python-dev-0.0.2/onqlave/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-03 06:07:02.000000 onqlave-python-dev-0.0.2/onqlave/utils/hasher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:07:21.955350 onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-08-03 06:07:21.000000 onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-03 06:07:21.000000 onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:07:21.000000 onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-03 06:07:21.000000 onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 06:07:21.000000 onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:07:21.955350 onqlave-python-dev-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-03 06:07:21.000000 onqlave-python-dev-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.965674 onqlave-python-dev-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-04 06:45:26.965674 onqlave-python-dev-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.957674 onqlave-python-dev-0.1.0/onqlave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.957674 onqlave-python-dev-0.1.0/onqlave/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/connection/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.957674 onqlave-python-dev-0.1.0/onqlave/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.957674 onqlave-python-dev-0.1.0/onqlave/contracts/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/contracts/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/contracts/requests/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.957674 onqlave-python-dev-0.1.0/onqlave/contracts/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/contracts/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/contracts/responses/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.957674 onqlave-python-dev-0.1.0/onqlave/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/credentials/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.961674 onqlave-python-dev-0.1.0/onqlave/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/encryption/encrypted_stream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/encryption/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/encryption/plain_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.961674 onqlave-python-dev-0.1.0/onqlave/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/errors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.961674 onqlave-python-dev-0.1.0/onqlave/keymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.961674 onqlave-python-dev-0.1.0/onqlave/keymanager/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/factories/aes_gcm_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/factories/xchacha20_poly1305_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/id_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/key_manager_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.961674 onqlave-python-dev-0.1.0/onqlave/keymanager/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/keys/aes_gcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/keys/xchacha_20_poly_1350.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.961674 onqlave-python-dev-0.1.0/onqlave/keymanager/onqlave_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/onqlave_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/onqlave_types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.961674 onqlave-python-dev-0.1.0/onqlave/keymanager/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/operations/aes_128_gcm_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/operations/aes_256_gcm_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.961674 onqlave-python-dev-0.1.0/onqlave/keymanager/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/primitives/aes_gcm_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/keymanager/random_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.965674 onqlave-python-dev-0.1.0/onqlave/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.965674 onqlave-python-dev-0.1.0/onqlave/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/messages/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.965674 onqlave-python-dev-0.1.0/onqlave/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-04 06:45:12.000000 onqlave-python-dev-0.1.0/onqlave/utils/hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:45:26.965674 onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-04 06:45:26.000000 onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-04 06:45:26.000000 onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 06:45:26.000000 onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-04 06:45:26.000000 onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 06:45:26.000000 onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 06:45:26.965674 onqlave-python-dev-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-04 06:45:26.000000 onqlave-python-dev-0.1.0/setup.py
```

### Comparing `onqlave-python-dev-0.0.2/LICENSE` & `onqlave-python-dev-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/PKG-INFO` & `onqlave-python-dev-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: onqlave-python-dev
-Version: 0.0.2
+Version: 0.1.0
 Summary: This Python SDK is designed to help developers easily integrate Onqlave Encryption As A Service into their python backend.
-Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
+Home-page: https://github.com/onqlavelabs/onqlave-python/
 Download-URL: https://pypi.org/project/onqlave-python-dev/#history
 Author: Onqlave Pty
 Author-email: product@onqlave.com
 Maintainer: DC
 Maintainer-email: dc@onqlave.com
 License: MIT
 Project-URL: Home Page, https://www.onqlave.com/
 Project-URL: Issue Tracker, https://github.com/onqlavelabs/onqlave-python/issues
-Project-URL: Source Code, https://github.com/onqlavelabs/onqlave-python/tree/dev
+Project-URL: Source Code, https://github.com/onqlavelabs/onqlave-python/
 Keywords: encryption,privacy,sdk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -24,19 +24,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Description
 This Python SDK is designed to help developers easily integrate Onqlave `Encryption As A Service` into their python backend.
 
-
-[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-go)](https://github.com/onqlavelabs/onqlave-go/blob/main/LICENSE)
+[![CI](https://img.shields.io/static/v1?label=CI&message=passing&color=green?style=plastic&logo=github)](https://github.com/onqlavelabs/onqlave-python/actions)
+[![GitHub release](https://img.shields.io/github/v/release/onqlavelabs/onqlave-go.svg)](https://github.com/onqlavelabs/onqlave-python/releases)
+[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-python)](https://github.com/onqlavelabs/onqlave-python/blob/main/LICENSE)
 
 
 # Table of Contents
 
 - [Description](#description)
 - [Table of Contents](#table-of-contents)
 	- [Features](#features)
@@ -62,15 +62,15 @@
 
 ### Configuration
 To install, simply using this command:
 
 ```bash
 pip install onqlave-python-sdk-pilot
 ```
-You can also check the [package detail on PyPI](https://pypi.org/project/onqlave-python-sdk-pilot)
+You can also check the [package detail on PyPI](https://pypi.org/project/onqlave-python)
 
 ## Usage
 To use this SDK, you firstly need to obtain credentials to access an Onqlave Arx by signing up to [Onqlave](https://onqlave.com) and following instruction to create your first Onqlave Arx. Documentation can be found at [Onqlave Technical Documentation](https://docs.onqlave.com).
 
 The [Onqlave Python](https://github.com/onqlavelabs/onqlave-python) module is used to perform operations on the configured Arx such as encrypting and decryptin for an Onqlave Arx. 
 
 To use this module, an Onqlave client should be initialized as follows.
```

### Comparing `onqlave-python-dev-0.0.2/README.md` & `onqlave-python-dev-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Description
 This Python SDK is designed to help developers easily integrate Onqlave `Encryption As A Service` into their python backend.
 
-
-[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-go)](https://github.com/onqlavelabs/onqlave-go/blob/main/LICENSE)
+[![CI](https://img.shields.io/static/v1?label=CI&message=passing&color=green?style=plastic&logo=github)](https://github.com/onqlavelabs/onqlave-python/actions)
+[![GitHub release](https://img.shields.io/github/v/release/onqlavelabs/onqlave-go.svg)](https://github.com/onqlavelabs/onqlave-python/releases)
+[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-python)](https://github.com/onqlavelabs/onqlave-python/blob/main/LICENSE)
 
 
 # Table of Contents
 
 - [Description](#description)
 - [Table of Contents](#table-of-contents)
 	- [Features](#features)
@@ -32,15 +32,15 @@
 
 ### Configuration
 To install, simply using this command:
 
 ```bash
 pip install onqlave-python-sdk-pilot
 ```
-You can also check the [package detail on PyPI](https://pypi.org/project/onqlave-python-sdk-pilot)
+You can also check the [package detail on PyPI](https://pypi.org/project/onqlave-python)
 
 ## Usage
 To use this SDK, you firstly need to obtain credentials to access an Onqlave Arx by signing up to [Onqlave](https://onqlave.com) and following instruction to create your first Onqlave Arx. Documentation can be found at [Onqlave Technical Documentation](https://docs.onqlave.com).
 
 The [Onqlave Python](https://github.com/onqlavelabs/onqlave-python) module is used to perform operations on the configured Arx such as encrypting and decryptin for an Onqlave Arx. 
 
 To use this module, an Onqlave client should be initialized as follows.
```

### Comparing `onqlave-python-dev-0.0.2/onqlave/connection/client.py` & `onqlave-python-dev-0.1.0/onqlave/connection/client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/connection/connection.py` & `onqlave-python-dev-0.1.0/onqlave/connection/connection.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/contracts/requests/requests.py` & `onqlave-python-dev-0.1.0/onqlave/contracts/requests/requests.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/contracts/responses/responses.py` & `onqlave-python-dev-0.1.0/onqlave/contracts/responses/responses.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/credentials/credentials.py` & `onqlave-python-dev-0.1.0/onqlave/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/encryption/encrypted_stream_processor.py` & `onqlave-python-dev-0.1.0/onqlave/encryption/encrypted_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/encryption/encryption.py` & `onqlave-python-dev-0.1.0/onqlave/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/encryption/options.py` & `onqlave-python-dev-0.1.0/onqlave/encryption/options.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/encryption/plain_stream_processor.py` & `onqlave-python-dev-0.1.0/onqlave/encryption/plain_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/errors/errors.py` & `onqlave-python-dev-0.1.0/onqlave/errors/errors.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/factories/aes_gcm_factory.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/factories/aes_gcm_factory.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/factories/xchacha20_poly1305_factory.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/factories/xchacha20_poly1305_factory.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/id_service.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/id_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/key_manager_client.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/key_manager_client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/keys/aes_gcm.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/keys/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/keys/xchacha_20_poly_1350.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/keys/xchacha_20_poly_1350.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/onqlave_types/types.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/onqlave_types/types.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/operations/aes_128_gcm_operation.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/operations/aes_128_gcm_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/operations/aes_256_gcm_operation.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/operations/aes_256_gcm_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/operations/xchacha20_poly1305_operation.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/operations/xchacha20_poly1305_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/primitives/aes_gcm_aead.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/primitives/aes_gcm_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/keymanager/random_service.py` & `onqlave-python-dev-0.1.0/onqlave/keymanager/random_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/messages/messages.py` & `onqlave-python-dev-0.1.0/onqlave/messages/messages.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave/utils/hasher.py` & `onqlave-python-dev-0.1.0/onqlave/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/PKG-INFO` & `onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: onqlave-python-dev
-Version: 0.0.2
+Version: 0.1.0
 Summary: This Python SDK is designed to help developers easily integrate Onqlave Encryption As A Service into their python backend.
-Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
+Home-page: https://github.com/onqlavelabs/onqlave-python/
 Download-URL: https://pypi.org/project/onqlave-python-dev/#history
 Author: Onqlave Pty
 Author-email: product@onqlave.com
 Maintainer: DC
 Maintainer-email: dc@onqlave.com
 License: MIT
 Project-URL: Home Page, https://www.onqlave.com/
 Project-URL: Issue Tracker, https://github.com/onqlavelabs/onqlave-python/issues
-Project-URL: Source Code, https://github.com/onqlavelabs/onqlave-python/tree/dev
+Project-URL: Source Code, https://github.com/onqlavelabs/onqlave-python/
 Keywords: encryption,privacy,sdk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -24,19 +24,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Description
 This Python SDK is designed to help developers easily integrate Onqlave `Encryption As A Service` into their python backend.
 
-
-[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-go)](https://github.com/onqlavelabs/onqlave-go/blob/main/LICENSE)
+[![CI](https://img.shields.io/static/v1?label=CI&message=passing&color=green?style=plastic&logo=github)](https://github.com/onqlavelabs/onqlave-python/actions)
+[![GitHub release](https://img.shields.io/github/v/release/onqlavelabs/onqlave-go.svg)](https://github.com/onqlavelabs/onqlave-python/releases)
+[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-python)](https://github.com/onqlavelabs/onqlave-python/blob/main/LICENSE)
 
 
 # Table of Contents
 
 - [Description](#description)
 - [Table of Contents](#table-of-contents)
 	- [Features](#features)
@@ -62,15 +62,15 @@
 
 ### Configuration
 To install, simply using this command:
 
 ```bash
 pip install onqlave-python-sdk-pilot
 ```
-You can also check the [package detail on PyPI](https://pypi.org/project/onqlave-python-sdk-pilot)
+You can also check the [package detail on PyPI](https://pypi.org/project/onqlave-python)
 
 ## Usage
 To use this SDK, you firstly need to obtain credentials to access an Onqlave Arx by signing up to [Onqlave](https://onqlave.com) and following instruction to create your first Onqlave Arx. Documentation can be found at [Onqlave Technical Documentation](https://docs.onqlave.com).
 
 The [Onqlave Python](https://github.com/onqlavelabs/onqlave-python) module is used to perform operations on the configured Arx such as encrypting and decryptin for an Onqlave Arx. 
 
 To use this module, an Onqlave client should be initialized as follows.
```

### Comparing `onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/SOURCES.txt` & `onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-dev-0.0.2/onqlave_python_dev.egg-info/requires.txt` & `onqlave-python-dev-0.1.0/onqlave_python_dev.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 attrs==23.1.0
 bleach==6.0.0
 build==0.10.0
-certifi==2023.5.7
+certifi==2023.7.22
 cffi==1.15.1
 charset-normalizer==3.1.0
-cryptography==41.0.1
+cryptography==41.0.3
 docutils==0.20.1
 frozenlist==1.4.0
 idna==3.4
 importlib-metadata==6.7.0
 importlib-resources==5.12.0
 jaraco-classes==3.2.3
 jeepney==0.8.0
```

### Comparing `onqlave-python-dev-0.0.2/setup.py` & `onqlave-python-dev-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 long_description = (this_directory / "README.md").read_text()
 
 package_name = 'onqlave-python-dev'
 download_url = format('https://pypi.org/project/%s/#history' % package_name)
 
 setup(
     name=package_name,
-    version='0.0.2',
+    version='0.1.0',
     author='Onqlave Pty',
     author_email='product@onqlave.com',
     maintainer='DC',
     maintainer_email='dc@onqlave.com',
     description='This Python SDK is designed to help developers easily integrate Onqlave Encryption As A Service into their python backend.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/onqlavelabs/onqlave-python/tree/dev', 
+    url='https://github.com/onqlavelabs/onqlave-python/', 
     download_url=download_url,
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
@@ -36,15 +36,15 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Security',
     ],
     project_urls = {
         "Home Page":"https://www.onqlave.com/",
         "Issue Tracker": "https://github.com/onqlavelabs/onqlave-python/issues",
-        "Source Code": "https://github.com/onqlavelabs/onqlave-python/tree/dev",
+        "Source Code": "https://github.com/onqlavelabs/onqlave-python/",
         
     },
 
     keywords=['encryption','privacy','sdk'],
     license='MIT',
 
     install_requires=requirements
```

