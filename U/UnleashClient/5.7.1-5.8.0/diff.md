# Comparing `tmp/UnleashClient-5.7.1.tar.gz` & `tmp/UnleashClient-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unleash-client-python/unleash-client-python/dist/.tmp-oxpjksgk/UnleashClient-5.7.1.tar", last modified: Fri Jun 30 16:11:07 2023, max compression
+gzip compressed data, was "/home/runner/work/unleash-client-python/unleash-client-python/dist/.tmp-psjybg99/UnleashClient-5.8.0.tar", last modified: Fri Aug  4 09:46:15 2023, max compression
```

## Comparing `UnleashClient-5.7.1.tar` & `UnleashClient-5.8.0.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.devcontainer/post_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/add-to-project.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/release-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.lift.toml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/api/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/api/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/api/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/deprecation_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/features/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/features/Feature.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/periodic_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/periodic_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/periodic_tasks/fetch_and_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/periodic_tasks/send_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/ApplicationHostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/Default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/FlexibleRolloutStrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutRandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutSessionId.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutUserId.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/RemoteAddress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/Strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/UserWithId.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/variants/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/variants/Variants.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/variants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/basecache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/customcache.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/customstrategies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/eventcallbacks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/filecache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/strategy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/unleashclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/wsgi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/scripts/get-spec.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/integration_tests/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/integration_tests/integration_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/integration_tests/integration_unleashheroku.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/integration_tests/integration_unleashhosted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/specification_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/specification_tests/test_client_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/unit_tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/api/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/api/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/api/test_register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/unit_tests/periodic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/periodic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/periodic/test_fetch_and_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_applicationhostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_defaultstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_flexiblerollout.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_gradualrolloutrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_remoteaddress.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_userwithids.py
--rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_custom_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/utilities/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_all_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_custom_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/utilities/old_code/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/old_code/StrategyV2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/old_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/testing_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.devcontainer/post_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/workflows/add-to-project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/workflows/release-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.lift.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient/
+-rw-r--r--   0 runner    (1001) docker     (123)    21519 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/api/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/deprecation_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/features/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient/periodic_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/periodic_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/periodic_tasks/fetch_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/periodic_tasks/send_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/ApplicationHostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/Default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/FlexibleRolloutStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/GradualRolloutRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/GradualRolloutSessionId.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/GradualRolloutUserId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/RemoteAddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/Strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/UserWithId.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient/variants/
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/variants/Variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/UnleashClient/variants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/UnleashClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/basecache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/customcache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/customstrategies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/eventcallbacks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/filecache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/strategy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/unleashclient.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/docs/wsgi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/scripts/get-spec.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/integration_tests/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/integration_tests/integration_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/integration_tests/integration_unleashheroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/integration_tests/integration_unleashhosted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/specification_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/specification_tests/test_client_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/unit_tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/api/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/api/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/api/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/unit_tests/periodic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/periodic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/periodic/test_fetch_and_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_applicationhostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_defaultstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_flexiblerollout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_gradualrolloutrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_remoteaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_strategy_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/strategies/test_userwithids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/test_custom_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/unit_tests/test_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/utilities/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/mocks/mock_all_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/mocks/mock_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/mocks/mock_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/mocks/mock_custom_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/mocks/mock_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/mocks/mock_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/mocks/mock_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:46:15.000000 UnleashClient-5.8.0/tests/utilities/old_code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/old_code/StrategyV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/old_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tests/utilities/testing_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-04 09:45:03.000000 UnleashClient-5.8.0/tox.ini
```

### Comparing `UnleashClient-5.7.1/.devcontainer/Dockerfile` & `UnleashClient-5.8.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.devcontainer/devcontainer.json` & `UnleashClient-5.8.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/bug_report.md` & `UnleashClient-5.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `UnleashClient-5.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.github/PULL_REQUEST_TEMPLATE.md` & `UnleashClient-5.8.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.github/workflows/codeql-analysis.yml` & `UnleashClient-5.8.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.github/workflows/pull_request.yml` & `UnleashClient-5.8.0/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.github/workflows/release-docs.yml` & `UnleashClient-5.8.0/.github/workflows/release-docs.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.github/workflows/release-package.yml` & `UnleashClient-5.8.0/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/.gitignore` & `UnleashClient-5.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/CHANGELOG.md` & `UnleashClient-5.8.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/CODE_OF_CONDUCT.md` & `UnleashClient-5.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/CONTRIBUTING.md` & `UnleashClient-5.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/LICENSE.md` & `UnleashClient-5.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/Makefile` & `UnleashClient-5.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/PKG-INFO` & `UnleashClient-5.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnleashClient
-Version: 5.7.1
+Version: 5.8.0
 Summary: Python client for the Unleash feature toggle system!
 Author-email: Ivan Lee <ivanklee86@gmail.com>
 Project-URL: Homepage, https://github.com/Unleash/unleash-client-python
 Project-URL: Documentation, https://docs.getunleash.io/unleash-client-python
 Project-URL: Changelog, https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/Unleash/unleash-client-python
 Project-URL: Issues, https://github.com/Unleash/unleash-client-python/issues
```

