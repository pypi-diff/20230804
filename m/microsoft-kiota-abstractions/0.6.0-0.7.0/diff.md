# Comparing `tmp/microsoft_kiota_abstractions-0.6.0.tar.gz` & `tmp/microsoft_kiota_abstractions-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_abstractions-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_abstractions-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_abstractions-0.6.0.tar` & `microsoft_kiota_abstractions-0.7.0.tar`

### file list

```diff
@@ -1,69 +1,73 @@
--rw-r--r--   0        0        0       82 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1987 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2538 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1097 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1799 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.gitignore
--rw-r--r--   0        0        0    15931 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.pylintrc
--rw-r--r--   0        0        0     1281 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/LICENSE
--rw-r--r--   0        0        0      335 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/Makefile
--rw-r--r--   0        0        0     2512 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/README.md
--rw-r--r--   0        0        0     2757 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/__init__.py
--rw-r--r--   0        0        0       23 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/_version.py
--rw-r--r--   0        0        0     3566 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/api_client_builder.py
--rw-r--r--   0        0        0      399 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/api_error.py
--rw-r--r--   0        0        0      673 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/__init__.py
--rw-r--r--   0        0        0      836 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/access_token_provider.py
--rw-r--r--   0        0        0     2120 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/allowed_hosts_validator.py
--rw-r--r--   0        0        0      607 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/anonymous_authentication_provider.py
--rw-r--r--   0        0        0     2341 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/api_key_authentication_provider.py
--rw-r--r--   0        0        0      473 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/authentication_provider.py
--rw-r--r--   0        0        0     1231 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
--rw-r--r--   0        0        0     1252 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/base_request_builder.py
--rw-r--r--   0        0        0      667 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/base_request_configuration.py
--rw-r--r--   0        0        0      372 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/default_query_parameters.py
--rw-r--r--   0        0        0      453 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/get_path_parameters.py
--rw-r--r--   0        0        0      529 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/method.py
--rw-r--r--   0        0        0      938 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/native_response_handler.py
--rw-r--r--   0        0        0     5164 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_adapter.py
--rw-r--r--   0        0        0     9048 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_information.py
--rw-r--r--   0        0        0      312 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_option.py
--rw-r--r--   0        0        0      965 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/response_handler.py
--rw-r--r--   0        0        0      679 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/__init__.py
--rw-r--r--   0        0        0      374 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/additional_data_holder.py
--rw-r--r--   0        0        0     1006 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parsable.py
--rw-r--r--   0        0        0      642 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parsable_factory.py
--rw-r--r--   0        0        0     5793 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node.py
--rw-r--r--   0        0        0      903 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_factory.py
--rw-r--r--   0        0        0     1972 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_factory_registry.py
--rw-r--r--   0        0        0      949 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_helper.py
--rw-r--r--   0        0        0     2424 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_proxy_factory.py
--rw-r--r--   0        0        0     9768 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer.py
--rw-r--r--   0        0        0      898 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_factory.py
--rw-r--r--   0        0        0     2025 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_factory_registry.py
--rw-r--r--   0        0        0     3132 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0      529 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/__init__.py
--rw-r--r--   0        0        0      398 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backed_model.py
--rw-r--r--   0        0        0     3892 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store.py
--rw-r--r--   0        0        0      424 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_factory.py
--rw-r--r--   0        0        0      237 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_factory_singleton.py
--rw-r--r--   0        0        0     1166 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_parse_node_factory.py
--rw-r--r--   0        0        0     1809 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0     4488 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/in_memory_backing_store.py
--rw-r--r--   0        0        0      380 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/in_memory_backing_store_factory.py
--rw-r--r--   0        0        0      899 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/utils.py
--rw-r--r--   0        0        0     1268 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1130 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/authentication/__init__.py
--rw-r--r--   0        0        0     2340 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/authentication/test_api_key_authentication_provider.py
--rw-r--r--   0        0        0     1041 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/authentication/test_base_bearer_token_authentication.py
--rw-r--r--   0        0        0      831 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     5109 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/test_request_information.py
--rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1987 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2538 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1097 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1799 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.gitignore
+-rw-r--r--   0        0        0    15931 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/.pylintrc
+-rw-r--r--   0        0        0     1497 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/LICENSE
+-rw-r--r--   0        0        0      335 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/Makefile
+-rw-r--r--   0        0        0     2512 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/README.md
+-rw-r--r--   0        0        0     2757 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/__init__.py
+-rw-r--r--   0        0        0       23 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/_version.py
+-rw-r--r--   0        0        0     3566 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/api_client_builder.py
+-rw-r--r--   0        0        0      399 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/api_error.py
+-rw-r--r--   0        0        0      673 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/__init__.py
+-rw-r--r--   0        0        0      836 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/access_token_provider.py
+-rw-r--r--   0        0        0     2120 2023-08-04 12:20:07.074132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/allowed_hosts_validator.py
+-rw-r--r--   0        0        0      607 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/anonymous_authentication_provider.py
+-rw-r--r--   0        0        0     2341 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/api_key_authentication_provider.py
+-rw-r--r--   0        0        0      473 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/authentication_provider.py
+-rw-r--r--   0        0        0     1231 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
+-rw-r--r--   0        0        0     1252 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/base_request_builder.py
+-rw-r--r--   0        0        0      667 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/base_request_configuration.py
+-rw-r--r--   0        0        0      372 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/default_query_parameters.py
+-rw-r--r--   0        0        0      453 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/get_path_parameters.py
+-rw-r--r--   0        0        0      529 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/method.py
+-rw-r--r--   0        0        0      938 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/native_response_handler.py
+-rw-r--r--   0        0        0     5758 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/request_adapter.py
+-rw-r--r--   0        0        0     9016 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/request_information.py
+-rw-r--r--   0        0        0      313 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/request_option.py
+-rw-r--r--   0        0        0      965 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/response_handler.py
+-rw-r--r--   0        0        0      679 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/__init__.py
+-rw-r--r--   0        0        0      374 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/additional_data_holder.py
+-rw-r--r--   0        0        0     1006 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parsable.py
+-rw-r--r--   0        0        0      642 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parsable_factory.py
+-rw-r--r--   0        0        0     5887 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node.py
+-rw-r--r--   0        0        0      903 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node_factory.py
+-rw-r--r--   0        0        0     1972 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node_factory_registry.py
+-rw-r--r--   0        0        0      949 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node_helper.py
+-rw-r--r--   0        0        0     2801 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node_proxy_factory.py
+-rw-r--r--   0        0        0     9885 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/serialization_writer.py
+-rw-r--r--   0        0        0      898 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/serialization_writer_factory.py
+-rw-r--r--   0        0        0     2025 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/serialization_writer_factory_registry.py
+-rw-r--r--   0        0        0     3532 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0      528 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/__init__.py
+-rw-r--r--   0        0        0     1226 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/backed_model.py
+-rw-r--r--   0        0        0     4599 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/backing_store.py
+-rw-r--r--   0        0        0      741 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/backing_store_factory.py
+-rw-r--r--   0        0        0     2283 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/backing_store_factory_singleton.py
+-rw-r--r--   0        0        0     1327 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/backing_store_parse_node_factory.py
+-rw-r--r--   0        0        0     2119 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0     8437 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/in_memory_backing_store.py
+-rw-r--r--   0        0        0      697 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/in_memory_backing_store_factory.py
+-rw-r--r--   0        0        0      899 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/kiota_abstractions/utils.py
+-rw-r--r--   0        0        0     1268 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1132 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/authentication/__init__.py
+-rw-r--r--   0        0        0     2269 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/authentication/test_api_key_authentication_provider.py
+-rw-r--r--   0        0        0     1041 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/authentication/test_base_bearer_token_authentication.py
+-rw-r--r--   0        0        0     4925 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/store/__init__.py
+-rw-r--r--   0        0        0     1270 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/store/test_backed_model.py
+-rw-r--r--   0        0        0     3140 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/store/test_backing_store_factory_singleton.py
+-rw-r--r--   0        0        0    11623 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/store/test_in_memory_backing_store.py
+-rw-r--r--   0        0        0     5109 2023-08-04 12:20:07.078132 microsoft_kiota_abstractions-0.7.0/tests/test_request_information.py
+-rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-0.7.0/PKG-INFO
```

