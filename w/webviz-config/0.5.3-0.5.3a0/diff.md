# Comparing `tmp/webviz-config-0.5.3.tar.gz` & `tmp/webviz-config-0.5.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webviz-config-0.5.3.tar", last modified: Fri Aug  4 07:45:52 2023, max compression
+gzip compressed data, was "webviz-config-0.5.3a0.tar", last modified: Thu Aug  3 06:57:44 2023, max compression
```

## Comparing `webviz-config-0.5.3.tar` & `webviz-config-0.5.3a0.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.130271 webviz-config-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.094270 webviz-config-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.094270 webviz-config-0.5.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-04 07:40:43.000000 webviz-config-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 07:40:43.000000 webviz-config-0.5.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-04 07:40:43.000000 webviz-config-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-04 07:40:43.000000 webviz-config-0.5.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.094270 webviz-config-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-08-04 07:40:43.000000 webviz-config-0.5.3/.github/workflows/webviz-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-04 07:40:43.000000 webviz-config-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-04 07:40:43.000000 webviz-config-0.5.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-08-04 07:40:43.000000 webviz-config-0.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-04 07:40:43.000000 webviz-config-0.5.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    25925 2023-08-04 07:40:43.000000 webviz-config-0.5.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-08-04 07:40:43.000000 webviz-config-0.5.3/INTRODUCTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 07:40:43.000000 webviz-config-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)   326542 2023-05-27 00:10:14.000000 webviz-config-0.5.3/LICENSE.chromedriver
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-08-04 07:45:52.126270 webviz-config-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-04 07:40:43.000000 webviz-config-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-08-04 07:40:43.000000 webviz-config-0.5.3/WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.098270 webviz-config-0.5.3/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/before-after-plugin-actions.png
--rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/before-after-settings.png
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/before-after-tabs-views.png
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/high-level-overview.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    59175 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/implement-plugin.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    62309 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/implement-settings-group.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    60748 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/implement-view-element.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    59578 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/implement-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)    70182 2023-08-04 07:40:43.000000 webviz-config-0.5.3/assets/webviz-layout-overview.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 07:40:43.000000 webviz-config-0.5.3/bandit.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.098270 webviz-config-0.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/basic_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/basic_example_advanced_menu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/basic_example_wlf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/demo_portable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/example-markdown.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    10746 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/example.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   553912 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/example_banner.png
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/example_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/example_javascript.js
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 07:40:43.000000 webviz-config-0.5.3/examples/example_stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-04 07:40:43.000000 webviz-config-0.5.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    39008 2023-08-04 07:40:43.000000 webviz-config-0.5.3/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-04 07:40:43.000000 webviz-config-0.5.3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 07:40:43.000000 webviz-config-0.5.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 07:45:52.130271 webviz-config-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-08-04 07:40:43.000000 webviz-config-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.102270 webviz-config-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.102270 webviz-config-0.5.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/data/basic_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/data/example_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_callback_typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_create_themed_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_data_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_docker_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_example_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_example_wlf_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_plugin_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_plugin_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_portable.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_syntax_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/test_table_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.102270 webviz-config-0.5.3/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/unit_tests/test_webviz_factory_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/unit_tests/test_webviz_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-04 07:40:43.000000 webviz-config-0.5.3/tests/unit_tests/test_webviz_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.106270 webviz-config-0.5.3/webviz_config/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_build_webviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    23853 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_config_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.110270 webviz-config-0.5.3/webviz_config/_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deployment/azure_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deployment/azure_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deployment/github_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deployment/interactive_terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deployment/radix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deployment/radix_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deployment/radix_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_deprecation_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.110270 webviz-config-0.5.3/webviz_config/_dockerize/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_dockerize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_dockerize/_create_docker_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_dockerize/_pip_git_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.110270 webviz-config-0.5.3/webviz_config/_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_docs/_build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_docs/_create_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_docs/open_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.114270 webviz-config-0.5.3/webviz_config/_docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/INTRODUCTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_docs/static/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/docsify-copy-code.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   251818 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/docsify-katex.js
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/docsify-tabs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   106239 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/docsify.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.118270 webviz-config-0.5.3/webviz_config/_docs/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29932 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22076 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32312 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-08-04 07:40:47.000000 webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_docs/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    22476 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/katex.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/prism-bash.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/prism-python.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/prism-yaml.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/search.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-08-04 07:40:46.000000 webviz-config-0.5.3/webviz_config/_docs/static/vue.css
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_docs/static/webviz-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_docs/static/webviz-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_is_reload_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_localhost_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_plugin_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_shared_settings_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_theme_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_user_data_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_user_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_webviz_settings_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/_write_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/common_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/deprecation_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.118270 webviz-config-0.5.3/webviz_config/generic_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_banner_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_data_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_embed_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_data_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_portable.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_tour.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.118270 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.118270 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/_shared_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.122270 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/_text_view_element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.122270 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.122270 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.122270 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_syntax_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20735 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/generic_plugins/_table_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.122270 webviz-config-0.5.3/webviz_config/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/plugins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.122270 webviz-config-0.5.3/webviz_config/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/static/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.122270 webviz-config-0.5.3/webviz_config/static/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/static/assets/webviz_config.css
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/static/assets/webviz_layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.126270 webviz-config-0.5.3/webviz_config/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2649 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/Dockerfile.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/README.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/argument_deprecations.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/copy_data_template.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/feedback.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/plugin_deprecations.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/plugin_docs.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/radixconfig.yaml.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/sidebar.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/webviz-doc.js.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/templates/webviz_template.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.126270 webviz-config-0.5.3/webviz_config/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/testing/_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/testing/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/testing/_webviz_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.126270 webviz-config-0.5.3/webviz_config/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/themes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/themes/_default_theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.126270 webviz-config-0.5.3/webviz_config/themes/default_assets/
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/themes/default_assets/default_theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.126270 webviz-config-0.5.3/webviz_config/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/_available_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/_callback_typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/_dash_component_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/_deprecate_webviz_settings_attribute_in_dash_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/_localhost_open_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/_silence_flask_startup.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/_str_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/utils/terminal_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_factory_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_instance_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.126270 webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/_layout_base_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/_layout_unique_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/_settings_group_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-08-04 07:40:43.000000 webviz-config-0.5.3/webviz_config/webviz_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:45:52.106270 webviz-config-0.5.3/webviz_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-08-04 07:45:51.000000 webviz-config-0.5.3/webviz_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-08-04 07:45:52.000000 webviz-config-0.5.3/webviz_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 07:45:51.000000 webviz-config-0.5.3/webviz_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-04 07:45:51.000000 webviz-config-0.5.3/webviz_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 07:41:05.000000 webviz-config-0.5.3/webviz_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-04 07:45:51.000000 webviz-config-0.5.3/webviz_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 07:45:51.000000 webviz-config-0.5.3/webviz_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.784086 webviz-config-0.5.3a0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.756086 webviz-config-0.5.3a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.756086 webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.756086 webviz-config-0.5.3a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/workflows/webviz-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25925 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/INTRODUCTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)   326542 2023-05-27 00:10:14.000000 webviz-config-0.5.3a0/LICENSE.chromedriver
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-08-03 06:57:44.784086 webviz-config-0.5.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.756086 webviz-config-0.5.3a0/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/before-after-plugin-actions.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/before-after-settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/before-after-tabs-views.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/high-level-overview.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59175 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/implement-plugin.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62309 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/implement-settings-group.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60748 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/implement-view-element.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59578 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/implement-view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    70182 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/webviz-layout-overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/bandit.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.760086 webviz-config-0.5.3a0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/basic_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/basic_example_advanced_menu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/basic_example_wlf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/demo_portable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example-markdown.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10746 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   553912 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example_banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example_javascript.js
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example_stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    39008 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:57:44.784086 webviz-config-0.5.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.760086 webviz-config-0.5.3a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.760086 webviz-config-0.5.3a0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/data/basic_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/data/example_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_callback_typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_create_themed_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_data_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_docker_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_example_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_example_wlf_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_plugin_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_plugin_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_portable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_syntax_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_table_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.760086 webviz-config-0.5.3a0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/unit_tests/test_webviz_factory_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/unit_tests/test_webviz_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/unit_tests/test_webviz_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.764086 webviz-config-0.5.3a0/webviz_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_build_webviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23853 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_config_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.768086 webviz-config-0.5.3a0/webviz_config/_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/azure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/azure_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/github_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/interactive_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/radix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/radix_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/radix_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deprecation_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.768086 webviz-config-0.5.3a0/webviz_config/_dockerize/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_dockerize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_dockerize/_create_docker_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_dockerize/_pip_git_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.768086 webviz-config-0.5.3a0/webviz_config/_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/_build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/_create_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/open_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.772086 webviz-config-0.5.3a0/webviz_config/_docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/INTRODUCTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-copy-code.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   251818 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-katex.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-tabs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106239 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/docsify.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.772086 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29932 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22076 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32312 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Typewriter-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22476 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/katex.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/prism-bash.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/prism-python.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/prism-yaml.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/search.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/vue.css
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/webviz-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/webviz-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_is_reload_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_localhost_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_plugin_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_shared_settings_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_theme_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_user_data_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_webviz_settings_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_write_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/common_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/deprecation_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_banner_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_data_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_embed_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_data_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_portable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_tour.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/_shared_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/_text_view_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_syntax_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20735 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_table_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/plugins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/assets/webviz_config.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/assets/webviz_layout.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2649 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/Dockerfile.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/README.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/argument_deprecations.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/copy_data_template.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/feedback.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/plugin_deprecations.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/plugin_docs.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/radixconfig.yaml.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/sidebar.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/webviz-doc.js.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/webviz_template.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/testing/_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/testing/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/testing/_webviz_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/themes/_default_theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/themes/default_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/themes/default_assets/default_theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_available_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_callback_typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_dash_component_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_deprecate_webviz_settings_attribute_in_dash_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_localhost_open_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_silence_flask_startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_str_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/terminal_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_factory_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_instance_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.784086 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_layout_base_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_layout_unique_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_settings_group_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.764086 webviz-config-0.5.3a0/webviz_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:53:03.000000 webviz-config-0.5.3a0/webviz_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/top_level.txt
```

### Comparing `webviz-config-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md` & `webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md` & `webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/.github/workflows/webviz-config.yml` & `webviz-config-0.5.3a0/.github/workflows/webviz-config.yml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/CHANGELOG.md` & `webviz-config-0.5.3a0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/CODE_OF_CONDUCT.md` & `webviz-config-0.5.3a0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/CONTRIBUTING.md` & `webviz-config-0.5.3a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/INTRODUCTION.md` & `webviz-config-0.5.3a0/INTRODUCTION.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/LICENSE` & `webviz-config-0.5.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/LICENSE.chromedriver` & `webviz-config-0.5.3a0/LICENSE.chromedriver`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/PKG-INFO` & `webviz-config-0.5.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviz-config
-Version: 0.5.3
+Version: 0.5.3a0
 Summary: Configuration file support for webviz
 Home-page: https://github.com/equinor/webviz-config
 Author: R&T Equinor
 Project-URL: Documentation, https://equinor.github.io/webviz-config
 Project-URL: Download, https://pypi.org/project/webviz-config
 Project-URL: Source, https://github.com/equinor/webviz-config
 Project-URL: Tracker, https://github.com/equinor/webviz-config/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_nn7c8p3m_/tmpzmdka3af_TarContainer/0/17", line 35, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_nn7c8p3m_/tmpzmdka3af_TarContainer/0/17", line 35, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: webviz-config Version: 0.5.3 Summary: Configuration
-file support for webviz Home-page: https://github.com/equinor/webviz-config
-Author: R&T Equinor Project-URL: Documentation, https://equinor.github.io/
-webviz-config Project-URL: Download, https://pypi.org/project/webviz-config
-Project-URL: Source, https://github.com/equinor/webviz-config Project-URL:
-Tracker, https://github.com/equinor/webviz-config/issues Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: OS
-Independent Classifier: Natural Language :: English Classifier: Environment ::
-Web Environment Classifier: Framework :: Dash Classifier: Framework :: Flask
+Metadata-Version: 2.1 Name: webviz-config Version: 0.5.3a0 Summary:
+Configuration file support for webviz Home-page: https://github.com/equinor/
+webviz-config Author: R&T Equinor Project-URL: Documentation, https://
+equinor.github.io/webviz-config Project-URL: Download, https://pypi.org/
+project/webviz-config Project-URL: Source, https://github.com/equinor/webviz-
+config Project-URL: Tracker, https://github.com/equinor/webviz-config/issues
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+OS Independent Classifier: Natural Language :: English Classifier: Environment
+:: Web Environment Classifier: Framework :: Dash Classifier: Framework :: Flask
 Classifier: Topic :: Multimedia :: Graphics Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License Requires-Python: ~=3.8
 Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
 deployment License-File: LICENSE License-File: LICENSE.chromedriver
 This package will be deprecated - we move instead all collaboration focus to
 the reusable React and Dash components in:
```

