# Comparing `tmp/django-cards-0.9.3.tar.gz` & `tmp/django-cards-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cards-0.9.3.tar", last modified: Tue Jun 20 11:28:39 2023, max compression
+gzip compressed data, was "django-cards-0.9.4.tar", last modified: Fri Aug  4 08:01:48 2023, max compression
```

## Comparing `django-cards-0.9.3.tar` & `django-cards-0.9.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.590906 django-cards-0.9.3/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 09:53:41.000000 django-cards-0.9.3/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       55 2023-01-16 09:53:41.000000 django-cards-0.9.3/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-06-20 11:28:39.590667 django-cards-0.9.3/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      130 2023-01-16 09:53:41.000000 django-cards-0.9.3/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.507187 django-cards-0.9.3/cards/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      166 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/apps.py
--rw-r--r--   0 tom        (501) staff       (20)    26056 2023-05-17 09:12:45.000000 django-cards-0.9.3/cards/base.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.518119 django-cards-0.9.3/cards/card_list/
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/card_list/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5753 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/card_list/base.py
--rw-r--r--   0 tom        (501) staff       (20)     3952 2023-02-20 18:38:25.000000 django-cards-0.9.3/cards/card_list/main.py
--rw-r--r--   0 tom        (501) staff       (20)     2468 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/card_list/tree.py
--rw-r--r--   0 tom        (501) staff       (20)      714 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/includes.py
--rw-r--r--   0 tom        (501) staff       (20)     5294 2023-06-19 15:48:35.000000 django-cards-0.9.3/cards/standard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.495785 django-cards-0.9.3/cards/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.495900 django-cards-0.9.3/cards/static/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.496959 django-cards-0.9.3/cards/static/cards/jstree/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.496177 django-cards-0.9.3/cards/static/cards/jstree/css/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.496567 django-cards-0.9.3/cards/static/cards/jstree/css/themes/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.521608 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/
--rw-r--r--   0 tom        (501) staff       (20)     5660 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     2215 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    31722 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27353 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.555163 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/
--rw-r--r--   0 tom        (501) staff       (20)     1525 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     6526 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    34459 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/style.css
--rw-r--r--   0 tom        (501) staff       (20)    29959 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.558178 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/
--rw-r--r--   0 tom        (501) staff       (20)     6423 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/30px.png
--rw-r--r--   0 tom        (501) staff       (20)     3333 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/32px.png
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.496825 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.573556 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
--rw-r--r--   0 tom        (501) staff       (20)    24108 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   134830 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    49936 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27344 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    24056 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   140377 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50224 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27108 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    25059 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   150837 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50788 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    28152 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    32574 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27752 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1720 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.574768 django-cards-0.9.3/cards/static/cards/jstree/js/
--rw-r--r--   0 tom        (501) staff       (20)   307794 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/js/jstree.js
--rw-r--r--   0 tom        (501) staff       (20)   141222 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/js/jstree.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.497211 django-cards-0.9.3/cards/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.498570 django-cards-0.9.3/cards/templates/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.575443 django-cards-0.9.3/cards/templates/cards/groups/
--rw-r--r--   0 tom        (501) staff       (20)      206 2023-01-18 12:35:38.000000 django-cards-0.9.3/cards/templates/cards/groups/groups.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.586255 django-cards-0.9.3/cards/templates/cards/standard/
--rw-r--r--   0 tom        (501) staff       (20)       69 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/templates/cards/standard/blank.html
--rw-r--r--   0 tom        (501) staff       (20)     1588 2023-01-26 20:53:02.000000 django-cards-0.9.3/cards/templates/cards/standard/card_group.html
--rw-r--r--   0 tom        (501) staff       (20)     2212 2023-06-20 11:24:38.000000 django-cards-0.9.3/cards/templates/cards/standard/datatable.html
--rw-r--r--   0 tom        (501) staff       (20)      778 2023-05-05 10:39:41.000000 django-cards-0.9.3/cards/templates/cards/standard/default.html
--rw-r--r--   0 tom        (501) staff       (20)     1661 2023-05-17 09:02:56.000000 django-cards-0.9.3/cards/templates/cards/standard/default_body.html
--rw-r--r--   0 tom        (501) staff       (20)     1079 2023-05-05 13:55:45.000000 django-cards-0.9.3/cards/templates/cards/standard/html.html
--rw-r--r--   0 tom        (501) staff       (20)     2606 2023-05-05 13:55:45.000000 django-cards-0.9.3/cards/templates/cards/standard/list_selection.html
--rw-r--r--   0 tom        (501) staff       (20)      576 2023-05-05 11:16:16.000000 django-cards-0.9.3/cards/templates/cards/standard/message.html
--rw-r--r--   0 tom        (501) staff       (20)      859 2023-05-05 11:16:16.000000 django-cards-0.9.3/cards/templates/cards/standard/table.html
--rw-r--r--   0 tom        (501) staff       (20)     1547 2023-05-19 09:31:19.000000 django-cards-0.9.3/cards/templates/cards/standard/table_body.html
--rw-r--r--   0 tom        (501) staff       (20)     2198 2023-05-05 13:55:45.000000 django-cards-0.9.3/cards/templates/cards/standard/tree_selection.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.587463 django-cards-0.9.3/cards/templatetags/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/templatetags/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      362 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/templatetags/django_cards_tags.py
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/url_converters.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.590114 django-cards-0.9.3/django_cards.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-06-20 11:28:39.000000 django-cards-0.9.3/django_cards.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     3065 2023-06-20 11:28:39.000000 django-cards-0.9.3/django_cards.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-20 11:28:39.000000 django-cards-0.9.3/django_cards.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-20 11:28:39.000000 django-cards-0.9.3/django_cards.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-20 11:28:39.590987 django-cards-0.9.3/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      645 2023-06-20 11:28:10.000000 django-cards-0.9.3/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.421514 django-cards-0.9.4/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 09:53:41.000000 django-cards-0.9.4/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       55 2023-01-16 09:53:41.000000 django-cards-0.9.4/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-08-04 08:01:48.421378 django-cards-0.9.4/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      130 2023-01-16 09:53:41.000000 django-cards-0.9.4/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.408532 django-cards-0.9.4/cards/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      166 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)    26625 2023-08-04 08:01:30.000000 django-cards-0.9.4/cards/base.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.409271 django-cards-0.9.4/cards/card_list/
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/card_list/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5753 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/card_list/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3952 2023-02-20 18:38:25.000000 django-cards-0.9.4/cards/card_list/main.py
+-rw-r--r--   0 tom        (501) staff       (20)     2468 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/card_list/tree.py
+-rw-r--r--   0 tom        (501) staff       (20)      714 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/includes.py
+-rw-r--r--   0 tom        (501) staff       (20)     5294 2023-06-19 15:48:35.000000 django-cards-0.9.4/cards/standard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.406090 django-cards-0.9.4/cards/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.406149 django-cards-0.9.4/cards/static/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.406569 django-cards-0.9.4/cards/static/cards/jstree/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.406234 django-cards-0.9.4/cards/static/cards/jstree/css/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.406400 django-cards-0.9.4/cards/static/cards/jstree/css/themes/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.410076 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/
+-rw-r--r--   0 tom        (501) staff       (20)     5660 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     2215 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    31722 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27353 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.410848 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/
+-rw-r--r--   0 tom        (501) staff       (20)     1525 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     6526 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    34459 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    29959 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.412029 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/
+-rw-r--r--   0 tom        (501) staff       (20)     6423 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/30px.png
+-rw-r--r--   0 tom        (501) staff       (20)     3333 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/32px.png
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.406508 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.415322 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
+-rw-r--r--   0 tom        (501) staff       (20)    24108 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   134830 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    49936 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27344 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    24056 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   140377 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50224 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27108 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    25059 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   150837 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50788 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    28152 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    32574 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27752 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1720 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.416077 django-cards-0.9.4/cards/static/cards/jstree/js/
+-rw-r--r--   0 tom        (501) staff       (20)   307794 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/js/jstree.js
+-rw-r--r--   0 tom        (501) staff       (20)   141222 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/static/cards/jstree/js/jstree.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.406672 django-cards-0.9.4/cards/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.406780 django-cards-0.9.4/cards/templates/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.416761 django-cards-0.9.4/cards/templates/cards/groups/
+-rw-r--r--   0 tom        (501) staff       (20)      206 2023-01-18 12:35:38.000000 django-cards-0.9.4/cards/templates/cards/groups/groups.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.420132 django-cards-0.9.4/cards/templates/cards/standard/
+-rw-r--r--   0 tom        (501) staff       (20)       69 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/templates/cards/standard/blank.html
+-rw-r--r--   0 tom        (501) staff       (20)     1588 2023-01-26 20:53:02.000000 django-cards-0.9.4/cards/templates/cards/standard/card_group.html
+-rw-r--r--   0 tom        (501) staff       (20)     2212 2023-06-20 11:24:38.000000 django-cards-0.9.4/cards/templates/cards/standard/datatable.html
+-rw-r--r--   0 tom        (501) staff       (20)      778 2023-05-05 10:39:41.000000 django-cards-0.9.4/cards/templates/cards/standard/default.html
+-rw-r--r--   0 tom        (501) staff       (20)     1661 2023-05-17 09:02:56.000000 django-cards-0.9.4/cards/templates/cards/standard/default_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     1079 2023-05-05 13:55:45.000000 django-cards-0.9.4/cards/templates/cards/standard/html.html
+-rw-r--r--   0 tom        (501) staff       (20)     2606 2023-05-05 13:55:45.000000 django-cards-0.9.4/cards/templates/cards/standard/list_selection.html
+-rw-r--r--   0 tom        (501) staff       (20)      576 2023-05-05 11:16:16.000000 django-cards-0.9.4/cards/templates/cards/standard/message.html
+-rw-r--r--   0 tom        (501) staff       (20)      859 2023-05-05 11:16:16.000000 django-cards-0.9.4/cards/templates/cards/standard/table.html
+-rw-r--r--   0 tom        (501) staff       (20)     1547 2023-05-19 09:31:19.000000 django-cards-0.9.4/cards/templates/cards/standard/table_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     2198 2023-05-05 13:55:45.000000 django-cards-0.9.4/cards/templates/cards/standard/tree_selection.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.420513 django-cards-0.9.4/cards/templatetags/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/templatetags/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      362 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/templatetags/django_cards_tags.py
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.4/cards/url_converters.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-04 08:01:48.421194 django-cards-0.9.4/django_cards.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-08-04 08:01:48.000000 django-cards-0.9.4/django_cards.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     3065 2023-08-04 08:01:48.000000 django-cards-0.9.4/django_cards.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-04 08:01:48.000000 django-cards-0.9.4/django_cards.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-08-04 08:01:48.000000 django-cards-0.9.4/django_cards.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-08-04 08:01:48.421558 django-cards-0.9.4/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      645 2023-08-04 08:01:30.000000 django-cards-0.9.4/setup.py
```

### Comparing `django-cards-0.9.3/LICENSE` & `django-cards-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/PKG-INFO` & `django-cards-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.9.3
+Version: 0.9.4
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-cards-0.9.3/cards/base.py` & `django-cards-0.9.4/cards/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,48 +120,52 @@
             extra_info['datatable_model'] = kwargs.get('datatable_model')
             if group_type == CARD_TYPE_ORDERED_DATATABLE:
                 extra_info['order_field'] = kwargs.get('order_field', 'order')
         elif group_type == CARD_TYPE_HTML:
             extra_info['html'] = kwargs.get('html')
 
     def add_boolean_entry(self, value, label=None, hidden=False, html_override=None,
-                          entry_css_class=None, css_class=None, menu=None, default_if=None, **kwargs):
+                          entry_css_class=None, css_class=None,
+                          menu=None, default_if=None, value_type=None, **kwargs):
         if value:
             entry = self._add_entry_internal(value='<i class="fas fa-check" style="color:green;"></i>',
                                              label=label,
                                              hidden=hidden,
                                              html_override=html_override,
                                              entry_css_class=entry_css_class,
                                              css_class=css_class,
                                              menu=menu,
                                              default_if=default_if,
+                                             value_type=value_type,
                                              **kwargs)
         else:
             entry = self._add_entry_internal(value='<i class="fas fa-times" style="color:red;"></i>',
                                              label=label,
                                              hidden=hidden,
                                              html_override=html_override,
                                              entry_css_class=entry_css_class,
                                              css_class=css_class,
                                              menu=menu,
                                              default_if=default_if,
+                                             value_type=value_type,
                                              **kwargs)
         return entry
 
     def add_date_entry(self, value, label=None, hidden=False, html_override=None,
-                       entry_css_class=None, css_class=None, menu=None, default_if=None, **kwargs):
+                       entry_css_class=None, css_class=None, menu=None, default_if=None, value_type=None, **kwargs):
         new_value = value.strftime('%d/%m/%y')
         return self._add_entry_internal(value=new_value,
                                         label=label,
                                         hidden=hidden,
                                         html_override=html_override,
                                         entry_css_class=entry_css_class,
                                         css_class=css_class,
                                         menu=menu,
                                         default_if=default_if,
+                                        value_type=value_type,
                                         **kwargs)
 
     def add_row(self, *args, extra_row_kwargs=None):
         if extra_row_kwargs is None:
             extra_row_kwargs = {}
         entries = []
         for arg in args:
@@ -254,15 +258,16 @@
 
                     if label is None:
                         label = self.label_from_field(field=field, field_type=field_type)
         return value, label, field_type
 
     def _add_many_to_many_field(self, label, query, query_filter=None, m2m_field=None,
                                 html_barge=None, default='N/A', html_override=None,
-                                entry_css_class=None, css_class=None, menu=None, default_if=None, **kwargs):
+                                entry_css_class=None, css_class=None, menu=None,
+                                default_if=None, value_type=None, **kwargs):
         if html_barge is None:
             html_barge = '<span class="small badge badge-pill badge-primary"> %1% </span> '
 
         if query_filter is None:
             results = query.all()
         else:
             results = query.filter(**query_filter)
@@ -282,14 +287,15 @@
                                         value=html,
                                         default=default,
                                         html_override=html_override,
                                         entry_css_class=entry_css_class,
                                         css_class=css_class,
                                         menu=menu,
                                         default_if=default_if,
+                                        value_type=value_type,
                                         **kwargs)
 
     def _add_entry_internal(self, value=None, field=None, label=None, default='N/A', link=None,
                             hidden=False, hidden_if_blank_or_none=False, html_override=None,
                             value_method=None, value_type=None,
                             entry_css_class=None, css_class=None, menu=None, default_if=None,
                             **kwargs):