### Comparing `microsoft_kiota_abstractions-0.6.0/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_abstractions-0.7.0/.github/workflows/auto-merge-dependabot.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/.github/workflows/build.yml` & `microsoft_kiota_abstractions-0.7.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_abstractions-0.7.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_abstractions-0.7.0/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/.github/workflows/publish.yml` & `microsoft_kiota_abstractions-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/.gitignore` & `microsoft_kiota_abstractions-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/.pylintrc` & `microsoft_kiota_abstractions-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/CHANGELOG.md` & `microsoft_kiota_abstractions-0.7.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.0] - 2023-07-27
+
+### Added
+- Added an abstract translator method that should convert a `RequestInformation` object into the native client HTTP request object.
+- Enable backing store for Python.
+
+### Changed
+
 ## [0.6.0] - 2023-06-27
 
 ### Added
 - API key authentication provider.
 
 ### Changed
```

### Comparing `microsoft_kiota_abstractions-0.6.0/LICENSE` & `microsoft_kiota_abstractions-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/README.md` & `microsoft_kiota_abstractions-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/SECURITY.md` & `microsoft_kiota_abstractions-0.7.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/SUPPORT.md` & `microsoft_kiota_abstractions-0.7.0/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/api_client_builder.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/__init__.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/access_token_provider.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/access_token_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/allowed_hosts_validator.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/allowed_hosts_validator.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/anonymous_authentication_provider.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/anonymous_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/api_key_authentication_provider.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/api_key_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/base_request_builder.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/base_request_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/base_request_configuration.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/base_request_configuration.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/method.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/method.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/native_response_handler.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/native_response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_adapter.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/request_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from io import BytesIO
-from typing import Callable, Dict, List, Optional, TypeVar
+from typing import Dict, Generic, List, Optional, TypeVar
 
 from .request_information import RequestInformation
 from .serialization import Parsable, ParsableFactory, SerializationWriterFactory
 from .store import BackingStoreFactory
 
 ResponseType = TypeVar("ResponseType", str, int, float, bool, datetime, BytesIO)
 ModelType = TypeVar("ModelType", bound=Parsable)