### Comparing `webviz-config-0.5.3/README.md` & `webviz-config-0.5.3a0/README.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md` & `webviz-config-0.5.3a0/WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/before-after-plugin-actions.png` & `webviz-config-0.5.3a0/assets/before-after-plugin-actions.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/before-after-settings.png` & `webviz-config-0.5.3a0/assets/before-after-settings.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/before-after-tabs-views.png` & `webviz-config-0.5.3a0/assets/before-after-tabs-views.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/high-level-overview.png` & `webviz-config-0.5.3a0/assets/high-level-overview.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/implement-plugin.svg` & `webviz-config-0.5.3a0/assets/implement-plugin.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/implement-settings-group.svg` & `webviz-config-0.5.3a0/assets/implement-settings-group.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/implement-view-element.svg` & `webviz-config-0.5.3a0/assets/implement-view-element.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/implement-view.svg` & `webviz-config-0.5.3a0/assets/implement-view.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/assets/webviz-layout-overview.png` & `webviz-config-0.5.3a0/assets/webviz-layout-overview.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/examples/basic_example.yaml` & `webviz-config-0.5.3a0/examples/basic_example.yaml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/examples/basic_example_advanced_menu.yaml` & `webviz-config-0.5.3a0/examples/basic_example_advanced_menu.yaml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/examples/basic_example_wlf.yaml` & `webviz-config-0.5.3a0/examples/basic_example_wlf.yaml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/examples/example-markdown.md` & `webviz-config-0.5.3a0/examples/example-markdown.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/examples/example.pdf` & `webviz-config-0.5.3a0/examples/example.pdf`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/examples/example_banner.png` & `webviz-config-0.5.3a0/examples/example_banner.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/mypy.ini` & `webviz-config-0.5.3a0/mypy.ini`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/package-lock.json` & `webviz-config-0.5.3a0/package-lock.json`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/package.json` & `webviz-config-0.5.3a0/package.json`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/setup.py` & `webviz-config-0.5.3a0/setup.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/data/basic_example.yaml` & `webviz-config-0.5.3a0/tests/data/basic_example.yaml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_callback_typecheck.py` & `webviz-config-0.5.3a0/tests/test_callback_typecheck.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_create_themed_layout.py` & `webviz-config-0.5.3a0/tests/test_create_themed_layout.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_data_table.py` & `webviz-config-0.5.3a0/tests/test_data_table.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_docker_setup.py` & `webviz-config-0.5.3a0/tests/test_docker_setup.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_docstring.py` & `webviz-config-0.5.3a0/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_example_plugin.py` & `webviz-config-0.5.3a0/tests/test_example_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_example_wlf_plugin.py` & `webviz-config-0.5.3a0/tests/test_example_wlf_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_plugin_init.py` & `webviz-config-0.5.3a0/tests/test_plugin_init.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_plugin_metadata.py` & `webviz-config-0.5.3a0/tests/test_plugin_metadata.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_portable.py` & `webviz-config-0.5.3a0/tests/test_portable.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_schema.py` & `webviz-config-0.5.3a0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_syntax_highlighter.py` & `webviz-config-0.5.3a0/tests/test_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/test_table_plotter.py` & `webviz-config-0.5.3a0/tests/test_table_plotter.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/unit_tests/test_webviz_factory_registry.py` & `webviz-config-0.5.3a0/tests/unit_tests/test_webviz_factory_registry.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/unit_tests/test_webviz_instance_info.py` & `webviz-config-0.5.3a0/tests/unit_tests/test_webviz_instance_info.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/tests/unit_tests/test_webviz_settings.py` & `webviz-config-0.5.3a0/tests/unit_tests/test_webviz_settings.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/__init__.py` & `webviz-config-0.5.3a0/webviz_config/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_build_webviz.py` & `webviz-config-0.5.3a0/webviz_config/_build_webviz.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_config_parser.py` & `webviz-config-0.5.3a0/webviz_config/_config_parser.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_deployment/azure_cli.py` & `webviz-config-0.5.3a0/webviz_config/_deployment/azure_cli.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_deployment/azure_configuration.py` & `webviz-config-0.5.3a0/webviz_config/_deployment/azure_configuration.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_deployment/github_cli.py` & `webviz-config-0.5.3a0/webviz_config/_deployment/github_cli.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_deployment/interactive_terminal.py` & `webviz-config-0.5.3a0/webviz_config/_deployment/interactive_terminal.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_deployment/radix.py` & `webviz-config-0.5.3a0/webviz_config/_deployment/radix.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_deployment/radix_cli.py` & `webviz-config-0.5.3a0/webviz_config/_deployment/radix_cli.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_deployment/radix_configuration.py` & `webviz-config-0.5.3a0/webviz_config/_deployment/radix_configuration.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_deprecation_store.py` & `webviz-config-0.5.3a0/webviz_config/_deprecation_store.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_dockerize/_create_docker_setup.py` & `webviz-config-0.5.3a0/webviz_config/_dockerize/_create_docker_setup.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_dockerize/_pip_git_url.py` & `webviz-config-0.5.3a0/webviz_config/_dockerize/_pip_git_url.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/_build_docs.py` & `webviz-config-0.5.3a0/webviz_config/_docs/_build_docs.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/_create_schema.py` & `webviz-config-0.5.3a0/webviz_config/_docs/_create_schema.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/open_docs.py` & `webviz-config-0.5.3a0/webviz_config/_docs/open_docs.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/INTRODUCTION.md` & `webviz-config-0.5.3a0/webviz_config/_docs/static/INTRODUCTION.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/README.md` & `webviz-config-0.5.3a0/webviz_config/_docs/static/README.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/docsify-copy-code.min.js` & `webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-copy-code.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/docsify-katex.js` & `webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-katex.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/docsify-tabs.min.js` & `webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-tabs.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/docsify.min.js` & `webviz-config-0.5.3a0/webviz_config/_docs/static/docsify.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_AMS-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Bold.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Bold.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Main-Bold.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Main-BoldItalic.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Main-Italic.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Main-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Math-BoldItalic.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Math-Italic.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Bold.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Italic.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Script-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Size1-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Size2-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Size3-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Size4-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/fonts/KaTeX_Typewriter-Regular.woff2` & `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/index.html` & `webviz-config-0.5.3a0/webviz_config/_docs/static/index.html`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/katex.min.css` & `webviz-config-0.5.3a0/webviz_config/_docs/static/katex.min.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/prism-bash.min.js` & `webviz-config-0.5.3a0/webviz_config/_docs/static/prism-bash.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/prism-python.min.js` & `webviz-config-0.5.3a0/webviz_config/_docs/static/prism-python.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/prism-yaml.min.js` & `webviz-config-0.5.3a0/webviz_config/_docs/static/prism-yaml.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/search.min.js` & `webviz-config-0.5.3a0/webviz_config/_docs/static/search.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/vue.css` & `webviz-config-0.5.3a0/webviz_config/_docs/static/vue.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_docs/static/webviz-logo.svg` & `webviz-config-0.5.3a0/webviz_config/_docs/static/webviz-logo.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_localhost_token.py` & `webviz-config-0.5.3a0/webviz_config/_localhost_token.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_oauth2.py` & `webviz-config-0.5.3a0/webviz_config/_oauth2.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_plugin_abc.py` & `webviz-config-0.5.3a0/webviz_config/_plugin_abc.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_shared_settings_subscriptions.py` & `webviz-config-0.5.3a0/webviz_config/_shared_settings_subscriptions.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_theme_class.py` & `webviz-config-0.5.3a0/webviz_config/_theme_class.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_user_preferences.py` & `webviz-config-0.5.3a0/webviz_config/_user_preferences.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_webviz_settings_class.py` & `webviz-config-0.5.3a0/webviz_config/_webviz_settings_class.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/_write_script.py` & `webviz-config-0.5.3a0/webviz_config/_write_script.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/command_line.py` & `webviz-config-0.5.3a0/webviz_config/command_line.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/common_cache.py` & `webviz-config-0.5.3a0/webviz_config/common_cache.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/deprecation_decorators.py` & `webviz-config-0.5.3a0/webviz_config/deprecation_decorators.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_banner_image.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_banner_image.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_data_table.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_data_table.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_embed_pdf.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_embed_pdf.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_assets.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_assets.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_data_download.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_data_download.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_plugin.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_portable.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_portable.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_tour.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_tour.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_plugin.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/_shared_settings.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/_shared_settings.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/_text_view_element.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/_text_view_element.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/_view.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/_view.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/_view.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/_view.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_markdown.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_markdown.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_pivot_table.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_pivot_table.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_syntax_highlighter.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/generic_plugins/_table_plotter.py` & `webviz-config-0.5.3a0/webviz_config/generic_plugins/_table_plotter.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/plugins/__init__.py` & `webviz-config-0.5.3a0/webviz_config/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/plugins/_utils.py` & `webviz-config-0.5.3a0/webviz_config/plugins/_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/static/README.md` & `webviz-config-0.5.3a0/webviz_config/static/README.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/static/assets/webviz_config.css` & `webviz-config-0.5.3a0/webviz_config/static/assets/webviz_config.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/static/assets/webviz_layout.css` & `webviz-config-0.5.3a0/webviz_config/static/assets/webviz_layout.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/templates/Dockerfile.jinja2` & `webviz-config-0.5.3a0/webviz_config/templates/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/templates/copy_data_template.py.jinja2` & `webviz-config-0.5.3a0/webviz_config/templates/copy_data_template.py.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/templates/feedback.md.jinja2` & `webviz-config-0.5.3a0/webviz_config/templates/feedback.md.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/templates/plugin_docs.md.jinja2` & `webviz-config-0.5.3a0/webviz_config/templates/plugin_docs.md.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/templates/radixconfig.yaml.jinja2` & `webviz-config-0.5.3a0/webviz_config/templates/radixconfig.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/templates/webviz-doc.js.jinja2` & `webviz-config-0.5.3a0/webviz_config/templates/webviz-doc.js.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/templates/webviz_template.py.jinja2` & `webviz-config-0.5.3a0/webviz_config/templates/webviz_template.py.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/testing/_composite.py` & `webviz-config-0.5.3a0/webviz_config/testing/_composite.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/testing/_plugin.py` & `webviz-config-0.5.3a0/webviz_config/testing/_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/themes/default_assets/default_theme.css` & `webviz-config-0.5.3a0/webviz_config/themes/default_assets/default_theme.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/utils/_available_port.py` & `webviz-config-0.5.3a0/webviz_config/utils/_available_port.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/utils/_callback_typecheck.py` & `webviz-config-0.5.3a0/webviz_config/utils/_callback_typecheck.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/utils/_dash_component_utils.py` & `webviz-config-0.5.3a0/webviz_config/utils/_dash_component_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/utils/_deprecate_webviz_settings_attribute_in_dash_app.py` & `webviz-config-0.5.3a0/webviz_config/utils/_deprecate_webviz_settings_attribute_in_dash_app.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/utils/_localhost_open_browser.py` & `webviz-config-0.5.3a0/webviz_config/utils/_localhost_open_browser.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/utils/_silence_flask_startup.py` & `webviz-config-0.5.3a0/webviz_config/utils/_silence_flask_startup.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_assets.py` & `webviz-config-0.5.3a0/webviz_config/webviz_assets.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_factory.py` & `webviz-config-0.5.3a0/webviz_config/webviz_factory.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_factory_registry.py` & `webviz-config-0.5.3a0/webviz_config/webviz_factory_registry.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_instance_info.py` & `webviz-config-0.5.3a0/webviz_config/webviz_instance_info.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/_layout_base_abc.py` & `webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_layout_base_abc.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/_layout_unique_id.py` & `webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_layout_unique_id.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/_settings_group_abc.py` & `webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_settings_group_abc.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_plugin_subclasses/_views.py` & `webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_views.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config/webviz_store.py` & `webviz-config-0.5.3a0/webviz_config/webviz_store.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config.egg-info/PKG-INFO` & `webviz-config-0.5.3a0/webviz_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviz-config
-Version: 0.5.3
+Version: 0.5.3a0
 Summary: Configuration file support for webviz
 Home-page: https://github.com/equinor/webviz-config
 Author: R&T Equinor
 Project-URL: Documentation, https://equinor.github.io/webviz-config
 Project-URL: Download, https://pypi.org/project/webviz-config
 Project-URL: Source, https://github.com/equinor/webviz-config
 Project-URL: Tracker, https://github.com/equinor/webviz-config/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_nn7c8p3m_/tmpzmdka3af_TarContainer/0/232", line 35, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_nn7c8p3m_/tmpzmdka3af_TarContainer/0/232", line 35, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: webviz-config Version: 0.5.3 Summary: Configuration
