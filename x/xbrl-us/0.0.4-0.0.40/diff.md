# Comparing `tmp/xbrl-us-0.0.4.tar.gz` & `tmp/xbrl-us-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbrl-us-0.0.4.tar", last modified: Fri Aug  4 02:01:25 2023, max compression
+gzip compressed data, was "xbrl-us-0.0.40.tar", last modified: Fri Aug  4 13:58:48 2023, max compression
```

## Comparing `xbrl-us-0.0.4.tar` & `xbrl-us-0.0.40.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.696681 xbrl-us-0.0.4/
--rw-r--r--   0 hamid      (501) staff       (20)      527 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/.bumpversion.cfg
--rw-r--r--   0 hamid      (501) staff       (20)     2015 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/.cookiecutterrc
--rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/.coveragerc
--rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/.editorconfig
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.620024 xbrl-us-0.0.4/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.630222 xbrl-us-0.0.4/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     3400 2023-07-14 19:39:33.000000 xbrl-us-0.0.4/.github/workflows/github-actions.yml
--rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.4/.readthedocs.yml
--rw-r--r--   0 hamid      (501) staff       (20)      694 2023-07-17 21:31:18.000000 xbrl-us-0.0.4/CHANGELOG.rst
--rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/CONTRIBUTING.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.4/LICENSE
--rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.4/MANIFEST.in
--rw-r--r--   0 hamid      (501) staff       (20)    13638 2023-08-04 02:01:25.696011 xbrl-us-0.0.4/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)    11606 2023-07-18 17:14:45.000000 xbrl-us-0.0.4/README.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.631184 xbrl-us-0.0.4/ci/
--rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/ci/bootstrap.py
--rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/ci/requirements.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.620423 xbrl-us-0.0.4/ci/templates/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.620524 xbrl-us-0.0.4/ci/templates/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.631586 xbrl-us-0.0.4/ci/templates/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.634965 xbrl-us-0.0.4/docs/
--rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/docs/changelog.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1155 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/docs/conf.py
--rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/docs/contributing.rst
--rw-r--r--   0 hamid      (501) staff       (20)      208 2023-07-17 22:11:31.000000 xbrl-us-0.0.4/docs/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)    10882 2023-07-19 13:02:53.000000 xbrl-us-0.0.4/docs/readme.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.635890 xbrl-us-0.0.4/docs/reference/
--rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.4/docs/reference/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.4/docs/reference/xbrl_us.rst
--rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.4/docs/requirements.txt
--rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/docs/spelling_wordlist.txt
--rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.4/pyproject.toml
--rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/pytest.ini
--rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.4/secrets.yml
--rw-r--r--   0 hamid      (501) staff       (20)       38 2023-08-04 02:01:25.696879 xbrl-us-0.0.4/setup.cfg
--rwxr-xr-x   0 hamid      (501) staff       (20)     3003 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/setup.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.621503 xbrl-us-0.0.4/src/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.639941 xbrl-us-0.0.4/src/xbrl_us/
--rw-r--r--   0 hamid      (501) staff       (20)       69 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/src/xbrl_us/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.4/src/xbrl_us/__main__.py
--rw-r--r--   0 hamid      (501) staff       (20)    17831 2023-08-04 00:05:41.000000 xbrl-us-0.0.4/src/xbrl_us/app.py
--rw-r--r--   0 hamid      (501) staff       (20)      373 2023-08-03 21:05:17.000000 xbrl-us-0.0.4/src/xbrl_us/cli.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.669978 xbrl-us-0.0.4/src/xbrl_us/methods/
--rw-r--r--   0 hamid      (501) staff       (20)    12479 2023-08-04 01:52:45.000000 xbrl-us-0.0.4/src/xbrl_us/methods/_definitions.yaml
--rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.4/src/xbrl_us/methods/assertion search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.4/src/xbrl_us/methods/assertion validate.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.4/src/xbrl_us/methods/concept name search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.4/src/xbrl_us/methods/concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/cube search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dimension search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/document search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept label.yml
--rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept name.yml
--rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept reference.yml
--rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id network search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id network.yml
--rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/entity id report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/entity id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/entity report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/entity search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.4/src/xbrl_us/methods/fact id.yml
--rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.4/src/xbrl_us/methods/fact search oim.yml
--rw-r--r--   0 hamid      (501) staff       (20)     3002 2023-08-04 00:06:26.000000 xbrl-us-0.0.4/src/xbrl_us/methods/fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/label dts id search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/label search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/network id relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/network id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/network relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/relationship tree search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report id delete.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report id fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report search.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.685848 xbrl-us-0.0.4/src/xbrl_us/schemas/
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/assertion_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/concept_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/cube_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/dimension_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/document_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/dts_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/entity_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/fact_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/label_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/network_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/relationship_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/report_details.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.692767 xbrl-us-0.0.4/src/xbrl_us/utils/
--rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.4/src/xbrl_us/utils/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)     1633 2023-07-16 19:19:32.000000 xbrl-us-0.0.4/src/xbrl_us/utils/exceptions.py
--rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.4/src/xbrl_us/utils/fields.py
--rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.4/src/xbrl_us/utils/paramters.py
--rw-r--r--   0 hamid      (501) staff       (20)    30836 2023-08-04 01:53:19.000000 xbrl-us-0.0.4/src/xbrl_us/xbrl_us.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.645747 xbrl-us-0.0.4/src/xbrl_us.egg-info/
--rw-r--r--   0 hamid      (501) staff       (20)    13638 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     2936 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/SOURCES.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/dependency_links.txt
--rw-r--r--   0 hamid      (501) staff       (20)       45 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/entry_points.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-08-03 23:15:34.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/not-zip-safe
--rw-r--r--   0 hamid      (501) staff       (20)      103 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/requires.txt
--rw-r--r--   0 hamid      (501) staff       (20)        8 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/top_level.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.694987 xbrl-us-0.0.4/tests/
--rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.4/tests/test_xbrl_us.py
--rw-r--r--   0 hamid      (501) staff       (20)     1486 2023-07-14 19:43:01.000000 xbrl-us-0.0.4/tox.ini
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.594250 xbrl-us-0.0.40/
+-rw-r--r--   0 hamid      (501) staff       (20)      528 2023-08-04 13:58:19.000000 xbrl-us-0.0.40/.bumpversion.cfg
+-rw-r--r--   0 hamid      (501) staff       (20)     2016 2023-08-04 13:58:19.000000 xbrl-us-0.0.40/.cookiecutterrc
+-rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/.coveragerc
+-rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/.editorconfig
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.529208 xbrl-us-0.0.40/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.536920 xbrl-us-0.0.40/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     3400 2023-07-14 19:39:33.000000 xbrl-us-0.0.40/.github/workflows/github-actions.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.40/.pre-commit-config.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.40/.readthedocs.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      817 2023-08-04 13:57:06.000000 xbrl-us-0.0.40/CHANGELOG.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/CONTRIBUTING.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.40/LICENSE
+-rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.40/MANIFEST.in
+-rw-r--r--   0 hamid      (501) staff       (20)    13762 2023-08-04 13:58:48.593469 xbrl-us-0.0.40/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)    11606 2023-07-18 17:14:45.000000 xbrl-us-0.0.40/README.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.537857 xbrl-us-0.0.40/ci/
+-rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/ci/bootstrap.py
+-rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/ci/requirements.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.529614 xbrl-us-0.0.40/ci/templates/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.529714 xbrl-us-0.0.40/ci/templates/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.538502 xbrl-us-0.0.40/ci/templates/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.542358 xbrl-us-0.0.40/docs/
+-rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/docs/changelog.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1156 2023-08-04 13:58:19.000000 xbrl-us-0.0.40/docs/conf.py
+-rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/docs/contributing.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      208 2023-07-17 22:11:31.000000 xbrl-us-0.0.40/docs/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)    10882 2023-07-19 13:02:53.000000 xbrl-us-0.0.40/docs/readme.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.543198 xbrl-us-0.0.40/docs/reference/
+-rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.40/docs/reference/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.40/docs/reference/xbrl_us.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.40/docs/requirements.txt
+-rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/docs/spelling_wordlist.txt
+-rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.40/pyproject.toml
+-rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.40/pytest.ini
+-rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.40/secrets.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       38 2023-08-04 13:58:48.594452 xbrl-us-0.0.40/setup.cfg
+-rwxr-xr-x   0 hamid      (501) staff       (20)     3004 2023-08-04 13:58:19.000000 xbrl-us-0.0.40/setup.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.530367 xbrl-us-0.0.40/src/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.545879 xbrl-us-0.0.40/src/xbrl_us/
+-rw-r--r--   0 hamid      (501) staff       (20)       70 2023-08-04 13:58:19.000000 xbrl-us-0.0.40/src/xbrl_us/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.40/src/xbrl_us/__main__.py
+-rw-r--r--   0 hamid      (501) staff       (20)    17831 2023-08-04 00:05:41.000000 xbrl-us-0.0.40/src/xbrl_us/app.py
+-rw-r--r--   0 hamid      (501) staff       (20)      373 2023-08-03 21:05:17.000000 xbrl-us-0.0.40/src/xbrl_us/cli.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.577568 xbrl-us-0.0.40/src/xbrl_us/methods/
+-rw-r--r--   0 hamid      (501) staff       (20)    12479 2023-08-04 01:52:45.000000 xbrl-us-0.0.40/src/xbrl_us/methods/_definitions.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.40/src/xbrl_us/methods/assertion search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.40/src/xbrl_us/methods/assertion validate.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.40/src/xbrl_us/methods/concept name search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.40/src/xbrl_us/methods/concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/cube search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/dimension search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/document search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/dts id concept label.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/dts id concept name.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/dts id concept reference.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/dts id concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/dts id network search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/dts id network.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/dts search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/entity id report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/entity id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/entity report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/entity search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.40/src/xbrl_us/methods/fact id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.40/src/xbrl_us/methods/fact search oim.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     3002 2023-08-04 00:06:26.000000 xbrl-us-0.0.40/src/xbrl_us/methods/fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/label dts id search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/label search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/network id relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/network id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/network relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.40/src/xbrl_us/methods/relationship tree search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.40/src/xbrl_us/methods/report fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.40/src/xbrl_us/methods/report id delete.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.40/src/xbrl_us/methods/report id fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.40/src/xbrl_us/methods/report id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.40/src/xbrl_us/methods/report search.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.587411 xbrl-us-0.0.40/src/xbrl_us/schemas/
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/assertion_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/concept_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/cube_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/dimension_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/document_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/dts_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/entity_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/fact_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/label_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/network_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/relationship_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.40/src/xbrl_us/schemas/report_details.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.590719 xbrl-us-0.0.40/src/xbrl_us/utils/
+-rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.40/src/xbrl_us/utils/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1633 2023-07-16 19:19:32.000000 xbrl-us-0.0.40/src/xbrl_us/utils/exceptions.py
+-rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.40/src/xbrl_us/utils/fields.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.40/src/xbrl_us/utils/paramters.py
+-rw-r--r--   0 hamid      (501) staff       (20)    30836 2023-08-04 01:53:19.000000 xbrl-us-0.0.40/src/xbrl_us/xbrl_us.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.551090 xbrl-us-0.0.40/src/xbrl_us.egg-info/
+-rw-r--r--   0 hamid      (501) staff       (20)    13762 2023-08-04 13:58:48.000000 xbrl-us-0.0.40/src/xbrl_us.egg-info/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)     2936 2023-08-04 13:58:48.000000 xbrl-us-0.0.40/src/xbrl_us.egg-info/SOURCES.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-08-04 13:58:48.000000 xbrl-us-0.0.40/src/xbrl_us.egg-info/dependency_links.txt
+-rw-r--r--   0 hamid      (501) staff       (20)       45 2023-08-04 13:58:48.000000 xbrl-us-0.0.40/src/xbrl_us.egg-info/entry_points.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-08-03 23:15:34.000000 xbrl-us-0.0.40/src/xbrl_us.egg-info/not-zip-safe
+-rw-r--r--   0 hamid      (501) staff       (20)      103 2023-08-04 13:58:48.000000 xbrl-us-0.0.40/src/xbrl_us.egg-info/requires.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        8 2023-08-04 13:58:48.000000 xbrl-us-0.0.40/src/xbrl_us.egg-info/top_level.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 13:58:48.592369 xbrl-us-0.0.40/tests/
+-rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.40/tests/test_xbrl_us.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1486 2023-07-14 19:43:01.000000 xbrl-us-0.0.40/tox.ini
```

### Comparing `xbrl-us-0.0.4/.bumpversion.cfg` & `xbrl-us-0.0.40/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.4
+current_version = 0.0.40
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `xbrl-us-0.0.4/.cookiecutterrc` & `xbrl-us-0.0.40/.cookiecutterrc`

 * *Files 8% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://python-xbrl-us.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
     test_matrix_separate_coverage: "no"
