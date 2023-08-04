# Comparing `tmp/xbrl-us-0.0.32.tar.gz` & `tmp/xbrl-us-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbrl-us-0.0.32.tar", last modified: Mon Jul 17 21:31:46 2023, max compression
+gzip compressed data, was "xbrl-us-0.0.4.tar", last modified: Fri Aug  4 02:01:25 2023, max compression
```

## Comparing `xbrl-us-0.0.32.tar` & `xbrl-us-0.0.4.tar`

### file list

```diff
@@ -1,112 +1,111 @@
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.556568 xbrl-us-0.0.32/
--rw-r--r--   0 hamid      (501) staff       (20)      528 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/.bumpversion.cfg
--rw-r--r--   0 hamid      (501) staff       (20)     2016 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/.cookiecutterrc
--rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/.coveragerc
--rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/.editorconfig
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.502129 xbrl-us-0.0.32/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.509956 xbrl-us-0.0.32/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     3400 2023-07-14 19:39:33.000000 xbrl-us-0.0.32/.github/workflows/github-actions.yml
--rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.32/.pre-commit-config.yaml
--rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.32/.readthedocs.yml
--rw-r--r--   0 hamid      (501) staff       (20)       71 2023-07-06 22:38:13.000000 xbrl-us-0.0.32/AUTHORS.rst
--rw-r--r--   0 hamid      (501) staff       (20)      694 2023-07-17 21:31:18.000000 xbrl-us-0.0.32/CHANGELOG.rst
--rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/CONTRIBUTING.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.32/LICENSE
--rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.32/MANIFEST.in
--rw-r--r--   0 hamid      (501) staff       (20)    13345 2023-07-17 21:31:46.555944 xbrl-us-0.0.32/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)    11286 2023-07-17 21:18:39.000000 xbrl-us-0.0.32/README.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.510751 xbrl-us-0.0.32/ci/
--rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/ci/bootstrap.py
--rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/ci/requirements.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.502553 xbrl-us-0.0.32/ci/templates/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.502663 xbrl-us-0.0.32/ci/templates/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.511228 xbrl-us-0.0.32/ci/templates/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.515162 xbrl-us-0.0.32/docs/
--rw-r--r--   0 hamid      (501) staff       (20)       28 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/docs/authors.rst
--rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/docs/changelog.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1156 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/docs/conf.py
--rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/docs/contributing.rst
--rw-r--r--   0 hamid      (501) staff       (20)      219 2023-07-09 12:54:31.000000 xbrl-us-0.0.32/docs/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)    10210 2023-07-16 13:55:28.000000 xbrl-us-0.0.32/docs/readme.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.516410 xbrl-us-0.0.32/docs/reference/
--rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.32/docs/reference/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.32/docs/reference/xbrl_us.rst
--rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.32/docs/requirements.txt
--rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/docs/spelling_wordlist.txt
--rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.32/pyproject.toml
--rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/pytest.ini
--rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.32/secrets.yml
--rw-r--r--   0 hamid      (501) staff       (20)       38 2023-07-17 21:31:46.556721 xbrl-us-0.0.32/setup.cfg
--rwxr-xr-x   0 hamid      (501) staff       (20)     3004 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/setup.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.503352 xbrl-us-0.0.32/src/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.519187 xbrl-us-0.0.32/src/xbrl_us/
--rw-r--r--   0 hamid      (501) staff       (20)       70 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/src/xbrl_us/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.32/src/xbrl_us/__main__.py
--rw-r--r--   0 hamid      (501) staff       (20)    16235 2023-07-15 18:40:11.000000 xbrl-us-0.0.32/src/xbrl_us/app.py
--rw-r--r--   0 hamid      (501) staff       (20)      373 2023-07-12 22:49:38.000000 xbrl-us-0.0.32/src/xbrl_us/cli.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.544228 xbrl-us-0.0.32/src/xbrl_us/methods/
--rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.32/src/xbrl_us/methods/assertion search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.32/src/xbrl_us/methods/assertion validate.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.32/src/xbrl_us/methods/concept name search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.32/src/xbrl_us/methods/concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/cube search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dimension search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/document search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept label.yml
--rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept name.yml
--rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept reference.yml
--rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id network search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id network.yml
--rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/entity id report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/entity id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/entity report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/entity search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.32/src/xbrl_us/methods/fact id.yml
--rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.32/src/xbrl_us/methods/fact search oim.yml
--rw-r--r--   0 hamid      (501) staff       (20)     9377 2023-07-15 18:41:16.000000 xbrl-us-0.0.32/src/xbrl_us/methods/fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/label dts id search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/label search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/network id relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/network id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/network relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/relationship tree search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report id delete.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report id fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report search.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.552208 xbrl-us-0.0.32/src/xbrl_us/schemas/
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/assertion_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/concept_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/cube_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/dimension_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/document_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/dts_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/entity_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/fact_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/label_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/network_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/relationship_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/report_details.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.554423 xbrl-us-0.0.32/src/xbrl_us/utils/
--rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.32/src/xbrl_us/utils/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)     1633 2023-07-16 19:19:32.000000 xbrl-us-0.0.32/src/xbrl_us/utils/exceptions.py
--rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.32/src/xbrl_us/utils/fields.py
--rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.32/src/xbrl_us/utils/paramters.py
--rw-r--r--   0 hamid      (501) staff       (20)    26901 2023-07-17 21:18:39.000000 xbrl-us-0.0.32/src/xbrl_us/xbrl_us.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.522855 xbrl-us-0.0.32/src/xbrl_us.egg-info/
--rw-r--r--   0 hamid      (501) staff       (20)    13345 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     2927 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/SOURCES.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/dependency_links.txt
--rw-r--r--   0 hamid      (501) staff       (20)       45 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/entry_points.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-14 20:24:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/not-zip-safe
--rw-r--r--   0 hamid      (501) staff       (20)      103 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/requires.txt
--rw-r--r--   0 hamid      (501) staff       (20)        8 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/top_level.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.555143 xbrl-us-0.0.32/tests/
--rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.32/tests/test_xbrl_us.py
--rw-r--r--   0 hamid      (501) staff       (20)     1486 2023-07-14 19:43:01.000000 xbrl-us-0.0.32/tox.ini
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.696681 xbrl-us-0.0.4/
+-rw-r--r--   0 hamid      (501) staff       (20)      527 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/.bumpversion.cfg
+-rw-r--r--   0 hamid      (501) staff       (20)     2015 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/.cookiecutterrc
+-rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/.coveragerc
+-rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/.editorconfig
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.620024 xbrl-us-0.0.4/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.630222 xbrl-us-0.0.4/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     3400 2023-07-14 19:39:33.000000 xbrl-us-0.0.4/.github/workflows/github-actions.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.4/.readthedocs.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      694 2023-07-17 21:31:18.000000 xbrl-us-0.0.4/CHANGELOG.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.4/LICENSE
+-rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.4/MANIFEST.in
+-rw-r--r--   0 hamid      (501) staff       (20)    13638 2023-08-04 02:01:25.696011 xbrl-us-0.0.4/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)    11606 2023-07-18 17:14:45.000000 xbrl-us-0.0.4/README.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.631184 xbrl-us-0.0.4/ci/
+-rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/ci/bootstrap.py
+-rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/ci/requirements.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.620423 xbrl-us-0.0.4/ci/templates/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.620524 xbrl-us-0.0.4/ci/templates/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.631586 xbrl-us-0.0.4/ci/templates/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.634965 xbrl-us-0.0.4/docs/
+-rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/docs/changelog.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1155 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/docs/conf.py
+-rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/docs/contributing.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      208 2023-07-17 22:11:31.000000 xbrl-us-0.0.4/docs/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)    10882 2023-07-19 13:02:53.000000 xbrl-us-0.0.4/docs/readme.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.635890 xbrl-us-0.0.4/docs/reference/
+-rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.4/docs/reference/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.4/docs/reference/xbrl_us.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.4/docs/requirements.txt
+-rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/docs/spelling_wordlist.txt
+-rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.4/pyproject.toml
+-rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.4/pytest.ini
+-rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.4/secrets.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       38 2023-08-04 02:01:25.696879 xbrl-us-0.0.4/setup.cfg
+-rwxr-xr-x   0 hamid      (501) staff       (20)     3003 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/setup.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.621503 xbrl-us-0.0.4/src/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.639941 xbrl-us-0.0.4/src/xbrl_us/
+-rw-r--r--   0 hamid      (501) staff       (20)       69 2023-08-04 02:00:49.000000 xbrl-us-0.0.4/src/xbrl_us/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.4/src/xbrl_us/__main__.py
+-rw-r--r--   0 hamid      (501) staff       (20)    17831 2023-08-04 00:05:41.000000 xbrl-us-0.0.4/src/xbrl_us/app.py
+-rw-r--r--   0 hamid      (501) staff       (20)      373 2023-08-03 21:05:17.000000 xbrl-us-0.0.4/src/xbrl_us/cli.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.669978 xbrl-us-0.0.4/src/xbrl_us/methods/
+-rw-r--r--   0 hamid      (501) staff       (20)    12479 2023-08-04 01:52:45.000000 xbrl-us-0.0.4/src/xbrl_us/methods/_definitions.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.4/src/xbrl_us/methods/assertion search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.4/src/xbrl_us/methods/assertion validate.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.4/src/xbrl_us/methods/concept name search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.4/src/xbrl_us/methods/concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/cube search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dimension search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/document search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept label.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept name.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept reference.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id network search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts id network.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/dts search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/entity id report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/entity id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/entity report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/entity search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.4/src/xbrl_us/methods/fact id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.4/src/xbrl_us/methods/fact search oim.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     3002 2023-08-04 00:06:26.000000 xbrl-us-0.0.4/src/xbrl_us/methods/fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/label dts id search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/label search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/network id relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/network id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/network relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.4/src/xbrl_us/methods/relationship tree search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report id delete.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report id fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.4/src/xbrl_us/methods/report search.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.685848 xbrl-us-0.0.4/src/xbrl_us/schemas/
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/assertion_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/concept_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/cube_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/dimension_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/document_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/dts_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/entity_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/fact_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/label_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/network_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/relationship_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.4/src/xbrl_us/schemas/report_details.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.692767 xbrl-us-0.0.4/src/xbrl_us/utils/
+-rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.4/src/xbrl_us/utils/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1633 2023-07-16 19:19:32.000000 xbrl-us-0.0.4/src/xbrl_us/utils/exceptions.py
+-rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.4/src/xbrl_us/utils/fields.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.4/src/xbrl_us/utils/paramters.py
+-rw-r--r--   0 hamid      (501) staff       (20)    30836 2023-08-04 01:53:19.000000 xbrl-us-0.0.4/src/xbrl_us/xbrl_us.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.645747 xbrl-us-0.0.4/src/xbrl_us.egg-info/
+-rw-r--r--   0 hamid      (501) staff       (20)    13638 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)     2936 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/SOURCES.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/dependency_links.txt
+-rw-r--r--   0 hamid      (501) staff       (20)       45 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/entry_points.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-08-03 23:15:34.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/not-zip-safe
+-rw-r--r--   0 hamid      (501) staff       (20)      103 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/requires.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        8 2023-08-04 02:01:25.000000 xbrl-us-0.0.4/src/xbrl_us.egg-info/top_level.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-08-04 02:01:25.694987 xbrl-us-0.0.4/tests/
+-rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.4/tests/test_xbrl_us.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1486 2023-07-14 19:43:01.000000 xbrl-us-0.0.4/tox.ini
```

### Comparing `xbrl-us-0.0.32/.bumpversion.cfg` & `xbrl-us-0.0.4/.bumpversion.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.32
+current_version = 0.0.4
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `xbrl-us-0.0.32/.cookiecutterrc` & `xbrl-us-0.0.4/.cookiecutterrc`

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
-    version: "0.0.32"
+    version: "0.0.4"
     version_manager: "bump2version"
     website: "https://hamidvakilzadeh.com"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `xbrl-us-0.0.32/.github/workflows/github-actions.yml` & `xbrl-us-0.0.4/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/.pre-commit-config.yaml` & `xbrl-us-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/CHANGELOG.rst` & `xbrl-us-0.0.4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/CONTRIBUTING.rst` & `xbrl-us-0.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/LICENSE` & `xbrl-us-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/PKG-INFO` & `xbrl-us-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.32
+Version: 0.0.4
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
@@ -24,15 +24,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-License-File: AUTHORS.rst
 
 ======================
 XBRL-US Python Library
 ======================
 
 |Workflow| |Docs| |license| |Versions|
 
@@ -109,14 +108,20 @@
 
 You can install this package using pip:
 
 .. code-block:: bash
 
     pip install xbrl-us
 
+If you are using Jupyter Notebook, you can install the package using the following command:
+
+.. code-block:: bash
+
+    !pip install xbrl-us
+
 .. caution::
 
         The XBRL US Python Wrapper is currently in beta and is subject to change.
         We welcome your feedback and suggestions for improvement.
         Please submit any issues or feature requests to
         the `GitHub repository <https://github.com/hamid-vakilzadeh/python-xbrl-us/issues>`_.
 