+RequestType = TypeVar("RequestType")
 
 
-class RequestAdapter(ABC):
+class RequestAdapter(ABC, Generic[ResponseType, ModelType, RequestType]):
     """Service responsible for translating abstract Request Info into concrete native HTTP requests.
     """
     # The base url for every request.
     base_url = str
 
     @abstractmethod
     def get_serialization_writer_factory(self) -> SerializationWriterFactory:
@@ -25,44 +26,46 @@
             SerializationWriterFactory: the serialization writer factory currently in use for the
             HTTP core service.
         """
         pass
 
     @abstractmethod
     async def send_async(
-        self, request_info: RequestInformation, type: ParsableFactory,
+        self, request_info: RequestInformation, parsable_factory: ParsableFactory,
         error_map: Dict[str, Optional[ParsableFactory]]
     ) -> Optional[ModelType]:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized response model.
 
         Args:
             request_info (RequestInformation): the request info to execute.
-            type (ParsableFactory): the class of response model to deserialize the response into.
+            parsable_factory (ParsableFactory): the class of response model to
+                deserialize the response into.
             error_map (Dict[str, Optional[ParsableFactory]]): the error dict to use in case
             of a failed request.
 
         Returns:
             ModelType: the deserialized response model.
         """
         pass
 
     @abstractmethod
     async def send_collection_async(
         self,
         request_info: RequestInformation,
-        type: ParsableFactory,
+        parsable_factory: ParsableFactory,
         error_map: Dict[str, Optional[ParsableFactory]],
     ) -> Optional[List[ModelType]]:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized response model collection.
 
         Args:
             request_info (RequestInformation): the request info to execute.