### Comparing `UnleashClient-5.7.1/README.md` & `UnleashClient-5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/__init__.py` & `UnleashClient-5.8.0/UnleashClient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,16 @@
                 )
 
                 # The feature doesn't exist, so create it to track metrics
                 new_feature = Feature.metrics_only_feature(feature_name)
                 self.features[feature_name] = new_feature
 
                 # Use the feature's get_variant method to count the call
-                return new_feature.get_variant(context)
+                variant_check = new_feature.get_variant(context)
+                return variant_check
         else:
             LOGGER.log(
                 self.unleash_verbose_log_level,
                 "Returning default flag/variation for feature: %s",
                 feature_name,
             )
             LOGGER.log(
```

### Comparing `UnleashClient-5.7.1/UnleashClient/api/features.py` & `UnleashClient-5.8.0/UnleashClient/api/features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/api/metrics.py` & `UnleashClient-5.8.0/UnleashClient/api/metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/api/register.py` & `UnleashClient-5.8.0/UnleashClient/api/register.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/cache.py` & `UnleashClient-5.8.0/UnleashClient/cache.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/constants.py` & `UnleashClient-5.8.0/UnleashClient/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Library
 SDK_NAME = "unleash-client-python"
 SDK_VERSION = version("UnleashClient")
 REQUEST_TIMEOUT = 30
 REQUEST_RETRIES = 3
 METRIC_LAST_SENT_TIME = "mlst"
-CLIENT_SPEC_VERSION = "4.2.2"
+CLIENT_SPEC_VERSION = "4.3.1"
 
 # =Unleash=
 APPLICATION_HEADERS = {
     "Content-Type": "application/json",
     "Unleash-Client-Spec": CLIENT_SPEC_VERSION,
 }
 DISABLED_VARIATION = {"name": "disabled", "enabled": False}
```

### Comparing `UnleashClient-5.7.1/UnleashClient/constraints/Constraint.py` & `UnleashClient-5.8.0/UnleashClient/constraints/Constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,18 +222,17 @@
                     ConstraintOperators.SEMVER_EQ,
                     ConstraintOperators.SEMVER_GT,
                     ConstraintOperators.SEMVER_LT,
                 ]:
                     constraint_check = self.check_semver_operators(
                         context_value=context_value
                     )
-            else:
-                # This is a special case in the client spec - so it's getting it's own handler here
-                if self.operator is ConstraintOperators.NOT_IN:  # noqa: PLR5501
-                    constraint_check = True
+            # This is a special case in the client spec - so it's getting it's own handler here
+            elif self.operator is ConstraintOperators.NOT_IN:  # noqa: PLR5501
+                constraint_check = True
 
         except Exception as excep:  # pylint: disable=broad-except
             LOGGER.info(
                 "Could not evaluate context %s!  Error: %s", self.context_name, excep
             )
 
         return not constraint_check if self.inverted else constraint_check
```

### Comparing `UnleashClient-5.7.1/UnleashClient/deprecation_warnings.py` & `UnleashClient-5.8.0/UnleashClient/deprecation_warnings.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def strategy_v2xx_deprecation_check(strategies: list) -> None:
     """
     Notify users of backwards incompatible changes in v3 for custom strategies.
     """
     for strategy in strategies:
         try:
             # Check if the __call__() method is overwritten (should only be true for custom strategies in v1.x or v2.x.
