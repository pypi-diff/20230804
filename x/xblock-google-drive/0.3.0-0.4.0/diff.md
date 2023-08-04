# Comparing `tmp/xblock-google-drive-0.3.0.tar.gz` & `tmp/xblock-google-drive-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-google-drive-0.3.0.tar", last modified: Tue Oct 25 12:19:47 2022, max compression
+gzip compressed data, was "xblock-google-drive-0.4.0.tar", last modified: Fri Aug  4 10:52:35 2023, max compression
```

## Comparing `xblock-google-drive-0.3.0.tar` & `xblock-google-drive-0.4.0.tar`

### file list

```diff
@@ -1,55 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.195865 xblock-google-drive-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35136 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-25 12:19:47.195865 xblock-google-drive-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5700 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/google_calendar.py
--rw-r--r--   0 runner    (1001) docker     (121)     5895 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/google_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/public/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/public/css/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/public/css/google_calendar.css
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/public/css/google_docs.css
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/public/css/google_edit.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/public/js/
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/public/js/google_calendar.js
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/public/js/google_calendar_edit.js
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/public/js/google_docs.js
--rw-r--r--   0 runner    (1001) docker     (121)     4275 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/public/js/google_docs_edit.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/templates/html/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/templates/html/google_calendar.html
--rw-r--r--   0 runner    (1001) docker     (121)     3716 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/templates/html/google_calendar_edit.html
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/templates/html/google_docs.html
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/templates/html/google_docs_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/translations/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/translations/eo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.195865 xblock-google-drive-0.3.0/google_drive/translations/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     6075 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (121)     7968 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/eo/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.195865 xblock-google-drive-0.3.0/google_drive/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (121)     5215 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.195865 xblock-google-drive-0.3.0/google_drive/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (121)     5036 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.191864 xblock-google-drive-0.3.0/google_drive/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.195865 xblock-google-drive-0.3.0/google_drive/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/google_drive/translations/ja_JP/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-25 12:19:47.195865 xblock-google-drive-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-10-25 12:19:44.000000 xblock-google-drive-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:19:47.195865 xblock-google-drive-0.3.0/xblock_google_drive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-25 12:19:47.000000 xblock-google-drive-0.3.0/xblock_google_drive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-10-25 12:19:47.000000 xblock-google-drive-0.3.0/xblock_google_drive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-25 12:19:47.000000 xblock-google-drive-0.3.0/xblock_google_drive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-25 12:19:47.000000 xblock-google-drive-0.3.0/xblock_google_drive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-25 12:19:47.000000 xblock-google-drive-0.3.0/xblock_google_drive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-25 12:19:47.000000 xblock-google-drive-0.3.0/xblock_google_drive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.904557 xblock-google-drive-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-08-04 10:52:35.904557 xblock-google-drive-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/conf/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/conf/locale/
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/conf/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/conf/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3686 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3686 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/conf/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/conf/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/eo/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     7968 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/eo/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/conf/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/conf/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/conf/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/conf/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2950 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/conf/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/conf/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5374 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/conf/locale/ja_JP/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5266 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/google_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5971 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/google_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/public/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/public/css/google_calendar.css
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/public/css/google_docs.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/public/css/google_edit.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/public/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/public/js/google_calendar.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/public/js/google_calendar_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1539 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/public/js/google_docs.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4275 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/public/js/google_docs_edit.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/templates/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/templates/html/google_calendar.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/templates/html/google_calendar_edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/templates/html/google_docs.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/templates/html/google_docs_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/translations/
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3686 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3686 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/translations/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/eo/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     7968 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/eo/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.900557 xblock-google-drive-0.4.0/google_drive/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.904557 xblock-google-drive-0.4.0/google_drive/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2950 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.896557 xblock-google-drive-0.4.0/google_drive/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.904557 xblock-google-drive-0.4.0/google_drive/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5374 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/google_drive/translations/ja_JP/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-08-04 10:52:35.904557 xblock-google-drive-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-08-04 10:52:30.000000 xblock-google-drive-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:52:35.904557 xblock-google-drive-0.4.0/xblock_google_drive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-08-04 10:52:35.000000 xblock-google-drive-0.4.0/xblock_google_drive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-08-04 10:52:35.000000 xblock-google-drive-0.4.0/xblock_google_drive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-08-04 10:52:35.000000 xblock-google-drive-0.4.0/xblock_google_drive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-08-04 10:52:35.000000 xblock-google-drive-0.4.0/xblock_google_drive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-04 10:52:35.000000 xblock-google-drive-0.4.0/xblock_google_drive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-08-04 10:52:35.000000 xblock-google-drive-0.4.0/xblock_google_drive.egg-info/top_level.txt
```

### Comparing `xblock-google-drive-0.3.0/LICENSE` & `xblock-google-drive-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/README.rst` & `xblock-google-drive-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/google_calendar.py` & `xblock-google-drive-0.4.0/google_drive/google_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,19 +88,24 @@
     def studio_view(self, context):  # pylint: disable=unused-argument
         """
         Editing view in Studio
         """
         fragment = Fragment()
         # Need to access protected members of fields to get their default value
         default_name = self.fields['display_name']._default  # pylint: disable=protected-access,unsubscriptable-object