-            type (ParsableFactory): the class of response model to deserialize the response into.
+            parsable_factory (ParsableFactory): the class of response model to
+                deserialize the response into.
             error_map (Dict[str, Optional[ParsableFactory]]): the error dict to use in
             case of a failed request.
 
         Returns:
             ModelType: the deserialized response model collection.
         """
         pass
@@ -127,7 +130,19 @@
     def enable_backing_store(self, backing_store_factory: Optional[BackingStoreFactory]) -> None:
         """Enables the backing store proxies for the SerializationWriters and ParseNodes in use.
 
         Args:
             backing_store_factory (Optional[BackingStoreFactory]): the backing store factory to use.
         """
         pass
+
+    @abstractmethod
+    async def convert_to_native_async(self, request_info: RequestInformation) -> RequestType:
+        """Translates the request information object into a native HTTP client request object.
+
+        Args:
+            request_info (RequestInformation): request information object to be converted.
+
+        Returns:
+            RequestType: the natively typed HTTP request of the client.
+        """
+        pass
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_information.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/request_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,17 +154,17 @@
             writer from.
             content_type (Optional[str]): the content type.
             values (Union[T, List[T]]): the models.
         """
         writer = self._get_serialization_writer(request_adapter, content_type, values)
 
         if isinstance(values, list):
-            writer.writer = writer.write_collection_of_object_values(None, values)
+            writer.write_collection_of_object_values(None, values)
         else:
-            writer.writer = writer.write_object_value(None, values)
+            writer.write_object_value(None, values)
 
         self._set_content_and_content_type_header(writer, content_type)
 
     def set_content_from_scalar(
         self, request_adapter: Optional['RequestAdapter'], content_type: Optional[str],
         values: Union[T, List[T]]
     ) -> None:
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/response_handler.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/__init__.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parsable.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parsable.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parsable_factory.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parsable_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,44 +170,48 @@
         """Get a bytearray value from the nodes
 
         Returns:
             bytearray: The bytearray value from the nodes
         """
         pass
 
+    @property
     @abstractmethod
-    def get_on_before_assign_field_values(self) -> Callable[[Parsable], None]:
+    def on_before_assign_field_values(self) -> Callable[[Parsable], None]:
         """Gets the callback called before the node is deserialized.
 
         Returns:
             Callable[[Parsable], None]: the callback called before the node is deserialized.
         """
         pass
 
+    @on_before_assign_field_values.setter
     @abstractmethod
-    def get_on_after_assign_field_values(self) -> Optional[Callable[[Parsable], None]]:
-        """Gets the callback called before the node is deserialized.
+    def on_before_assign_field_values(self, value: Callable[[Parsable], None]) -> None:
+        """Sets the callback called before the node is deserialized.
 
-        Returns:
-            Callable[[Parsable], None]: the callback called before the node is deserialized.
+        Args:
+            value (Callable[[Parsable], None]): the callback called before the node is
+            deserialized.
         """
         pass
 
+    @property
     @abstractmethod
-    def set_on_before_assign_field_values(self, value: Callable[[Parsable], None]) -> None:
-        """Sets the callback called before the node is deserialized.
+    def on_after_assign_field_values(self) -> Optional[Callable[[Parsable], None]]:
+        """Gets the callback called after the node is deserialized.
 
-        Args:
-            value (Callable[[Parsable], None]): the callback called before the node is
-            deserialized.
+        Returns:
+            Callable[[Parsable], None]: the callback called before the node is deserialized.
         """
         pass
 
+    @on_after_assign_field_values.setter
     @abstractmethod
-    def set_on_after_assign_field_values(self, value: Callable[[Parsable], None]) -> None:
+    def on_after_assign_field_values(self, value: Callable[[Parsable], None]) -> None:
         """Sets the callback called after the node is deserialized.
 
         Args:
             value (Callable[[Parsable], None]): the callback called after the node is
             deserialized.
         """
         pass
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_factory.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_factory_registry.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_helper.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node_helper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_proxy_factory.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/parse_node_proxy_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# ------------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation.  All Rights Reserved.
+# Licensed under the MIT License.
+# See License in the project root for license information.
+# ------------------------------------------------------------------------------
+
 from io import BytesIO
 from typing import Callable
 
 from .parsable import Parsable
 from .parse_node import ParseNode
 from .parse_node_factory import ParseNodeFactory
 