-            if strategy.__call__ != Strategy.__call__:
+            if strategy.__call__ != Strategy.__call__:  # type:ignore
                 warnings.warn(
                     f"unleash-client-python v3.x.x requires overriding the execute() method instead of the __call__() method. Error in: {strategy.__name__}",
                     DeprecationWarning,
                 )
         except AttributeError:
             # Ignore if not.
             pass
```

### Comparing `UnleashClient-5.7.1/UnleashClient/events.py` & `UnleashClient-5.8.0/UnleashClient/events.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/features/Feature.py` & `UnleashClient-5.8.0/UnleashClient/features/Feature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # pylint: disable=invalid-name
+import copy
 from typing import Dict, Optional, cast
 
 from UnleashClient.constants import DISABLED_VARIATION
+from UnleashClient.strategies import EvaluationResult, Strategy
 from UnleashClient.utils import LOGGER
 from UnleashClient.variants import Variants
 
 
 # pylint: disable=dangerous-default-value, broad-except
 class Feature:
     def __init__(
@@ -69,62 +71,72 @@
         Count a specific variant.
 
         :param variant_name: The name of the variant to count.
         :return:
         """
         self.variant_counts[variant_name] = self.variant_counts.get(variant_name, 0) + 1
 
-    def is_enabled(
-        self, context: dict = None, default_value: bool = False
-    ) -> bool:  # pylint: disable=unused-argument
+    def is_enabled(self, context: dict = None) -> bool:
         """
         Checks if feature is enabled.
 
         :param context: Context information
-        :param default_value: Deprecated!  Users should use the fallback_function on the main is_enabled() method.
         :return:
         """
-        flag_value = False
+        evaluation_result = self._get_evaluation_result(context)
 
-        if self.enabled:
-            try:
-                if self.strategies:
-                    strategy_result = any(x.execute(context) for x in self.strategies)
-                else:
-                    # If no strategies are present, should default to true. This isn't possible via UI.
-                    strategy_result = True
-
-                flag_value = strategy_result
-            except Exception as strategy_except:
-                LOGGER.warning("Error checking feature flag: %s", strategy_except)
-
-        self.increment_stats(flag_value)
-
-        LOGGER.info("Feature toggle status for feature %s: %s", self.name, flag_value)
+        flag_value = evaluation_result.enabled
 
         return flag_value
 
     def get_variant(self, context: dict = None) -> dict:
         """
         Checks if feature is enabled and, if so, get the variant.
 
         :param context: Context information
         :return:
         """
-        variant = DISABLED_VARIATION
-        is_feature_enabled = self.is_enabled(context)
-
-        if is_feature_enabled and self.variants is not None:
+        evaluation_result = self._get_evaluation_result(context)
+        is_feature_enabled = evaluation_result.enabled
+        variant = evaluation_result.variant
+        if variant is None or (is_feature_enabled and variant == DISABLED_VARIATION):
             try:
-                variant = self.variants.get_variant(context)
-                variant["enabled"] = is_feature_enabled
+                LOGGER.debug("Getting variant from feature: %s", self.name)
+                variant = (
+                    self.variants.get_variant(context, is_feature_enabled)
+                    if is_feature_enabled
+                    else copy.deepcopy(DISABLED_VARIATION)
+                )
+
             except Exception as variant_exception:
                 LOGGER.warning("Error selecting variant: %s", variant_exception)
 
         self._count_variant(cast(str, variant["name"]))
         return variant
 
+    def _get_evaluation_result(self, context: dict = None) -> EvaluationResult:
+        strategy_result = EvaluationResult(False, None)
+        if self.enabled:
+            try:
+                if self.strategies:
+                    enabled_strategy: Strategy = next(
+                        (x for x in self.strategies if x.execute(context)), None
+                    )
+                    if enabled_strategy is not None:
+                        strategy_result = enabled_strategy.get_result(context)
+
+                else:
+                    # If no strategies are present, should default to true. This isn't possible via UI.
+                    strategy_result = EvaluationResult(True, None)
+
+            except Exception as evaluation_except:
+                LOGGER.warning("Error getting evaluation result: %s", evaluation_except)
+
+        self.increment_stats(strategy_result.enabled)
+        LOGGER.info("%s evaluation result: %s", self.name, strategy_result)
+        return strategy_result
+
     @staticmethod
     def metrics_only_feature(feature_name: str):
         feature = Feature(feature_name, False, [])
         feature.only_for_metrics = True
         return feature
```

### Comparing `UnleashClient-5.7.1/UnleashClient/loader.py` & `UnleashClient-5.8.0/UnleashClient/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,23 @@
                 constraint_provisioning = {}
 
             if "segments" in strategy.keys():
                 segment_provisioning = strategy["segments"]
             else:
                 segment_provisioning = []
 
+            if "variants" in strategy.keys():
+                variant_provisioning = strategy["variants"]
+            else:
+                variant_provisioning = []
+
             feature_strategies.append(
                 strategy_mapping[strategy["name"]](
                     constraints=constraint_provisioning,
+                    variants=variant_provisioning,
                     parameters=strategy_provisioning,
                     global_segments=global_segments,
                     segment_ids=segment_provisioning,
                 )
             )
         except Exception as excep:
             strategies = cache.get(FAILED_STRATEGIES, [])
```

### Comparing `UnleashClient-5.7.1/UnleashClient/periodic_tasks/fetch_and_load.py` & `UnleashClient-5.8.0/UnleashClient/periodic_tasks/fetch_and_load.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/periodic_tasks/send_metrics.py` & `UnleashClient-5.8.0/UnleashClient/periodic_tasks/send_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/strategies/FlexibleRolloutStrategy.py` & `UnleashClient-5.8.0/UnleashClient/strategies/FlexibleRolloutStrategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutSessionId.py` & `UnleashClient-5.8.0/UnleashClient/strategies/GradualRolloutSessionId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutUserId.py` & `UnleashClient-5.8.0/UnleashClient/strategies/GradualRolloutUserId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/strategies/RemoteAddress.py` & `UnleashClient-5.8.0/UnleashClient/strategies/RemoteAddress.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,13 +57,12 @@
             ]:
                 if isinstance(
                     addr_or_range, (ipaddress.IPv4Address, ipaddress.IPv6Address)
                 ):
                     if context_ip == addr_or_range:
                         return_value = True
                         break
-                else:
-                    if context_ip in addr_or_range:  # noqa: PLR5501
-                        return_value = True
-                        break
+                elif context_ip in addr_or_range:  # noqa: PLR5501
+                    return_value = True
+                    break
 
         return return_value
```

### Comparing `UnleashClient-5.7.1/UnleashClient/strategies/Strategy.py` & `UnleashClient-5.8.0/UnleashClient/strategies/Strategy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 # pylint: disable=invalid-name,dangerous-default-value
 import warnings
-from typing import Iterator
+from dataclasses import dataclass
+from typing import Iterator, Optional
 
 from UnleashClient.constraints import Constraint
+from UnleashClient.variants import Variants
+
+
+@dataclass
+class EvaluationResult:
+    enabled: bool
+    variant: Optional[dict]
 
 
 class Strategy:
     """
     The parent class for default and custom strategies.
 
     In general, default & custom classes should only need to override:
 
     - ``__init__()`` - Depending on the parameters your feature needs
     - ``apply()`` - Your feature provisioning
 
     :param constraints: List of 'constraints' objects derived from strategy section (...from feature section) of `/api/clients/features` Unleash server response.
+    :param variants: List of 'variant' objects derived from strategy section (...from feature section) of `/api/clients/features` Unleash server response.
     :param parameters: The 'parameter' objects from the strategy section (...from feature section) of `/api/clients/features` Unleash server response.
     """
 
     def __init__(
         self,
         constraints: list = [],
         parameters: dict = {},
         segment_ids: list = None,
         global_segments: dict = None,
+        variants: list = None,
     ) -> None:
         self.parameters = parameters
         self.constraints = constraints
+        self.variants = variants or []
         self.segment_ids = segment_ids or []
         self.global_segments = global_segments or {}
         self.parsed_provisioning = self.load_provisioning()
 
     def __call__(self, context: dict = None):
         warnings.warn(
             "unleash-client-python v3.x.x requires overriding the execute() method instead of the __call__() method.",
@@ -52,24 +63,41 @@
         flag_state = False
 
         if all(constraint.apply(context) for constraint in self.parsed_constraints):
             flag_state = self.apply(context)
 
         return flag_state
 
+    def get_result(self, context) -> EvaluationResult:
+        enabled = self.execute(context)
+        variant = None
+        if enabled:
+            variant = self.parsed_variants.get_variant(context, enabled)
+
+        result = EvaluationResult(enabled, variant)
+        return result
+
     @property
     def parsed_constraints(self) -> Iterator[Constraint]:
         for constraint_dict in self.constraints:
             yield Constraint(constraint_dict=constraint_dict)
 
         for segment_id in self.segment_ids:
             segment = self.global_segments[segment_id]
             for constraint in segment["constraints"]:
                 yield Constraint(constraint_dict=constraint)
 
+    @property
+    def parsed_variants(self) -> Variants:
+        return Variants(
+            variants_list=self.variants,
+            group_id=self.parameters.get("groupId"),
+            is_feature_variants=False,
+        )
+
     def load_provisioning(self) -> list:  # pylint: disable=no-self-use
         """
         Loads strategy provisioning from Unleash feature flag configuration.
 
         This should parse the raw values in ``self.parameters`` into format Python can comprehend.
         """
         return []
```

### Comparing `UnleashClient-5.7.1/UnleashClient/strategies/UserWithId.py` & `UnleashClient-5.8.0/UnleashClient/strategies/UserWithId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/utils.py` & `UnleashClient-5.8.0/UnleashClient/utils.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/UnleashClient/variants/Variants.py` & `UnleashClient-5.8.0/UnleashClient/variants/Variants.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # pylint: disable=invalid-name, too-few-public-methods
 import copy
 import random
-from typing import Dict  # noqa: F401
+from typing import Dict, Optional  # noqa: F401
 
 from UnleashClient import utils
 from UnleashClient.constants import DISABLED_VARIATION
 
 
 class Variants:
-    def __init__(self, variants_list: list, feature_name: str) -> None:
+    def __init__(
+        self, variants_list: list, group_id: str, is_feature_variants: bool = True
+    ) -> None:
         """
         Represents an A/B test
 
         variants_list = From the strategy document.
         """
         self.variants = variants_list
-        self.feature_name = feature_name
+        self.group_id = group_id
+        self.is_feature_variants = is_feature_variants
 
     def _apply_overrides(self, context: dict) -> dict:
         """
         Figures out if an override should be applied based on a context.
 
         Notes:
             - This matches only the first variant found.
@@ -56,53 +59,57 @@
                 context.get(stickiness_selector)
                 or context.get("properties")[stickiness_selector]
             )
 
         return seed
 
     @staticmethod