@@ -337,21 +342,32 @@
 Getting started is as simple as ever.
 First, ensure you have the latest version of ``xbrl-us`` installed by running the following code:
 
 .. code-block:: bash
 
     pip install xbrl-us --upgrade
 
+or if you are on a Jupyter Notebook:
+
+.. code-block:: bash
+
+    !pip install xbrl-us --upgrade
 
 Next, launch the new Browser Interface from the package menu:
 
 .. code-block:: bash
 
     python -m xbrl_us
 
+or if you are on a Jupyter Notebook:
+
+.. code-block:: bash
+
+    !python -m xbrl_us
+
 That is it!
 You should now see the new Browser Interface open in your default web browser.
 
 Happy data exploring!
 
 .. note::
```

### Comparing `xbrl-us-0.0.32/README.rst` & `xbrl-us-0.0.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,20 @@
 
 You can install this package using pip:
 
 .. code-block:: bash
 
     pip install xbrl-us
 
+If you are using Jupyter Notebook, you can install the package using the following command:
+
+.. code-block:: bash
+
+    !pip install xbrl-us
+
 .. caution::
 
         The XBRL US Python Wrapper is currently in beta and is subject to change.
         We welcome your feedback and suggestions for improvement.
         Please submit any issues or feature requests to
         the `GitHub repository <https://github.com/hamid-vakilzadeh/python-xbrl-us/issues>`_.
 