-file support for webviz Home-page: https://github.com/equinor/webviz-config
-Author: R&T Equinor Project-URL: Documentation, https://equinor.github.io/
-webviz-config Project-URL: Download, https://pypi.org/project/webviz-config
-Project-URL: Source, https://github.com/equinor/webviz-config Project-URL:
-Tracker, https://github.com/equinor/webviz-config/issues Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: OS
-Independent Classifier: Natural Language :: English Classifier: Environment ::
-Web Environment Classifier: Framework :: Dash Classifier: Framework :: Flask
+Metadata-Version: 2.1 Name: webviz-config Version: 0.5.3a0 Summary:
+Configuration file support for webviz Home-page: https://github.com/equinor/
+webviz-config Author: R&T Equinor Project-URL: Documentation, https://
+equinor.github.io/webviz-config Project-URL: Download, https://pypi.org/
+project/webviz-config Project-URL: Source, https://github.com/equinor/webviz-
+config Project-URL: Tracker, https://github.com/equinor/webviz-config/issues
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+OS Independent Classifier: Natural Language :: English Classifier: Environment
+:: Web Environment Classifier: Framework :: Dash Classifier: Framework :: Flask
 Classifier: Topic :: Multimedia :: Graphics Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License Requires-Python: ~=3.8
 Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
 deployment License-File: LICENSE License-File: LICENSE.chromedriver
 This package will be deprecated - we move instead all collaboration focus to
 the reusable React and Dash components in:
```

### Comparing `webviz-config-0.5.3/webviz_config.egg-info/SOURCES.txt` & `webviz-config-0.5.3a0/webviz_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config.egg-info/entry_points.txt` & `webviz-config-0.5.3a0/webviz_config.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3/webviz_config.egg-info/requires.txt` & `webviz-config-0.5.3a0/webviz_config.egg-info/requires.txt`

 * *Files identical despite different names*