-    def _format_variation(variation: dict) -> dict:
+    def _format_variation(variation: dict, flag_status: Optional[bool] = None) -> dict:
         formatted_variation = copy.deepcopy(variation)
         del formatted_variation["weight"]
         if "overrides" in formatted_variation:
             del formatted_variation["overrides"]
         if "stickiness" in formatted_variation:
             del formatted_variation["stickiness"]
+        if "enabled" not in formatted_variation and flag_status is not None:
+            formatted_variation["enabled"] = flag_status
         return formatted_variation
 
-    def get_variant(self, context: dict) -> dict:
+    def get_variant(self, context: dict, flag_status: Optional[bool] = None) -> dict:
         """
         Determines what variation a user is in.
 
         :param context:
+        :param flag_status:
         :return:
         """
         fallback_variant = copy.deepcopy(DISABLED_VARIATION)
 
         if self.variants:
             override_variant = self._apply_overrides(context)
             if override_variant:
-                return self._format_variation(override_variant)
+                return self._format_variation(override_variant, flag_status)
 
             total_weight = sum(x["weight"] for x in self.variants)
             if total_weight <= 0:
                 return fallback_variant
 
             stickiness_selector = (
                 self.variants[0]["stickiness"]
                 if "stickiness" in self.variants[0].keys()
                 else "default"
             )