-        fragment.add_content(RESOURCE_LOADER.render_template(CALENDAR_EDIT_TEMPLATE, {
-            'self': self,
-            'defaultName': default_name,
-            'defaultID': self.fields['calendar_id']._default  # pylint: disable=protected-access,unsubscriptable-object
-        }))
+        default_id = self.fields['calendar_id']._default  # pylint: disable=protected-access,unsubscriptable-object
+        fragment.add_content(RESOURCE_LOADER.render_django_template(
+            CALENDAR_EDIT_TEMPLATE,
+            context={
+                'self': self,
+                'defaultName': default_name,
+                'defaultID': default_id
+            },
+            i18n_service=self.runtime.service(self, "i18n"),
+        ))
         fragment.add_javascript(RESOURCE_LOADER.load_unicode('public/js/google_calendar_edit.js'))
         fragment.add_css(RESOURCE_LOADER.load_unicode('public/css/google_edit.css'))
 
         fragment.initialize_js('GoogleCalendarEditBlock')
 
         return fragment
```

### Comparing `xblock-google-drive-0.3.0/google_drive/google_docs.py` & `xblock-google-drive-0.4.0/google_drive/google_docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,18 +97,19 @@
     def studio_view(self, context):  # pylint: disable=unused-argument
         """
         Editing view in Studio
         """
         fragment = Fragment()
         # Need to access protected members of fields to get their default value
         default_name = self.fields['display_name']._default  # pylint: disable=protected-access,unsubscriptable-object
-        fragment.add_content(RESOURCE_LOADER.render_template(DOCUMENT_EDIT_TEMPLATE, {
-            'self': self,
-            'defaultName': default_name,
-        }))
+        fragment.add_content(RESOURCE_LOADER.render_django_template(
+            DOCUMENT_EDIT_TEMPLATE,
+            context={'self': self, 'defaultName': default_name},
+            i18n_service=self.runtime.service(self, 'i18n'),
+        ))
         fragment.add_javascript(RESOURCE_LOADER.load_unicode('public/js/google_docs_edit.js'))
         fragment.add_css(RESOURCE_LOADER.load_unicode('public/css/google_edit.css'))
 
         fragment.initialize_js('GoogleDocumentEditBlock')
 
         return fragment