@@ -305,21 +311,32 @@
 Getting started is as simple as ever.
 First, ensure you have the latest version of ``xbrl-us`` installed by running the following code:
 
 .. code-block:: bash
 
     pip install xbrl-us --upgrade
 
+or if you are on a Jupyter Notebook:
+
+.. code-block:: bash
+
+    !pip install xbrl-us --upgrade
 
 Next, launch the new Browser Interface from the package menu:
 
 .. code-block:: bash
 
     python -m xbrl_us
 
+or if you are on a Jupyter Notebook:
+
+.. code-block:: bash
+
+    !python -m xbrl_us
+
 That is it!
 You should now see the new Browser Interface open in your default web browser.
 
 Happy data exploring!
 
 .. note::
```

### Comparing `xbrl-us-0.0.32/ci/bootstrap.py` & `xbrl-us-0.0.4/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/ci/templates/.github/workflows/github-actions.yml` & `xbrl-us-0.0.4/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/docs/conf.py` & `xbrl-us-0.0.4/docs/conf.py`

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
-version = release = "0.0.32"
+version = release = "0.0.4"
 
 pygments_style = "emacs"
 highlight_language = "python"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/issues/%s", "#"),
     "pr": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/pull/%s", "PR #"),
```

### Comparing `xbrl-us-0.0.32/docs/readme.rst` & `xbrl-us-0.0.4/docs/readme.rst`

 * *Files 6% similar despite different names*

```diff
@@ -51,17 +51,29 @@
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/.
 * **XBRL-US OAuth2 Access**.
   You can obtain your client ID and client secret by registering for a
   filling the request form at https://xbrl.us/home/use/xbrl-api/access-token/.
 
 You can install this package using pip:
 
-.. code-block:: bash
+.. list-table::
+    :widths: 30 70
+    :stub-columns: 1
 
-    pip install xbrl-us
+    * - Command Line
+      - .. code-block:: bash
+
+            pip install xbrl-us
+
+    * - Jupyter Notebook
+      - .. code-block:: bash
+
+            !pip install xbrl-us
+
+If ``!`` does not work in Jupyter Notebook, use ``%`` instead.
 
 .. caution::
 
         The XBRL US Python Wrapper is currently in beta and is subject to change.
         We welcome your feedback and suggestions for improvement.
         Please submit any issues or feature requests to
         the `GitHub repository <https://github.com/hamid-vakilzadeh/python-xbrl-us/issues>`_.
@@ -279,24 +291,43 @@
 
 Getting Started with the Browser Interface
 ------------------------------------------
 
 Getting started is as simple as ever.
 First, ensure you have the latest version of ``xbrl-us`` installed by running the following code:
 
-.. code-block:: bash
+.. list-table::
+    :widths: 30 70
+    :stub-columns: 1
+
+    * - Command Line
+      - .. code-block:: bash
+
+            pip install xbrl-us --upgrade
+
+    * - Jupyter Notebook
+      - .. code-block:: bash
+
+            !pip install xbrl-us --upgrade
+
+Next, launch the new Browser Interface from the package menu from the command line by running the following code:
 
-    pip install xbrl-us --upgrade
+.. list-table::
+    :widths: 30 70
+    :stub-columns: 1
 
+    * - Command Line
+      - .. code-block:: bash
 
-Next, launch the new Browser Interface from the package menu:
+            python -m xbrl_us
 
-.. code-block:: bash
+    * - Jupyter Notebook
+      - .. code-block:: bash
 
-    python -m xbrl_us
+            !python -m xbrl_us
 
 That is it!
 You should now see the new Browser Interface open in your default web browser.
 
 Happy data exploring!
 
 .. note::
```

### Comparing `xbrl-us-0.0.32/pyproject.toml` & `xbrl-us-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/pytest.ini` & `xbrl-us-0.0.4/pytest.ini`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/setup.py` & `xbrl-us-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="xbrl-us",
-    version="0.0.32",
+    version="0.0.4",
     license="MIT",
     description="Python wrapper for xbrl.us API",
     long_description_content_type="text/x-rst",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
@@ -62,15 +62,15 @@
         # eg: "xbrl-us", "xbrl", "sec",
     ],
     python_requires=">=3.8",
     install_requires=[
         "requests>=2.25.1",
         "pandas>= 1.3.0, < 3",
         "PyYAML>=5.3",
-        "streamlit>=1.24.0",
+        "streamlit>=1.25.0",
         "retry>=0.9.2",
         "tqdm>=4.61.2",
         "stqdm>=0.0.5",
     ],
     extras_require={
         # eg:
         #   "rst": ["docutils>=0.11"],
```

### Comparing `xbrl-us-0.0.32/src/xbrl_us/app.py` & `xbrl-us-0.0.4/src/xbrl_us/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+from pathlib import Path
+
 import streamlit as st
 
 from xbrl_us import XBRL
 
+user_info_path = Path.home() / ".xbrl-us"
+
 
-def try_credentials(user_name: str, pass_word: str, client_id: str, client_secret: str):
+def try_credentials(user_name: str, pass_word: str, client_id: str, client_secret: str, store: bool = False):
     try:
+        if store:
+            store = "y"
+        else:
+            store = "n"
         with st.spinner(text="Validating credentials..."):