+
             target = utils.normalized_hash(
                 self._get_seed(context, stickiness_selector),
-                self.feature_name,
+                self.group_id,
                 total_weight,
             )
             counter = 0
             for variation in self.variants:
                 counter += variation["weight"]
 
                 if counter >= target:
-                    return self._format_variation(variation)
+                    return self._format_variation(variation, flag_status)
 
         # Catch all return.
         return fallback_variant
```

### Comparing `UnleashClient-5.7.1/UnleashClient.egg-info/PKG-INFO` & `UnleashClient-5.8.0/UnleashClient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnleashClient
-Version: 5.7.1
+Version: 5.8.0
 Summary: Python client for the Unleash feature toggle system!
 Author-email: Ivan Lee <ivanklee86@gmail.com>
 Project-URL: Homepage, https://github.com/Unleash/unleash-client-python
 Project-URL: Documentation, https://docs.getunleash.io/unleash-client-python
 Project-URL: Changelog, https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/Unleash/unleash-client-python
 Project-URL: Issues, https://github.com/Unleash/unleash-client-python/issues
```

### Comparing `UnleashClient-5.7.1/UnleashClient.egg-info/SOURCES.txt` & `UnleashClient-5.8.0/UnleashClient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 tests/unit_tests/strategies/test_applicationhostname.py
 tests/unit_tests/strategies/test_defaultstrategy.py
 tests/unit_tests/strategies/test_flexiblerollout.py
 tests/unit_tests/strategies/test_gradualrolloutrandom.py
 tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
 tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
 tests/unit_tests/strategies/test_remoteaddress.py