@@ -16,19 +22,21 @@
     ) -> None:
         """Creates a new proxy factory that wraps the specified concrete factory while composing
         the before and after callbacks.
 
         Args:
             concrete (ParseNodeFactory): The concrete factory to wrap.
             on_before (Callable[[Parsable], None]): The callback to invoke before the
-            deserialization
-            of any model object.
+            deserialization of any model object.
             on_after (Callable[[Parsable], None]): The callback to invoke after the deserialization
             of any model object.
         """
+        if not concrete:
+            raise ValueError("Concrete factory cannot be None")
+
         self._concrete = concrete
         self._on_before = on_before
         self._on_after = on_after
 
     def get_valid_content_type(self) -> str:
         """
         Returns:
@@ -43,27 +51,27 @@
             content_type (str): The content type of the parse node.
             content (BytesIO): The stream to read the parse node from.
 
         Returns:
             ParseNode: A parse node.
         """
         node = self._concrete.get_root_parse_node(content_type, content)
-        original_before = node.get_on_before_assign_field_values()
-        original_after = node.get_on_after_assign_field_values()
+        original_before = node.on_before_assign_field_values
+        original_after = node.on_after_assign_field_values
 
         def before_callback(value):
             if self._on_before:
                 self._on_before(value)
             if callable(original_before):
                 original_before(value)
 
-        node.set_on_before_assign_field_values(before_callback)
+        node.on_before_assign_field_values = before_callback
 
         def after_callback(value):
             if self._on_after:
                 self._on_after(value)
             if callable(original_after):
                 original_after(value)
 
-        node.set_on_after_assign_field_values(after_callback)
+        node.on_after_assign_field_values = after_callback
 
         return node
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/serialization_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,72 +202,74 @@
         """Gets the value of the serialized content.
 
         Returns:
             BytesIO: The value of the serialized content.
         """
         pass
 
+    @property
     @abstractmethod
-    def get_on_before_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
+    def on_before_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
         """Gets the callback called before the object gets serialized.
 
         Returns:
             Optional[Callable[[Parsable], None]]:the callback called before the object
             gets serialized.
         """
         pass
 
+    @on_before_object_serialization.setter
     @abstractmethod
-    def get_on_after_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
-        """Gets the callback called after the object gets serialized.
+    def on_before_object_serialization(self, value: Optional[Callable[[Parsable], None]]) -> None:
+        """Sets the callback called before the objects gets serialized.
 
-        Returns:
-            Optional[Optional[Callable[[Parsable], None]]]: the callback called after the object
+        Args:
+            value (Optional[Callable[[Parsable], None]]): the callback called before the objects
             gets serialized.
         """
         pass
 
+    @property
     @abstractmethod
-    def get_on_start_object_serialization(
-        self
-    ) -> Optional[Callable[[Parsable, SerializationWriter], None]]:
-        """Gets the callback called right after the serialization process starts.
+    def on_after_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
+        """Gets the callback called after the object gets serialized.
 
         Returns:
-            Optional[Callable[[Parsable, SerializationWriter], None]]: the callback called
-            right after the serialization process starts.
+            Optional[Optional[Callable[[Parsable], None]]]: the callback called after the object
+            gets serialized.
         """
         pass
 
+    @on_after_object_serialization.setter
     @abstractmethod
-    def set_on_before_object_serialization(
-        self, value: Optional[Callable[[Parsable], None]]
-    ) -> None:
-        """Sets the callback called before the objects gets serialized.
+    def on_after_object_serialization(self, value: Optional[Callable[[Parsable], None]]) -> None:
+        """Sets the callback called after the objects gets serialized.
 
         Args:
-            value (Optional[Callable[[Parsable], None]]): the callback called before the objects
+            value (Optional[Callable[[Parsable], None]]): the callback called after the objects
             gets serialized.
         """
         pass
 
+    @property
     @abstractmethod
-    def set_on_after_object_serialization(
-        self, value: Optional[Callable[[Parsable], None]]
-    ) -> None:
-        """Sets the callback called after the objects gets serialized.
+    def on_start_object_serialization(
+        self
+    ) -> Optional[Callable[[Parsable, SerializationWriter], None]]:
+        """Gets the callback called right after the serialization process starts.
 
-        Args:
-            value (Optional[Callable[[Parsable], None]]): the callback called after the objects
-            gets serialized.
+        Returns:
+            Optional[Callable[[Parsable, SerializationWriter], None]]: the callback called
+            right after the serialization process starts.
         """
         pass
 
