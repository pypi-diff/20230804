# Comparing `tmp/thipster-0.23.5.tar.gz` & `tmp/thipster-0.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.23.5.tar", last modified: Wed Aug  2 07:13:30 2023, max compression
+gzip compressed data, was "thipster-0.23.6.tar", last modified: Fri Aug  4 12:28:43 2023, max compression
```

## Comparing `thipster-0.23.5.tar` & `thipster-0.23.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.013070 thipster-0.23.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-02 07:13:08.000000 thipster-0.23.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-02 07:13:08.000000 thipster-0.23.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-02 07:13:30.013070 thipster-0.23.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-02 07:13:08.000000 thipster-0.23.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-02 07:13:08.000000 thipster-0.23.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 07:13:08.000000 thipster-0.23.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 07:13:30.013070 thipster-0.23.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-02 07:13:09.000000 thipster-0.23.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.993069 thipster-0.23.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.993069 thipster-0.23.5/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/engine/test_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.993069 thipster-0.23.5/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.997069 thipster-0.23.5/tests/parser/dsl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    18947 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/test_parsedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/test_parserfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.997069 thipster-0.23.5/tests/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/repository/test_github_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/repository/test_local_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/repository/test_resourcemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.997069 thipster-0.23.5/thipster/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.001069 thipster-0.23.5/thipster/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/auth/google.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.001069 thipster-0.23.5/thipster/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/i_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/i_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/i_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/i_terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/parsed_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.005069 thipster-0.23.5/thipster/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.005069 thipster-0.23.5/thipster/parser/dsl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24598 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/parser_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.009070 thipster-0.23.5/thipster/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.013070 thipster-0.23.5/thipster/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/terraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/terraform/cdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/terraform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.001069 thipster-0.23.5/thipster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.558070 thipster-0.23.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-04 12:28:23.000000 thipster-0.23.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-04 12:28:23.000000 thipster-0.23.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-04 12:28:43.558070 thipster-0.23.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-04 12:28:23.000000 thipster-0.23.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-04 12:28:23.000000 thipster-0.23.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-04 12:28:23.000000 thipster-0.23.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:28:43.558070 thipster-0.23.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-04 12:28:24.000000 thipster-0.23.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.546070 thipster-0.23.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.546070 thipster-0.23.6/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/engine/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.546070 thipster-0.23.6/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/tests/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/test_parsedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/test_parserfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/tests/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/repository/test_github_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/repository/test_local_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/thipster/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/thipster/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/auth/google.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.554070 thipster-0.23.6/thipster/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/i_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/i_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/i_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/i_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/parsed_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.554070 thipster-0.23.6/thipster/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.554070 thipster-0.23.6/thipster/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/parser_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.558070 thipster-0.23.6/thipster/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.558070 thipster-0.23.6/thipster/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/terraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/terraform/cdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/terraform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/thipster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.23.5/LICENSE` & `thipster-0.23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/PKG-INFO` & `thipster-0.23.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.5
+Version: 0.23.6
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: google
+Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: google
 Provides-Extra: dev
-Provides-Extra: test
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.5 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.6 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: google Provides-Extra:
-doc Provides-Extra: dev Provides-Extra: test License-File: LICENSE # THipster
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+doc Provides-Extra: google Provides-Extra: dev License-File: LICENSE # THipster
 THipster is a tool dedicated to simplifying the difficulty associated with
 writing Terraform files. It allows users to write infrastructure as code in a
 simplified format, using either YAML (with JINJA) or the dedicated Thipster
 DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
 create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
                                versions] [Ruff]
```

### Comparing `thipster-0.23.5/README.md` & `thipster-0.23.6/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/pyproject.toml` & `thipster-0.23.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/setup.py` & `thipster-0.23.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.23.5'
+__version__ = '0.23.6'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.23.5/tests/engine/test_engine.py` & `thipster-0.23.6/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/engine/test_generation.py` & `thipster-0.23.6/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/parser/dsl_parser/test_ast.py` & `thipster-0.23.6/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.23.6/tests/parser/dsl_parser/test_dslparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,22 +687,23 @@
 \tregion euw
             """
     __test_syntax_error(
         mocker, input_file=input_file, ln=3, col=9,
         expected=TT.COLON, got=TT.STRING,
     )
 
-    # MISSING TAB
+    # MISSING TAB :
+    # MEANS THAT NEXT LINE SHOULD BE CONSIDERED AS RESOURCE : ERROR ON COLON
     input_file = """
 bucket my-bucket:
 region: euw
             """
     __test_syntax_error(
-        mocker, input_file=input_file, ln=3, col=1,
-        expected=TT.TAB, got=TT.STRING,
+        mocker, input_file=input_file, ln=3, col=7,
+        expected=[TT.STRING, TT.VAR], got=TT.COLON,
     )
 
     # MISSING VALUE
     input_file = """
 bucket my-bucket:
 \ttest:
 \tregion: euw