+tests/unit_tests/strategies/test_strategy_variants.py
 tests/unit_tests/strategies/test_userwithids.py
 tests/utilities/__init__.py
 tests/utilities/data_generator.py
 tests/utilities/testing_constants.py
 tests/utilities/mocks/__init__.py
 tests/utilities/mocks/mock_all_features.py
 tests/utilities/mocks/mock_bootstrap.json
```

### Comparing `UnleashClient-5.7.1/docs/Makefile` & `UnleashClient-5.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/celery.rst` & `UnleashClient-5.8.0/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/conf.py` & `UnleashClient-5.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/customcache.rst` & `UnleashClient-5.8.0/docs/customcache.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/customstrategies.rst` & `UnleashClient-5.8.0/docs/customstrategies.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/development.rst` & `UnleashClient-5.8.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/eventcallbacks.rst` & `UnleashClient-5.8.0/docs/eventcallbacks.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/index.rst` & `UnleashClient-5.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/make.bat` & `UnleashClient-5.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/usage.rst` & `UnleashClient-5.8.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/docs/wsgi.rst` & `UnleashClient-5.8.0/docs/wsgi.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/pyproject.toml` & `UnleashClient-5.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/conftest.py` & `UnleashClient-5.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/integration_tests/integration.py` & `UnleashClient-5.8.0/tests/integration_tests/integration.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/integration_tests/integration_gitlab.py` & `UnleashClient-5.8.0/tests/integration_tests/integration_gitlab.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/integration_tests/integration_unleashheroku.py` & `UnleashClient-5.8.0/tests/integration_tests/integration_unleashheroku.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/integration_tests/integration_unleashhosted.py` & `UnleashClient-5.8.0/tests/integration_tests/integration_unleashhosted.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/specification_tests/test_client_specs.py` & `UnleashClient-5.8.0/tests/specification_tests/test_client_specs.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,37 +23,51 @@
 
 
 def load_specs():
     with open(path.join(CLIENT_SPEC_PATH, "index.json")) as _f:
         return json.load(_f)
 
 
+def get_client(state, test_context=None):
+    cache = FileCache("MOCK_CACHE")
+    cache.bootstrap_from_dict(state)
+    env = "default"
+    if test_context is not None and "environment" in test_context:
+        env = test_context["environment"]
+
+    unleash_client = UnleashClient(
+        url=URL,
+        app_name=APP_NAME,
+        instance_id="pytest_%s" % uuid.uuid4(),
+        disable_metrics=True,
+        disable_registration=True,
+        cache=cache,
+        environment=env,
+    )
+
+    unleash_client.initialize_client(fetch_toggles=False)
+    return unleash_client
+
+
 def iter_spec():
     for spec in load_specs():
         name, state, tests, variant_tests = load_spec(spec)
 