-    version: "0.0.4"
+    version: "0.0.40"
     version_manager: "bump2version"
     website: "https://hamidvakilzadeh.com"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `xbrl-us-0.0.4/.github/workflows/github-actions.yml` & `xbrl-us-0.0.40/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/.pre-commit-config.yaml` & `xbrl-us-0.0.40/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/CHANGELOG.rst` & `xbrl-us-0.0.40/CHANGELOG.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 
 Changelog
 =========
 
+0.0.40 (2023-08-03)
+~~~~~~~~~~~~~~~~~~~
+
+* Improved Browser Interface
+* improved error handling for requests
+* Bug fixes
+
+
 0.0.32 (2023-07-17)
 ~~~~~~~~~~~~~~~~~~~
 
 * Improved Browser Interface
 * Added ``unique`` keyword to ``query`` method
 * Bug fixes
```

### Comparing `xbrl-us-0.0.4/CONTRIBUTING.rst` & `xbrl-us-0.0.40/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/LICENSE` & `xbrl-us-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/PKG-INFO` & `xbrl-us-0.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.4
+Version: 0.0.40
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
@@ -405,14 +405,22 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+0.0.40 (2023-08-03)
+~~~~~~~~~~~~~~~~~~~
+
+* Improved Browser Interface
+* improved error handling for requests
+* Bug fixes
+
+
 0.0.32 (2023-07-17)
 ~~~~~~~~~~~~~~~~~~~
 
 * Improved Browser Interface
 * Added ``unique`` keyword to ``query`` method
 * Bug fixes