-            XBRL(username=user_name, password=pass_word, client_id=client_id, client_secret=client_secret)._get_token()
+            XBRL(username=user_name, password=pass_word, client_id=client_id, client_secret=client_secret)._get_token(store=store)
             st.session_state.username = user_name
             st.session_state.password = pass_word
             st.session_state.client_id = client_id
             st.session_state.client_secret = client_secret
     except Exception as e:
         st.error(f"Invalid credentials. Please try again. {e}")
         st.stop()
@@ -54,27 +62,35 @@
 
     client_secret = st.text_input(
         "Client Secret",
         type="password",
         help="Your client secret for the [XBRL.US](https://www.xbrl.us) API.",
     )
 
+    # checkbox for remember me
+    remember_me = st.checkbox(
+        label="Remember me",
+        value=False,
+        key="remember_me",
+    )
+
     disable_login_btn = False
     if username == "" or password == "" or client_id == "" or client_secret == "":
         disable_login_btn = True
 
     verify_api = st.button(
         label="Create a New Session",
         type="primary",
         use_container_width=True,
         disabled=disable_login_btn,
     )
+
     if verify_api:
         # try the credentials before creating xbrl object
-        try_credentials(user_name=username, pass_word=password, client_id=client_id, client_secret=client_secret)
+        try_credentials(user_name=username, pass_word=password, client_id=client_id, client_secret=client_secret, store=remember_me)
         st.experimental_rerun()
 
 
 def input_number_for_integers(key):
     st.number_input(
         label=f"Input **{key}**:",
         value=0,
@@ -156,45 +172,63 @@
             label=f"{key}",
             options=list(range(values["min"], values["max"])),
             key=f"{key}",
             label_visibility="collapsed",
         )
 
 
-def text_box_for_array_strings_no_ops(key):
+def text_box_for_array_strings_no_ops(key, palceholder):
     st.text_area(
         label=f"**{key}**",
+        placeholder=f"{palceholder}",
         key=f"{key}",
     )
 
 
+def restart_everything():
+    st.session_state.clear()
+    st.session_state.update({"returning_user": False})
+
+
 if __name__ == "__main__":
     st.set_page_config(
         page_title="XBRL.US API Explorer",
         page_icon="📄",
         layout="centered",
         initial_sidebar_state="expanded",
     )
 
     st.title("Explore XBRL.us Data")
 
     sidebar = st.sidebar
+    if user_info_path.exists():
+        if "returning_user" not in st.session_state:
+            st.session_state.returning_user = True
+            temp_xbrl = XBRL()
+            # show button to continue with the username
+            st.session_state.username = temp_xbrl.username
+            st.session_state.password = temp_xbrl.password
+            st.session_state.client_id = temp_xbrl.client_id
+            st.session_state.client_secret = temp_xbrl.client_secret
+
     if "username" not in st.session_state:
         st.error("Please enter your credentials to begin.")
 
         with sidebar:
+            st.success(f"Logged in as {st.session_state.username}")
             show_login()
         st.stop()
     else:
         with sidebar:
+            st.success(f"Logged in as {st.session_state.username}")
             st.button(
                 label="Log out",
                 type="secondary",
                 use_container_width=True,
-                on_click=lambda: st.session_state.clear(),
+                on_click=lambda: restart_everything(),
                 key="logout",
             )
 
         xbrl = XBRL(
             username=st.session_state.username,
             password=st.session_state.password,
             client_id=st.session_state.client_id,
@@ -215,17 +249,35 @@
         )
 
         # get the acceptable parameters for the method
         st.session_state.method_params = xbrl.acceptable_params(method)
         # parameters_options = dict(sorted(method_params.parameters.items(), key=lambda x: x[1]['type']))
         # print the name of the method
         st.header(method)
-        st.markdown(st.session_state.method_params.description)
-        st.caption(f"**API end-point**: {xbrl.acceptable_params(method).url}")
-        # print the url of the method
+
+        # two tabs
+        method_summary, definitions = st.tabs(["Summary", "Search Definitions"])
+
+        with method_summary:
+            st.markdown(st.session_state.method_params.description)
+            st.markdown(
+                f"{st.session_state.method_params.long_description} <sup>[1]({st.session_state.method_params.reference})</sup>",
+                unsafe_allow_html=True,
+            )
+            st.markdown(f"**Glossary**: {st.session_state.method_params.reference}")
+            st.caption(f"**API end-point**: {xbrl.acceptable_params(method).url}")
+            # print the url of the method
+
+        with definitions:
+            with st.expander("Search Definitions", expanded=True):
+                if "fields" in st.session_state and len(st.session_state.fields) > 0:
+                    st.markdown(f"**Field Name**: *{st.session_state.fields[-1]}*")
+                    st.markdown(f"**Description**: {xbrl.define(st.session_state.fields[-1])['description']}")
+                else:
+                    st.info("Select a field to see the definition")
 
         # show the list of fields in the sidebar
         with st.container():
             sidebar.multiselect(
                 label="Fields :red[*]",
                 options=st.session_state.method_params.fields,
                 key="fields",
@@ -303,33 +355,38 @@
                         key=f"{field}_sort",
                     )
                     st.session_state.sort_params[field] = "asc" if sort_order == "Ascending" else "desc"
                 st.markdown("---")
 
             for param in st.session_state.parameters:
                 st.subheader(f"**{param}**:")
-                st.write(st.session_state.method_params.parameters[param]["description"])
+                param_info = xbrl.define(param)
+                st.markdown(param_info["description"])
+                type = param_info["type"]
 
-                if st.session_state.method_params.parameters[param]["type"] == "boolean":
+                if type == "boolean":
                     boolean_input_for_booleans(param)
 
-                elif st.session_state.method_params.parameters[param]["type"] == "integer":
+                elif type == "integer":
                     input_number_for_integers(param)
 
-                elif st.session_state.method_params.parameters[param]["type"] == "string":
+                elif type == "string":
                     text_input_for_strings(param)
 
-                elif st.session_state.method_params.parameters[param]["type"] == "array[integer]":
+                elif type == "array[integer]":
                     range_and_slider_for_array_integers(
                         param,
-                        st.session_state.method_params.parameters[param]["values"],
+                        param_info["values"],
                     )
 
-                elif st.session_state.method_params.parameters[param]["type"] == "array[string]":
-                    text_box_for_array_strings_no_ops(param)
+                elif type == "array[string]":
+                    text_box_for_array_strings_no_ops(
+                        param,
+                        param_info["placeholder"],
+                    )
 
             st.session_state.query_params = {"fields": st.session_state.fields}
 
             if len(st.session_state.parameters) > 0:
                 st.session_state.query_params["parameters"] = {}
                 for param in st.session_state.parameters:
                     st.session_state.query_params["parameters"][param] = st.session_state[param]