```

### Comparing `xblock-google-drive-0.3.0/google_drive/public/css/google_edit.css` & `xblock-google-drive-0.4.0/google_drive/public/css/google_edit.css`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/public/js/google_calendar.js` & `xblock-google-drive-0.4.0/google_drive/public/js/google_calendar.js`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/public/js/google_calendar_edit.js` & `xblock-google-drive-0.4.0/google_drive/public/js/google_calendar_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/public/js/google_docs.js` & `xblock-google-drive-0.4.0/google_drive/public/js/google_docs.js`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/public/js/google_docs_edit.js` & `xblock-google-drive-0.4.0/google_drive/public/js/google_docs_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/templates/html/google_calendar_edit.html` & `xblock-google-drive-0.4.0/google_drive/templates/html/google_calendar_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/templates/html/google_docs_edit.html` & `xblock-google-drive-0.4.0/google_drive/templates/html/google_docs_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/en/LC_MESSAGES/text.po` & `xblock-google-drive-0.4.0/google_drive/conf/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/eo/LC_MESSAGES/text.mo` & `xblock-google-drive-0.4.0/google_drive/conf/locale/eo/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/eo/LC_MESSAGES/text.po` & `xblock-google-drive-0.4.0/google_drive/conf/locale/eo/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/es_419/LC_MESSAGES/text.mo` & `xblock-google-drive-0.4.0/google_drive/conf/locale/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/es_419/LC_MESSAGES/text.po` & `xblock-google-drive-0.4.0/google_drive/conf/locale/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/fr_CA/LC_MESSAGES/text.mo` & `xblock-google-drive-0.4.0/google_drive/conf/locale/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/fr_CA/LC_MESSAGES/text.po` & `xblock-google-drive-0.4.0/google_drive/conf/locale/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/ja_JP/LC_MESSAGES/text.mo` & `xblock-google-drive-0.4.0/google_drive/conf/locale/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/google_drive/translations/ja_JP/LC_MESSAGES/text.po` & `xblock-google-drive-0.4.0/google_drive/conf/locale/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-google-drive-0.3.0/setup.py` & `xblock-google-drive-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 data.append(os.path.relpath(os.path.join(dirname, fname), pkg))
 
     return {pkg: data}
 
 
 setup(
     name='xblock-google-drive',
-    version='0.3.0',
+    version='0.4.0',
     description='An XBlock which allows embedding of Google documents and calendar within an edX course',
     packages=[
         'google_drive',
     ],
     install_requires=[
         'mako',
         'XBlock',
@@ -40,9 +40,9 @@
     ],
     entry_points={
         'xblock.v1': [
             'google-document = google_drive:GoogleDocumentBlock',
             'google-calendar = google_drive:GoogleCalendarBlock'
         ]
     },
-    package_data=package_data("google_drive", ["static", "templates", "public", "translations"]),
+    package_data=package_data("google_drive", ["static", "templates", "public", "translations", "conf"]),
 )
```

### Comparing `xblock-google-drive-0.3.0/xblock_google_drive.egg-info/SOURCES.txt` & `xblock-google-drive-0.4.0/xblock_google_drive.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 google_drive/__init__.py
 google_drive/google_calendar.py
 google_drive/google_docs.py
+google_drive/conf/locale/config.yaml
+google_drive/conf/locale/en/LC_MESSAGES/django.po
+google_drive/conf/locale/en/LC_MESSAGES/text.po
+google_drive/conf/locale/eo/LC_MESSAGES/text.mo
+google_drive/conf/locale/eo/LC_MESSAGES/text.po
+google_drive/conf/locale/es_419/LC_MESSAGES/text.mo
+google_drive/conf/locale/es_419/LC_MESSAGES/text.po
+google_drive/conf/locale/fr_CA/LC_MESSAGES/text.mo
+google_drive/conf/locale/fr_CA/LC_MESSAGES/text.po
+google_drive/conf/locale/ja_JP/LC_MESSAGES/text.mo
+google_drive/conf/locale/ja_JP/LC_MESSAGES/text.po
 google_drive/public/css/google_calendar.css
 google_drive/public/css/google_docs.css
 google_drive/public/css/google_edit.css
 google_drive/public/js/google_calendar.js
 google_drive/public/js/google_calendar_edit.js
 google_drive/public/js/google_docs.js
 google_drive/public/js/google_docs_edit.js
 google_drive/templates/html/google_calendar.html
 google_drive/templates/html/google_calendar_edit.html
 google_drive/templates/html/google_docs.html
 google_drive/templates/html/google_docs_edit.html
 google_drive/translations/config.yaml
-google_drive/translations/en/LC_MESSAGES/text.mo
+google_drive/translations/en/LC_MESSAGES/django.po
 google_drive/translations/en/LC_MESSAGES/text.po
 google_drive/translations/eo/LC_MESSAGES/text.mo
 google_drive/translations/eo/LC_MESSAGES/text.po
 google_drive/translations/es_419/LC_MESSAGES/text.mo
 google_drive/translations/es_419/LC_MESSAGES/text.po
 google_drive/translations/fr_CA/LC_MESSAGES/text.mo
 google_drive/translations/fr_CA/LC_MESSAGES/text.po
```