+    @on_start_object_serialization.setter
     @abstractmethod
-    def set_on_start_object_serialization(
+    def on_start_object_serialization(
         self, value: Optional[Callable[[Parsable, SerializationWriter], None]]
     ) -> None:
         """Sets the callback called right after the serialization process starts.
 
         Args:
             value (Optional[Callable[[Parsable, SerializationWriter], None]]): the callback
             called right after the serialization process starts.
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_factory.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_factory_registry.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/serialization_writer_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/serialization/serialization_writer_proxy_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# ------------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation.  All Rights Reserved.
+# Licensed under the MIT License.
+# See License in the project root for license information.
+# ------------------------------------------------------------------------------
+
 from typing import Callable, Optional
 
 from .parsable import Parsable
 from .serialization_writer import SerializationWriter
 from .serialization_writer_factory import SerializationWriterFactory
 
 
@@ -22,14 +28,17 @@
             on_before (Optional[Callable[[Parsable], None]]): the callback to invoke before the
             serialization of any model object.
             on_after (Optional[Callable[[Parsable], None]]): the callback to invoke after the
             serialization of any model object.
             on_start (Optional[Callable[[Parsable, SerializationWriter], None]]): the callback to
             invoke when the serialization of a model object starts
         """
+        if not concrete:
+            raise ValueError("concrete SerializationWriterFactory cannot be None.")
+
         self._concrete = concrete
         self._on_before = on_before
         self._on_after = on_after
         self._on_start = on_start
 
     def get_valid_content_type(self) -> str:
         """
@@ -44,36 +53,36 @@
         Args:
             content_type (str): the content type to create a serialization writer for.
 
         Returns:
             SerializationWriter: A new SerializationWriter instance for the given content type.
         """
         writer = self._concrete.get_serialization_writer(content_type)
-        original_before = writer.get_on_before_object_serialization()
-        original_after = writer.get_on_after_object_serialization()
-        original_start = writer.get_on_start_object_serialization()
+        original_before = writer.on_before_object_serialization
+        original_after = writer.on_after_object_serialization
+        original_start = writer.on_start_object_serialization
 
         def before_callback(value):
             if self._on_before:
                 self._on_before(value)
             if original_before:
                 original_before(value)
 
-        writer.set_on_before_object_serialization(before_callback)
+        writer.on_before_object_serialization = before_callback
 
         def after_callback(value):
             if self._on_after:
                 self._on_after(value)
             if original_after:
                 original_after(value)
 
-        writer.set_on_after_object_serialization(after_callback)
+        writer.on_after_object_serialization = after_callback
 
         def start_callback(value1, value2):
             if self._on_start:
                 self._on_start(value1, value2)
             if original_start:
                 original_start(value1, value2)
 
-        writer.set_on_start_object_serialization(start_callback)
+        writer.on_start_object_serialization = start_callback
 
         return writer
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/__init__.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .backed_model import BackingStore
+from .backed_model import BackedModel
 from .backing_store import BackingStore
 from .backing_store_factory import BackingStoreFactory
 from .backing_store_factory_singleton import BackingStoreFactorySingleton
 from .backing_store_parse_node_factory import BackingStoreParseNodeFactory
 from .backing_store_serialization_writer_proxy_factory import (
     BackingStoreSerializationWriterProxyFactory,
 )
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/backing_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+# ------------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation.  All Rights Reserved.
+# Licensed under the MIT License.
+# See License in the project root for license information.
+# ------------------------------------------------------------------------------
+
 from abc import ABC, abstractmethod
-from typing import Any, Callable, List, Optional, Tuple, TypeVar
+from typing import Any, Callable, Generic, List, Optional, Tuple, TypeVar
 
 T = TypeVar("T")
 
 
-class BackingStore(ABC):
+class BackingStore(ABC, Generic[T]):
     """Stores model information in a different location than the object properties.
     Implementations can provide dirty tracking capabilities, caching capabilities
-    or integration with 3rd party stores
-    """
+    or integration with 3rd party stores"""
 
     @abstractmethod
     def get(self, key: str) -> Optional[T]:
         """Gets a value from the backing store based on its key. Returns null if the value hasn't
         changed and "ReturnOnlyChangedValues" is true.
 
         Args:
@@ -50,15 +55,17 @@
         Returns:
             List[str]: The keys for the values that changed to null.
         """
         pass
 
     @abstractmethod
     def subscribe(
-        self, callback: Callable[[str, Any, Any], None], subscription_id: Optional[str]
+        self,
+        callback: Callable[[str, Any, Any], None],
+        subscription_id: Optional[str] = None
     ) -> str:
         """Creates a subscription to any data change happening.
 
         Args:
             callback (Callable[[str, Any, Any], None]):Callback to be invoked on data changes
             where the first parameter is the data key, the second the previous value and the third
             the new value.
@@ -76,47 +83,54 @@
         Args:
             subscription_id (str): The Id of the subscription to remove.
         """
         pass
 
     @abstractmethod
     def clear(self) -> None:
-        """Clears the data stored in the backing store. Doesn't trigger any subscription.
-        """
+        """Clears the data stored in the backing store. Doesn't trigger any subscription."""
         pass
 
+    @property
     @abstractmethod
-    def get_is_initialization_completed(self) -> bool:
+    def is_initialization_completed(self) -> bool:
         """Whether the initialization of the object and/or the initial deserialization has been
         completed to track whether objects have changed.
 
         Returns:
             bool:
         """
         pass
 
+    @is_initialization_completed.setter
     @abstractmethod
-    def set_is_initialization_completed(self, bool) -> None:
-        """Sets whether the initialization of the object and/or the initial deserialization has been
-        completed to track whether objects have changed.
+    def is_initialization_completed(self, completed: bool) -> None:
+        """Sets the initialization completed state of the object.
+
+        Args:
+            completed (bool): Whether the initialization of the object and/or the initial
+            deserialization has been completed to track whether objects have changed.
         """
         pass
 
+    @property
     @abstractmethod
-    def get_return_only_changed_values(self) -> bool:
+    def return_only_changed_values(self) -> bool:
         """Whether to return only values that have changed since the initialization of the object
         when calling the Get and Enumerate methods.
 
         Returns:
             bool:
         """
         pass
 
+    @return_only_changed_values.setter
     @abstractmethod
-    def set_return_only_changed_values(self, bool) -> None:
+    def return_only_changed_values(self, changed: bool) -> None:
         """Sets whether to return only values that have changed since the initialization of the
         object when calling the Get and Enumerate methods.
 
-        Returns:
-            bool:
+        Args:
+            changed (bool): Whether to return only values that have changed since the
+            initialization of the object when calling the Get and Enumerate methods.
         """
         pass
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# ------------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation.  All Rights Reserved.
+# Licensed under the MIT License.
+# See License in the project root for license information.
+# ------------------------------------------------------------------------------
+
 from ..serialization import SerializationWriterFactory, SerializationWriterProxyFactory
 from .backed_model import BackedModel
 
 
 class BackingStoreSerializationWriterProxyFactory(SerializationWriterProxyFactory):
     """Proxy implementation of SerializationWriterFactory for the backing store that
     automatically sets the state of the backing store when serializing.
@@ -12,32 +18,32 @@
         given a concrete implementation of SerializationWriterFactory.
 
         Args:
             concrete (SerializationWriterFactory):  a concrete implementation of
             SerializationWriterFactory to wrap.
         """
 
-        def func1(x):
+        def on_before(x):
             if isinstance(x, BackedModel):
                 backed_model = x
-                backing_store = backed_model.get_backing_store()
+                backing_store = backed_model.backing_store
                 if backing_store:
-                    backing_store.set_return_only_changed_values(True)
+                    backing_store.return_only_changed_values = True
 
-        def func2(x):
+        def on_after(x):
             if isinstance(x, BackedModel):
                 backed_model = x
-                backing_store = backed_model.get_backing_store()
+                backing_store = backed_model.backing_store
                 if backing_store:
-                    backing_store.set_return_only_changed_values(False)
-                    backing_store.set_is_initialization_completed(True)
+                    backing_store.return_only_changed_values = False
+                    backing_store.is_initialization_completed = True
 
-        def func3(x, y):
+        def on_start(x, y):
             if isinstance(x, BackedModel):
                 backed_model = x
-                backing_store = backed_model.get_backing_store()
+                backing_store = backed_model.backing_store
                 if backing_store:
                     keys = backing_store.enumerate_keys_for_values_changed_to_null()
                     for key in keys:
                         y.write_null_value(key)
 
-        super().__init__(concrete, func1, func2, func3)
+        super().__init__(concrete, on_before, on_after, on_start)
```

### Comparing `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/utils.py` & `microsoft_kiota_abstractions-0.7.0/kiota_abstractions/utils.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/pyproject.toml` & `microsoft_kiota_abstractions-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/requirements-dev.txt` & `microsoft_kiota_abstractions-0.7.0/requirements-dev.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 -i https://pypi.org/simple
 
-astroid==2.15.5 ; python_full_version >= '3.7.2'
+astroid==2.15.6 ; python_full_version >= '3.7.2'
 
-certifi==2023.5.7 ; python_version >= '3.6'
+certifi==2023.7.22 ; python_version >= '3.6'
 
-charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'
+charset-normalizer==3.2.0 ; python_full_version >= '3.7.0'
 
 colorama==0.4.6 ; sys_platform == 'win32'
 
 dill==0.3.6 ; python_version < '3.11'
 
 docutils==0.20.1 ; python_version >= '3.7'
 
@@ -28,37 +28,37 @@
 
 mypy==1.4.1
 
 mypy-extensions==1.0.0 ; python_version >= '3.5'
 
 packaging==23.1 ; python_version >= '3.7'
 
-platformdirs==3.8.0 ; python_version >= '3.7'
+platformdirs==3.10.0 ; python_version >= '3.7'
 
 pluggy==1.2.0 ; python_version >= '3.6'
 
-pylint==2.17.4
+pylint==2.17.5
 
 pytest==7.4.0
 
-pytest-asyncio==0.21.0
+pytest-asyncio==0.21.1
 
 requests==2.31.0
 
 toml==0.10.2
 
 tomli==2.0.1 ; python_version < '3.11'
 
 tomli-w==1.0.0 ; python_version >= '3.7'
 
-tomlkit==0.11.8 ; python_version >= '3.7'
+tomlkit==0.12.1 ; python_version >= '3.7'
 
-typing-extensions==4.6.3 ; python_version >= '3.7'
+typing-extensions==4.7.1 ; python_version >= '3.7'
 
-urllib3==2.0.3 ; python_version >= '3.7'
+urllib3==2.0.4 ; python_version >= '3.7'
 
 wrapt==1.15.0 ; python_version < '3.11'
 
 yapf==0.40.1
 
 uritemplate==4.1.1
```

### Comparing `microsoft_kiota_abstractions-0.6.0/tests/authentication/test_api_key_authentication_provider.py` & `microsoft_kiota_abstractions-0.7.0/tests/authentication/test_api_key_authentication_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 from kiota_abstractions.authentication import (
     ApiKeyAuthenticationProvider,
     KeyLocation,
     AuthenticationProvider,
 )
 
-from kiota_abstractions.request_information import RequestInformation
-
 allowed_hosts = ["https://example.com"]
 
 
 def test_initialization():
     provider = ApiKeyAuthenticationProvider(
         KeyLocation.Header, "test_key_string", "api_key", allowed_hosts
     )
```

### Comparing `microsoft_kiota_abstractions-0.6.0/tests/authentication/test_base_bearer_token_authentication.py` & `microsoft_kiota_abstractions-0.7.0/tests/authentication/test_base_bearer_token_authentication.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/tests/test_request_information.py` & `microsoft_kiota_abstractions-0.7.0/tests/test_request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.6.0/PKG-INFO` & `microsoft_kiota_abstractions-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-abstractions
-Version: 0.6.0
+Version: 0.7.0
 Summary: Core abstractions for kiota generated libraries in Python
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