@@ -365,25 +422,19 @@
     )
     new_results_placeholder = st.empty()
     if st.session_state.run_query:
         try:
             with st.spinner("Running query..."):
                 st.session_state.pop("last_query", None)
                 st.session_state.last_query = xbrl.query(
-                    **st.session_state.query_params, as_dataframe=True, print_query=True, streamlit=True
+                    **st.session_state.query_params, as_dataframe=True, print_query=True, streamlit=True, timeout=10
                 )
 
         except Exception as e:
-            new_results_placeholder.warning(
-                f"Your query is taking a long time... \n"
-                f"The server may still be working on this query. "
-                f"You can wait and try again in a few minutes. "
-                f"Or try narrowing your search criteria. \n"
-                f"\n {e}"
-            )
+            new_results_placeholder.error(f"{e}")
             st.stop()
 
     with new_results_placeholder.container():
         # show the dataframe
         st.subheader("Last Query Results")
         if "last_query" not in st.session_state:
             st.info("No **Query** has been run yet.")
```

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/assertion search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/assertion search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/concept name search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/concept name search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/concept search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/cube search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/cube search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/dimension search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/dimension search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/document search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/document search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept name.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept name.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept reference.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept reference.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/dts id concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/dts id network search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/dts id network search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/dts id network.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/dts id network.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/dts search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/dts search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/entity id report search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/entity id report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/entity report search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/entity report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/fact id.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/fact id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/fact search oim.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/fact search oim.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/label dts id search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/label dts id search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/network id relationship search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/network id relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/network relationship search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/network relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/relationship search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/relationship tree search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/relationship tree search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/report fact search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/report fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/report id fact search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/report id fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/report id.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/report id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/methods/report search.yml` & `xbrl-us-0.0.4/src/xbrl_us/methods/report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/schemas/concept_details.py` & `xbrl-us-0.0.4/src/xbrl_us/schemas/concept_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/schemas/dimension_details.py` & `xbrl-us-0.0.4/src/xbrl_us/schemas/dimension_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/utils/exceptions.py` & `xbrl-us-0.0.4/src/xbrl_us/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/utils/paramters.py` & `xbrl-us-0.0.4/src/xbrl_us/utils/paramters.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/src/xbrl_us/xbrl_us.py` & `xbrl-us-0.0.4/src/xbrl_us/xbrl_us.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,42 @@
 from retry import retry
 from tqdm import tqdm
 from yaml import safe_load
 
 from .utils import Parameters
 from .utils import exceptions
 
-logging.basicConfig()
-
 _dir = Path(__file__).resolve()
 
+# Get the home directory path as a Path object
+_home_directory = Path.home()
+
+# Join the home directory path with the file name to get the full file path
+user_info_path = _home_directory / ".xbrl-us"
+
+
+# logging.basicConfig()
+class OneTimeWarningFilter(logging.Filter):
+    def __init__(self):
+        super().__init__()
+        self.msgs = set()
+
+    def filter(self, record):
+        if record.msg not in self.msgs:
+            self.msgs.add(record.msg)
+            return True
+        return False
+
+
+logger = logging.getLogger(__name__)
+handler = logging.StreamHandler()
+handler.addFilter(OneTimeWarningFilter())
+logger.addHandler(handler)
+logger.setLevel(logging.WARNING)
+
 
 def _remove_special_fields(fields):
     # Define the patterns to be removed
     patterns = [r"(.+)\.(sort\((.+)\))?$", r"(.+)\.(limit\((\d+)\))?$", r"(.+)\.(offset\((\d+)\))?$"]
 
     # For each field, check if it matches any of the patterns. If it does, remove it.
     for field in fields[:]:  # iterate over a slice copy of the list to safely modify it during iteration
@@ -83,15 +107,15 @@
             fields = kwargs.get("fields")
             limit = kwargs.get("limit")
             sort = kwargs.get("sort")
             offset = kwargs.get("offset")
             kwargs.get("print_query")
 
             # get the allowed parameters, fields, limit, sort, and offset from the yaml file
-            allowed_params = list(allowed_for_query.get("parameters", set()).keys())
+            allowed_params = allowed_for_query.get("parameters", set())
             allowed_fields = allowed_for_query.get("fields", set())
             allowed_limit_fields = allowed_for_query.get("limit", set())
             allowed_sort_fields = [field for field in allowed_fields if "*" not in field]
             allowed_offset_fields = allowed_limit_fields
 
             # Validate fields
             if not fields:
@@ -119,17 +143,17 @@
             # Validate limit
             if limit:
                 # if not dict or an int, raise an error
                 if not isinstance(limit, int):
                     raise exceptions.XBRLInvalidTypeError(key=limit, expected_type=int, received_type=type(limit))
 
             else:
-                warnings.warn(
-                    "You have not set a limit; returning the first page only.",
-                    UserWarning,
+                logger.warning(
+                    "No limit set: this will automatically limit the number of results to your account limit."
+                    " if you want more results, set the limit.",
                     stacklevel=2,
                 )
 
             # Validate sort
             if sort:
                 if not isinstance(sort, dict):
                     raise ValueError("Sort must be a dictionary")
@@ -138,17 +162,16 @@
                     if key not in allowed_sort_fields:
                         raise exceptions.XBRLInvalidValueError(
                             key=key, param="sort", expected_value=allowed_sort_fields, method=method_name
                         )
                     if value.lower() not in ["asc", "desc"]:
                         raise exceptions.XBRLInvalidValueError(key=value, param="sort", expected_value=["asc", "desc"])
             else:
-                warnings.warn(
-                    "You have not passed a sort value; for reliable results, set a field to sort.",
-                    UserWarning,
+                logger.warning(
+                    "No sort field: It is recommended to sort by a field for reliable results.",
                     stacklevel=2,
                 )
 
             # Validate offset
             if offset:
                 if not isinstance(offset, int):
                     raise exceptions.XBRLInvalidTypeError(key=offset, expected_type=int, received_type=type(offset))
@@ -221,50 +244,53 @@
         offset_field (str): The offset field accepted for the chosen method (which is usually the same as the
             ``limit_filed``).
 
     Returns:
         dict: The query parameters that will be submitted to the API.
     """
     query_params = {}
+    fields_copy = fields[:]
 
     if parameters:
         # convert the parameters to a string and add it to the query_params
         query_params.update(
             {f"{k}": ",".join(map(str, v)) if isinstance(v, Iterable) and not isinstance(v, str) else str(v) for k, v in parameters.items()}
         )
 
     # Handle sort
     if sort:
+        sort_copy = dict(sort)
+
         # check if the sort field is in the fields list
-        for field, direction in sort.items():
+        for field, direction in sort_copy.items():
             # name the field name followed by .sort(value)
             sorted_arg = f"{field}.sort({direction.upper()})"
-            if field in fields:
+            if field in fields_copy:
                 # if the field is in the fields list, remove the field
-                fields.remove(field)
-            fields.append(sorted_arg)
+                fields_copy.remove(field)
+            fields_copy.append(sorted_arg)
 
     # Handle limit
     if limit:
         # name and add the field name followed by .limit(value)
         limit_arg = f"{limit_field}.limit({limit})"
-        if limit_field in fields:
+        if limit_field in fields_copy:
             # if the field is in the fields list, remove the field
-            fields.remove(limit_field)
-        fields.append(limit_arg)
+            fields_copy.remove(limit_field)
+        fields_copy.append(limit_arg)
 
     # Handle offset
     if offset:
         # name and add the field name followed by .offset(value)
         offset_arg = f"{offset_field}.offset({offset})"
-        if offset_field in fields:
-            fields.remove(offset_field)
-        fields.append(offset_arg)
+        if offset_field in fields_copy:
+            fields_copy.remove(offset_field)
+        fields_copy.append(offset_arg)
 
-    query_params["fields"] = ",".join(fields)
+    query_params["fields"] = ",".join(fields_copy)
 
     return query_params
 
 
 class XBRL:
     """
     XBRL US API client. Initializes an instance of XBRL authorized connection.
@@ -281,107 +307,130 @@
             * default - "password"
     """
 
     _query_exceptions = (requests.exceptions.ConnectionError, requests.exceptions.Timeout, requests.exceptions.ReadTimeout)
 
     def __init__(
         self,
-        client_id: str,
-        client_secret: str,
-        username: str,
-        password: str,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
         grant_type: str = "password",
     ):
         self._url = "https://api.xbrl.us/oauth2/token"
         self.client_id = client_id
         self.client_secret = client_secret
         self.username = username
         self.password = password
         self.grant_type = grant_type
         self.access_token = None
         self.refresh_token = None
         self.account_limit = None
         self._access_token_expires_at = 0
         self._refresh_token_expires_at = 0
 
+        # If the class was initiated without any arguments, try finding the user info file
+        if not (client_id and client_secret and username and password):
+            self._get_user()
+
     @staticmethod
     def methods():
         """
-        Get the names of the attributes that are allowed to be used for
-            the given method. A list of available methods are:
+        Get the names of the methods that are allowed to be used for
+            as a ``method`` name. A list of available methods along with
+            their corresponding API endpoints is shown below.
 
             ===================================  ==================================================
             Method                               API Endpoint
             ===================================  ==================================================
-            ``assertion search``                  ``/api/v1/assertion/search``
-            ``assertion validate``                ``/api/v1/assertion/validate``
-            ``concept name search``               ``/api/v1/concept/{concept.local-name}/search``
-            ``concept search``                    ``/api/v1/concept/search``
-            ``cube search``                       ``/api/v1/cube/search``
-            ``dimension search``                  ``/api/v1/dimension/search``
-            ``document search``                   ``/api/v1/document/search``
-            ``dts id concept label``              ``/api/v1/dts/{dts.id}/concept/{concept.local-name}/label``
-            ``dts id concept name``               ``/api/v1/dts/{dts.id}/concept/{concept.local-name}``
-            ``dts id concept reference``          ``/api/v1/dts/{dts.id}/concept/{concept.local-name}/reference``
-            ``dts id concept search``             ``/api/v1/dts/{dts.id}/concept/search``
-            ``dts id network``                    ``/api/v1/dts/{dts.id}/network``
-            ``dts id network search``             ``/api/v1/dts/{dts.id}/network/search``
-            ``dts search``                        ``/api/v1/dts/search``
-            ``entity id``                         ``/api/v1/entity/{entity.id}``
-            ``entity id report search``           ``/api/v1/entity/{entity.id}/report/search``
-            ``entity report search``              ``/api/v1/entity/report/search``
-            ``entity search``                     ``/api/v1/entity/search``
-            ``fact id``                           ``/api/v1/fact/{fact.id}``
-            ``fact search``                       ``/api/v1/fact/search``
-            ``fact search oim``                   ``/api/v1/fact/oim/search``
-            ``label dts id search``               ``/api/v1/label/{dts.id}/search``
-            ``label search``                      ``/api/v1/label/search``
-            ``network id``                        ``/api/v1/network/{network.id}``
-            ``network id relationship search``    ``/api/v1/network/{network.id}/relationship/search``
-            ``network relationship search``       ``/api/v1/network/relationship/search``
-            ``relationship search``               ``/api/v1/relationship/search``
-            ``relationship tree search``          ``/api/v1/relationship/tree/search``
-            ``report fact search``                ``/api/v1/report/fact/search``
-            ``report id``                         ``/api/v1/report/{report.id}``
-            ``report id delete``                  ``/api/v1/report/{report.id}/delete``
-            ``report id fact``                    ``/api/v1/report/{report.id}/fact/search``
-            ``report search``                     ``/api/v1/report/search``
+            ``assertion search``                  */api/v1/assertion/search*
+            ``concept name search``               */api/v1/concept/{concept.local-name}/search*
+            ``concept search``                    */api/v1/concept/search*
+            ``cube search``                       */api/v1/cube/search*
+            ``dimension search``                  */api/v1/dimension/search*
+            ``document search``                   */api/v1/document/search*
+            ``dts id concept label``              */api/v1/dts/{dts.id}/concept/{concept.local-name}/label*
+            ``dts id concept name``               */api/v1/dts/{dts.id}/concept/{concept.local-name}*
+            ``dts id concept reference``          */api/v1/dts/{dts.id}/concept/{concept.local-name}/reference*
+            ``dts id concept search``             */api/v1/dts/{dts.id}/concept/search*
+            ``dts id network``                    */api/v1/dts/{dts.id}/network*
+            ``dts id network search``             */api/v1/dts/{dts.id}/network/search*
+            ``dts search``                        */api/v1/dts/search*
+            ``entity id``                         */api/v1/entity/{entity.id}*
+            ``entity id report search``           */api/v1/entity/{entity.id}/report/search*
+            ``entity report search``              */api/v1/entity/report/search*
+            ``entity search``                     */api/v1/entity/search*
+            ``fact id``                           */api/v1/fact/{fact.id}*
+            ``fact search``                       */api/v1/fact/search*
+            ``fact search oim``                   */api/v1/fact/oim/search*
+            ``label dts id search``               */api/v1/label/{dts.id}/search*
+            ``label search``                      */api/v1/label/search*
+            ``network id``                        */api/v1/network/{network.id}*
+            ``network id relationship search``    */api/v1/network/{network.id}/relationship/search*
+            ``network relationship search``       */api/v1/network/relationship/search*
+            ``relationship search``               */api/v1/relationship/search*
+            ``relationship tree search``          */api/v1/relationship/tree/search*
+            ``report fact search``                */api/v1/report/fact/search*
+            ``report id``                         */api/v1/report/{report.id}*
+            ``report id fact search``             */api/v1/report/{report.id}/fact/search*
+            ``report search``                     */api/v1/report/search*
             ===================================  ==================================================
 
         """
+        # TODO: add support for report delete, assertion validate,
         return _methods()
 
     @staticmethod
-    def acceptable_params(method_name: str):
+    def acceptable_params(method: str):
         """
-        Get the names of the attributes that are allowed to be used for
-            the given method.
+        Get the names of the attributes (e.g. acceptable ``fields``, ``parameters``, ``sort``, ``limit``, etc.)
+            that are allowed to be used for a given ``method``.
 
         Args:
-            method_name (str): The name of the API method to get the acceptable parameters for (e.g. "search_fact").
+            method (str): The name of the API method to get the acceptable parameters for (e.g. "fact search").
 
         Returns:
+            A class where the attributes are the acceptable parameters for the given ``method``.
 
         """
-        file_path = _dir.parent / "methods" / f"{method_name.lower()}.yml"
+        file_path = _dir.parent / "methods" / f"{method.lower()}.yml"
 
         with file_path.open("r") as file:
             method_features = safe_load(file)
 
-        _attributes = {"method_name": method_name}
+        _attributes = {"method_name": method}
         for key, _value in method_features.items():
             _attributes[f"{key}"] = method_features.get(key)
 
         _attributes["sort"] = [value for value in _attributes["fields"] if "*" not in value]
 
         # Create the dynamic class using type()
-        _class = type(method_name, (), _attributes)
+        _class = type(method, (), _attributes)
         return _class()
 
-    def _get_token(self, grant_type: Optional[str] = None, refresh_token=None):
+    @staticmethod
+    def define(parameter: str):
+        """
+        Get the definition of any parameter.
+        Args:
+            parameter:
+
+        Returns:
+            dict: The definition of the parameter with the type, description, etc.
+        """
+        # load definitions file
+        file_path = _dir.parent / "methods" / "_definitions.yaml"
+
+        with file_path.open("r") as file:
+            definitions = safe_load(file)
+
+        return definitions.get(parameter)
+
+    def _get_token(self, grant_type: Optional[str] = None, refresh_token=None, **kwargs):
         """
         Retrieves an access token from the token URL.
 
         Args:
             grant_type (str): The grant type (default: "password").
             refresh_token (str): The refresh token (default: None).
         """
@@ -402,14 +451,20 @@
 
         if response.status_code == 200:
             token_info = response.json()
             self.access_token = token_info["access_token"]
             self.refresh_token = token_info["refresh_token"]
             self._access_token_expires_at = time.time() + token_info["expires_in"]
             self._refresh_token_expires_at = time.time() + token_info["refresh_token_expires_in"]
+            if not user_info_path.exists():
+                store = kwargs.get("store", None)
+                if store is None:
+                    store = input("Do you want to store your credentials for future use on this computer? (y/n): ")
+                if store.lower() == "y":
+                    self._set_user()
         else:
             raise ValueError(f"Unable to retrieve token: {response.json()}. Please check your credentials.")
 
     def _is_access_token_expired(self):
         return time.time() >= self._access_token_expires_at
 
     def _is_refresh_token_expired(self):
@@ -436,19 +491,32 @@
             requests.Response: The response object.
         """
         self._ensure_access_token()
 
         headers = kwargs.get("headers", {})
         headers.update({"Authorization": f"Bearer {self.access_token}"})
         kwargs["headers"] = headers
-        try:
-            response = requests.request(method, url, **kwargs)
-            return response
-        except Exception as e:
-            raise e
+        response = requests.request(method, url, **kwargs)
+        if response.status_code == 200:
+            if "error" not in response.json():
+                return response
+            else:
+                if "user limit amount" in response.text:
+                    return response
+                else:
+                    raise ValueError(
+                        f"Unable to retrieve data! {response.json()['error']}: {response.json()['error_description']}"
+                    ) from None
+
+        elif response.status_code == 503:
+            raise f"Error {response.status_code}: {response.text}"
+        elif response.status_code == 404:
+            raise ValueError(f"Error {response.status_code}: {response.json()['error_description']}") from None
+        else:
+            raise ValueError(f"Error {response.status_code}: {response.text}") from None
 
     def _get_account_limit(
         self,
         url: str,
         params: dict,
     ):
         # Query the API with a limit of more than 5000.
@@ -466,14 +534,36 @@
         match = re.search(r"user limit amount is (\d+)", response.text)
         if match:
             self.account_limit = int(match.group(1))
         else:
             print(f"Error: {response.status_code}")
             self.account_limit = None
 
+    def _set_user(self):
+        # Write info file
+        with user_info_path.open("w") as file:
+            file.write("\n".join([self.username, self.password, self.client_id, self.client_secret]))
+
+        print("Remember me enabled.")
+
+    def _get_user(self):
+        try:
+            with user_info_path.open("r") as file:
+                lines = file.readlines()
+
+            self.username = lines[0].strip()  # set username
+            self.password = lines[1].strip()  # set password
+            self.client_id = lines[2].strip()  # set client id
+            self.client_secret = lines[3].strip()  # set client secret
+
+        except FileNotFoundError:
+            raise FileNotFoundError("Credentials file not found. Please initialize the client with your credentials.") from None
+        except Exception as e:
+            raise ValueError("Error reading credentials from file:", str(e)) from None
+
     def _get_method_url(self, method_name: str, parameters: dict, unique: bool) -> str:
         """
         Get the URL for the specified method from the YAML file.
 
         Args:
             method_name (str): The name of the method.
             parameters: The parameters for the method.
@@ -525,44 +615,46 @@
         **kwargs,
     ) -> Union[dict, DataFrame]:
         """
 
         Args:
             method (str): The name of the method to query.
             fields (list): The fields query parameter establishes the details of the data to return for the specific query.
-            parameters (dict | Parameters): The parameters for the query.
-            limit (int): A limit restricts the number of results returned by the query.
-                The limit attribute can only be added to an object type and not a property.
-                For example, to limit the number of facts in a query, {"fact": 10}.
-            sort (dict): Any returned value can be sorted in ascending or descending order,
-                using ``ASC`` or ``DESC`` (i.e. {"report.document-type": "DESC"}.
+            parameters (Optional[dict | Parameters]): The search parameters for the query.
+            limit (Optional[int]): A limit restricts the number of results returned by the query.
+                For example, in a *"fact search"* ``limit=10`` would return 10 observations.
+                You can also use ``limit="all"`` to return all results (which is not recommended unless
+                you know what you are doing!). The default is *None* which returns one response with
+                upto your account limit. For example, if your account limit is 5000, then the default
+                will return the smallest of 5000 or the number of results.
+            sort (Optional[dict]): Any returned value can be sorted in ascending or descending order,
+                using *ASC* or *DESC* (i.e. ``{"report.document-type": "DESC"}``.
                 Multiple sort criteria can be defined and the sort sequence is determined by
                 the order of the items in the dictionary.
-            unique (bool): If ``True`` returns only unique values.
-            as_dataframe (bool): If ``True`` returns the results as a ``DataFrame`` else returns the data
-                as ``json``.
-            print_query (bool=False): Whether to print the query.
-            timeout: The number of seconds to wait for a response from the server. Defaults to 5 seconds.
-                If ``None`` will wait indefinitely.
+            unique (Optional[bool]=False): If *True* returns only unique values. Default is *False*.
+            as_dataframe (Optional[bool]=False): If *True* returns the results as a *DataFrame* else returns the data
+                as *json*. The default is *False* which returns the results in *json* format
+            print_query (bool=False): Whether to print the query text.
+            timeout (int=5): The number of seconds to wait for a response from the server. Defaults to 5 seconds.
+                If *None* will wait indefinitely.
 
         Returns:
-            dict | DataFrame: The results of the query.
+            json | DataFrame: The results of the query.
         """
 
         method_url = self._get_method_url(method_name=method, parameters=parameters, unique=unique)
         # if limit is all
         if limit == "all":
             # arbitrary large number
             limit = 999999999
 
         query_params = _build_query_params(
             method=method,
             fields=fields,
             parameters=parameters,
-            limit=limit,
             sort=sort,
         )
 
         if print_query:
             print(query_params)
 
         # check if the account limit has been set
@@ -572,18 +664,18 @@
         # ensure the limit is not greater than the account limit
         account_limit = min(limit, self.account_limit) if limit is not None else self.account_limit
 
         streamlit_indicator = kwargs.get("streamlit", False)
         if streamlit_indicator:
             from stqdm import stqdm
 
-            pbar = stqdm(total=None, desc="Matches Found", ncols=80)
+            pbar = stqdm(total=None, desc="Running Query, Please Wait", ncols=80)
         else:
             # create a progress bar
-            pbar = tqdm(total=None, desc="Matches Found", ncols=80, position=0, leave=True)
+            pbar = tqdm(total=None, desc="Running Query, Please Wait", ncols=80, position=0, leave=True)
 
         # update the limit in the query params with the new limit
         query_params = _build_query_params(
             method=method,
             fields=fields,
             parameters=parameters,
             limit=account_limit,
@@ -593,16 +685,16 @@
         try:
             response = self._make_request(
                 method="get",
                 url=method_url,
                 params=query_params,
                 timeout=timeout,
             )
-        except requests.exceptions.ReadTimeout as e:
-            raise exceptions.XBRLTimeOutError(e) from e
+        except Exception as e:
+            raise e
 
         response_data = response.json()
 
         if response.status_code != 200:
             raise response_data["message"]
         elif "data" not in response_data:
             warnings.warn("No data returned from the query.", UserWarning, stacklevel=2)
```