-        cache = FileCache("MOCK_CACHE")
-        cache.bootstrap_from_dict(state)
-
-        unleash_client = UnleashClient(
-            url=URL,
-            app_name=APP_NAME,
-            instance_id="pytest_%s" % uuid.uuid4(),
-            disable_metrics=True,
-            disable_registration=True,
-            cache=cache,
-        )
-
-        unleash_client.initialize_client(fetch_toggles=False)
+        unleash_client = get_client(state=state)
 
         for test in tests:
             yield name, test["description"], unleash_client, test, False
 
         for variant_test in variant_tests:
-            yield name, test["description"], unleash_client, variant_test, True
+            test_context = {}
+            if "context" in variant_test:
+                test_context = variant_test["context"]
+
+            unleash_client = get_client(state, test_context)
+            yield name, variant_test["description"], unleash_client, variant_test, True
 
         unleash_client.destroy()
 
 
 try:
     ALL_SPECS = list(iter_spec())
     TEST_DATA = [x[2:] for x in ALL_SPECS]
@@ -73,10 +87,9 @@
         expected = test_data["expectedResult"]
         context = test_data.get("context")
         assert unleash_client.is_enabled(toggle_name, context) == expected
     else:
         toggle_name = test_data["toggleName"]
         expected = test_data["expectedResult"]
         context = test_data.get("context")
-
         variant = unleash_client.get_variant(toggle_name, context)
         assert variant == expected
```

### Comparing `UnleashClient-5.7.1/tests/unit_tests/api/test_feature.py` & `UnleashClient-5.8.0/tests/unit_tests/api/test_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     )
 
     assert len(responses.calls) == 4
     assert not etag
 
 
 @pytest.mark.skipif(
-    date.today() < date(2023, 7, 1),
+    date.today() < date(2023, 9, 1),
     reason="This is currently breaking due to a dependency or the test setup. Skipping this allows us to run tests in CI without this popping up as an error all the time.",
 )
 @responses.activate
 def test_get_feature_toggle_etag_present():
     responses.add(
         responses.GET, PROJECT_URL, json={}, status=304, headers={"etag": ETAG_VALUE}
     )
```

### Comparing `UnleashClient-5.7.1/tests/unit_tests/api/test_metrics.py` & `UnleashClient-5.8.0/tests/unit_tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/api/test_register.py` & `UnleashClient-5.8.0/tests/unit_tests/api/test_register.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py` & `UnleashClient-5.8.0/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/periodic/test_fetch_and_load.py` & `UnleashClient-5.8.0/tests/unit_tests/periodic/test_fetch_and_load.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/strategies/test_flexiblerollout.py` & `UnleashClient-5.8.0/tests/unit_tests/strategies/test_flexiblerollout.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/strategies/test_remoteaddress.py` & `UnleashClient-5.8.0/tests/unit_tests/strategies/test_remoteaddress.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/test_client.py` & `UnleashClient-5.8.0/tests/unit_tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,16 +472,15 @@
     for api_call in responses.calls:
         assert "/api/client/features" in api_call.request.url
 
 
 @responses.activate
 def test_uc_server_error(unleash_client):
     # Verify that Unleash Client will still fall back gracefully if SERVER ANGRY RAWR, and then recover gracefully.
-
-    unleash_client = unleash_client
+    unleash_client = unleash_client  # noqa
     # Set up APIs
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=401)
     responses.add(responses.GET, URL + FEATURES_URL, status=500)
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=401)
 
     unleash_client.initialize_client()
     assert not unleash_client.is_enabled("testFlag")
```

### Comparing `UnleashClient-5.7.1/tests/unit_tests/test_constraints.py` & `UnleashClient-5.8.0/tests/unit_tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/test_custom_strategy.py` & `UnleashClient-5.8.0/tests/unit_tests/test_custom_strategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/test_features.py` & `UnleashClient-5.8.0/tests/unit_tests/test_features.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import pytest
 
 from tests.utilities import generate_email_list
