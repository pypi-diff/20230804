# Comparing `tmp/django-sphinx-hosting-1.2.3.tar.gz` & `tmp/django-sphinx-hosting-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sphinx-hosting-1.2.3.tar", last modified: Wed Aug  2 22:50:52 2023, max compression
+gzip compressed data, was "django-sphinx-hosting-1.3.0.tar", last modified: Thu Aug  3 22:48:35 2023, max compression
```

## Comparing `django-sphinx-hosting-1.2.3.tar` & `django-sphinx-hosting-1.3.0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.253510 django-sphinx-hosting-1.2.3/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.2.3/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.2.3/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-08-02 22:50:52.253738 django-sphinx-hosting-1.2.3/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.2.3/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.162234 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     2947 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1281 2023-08-02 22:50:52.255389 django-sphinx-hosting-1.2.3/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-08-02 22:46:23.000000 django-sphinx-hosting-1.2.3/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.177356 django-sphinx-hosting-1.2.3/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-08-02 22:46:23.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.184586 django-sphinx-hosting-1.2.3/sphinx_hosting/api/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1122 2023-07-31 22:42:09.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/permissions.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5706 2023-07-27 18:03:47.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/serializers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1357 2023-07-27 20:06:34.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    13981 2023-07-31 19:04:28.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/views.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/exc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/fields.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.189556 django-sphinx-hosting-1.2.3/sphinx_hosting/fixtures/
--rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/fixtures/classifiers.json
--rw-rw-r--   0 cmalek     (501) admin       (80)      445 2023-07-26 17:59:23.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/form_fields.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8372 2023-07-27 17:56:55.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    24175 2023-07-31 22:51:10.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/importers.py
--rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/logging.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.193230 django-sphinx-hosting-1.2.3/sphinx_hosting/management/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.204980 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2649 2023-07-26 23:13:05.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/fix_broken_hrefs.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2566 2023-07-26 17:58:46.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/import_docs.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1624 2023-07-26 17:58:54.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/parse_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/print_classifier_tree.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2286 2023-07-26 17:59:35.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/print_doctree.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.228230 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/
--rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0001_initial.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0002_original_html.py
--rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0003_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0004_next_page_FK.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0005_orig_global_toc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0007_load_classifiers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0008_Version_archived.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0010_add_groups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0011_machinenamefield.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1838 2023-07-26 18:06:51.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0012_project_relatedlinks.py
--rw-r--r--   0 cmalek     (501) admin       (80)      521 2023-07-27 17:59:47.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    33617 2023-07-27 17:55:22.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/models.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/search_indexes.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      776 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/signals.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.155223 django-sphinx-hosting-1.2.3/sphinx_hosting/static/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.155734 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.236200 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
--rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
--rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.237204 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/images/
--rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.156545 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.156215 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/search/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.156340 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/search/indexes/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.241128 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
--rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.242638 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/sphinx_hosting/base.html
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.243916 django-sphinx-hosting-1.2.3/sphinx_hosting/templatetags/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/templatetags/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/templatetags/sphinx_hosting.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/types.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2205 2023-07-26 17:16:32.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1103 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/validators.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    26582 2023-07-31 19:00:50.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/views.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.251230 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/classifier.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.253008 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/core/
--rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/core/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/core/basic.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4701 2023-05-04 19:20:06.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/navigation.py
--rw-r--r--   0 cmalek     (501) admin       (80)    19342 2023-08-02 17:26:20.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/project.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/search.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8924 2023-07-27 18:29:50.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/sphinx_page.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/version.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.951184 django-sphinx-hosting-1.3.0/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.3.0/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.3.0/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2521 2023-08-03 22:48:35.951294 django-sphinx-hosting-1.3.0/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.3.0/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.934055 django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2521 2023-08-03 22:48:35.000000 django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3006 2023-08-03 22:48:35.000000 django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-08-03 22:48:35.000000 django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-08-03 22:48:35.000000 django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/not-zip-safe
+-rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-08-03 22:48:35.000000 django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-08-03 22:48:35.000000 django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/top_level.txt
+-rw-r--r--   0 cmalek     (501) admin       (80)      116 2023-08-03 22:45:43.000000 django-sphinx-hosting-1.3.0/pyproject.toml
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3022 2023-08-03 22:48:35.952993 django-sphinx-hosting-1.3.0/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)       68 2023-08-03 22:43:55.000000 django-sphinx-hosting-1.3.0/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.937961 django-sphinx-hosting-1.3.0/sphinx_hosting/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       21 2023-08-03 22:48:33.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.939445 django-sphinx-hosting-1.3.0/sphinx_hosting/api/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/api/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/api/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1122 2023-07-31 22:42:09.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/api/permissions.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5706 2023-07-27 18:03:47.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/api/serializers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1357 2023-07-27 20:06:34.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/api/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    13981 2023-07-31 19:04:28.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/api/views.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/exc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/fields.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.939689 django-sphinx-hosting-1.3.0/sphinx_hosting/fixtures/
+-rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/fixtures/classifiers.json
+-rw-rw-r--   0 cmalek     (501) admin       (80)      445 2023-07-26 17:59:23.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/form_fields.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8372 2023-07-27 17:56:55.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    24621 2023-08-03 22:23:56.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/importers.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/logging.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.939935 django-sphinx-hosting-1.3.0/sphinx_hosting/management/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/management/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.941799 django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2649 2023-07-26 23:13:05.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/fix_broken_hrefs.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2566 2023-07-26 17:58:46.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/import_docs.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1624 2023-07-26 17:58:54.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/parse_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/print_classifier_tree.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2286 2023-07-26 17:59:35.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/print_doctree.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.946224 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0001_initial.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0002_original_html.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0003_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0004_next_page_FK.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0005_orig_global_toc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0007_load_classifiers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0008_Version_archived.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0010_add_groups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0011_machinenamefield.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1838 2023-07-26 18:06:51.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0012_project_relatedlinks.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      521 2023-07-27 17:59:47.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    33617 2023-07-27 17:55:22.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/py.typed
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/search_indexes.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      776 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/signals.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.931249 django-sphinx-hosting-1.3.0/sphinx_hosting/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.931385 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.947164 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
+-rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.947845 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/images/
+-rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.931659 django-sphinx-hosting-1.3.0/sphinx_hosting/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.931550 django-sphinx-hosting-1.3.0/sphinx_hosting/templates/search/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.931595 django-sphinx-hosting-1.3.0/sphinx_hosting/templates/search/indexes/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.948068 django-sphinx-hosting-1.3.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.948225 django-sphinx-hosting-1.3.0/sphinx_hosting/templates/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/templates/sphinx_hosting/base.html
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.948501 django-sphinx-hosting-1.3.0/sphinx_hosting/templatetags/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/templatetags/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/templatetags/sphinx_hosting.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/types.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2205 2023-07-26 17:16:32.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1103 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/validators.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    26582 2023-08-03 22:24:02.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/views.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.950748 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/classifier.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-03 22:48:35.951069 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/core/
+-rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/core/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/core/basic.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4147 2023-08-03 22:33:18.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/navigation.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    19342 2023-08-03 22:36:48.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/project.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/search.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8924 2023-07-27 18:29:50.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/sphinx_page.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.2.3/LICENSE.txt` & `django-sphinx-hosting-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/PKG-INFO` & `django-sphinx-hosting-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.2.3
+Version: 1.3.0
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
+Project-URL: Documentation, https://django-sphinx-hosting.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/caltechads/django-sphinx-hosting
+Project-URL: Issues, https://github.com/caltechads/django-sphinx-hosting/issues
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
-Description-Content-Type: text/markdown
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
 
 # django-sphinx-hosting
 
 **Documentation**: [django-sphinx-hosting.readthedocs.org](https://django-sphinx-hosting.readthedocs.org)
 
 This reusable Django application provides models, views, permissions, REST API
```

### Comparing `django-sphinx-hosting-1.2.3/README.md` & `django-sphinx-hosting-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/PKG-INFO` & `django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.2.3
+Version: 1.3.0
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
+Project-URL: Documentation, https://django-sphinx-hosting.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/caltechads/django-sphinx-hosting
+Project-URL: Issues, https://github.com/caltechads/django-sphinx-hosting/issues
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
-Description-Content-Type: text/markdown
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
 
 # django-sphinx-hosting
 
 **Documentation**: [django-sphinx-hosting.readthedocs.org](https://django-sphinx-hosting.readthedocs.org)
 
 This reusable Django application provides models, views, permissions, REST API
```

### Comparing `django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/SOURCES.txt` & `django-sphinx-hosting-1.3.0/django_sphinx_hosting.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 django_sphinx_hosting.egg-info/PKG-INFO
 django_sphinx_hosting.egg-info/SOURCES.txt
 django_sphinx_hosting.egg-info/dependency_links.txt
+django_sphinx_hosting.egg-info/not-zip-safe
 django_sphinx_hosting.egg-info/requires.txt
 django_sphinx_hosting.egg-info/top_level.txt
 sphinx_hosting/__init__.py
 sphinx_hosting/apps.py
 sphinx_hosting/exc.py
 sphinx_hosting/fields.py
 sphinx_hosting/form_fields.py
```

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/api/permissions.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/api/serializers.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/api/urls.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/api/views.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/fields.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/fields.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/fixtures/classifiers.json` & `django-sphinx-hosting-1.3.0/sphinx_hosting/fixtures/classifiers.json`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/forms.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/forms.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/importers.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/importers.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,23 +277,24 @@
         if 'title' not in data:
             # Some of the special pages don't have 'title' keys
             if 'indextitle' in data:
                 data['title'] = data['indextitle']
             else:
                 data['title'] = SphinxPage.SPECIAL_PAGES[path]
 
-    def _fix_link_hrefs(self, body: str) -> str:
+    def _fix_link_hrefs(self, path: str, body: str) -> str:
         """
         Given an HTML body of a Sphinx page, update the ``<a href="path">``
         references for "path" to be rendered at page render time.  If we don't
         do this, a lot of links won't work, because they do
         index page, instead of being relative to the root of the docs, and won't
         work.
 
         Args:
+            path: the path to the current page
             body: the HTML body of a Sphinx document
 
         Returns:
             ``body`` with its ``<a>`` urls and updated
         """
         if not body:
             return ''
@@ -308,55 +309,61 @@
         for link in links:
             href = link.attrib['href']
             anchor = None
             if '#' in href:
                 href, anchor = href.split('#')
             if href.endswith('/'):
                 href = href[:-1]
-            href = re.sub('^(../)*', '', href)
-            link.attrib['href'] = "{{% url 'sphinx_hosting:sphinxpage--detail' project_slug='{}' version='{}' path='{}' %}}".format(
+            # To deal with relative links, we need to know our current path
+            # and then compute the absolute path from that.
+            levels = href.count('../')
+            if levels:
+                href = re.sub('^(../)*', '', href)
+                href = '/'.join(path.split('/')[:-(levels)] + [href])
+            link.attrib['href'] = "{{% url 'sphinx_hosting:sphinxpage--detail' project_slug='{}' version='{}' path='{}' %}}".format(  # noqa:E501  # pylint: disable=line-too-long
                 self.config['project'],
                 self.config['release'],
                 href
             )
             if anchor:
                 link.attrib['href'] += f'#{anchor}'
 
         # Return the updated HTML body
         return lxml.html.tostring(html).decode('utf-8')
 
-    def _fix_page_body(self, data: Dict[str, Any]) -> None:
+    def _fix_page_body(self, path: str, data: Dict[str, Any]) -> None:
         """
         Do any work needed to prepare the page body before inserting into the
         database.  This means:
 
         * Ensure the ``body`` key exists in ``data``
         * Update the ``img`` sources to point to our Django storage location.
           We uploaded them to our storage during :py:meth:`import_images`.
         * Update the ``href``s for any ``<a>`` links to be rendered at page
           render time.
         * Update the ``<table>``s to have the CSS classes we need for them to
           display nicely.
 
         Args:
+            path: the path to the current page
             data: the JSON data from our file
         """
         if 'body' not in data or data['body'] is None:
             # Ensure we always have data['body'] defined as a string, for when
             # we create the SphinxPage, below
             data['body'] = ''
         data['orig_body'] = data['body']
         if data['body']:
             # Update the img src for any images in data['body'] for to point to our
             # Django storage locations
             data['body'] = self._update_image_src(data['body'])
             # Update the hrefs for any <a> links to be absolute.  The relative
             # paths we get from Sphinx end up being relative to the Sphinx index
             # document instead of to the root of the docs
-            data['body'] = self._fix_link_hrefs(data['body'])
+            data['body'] = self._fix_link_hrefs(path, data['body'])
             html = lxml.html.fromstring(data['body'])
             # remove the first <h1> -- we'll display the page title another way
             first_h1 = html.cssselect('h1')
             if first_h1:
                 first_h1[0].getparent().remove(first_h1[0])
             # Fix our tables to look better
             tables = html.cssselect('table')
@@ -484,15 +491,15 @@
             path: str = str(Path(*Path(member.name).parts[1:]))
             if path.endswith('.fjson'):
                 # files that contain page data will have a .fjson extension
                 path = path.replace('.fjson', '')
                 fd = cast(io.BufferedReader, package.extractfile(member))
                 data = json.loads(fd.read())
                 self._fix_page_title(path, data)
-                self._fix_page_body(data)
+                self._fix_page_body(path, data)
                 self._fix_toc(data)
                 page = SphinxPage(
                     version=version,
                     relative_path=path,
                     content=json.dumps(data),
                     title=data['title'],
                     orig_body=data['orig_body'],
```

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/fix_broken_hrefs.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/fix_broken_hrefs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/import_docs.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/import_docs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/parse_globaltoc.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/parse_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/print_classifier_tree.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/print_classifier_tree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/print_doctree.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/management/commands/print_doctree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0001_initial.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0002_original_html.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0002_original_html.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0003_globaltoc.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0003_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0004_next_page_FK.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0004_next_page_FK.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0005_orig_global_toc.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0005_orig_global_toc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0007_load_classifiers.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0007_load_classifiers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0009_SphinxPage_searchable.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0010_add_groups.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0010_add_groups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0011_machinenamefield.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0011_machinenamefield.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0012_project_relatedlinks.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0012_project_relatedlinks.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/models.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/models.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/search_indexes.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/settings.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/settings.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/signals.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/signals.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss` & `django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss` & `django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss` & `django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css` & `django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss` & `django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/images/logo.jpg` & `django-sphinx-hosting-1.3.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/templates/sphinx_hosting/base.html` & `django-sphinx-hosting-1.3.0/sphinx_hosting/templates/sphinx_hosting/base.html`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/urls.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/validators.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/validators.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/views.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/classifier.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/classifier.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/navigation.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/navigation.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,63 +37,49 @@
         MenuItem(
             text='Projects',
             icon='bookshelf',
             url=reverse_lazy('sphinx_hosting:project--list')
         )
     ]
 
-
-class SphinxHostingLookupsMenu(Menu):
-    """
-    This is a second menu that appears in :py:class:`SphinxHostingSidebar` below
-    the main menu, :py:class:`SphinxHostingMainMenu`.  This gives access to our
-    various lookup models like :py:class:`sphinx_hosting.models.Classifier` for
-    those users that have rights to work with them directly.
-    """
-    title: Optional[str] = "Lookups"
-    css_class: str = 'mt-3'
-
     def __init__(self, *items, **kwargs) -> None:
         self.active_item: Optional[str] = None
         super().__init__(*items, **kwargs)
 
     def build_menu(self, items: List[MenuItem]) -> None:
         """
         Programatically build our menu here.  We have this code because the
-        presence of items in this menu depends on the user's permissions.
+        presence of some items in this menu depends on the user's permissions.
 
         We have to do it here because if we do it in ``__init__``, that's too
         early in the Django boostrap and the global Django ``urlpatterns`` have
-        not finished building.
+        not finished building, and even ``reverse_lazy`` fails.
         """
         request: HttpRequest = CrequestMiddleware.get_request()
         user: AbstractUser = cast(AbstractUser, request.user)
         if user.has_perm('sphinxhostingcore.view_classifier'):
             item = MenuItem(
                 text='Classifiers',
                 icon='bookshelf',
                 url=reverse_lazy('sphinx_hosting:classifier--index')
             )
+            items.append(item)
+        for item in items:
             if self.active_item is not None:
                 item.set_active(self.active_item)
-            items.append(item)
-        if not items:
-            # If there's nothing left, hide the title so that the menu
-            # doesn't show up at all
-            self.title = None
         super().build_menu(items)
 
     def activate(self, text: str) -> bool:
         """
         Normally, how activate works is that it looks through our menu items,
         finds the one whose ``text`` or ``url`` matches ``text``.
 
-        In our case, we're building the menu items in :py:meth:`build_menu`, which
-        occurs after :py:meth:`activate` would be called, so we have to save the
-        ``text`` here, and use it later in :py:meth:`build_menu`.
+        In our case, we're building the menu items in :py:meth:`build_menu`,
+        which occurs after :py:meth:`activate` would be called, so we have to
+        save the ``text`` here, and use it later in :py:meth:`build_menu`.
 
         Args:
             text: the text to search for among our :py:attr:`items`
 
         Returns:
             We always return ``True`` here, since we won't know if we match
             until later.
@@ -123,15 +109,14 @@
             url=LOGO_URL
         ),
         GlobalSearchFormWidget(css_class='ms-auto ms-xl-0 align-self-center mt-3'),
         css_class='d-flex flex-row flex-xl-column justify-content-between flex-grow-1 flex-xl-grow-0'
     )
     contents = [
         SphinxHostingMainMenu(),
-        SphinxHostingLookupsMenu(),
     ]
     wide: bool = True
 
 
 class SphinxHostingBreadcrumbs(BreadcrumbBlock):
 
     items: List[BreadcrumbItem] = [
```

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/project.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/project.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/search.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/search.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/sphinx_page.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/sphinx_page.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/version.py` & `django-sphinx-hosting-1.3.0/sphinx_hosting/wildewidgets/version.py`

 * *Files identical despite different names*