### Comparing `xbrl-us-0.0.32/src/xbrl_us.egg-info/PKG-INFO` & `xbrl-us-0.0.4/src/xbrl_us.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.32
+Version: 0.0.4
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
@@ -24,15 +24,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-License-File: AUTHORS.rst
 
 ======================
 XBRL-US Python Library
 ======================
 
 |Workflow| |Docs| |license| |Versions|
 
@@ -109,14 +108,20 @@
 
 You can install this package using pip:
 
 .. code-block:: bash
 
     pip install xbrl-us
 
+If you are using Jupyter Notebook, you can install the package using the following command:
+
+.. code-block:: bash
+
+    !pip install xbrl-us
+
 .. caution::
 
         The XBRL US Python Wrapper is currently in beta and is subject to change.
         We welcome your feedback and suggestions for improvement.
         Please submit any issues or feature requests to
         the `GitHub repository <https://github.com/hamid-vakilzadeh/python-xbrl-us/issues>`_.
 
@@ -337,21 +342,32 @@
 Getting started is as simple as ever.
 First, ensure you have the latest version of ``xbrl-us`` installed by running the following code:
 
 .. code-block:: bash
 
     pip install xbrl-us --upgrade
 
+or if you are on a Jupyter Notebook:
+
+.. code-block:: bash
+
+    !pip install xbrl-us --upgrade
 
 Next, launch the new Browser Interface from the package menu:
 
 .. code-block:: bash
 
     python -m xbrl_us
 