@@ -303,32 +309,35 @@
                                           label=label,
                                           hidden=hidden,
                                           html_override=html_override,
                                           entry_css_class=entry_css_class,
                                           css_class=entry_css_class,
                                           menu=menu,
                                           default_if=default_if,
+                                          value_type=value_type,
                                           **kwargs)
         elif isinstance(value, datetime.date):
             return self.add_date_entry(value=value,
                                        label=label,
                                        hidden=hidden,
                                        html_override=html_override,
                                        menu=menu,
                                        default_if=default_if,
+                                       value_type=value_type,
                                        **kwargs)
         elif hasattr(value, 'through'):
             return self._add_many_to_many_field(label=label,
                                                 query=value,
                                                 default=default,
                                                 html_override=html_override,
                                                 entry_css_class=entry_css_class,
                                                 css_class=entry_css_class,
                                                 menu=menu,
                                                 default_if=default_if,
+                                                value_type=value_type,
                                                 **kwargs)
         else:
             if value is None or value == '' or default_if:
                 value = default
                 is_default = True
             else:
                 is_default = False
```

### Comparing `django-cards-0.9.3/cards/card_list/base.py` & `django-cards-0.9.4/cards/card_list/base.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/card_list/main.py` & `django-cards-0.9.4/cards/card_list/main.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/card_list/tree.py` & `django-cards-0.9.4/cards/card_list/tree.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/includes.py` & `django-cards-0.9.4/cards/includes.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/standard.py` & `django-cards-0.9.4/cards/standard.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/32px.png` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/40px.png` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/style.css` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/style.min.css` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/throbber.gif` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/32px.png` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/40px.png` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/style.css` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/style.min.css` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/throbber.gif` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/default-dark/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/30px.png` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/30px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/32px.png` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/style.css` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/style.min.css` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/throbber.gif` & `django-cards-0.9.4/cards/static/cards/jstree/css/themes/proton/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/js/jstree.js` & `django-cards-0.9.4/cards/static/cards/jstree/js/jstree.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/static/cards/jstree/js/jstree.min.js` & `django-cards-0.9.4/cards/static/cards/jstree/js/jstree.min.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/card_group.html` & `django-cards-0.9.4/cards/templates/cards/standard/card_group.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/datatable.html` & `django-cards-0.9.4/cards/templates/cards/standard/datatable.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/default.html` & `django-cards-0.9.4/cards/templates/cards/standard/default.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/default_body.html` & `django-cards-0.9.4/cards/templates/cards/standard/default_body.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/html.html` & `django-cards-0.9.4/cards/templates/cards/standard/html.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/list_selection.html` & `django-cards-0.9.4/cards/templates/cards/standard/list_selection.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/message.html` & `django-cards-0.9.4/cards/templates/cards/standard/message.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/table.html` & `django-cards-0.9.4/cards/templates/cards/standard/table.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/table_body.html` & `django-cards-0.9.4/cards/templates/cards/standard/table_body.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/cards/templates/cards/standard/tree_selection.html` & `django-cards-0.9.4/cards/templates/cards/standard/tree_selection.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/django_cards.egg-info/PKG-INFO` & `django-cards-0.9.4/django_cards.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.9.3
+Version: 0.9.4
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-cards-0.9.3/django_cards.egg-info/SOURCES.txt` & `django-cards-0.9.4/django_cards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.3/setup.py` & `django-cards-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-cards",
-    version="0.9.3",
+    version="0.9.4",
     author="Thomas Turner",
     description="Django app that allows you make cards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-cards",
     include_package_data=True,
     packages=['cards'],
```