```

### Comparing `xbrl-us-0.0.4/README.rst` & `xbrl-us-0.0.40/README.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/ci/bootstrap.py` & `xbrl-us-0.0.40/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/ci/templates/.github/workflows/github-actions.yml` & `xbrl-us-0.0.40/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/docs/conf.py` & `xbrl-us-0.0.40/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "xbrl-us"
 year = "2023"
 author = "hamid-vakilzadeh"
 copyright = f"{year}, {author}"
-version = release = "0.0.4"
+version = release = "0.0.40"
 
 pygments_style = "emacs"
 highlight_language = "python"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/issues/%s", "#"),
     "pr": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/pull/%s", "PR #"),
```

### Comparing `xbrl-us-0.0.4/docs/readme.rst` & `xbrl-us-0.0.40/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/pyproject.toml` & `xbrl-us-0.0.40/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/pytest.ini` & `xbrl-us-0.0.40/pytest.ini`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/setup.py` & `xbrl-us-0.0.40/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="xbrl-us",
-    version="0.0.4",
+    version="0.0.40",
     license="MIT",
     description="Python wrapper for xbrl.us API",
     long_description_content_type="text/x-rst",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
```

### Comparing `xbrl-us-0.0.4/src/xbrl_us/app.py` & `xbrl-us-0.0.40/src/xbrl_us/app.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/_definitions.yaml` & `xbrl-us-0.0.40/src/xbrl_us/methods/_definitions.yaml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/assertion search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/assertion search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/concept name search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/concept name search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/concept search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/cube search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/cube search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/dimension search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/dimension search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/document search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/document search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept name.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/dts id concept name.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept reference.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/dts id concept reference.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/dts id concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/dts id network search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/dts id network search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/dts id network.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/dts id network.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/dts search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/dts search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/entity id report search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/entity id report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/entity report search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/entity report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/fact id.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/fact id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/fact search oim.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/fact search oim.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/fact search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/label dts id search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/label dts id search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/network id relationship search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/network id relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/network relationship search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/network relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/relationship search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/relationship tree search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/relationship tree search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/report fact search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/report fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/report id fact search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/report id fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/report id.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/report id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/methods/report search.yml` & `xbrl-us-0.0.40/src/xbrl_us/methods/report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/schemas/concept_details.py` & `xbrl-us-0.0.40/src/xbrl_us/schemas/concept_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/schemas/dimension_details.py` & `xbrl-us-0.0.40/src/xbrl_us/schemas/dimension_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/utils/exceptions.py` & `xbrl-us-0.0.40/src/xbrl_us/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/utils/paramters.py` & `xbrl-us-0.0.40/src/xbrl_us/utils/paramters.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us/xbrl_us.py` & `xbrl-us-0.0.40/src/xbrl_us/xbrl_us.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/src/xbrl_us.egg-info/PKG-INFO` & `xbrl-us-0.0.40/src/xbrl_us.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.4
+Version: 0.0.40
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
@@ -405,14 +405,22 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+0.0.40 (2023-08-03)
+~~~~~~~~~~~~~~~~~~~
+
+* Improved Browser Interface
+* improved error handling for requests
+* Bug fixes
+
+
 0.0.32 (2023-07-17)
 ~~~~~~~~~~~~~~~~~~~
 
 * Improved Browser Interface
 * Added ``unique`` keyword to ``query`` method
 * Bug fixes
```

### Comparing `xbrl-us-0.0.4/src/xbrl_us.egg-info/SOURCES.txt` & `xbrl-us-0.0.40/src/xbrl_us.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/tests/test_xbrl_us.py` & `xbrl-us-0.0.40/tests/test_xbrl_us.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.4/tox.ini` & `xbrl-us-0.0.40/tox.ini`

 * *Files identical despite different names*