+or if you are on a Jupyter Notebook:
+
+.. code-block:: bash
+
+    !python -m xbrl_us
+
 That is it!
 You should now see the new Browser Interface open in your default web browser.
 
 Happy data exploring!
 
 .. note::
```

### Comparing `xbrl-us-0.0.32/src/xbrl_us.egg-info/SOURCES.txt` & `xbrl-us-0.0.4/src/xbrl_us.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 .bumpversion.cfg
 .cookiecutterrc
 .coveragerc
 .editorconfig
 .pre-commit-config.yaml
 .readthedocs.yml
-AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 pytest.ini
 secrets.yml
 setup.py
 tox.ini
 .github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
-docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/readme.rst
 docs/requirements.txt
 docs/spelling_wordlist.txt
@@ -37,14 +35,15 @@
 src/xbrl_us.egg-info/PKG-INFO
 src/xbrl_us.egg-info/SOURCES.txt
 src/xbrl_us.egg-info/dependency_links.txt
 src/xbrl_us.egg-info/entry_points.txt
 src/xbrl_us.egg-info/not-zip-safe
 src/xbrl_us.egg-info/requires.txt
 src/xbrl_us.egg-info/top_level.txt
+src/xbrl_us/methods/_definitions.yaml
 src/xbrl_us/methods/assertion search.yml
 src/xbrl_us/methods/assertion validate.yml
 src/xbrl_us/methods/concept name search.yml
 src/xbrl_us/methods/concept search.yml
 src/xbrl_us/methods/cube search.yml
 src/xbrl_us/methods/dimension search.yml
 src/xbrl_us/methods/document search.yml
```

### Comparing `xbrl-us-0.0.32/tests/test_xbrl_us.py` & `xbrl-us-0.0.4/tests/test_xbrl_us.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.32/tox.ini` & `xbrl-us-0.0.4/tox.ini`

 * *Files identical despite different names*