-from tests.utilities.mocks.mock_variants import VARIANTS
+from tests.utilities.mocks.mock_variants import VARIANTS, VARIANTS_WITH_STICKINESS
 from tests.utilities.testing_constants import IP_LIST
 from UnleashClient.features import Feature
-from UnleashClient.strategies import Default, RemoteAddress, UserWithId
+from UnleashClient.strategies import Default, FlexibleRollout, RemoteAddress, UserWithId
 from UnleashClient.variants import Variants
 
 (EMAIL_LIST, CONTEXT) = generate_email_list(20)
 
+BASE_FLEXIBLE_ROLLOUT_DICT = {
+    "name": "flexibleRollout",
+    "parameters": {"rollout": 50, "stickiness": "userId", "groupId": "AB12A"},
+    "variants": VARIANTS_WITH_STICKINESS,
+    "constraints": [],
+}
+
 
 @pytest.fixture()
 def test_feature():
     strategies = [
         RemoteAddress(parameters={"IPs": IP_LIST}),
         UserWithId(parameters={"userIds": EMAIL_LIST}),
     ]
@@ -22,14 +29,27 @@
 @pytest.fixture()
 def test_feature_variants():
     strategies = [Default()]
     variants = Variants(VARIANTS, "My Feature")
     yield Feature("My Feature", True, strategies, variants)
 
 
+@pytest.fixture()
+def test_feature_strategy_variants():
+    strategies = [
+        FlexibleRollout(
+            BASE_FLEXIBLE_ROLLOUT_DICT["constraints"],
+            BASE_FLEXIBLE_ROLLOUT_DICT["parameters"],
+            variants=VARIANTS_WITH_STICKINESS,
+        )
+    ]
+    variants = Variants(VARIANTS, "My Feature")
+    yield Feature("My Feature", True, strategies, variants)
+
+
 def test_create_feature_true(test_feature):
     my_feature = test_feature
 
     CONTEXT["remoteAddress"] = "69.208.0.1"
     assert my_feature.is_enabled(CONTEXT)
     assert my_feature.yes_count == 1
 
@@ -100,7 +120,23 @@
         assert test_feature_variants.variant_counts["disabled"] == iteration
 
 
 def test_variant_metrics_feature_has_no_variants(test_feature):
     for iteration in range(1, 7):
         test_feature.get_variant({})
         assert test_feature.variant_counts["disabled"] == iteration
+
+
+def test_strategy_variant_is_returned(test_feature_strategy_variants):
+    context = {
+        "userId": "122",
+        "appName": "test",
+        "environment": "prod",
+        "customField": "1",
+    }
+    variant = test_feature_strategy_variants.get_variant(context)
+
+    assert variant == {
+        "enabled": True,
+        "name": "VarB",
+        "payload": {"type": "string", "value": "Test 2"},
+    }
```

### Comparing `UnleashClient-5.7.1/tests/unit_tests/test_loader.py` & `UnleashClient-5.8.0/tests/unit_tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/unit_tests/test_variants.py` & `UnleashClient-5.8.0/tests/unit_tests/test_variants.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/utilities/mocks/mock_all_features.py` & `UnleashClient-5.8.0/tests/utilities/mocks/mock_all_features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/utilities/mocks/mock_constraints.py` & `UnleashClient-5.8.0/tests/utilities/mocks/mock_constraints.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/utilities/mocks/mock_custom_strategy.py` & `UnleashClient-5.8.0/tests/utilities/mocks/mock_custom_strategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/utilities/mocks/mock_features.py` & `UnleashClient-5.8.0/tests/utilities/mocks/mock_features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/utilities/mocks/mock_variants.py` & `UnleashClient-5.8.0/tests/utilities/mocks/mock_variants.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/utilities/old_code/StrategyV2.py` & `UnleashClient-5.8.0/tests/utilities/old_code/StrategyV2.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.1/tests/utilities/testing_constants.py` & `UnleashClient-5.8.0/tests/utilities/testing_constants.py`

 * *Files identical despite different names*