```

### Comparing `thipster-0.23.5/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.23.6/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/parser/dsl_parser/test_token.py` & `thipster-0.23.6/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.23.6/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/parser/test_parsedfile.py` & `thipster-0.23.6/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/parser/test_parserfactory.py` & `thipster-0.23.6/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/parser/test_yamlparser.py` & `thipster-0.23.6/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/repository/test_github_repository.py` & `thipster-0.23.6/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/repository/test_local_repository.py` & `thipster-0.23.6/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/repository/test_resourcemodel.py` & `thipster-0.23.6/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/test_e2e.py` & `thipster-0.23.6/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/tests/test_tools.py` & `thipster-0.23.6/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/auth/google.py` & `thipster-0.23.6/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/engine/engine.py` & `thipster-0.23.6/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/engine/i_parser.py` & `thipster-0.23.6/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/engine/i_repository.py` & `thipster-0.23.6/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/engine/i_terraform.py` & `thipster-0.23.6/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/engine/parsed_file.py` & `thipster-0.23.6/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/engine/resource_model.py` & `thipster-0.23.6/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/helpers.py` & `thipster-0.23.6/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/dsl_parser/ast.py` & `thipster-0.23.6/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.23.6/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.23.6/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/dsl_parser/lexer.py` & `thipster-0.23.6/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.23.6/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/dsl_parser/parser.py` & `thipster-0.23.6/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/dsl_parser/token.py` & `thipster-0.23.6/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.23.6/thipster/parser/dsl_parser/token_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,20 +31,20 @@
             self.__trim_newlines()
             while self.__get_next_type() != TT.EOF:
                 self.__trim_newlines()
 
                 match self.__get_next_type():
                     case TT.VAR:
                         file_node.variables.append(
-                            self.__variable_definition(),
+                            self.__get_assignment(),
                         )
                     case TT.STRING:
                         file_node.resources.append(self.__create_resource())
                     case TT.OUTPUT:
-                        self.__output_block(file_node)
+                        self.__get_outputs(file_node)
                     case _:
                         raise DSLSyntaxError(
                             self.__next(), [TT.VAR, TT.STRING, TT.OUTPUT],
                         )
                 self.__trim_newlines()
         except Exception as e:
             raise e
@@ -178,15 +178,15 @@
         if_ctrl = self.__get_if_ctrl()
         self.__get_whitespaces()
         nb_ctrl = self.__get_nb_ctrl()
         self.__get_whitespaces()
 
         self.__get_newline()
 
-        properties = self.__get_properties(indent+1)
+        properties = self.__get_dict(indent+1)
 
         resource = ast.ResourceNode(
             resource_type=resource_type,
             name=name,
             parameters=properties,
         )
 
@@ -196,14 +196,39 @@
 
         if nb_ctrl:
             nb_ctrl.node = resource
             resource = nb_ctrl
 
         return resource
 
+    def __get_assignment(self):
+        name = self.__next(TT.VAR)
+        self.__get_whitespaces()
+        self.__next(TT.EQ)
+        self.__get_whitespaces()
+        value = self.__get_value()
+        self.__get_whitespaces()
+
+        return ast.VariableDefinitionNode(name, value)
+
+    def __get_outputs(self, file_node: ast.FileNode):
+        output_token = self.__next(TT.OUTPUT)
+        self.__get_whitespaces()
+        self.__next(TT.COLON)
+        self.__get_whitespaces()
+        self.__get_newline()
+        output_list = self.__get_list(1)
+
+        for output in output_list.value:
+            if not isinstance(output, ast.StringExprNode):
+                raise DSLSyntaxError(output, TT.STRING)
+            file_node.outputs.append(
+                ast.OutputNode(output_token.position, output),
+            )
+
     def __get_parameter(self, indent: int) -> ast.ParameterNode:
         r"""Create an AST Parameter node.
 
         Format: name, ":", (value, [if_else_ctrl] | [if_ctrl], "\\n", (list | dict)).
         """
         try:
             name = self.__next(TT.STRING)
@@ -743,32 +768,7 @@
                             TT.MINUS,
                         ).position, TT.STRING, '-',
                     )
                     values.append(ast.StringNode(token))
             next_token_type = self.__get_next_type()
 
         return ast.StringExprNode(values)
-
-    def __variable_definition(self):
-        name = self.__next(TT.VAR)
-        self.__get_whitespaces()
-        self.__next(TT.EQ)
-        self.__get_whitespaces()
-        value = self.__get_value()
-        self.__get_whitespaces()
-
-        return ast.VariableDefinitionNode(name, value)
-
-    def __output_block(self, file_node: ast.FileNode):
-        output_token = self.__next(TT.OUTPUT)
-        self.__get_whitespaces()
-        self.__next(TT.COLON)
-        self.__get_whitespaces()
-        self.__get_newline()
-        output_list = self.__get_list(1)
-
-        for output in output_list.value:
-            if not isinstance(output, ast.StringExprNode):
-                raise DSLSyntaxError(output, TT.STRING)
-            file_node.outputs.append(
-                ast.OutputNode(output_token.position, output),
-            )
```

### Comparing `thipster-0.23.5/thipster/parser/exceptions.py` & `thipster-0.23.6/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/parser_factory.py` & `thipster-0.23.6/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/parser/yaml_parser.py` & `thipster-0.23.6/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/repository/exceptions.py` & `thipster-0.23.6/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/repository/github.py` & `thipster-0.23.6/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/repository/json.py` & `thipster-0.23.6/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/repository/local.py` & `thipster-0.23.6/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/terraform/cdk.py` & `thipster-0.23.6/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster/terraform/exceptions.py` & `thipster-0.23.6/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.5/thipster.egg-info/PKG-INFO` & `thipster-0.23.6/thipster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.5
+Version: 0.23.6
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: google
+Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: google
 Provides-Extra: dev
-Provides-Extra: test
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.5 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.6 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: google Provides-Extra:
-doc Provides-Extra: dev Provides-Extra: test License-File: LICENSE # THipster
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+doc Provides-Extra: google Provides-Extra: dev License-File: LICENSE # THipster
 THipster is a tool dedicated to simplifying the difficulty associated with
 writing Terraform files. It allows users to write infrastructure as code in a
 simplified format, using either YAML (with JINJA) or the dedicated Thipster
 DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
 create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
                                versions] [Ruff]
```

### Comparing `thipster-0.23.5/thipster.egg-info/SOURCES.txt` & `thipster-0.23.6/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

