# Comparing `tmp/django-htmx-autocomplete-0.8.2.tar.gz` & `tmp/django-htmx-autocomplete-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-autocomplete-0.8.2.tar", last modified: Fri Jul  7 19:08:45 2023, max compression
+gzip compressed data, was "django-htmx-autocomplete-0.8.3.tar", last modified: Fri Aug  4 19:27:43 2023, max compression
```

## Comparing `django-htmx-autocomplete-0.8.2.tar` & `django-htmx-autocomplete-0.8.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    25303 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-07 19:08:45.000000 django-htmx-autocomplete-0.8.2/autocomplete/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-07 19:08:45.000000 django-htmx-autocomplete-0.8.2/autocomplete/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/static/autocomplete/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/autocomplete/static/autocomplete/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/static/autocomplete/css/autocomplete.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/autocomplete/static/autocomplete/js/
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/static/autocomplete/js/autocomplete.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.444434 django-htmx-autocomplete-0.8.2/autocomplete/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/ac_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/chip.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/chip_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/component.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/head.html
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/indicator-icon.html
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/item.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/item_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/scripts.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/available_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/backspace_instruction.html
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/item_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/more_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/multiselect.html
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/no_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/nothing_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/strings/selected.html
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/textinput.html
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/autocomplete/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/templatetags/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/autocomplete/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/django_htmx_autocomplete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-07 19:08:45.000000 django-htmx-autocomplete-0.8.2/django_htmx_autocomplete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-07 19:08:45.000000 django-htmx-autocomplete-0.8.2/django_htmx_autocomplete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:08:45.000000 django-htmx-autocomplete-0.8.2/django_htmx_autocomplete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 19:08:45.000000 django-htmx-autocomplete-0.8.2/django_htmx_autocomplete.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 19:08:45.000000 django-htmx-autocomplete-0.8.2/django_htmx_autocomplete.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-07 19:08:45.448434 django-htmx-autocomplete-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-07 19:08:22.000000 django-htmx-autocomplete-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.255716 django-htmx-autocomplete-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-08-04 19:27:43.255716 django-htmx-autocomplete-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.251716 django-htmx-autocomplete-0.8.3/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25303 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.247715 django-htmx-autocomplete-0.8.3/autocomplete/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.247715 django-htmx-autocomplete-0.8.3/autocomplete/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.251716 django-htmx-autocomplete-0.8.3/autocomplete/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-04 19:27:43.000000 django-htmx-autocomplete-0.8.3/autocomplete/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.247715 django-htmx-autocomplete-0.8.3/autocomplete/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.251716 django-htmx-autocomplete-0.8.3/autocomplete/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-04 19:27:43.000000 django-htmx-autocomplete-0.8.3/autocomplete/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.247715 django-htmx-autocomplete-0.8.3/autocomplete/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.247715 django-htmx-autocomplete-0.8.3/autocomplete/static/autocomplete/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.251716 django-htmx-autocomplete-0.8.3/autocomplete/static/autocomplete/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/static/autocomplete/css/autocomplete.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.251716 django-htmx-autocomplete-0.8.3/autocomplete/static/autocomplete/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/static/autocomplete/js/autocomplete.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.247715 django-htmx-autocomplete-0.8.3/autocomplete/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.251716 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/ac_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/chip.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/chip_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/component.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/indicator-icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/item_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/scripts.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.255716 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/available_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/backspace_instruction.html
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/item_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/more_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/multiselect.html
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/no_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/nothing_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/strings/selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/textinput.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.255716 django-htmx-autocomplete-0.8.3/autocomplete/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/templatetags/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/autocomplete/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:43.255716 django-htmx-autocomplete-0.8.3/django_htmx_autocomplete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-08-04 19:27:43.000000 django-htmx-autocomplete-0.8.3/django_htmx_autocomplete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-04 19:27:43.000000 django-htmx-autocomplete-0.8.3/django_htmx_autocomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:27:43.000000 django-htmx-autocomplete-0.8.3/django_htmx_autocomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 19:27:43.000000 django-htmx-autocomplete-0.8.3/django_htmx_autocomplete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 19:27:43.000000 django-htmx-autocomplete-0.8.3/django_htmx_autocomplete.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-04 19:27:43.255716 django-htmx-autocomplete-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-04 19:27:15.000000 django-htmx-autocomplete-0.8.3/setup.py
```

### Comparing `django-htmx-autocomplete-0.8.2/LICENSE` & `django-htmx-autocomplete-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/PKG-INFO` & `django-htmx-autocomplete-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-autocomplete
-Version: 0.8.2
+Version: 0.8.3
 Summary: A Django autocomplete component powered by htmx
 Home-page: https://github.com/PHACDataHub/django-htmx-autocomplete
 Author: Luc Belliveau
 Author-email: luc.belliveau@canada.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.8.2 Summary: A
+Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.8.3 Summary: A
 Django autocomplete component powered by htmx Home-page: https://github.com/
 PHACDataHub/django-htmx-autocomplete Author: Luc Belliveau Author-email:
 luc.belliveau@canada.ca License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `django-htmx-autocomplete-0.8.2/README.md` & `django-htmx-autocomplete-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/autocomplete.py` & `django-htmx-autocomplete-0.8.3/autocomplete/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/locale/en/LC_MESSAGES/django.po` & `django-htmx-autocomplete-0.8.3/autocomplete/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/locale/fr/LC_MESSAGES/django.mo` & `django-htmx-autocomplete-0.8.3/autocomplete/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/locale/fr/LC_MESSAGES/django.po` & `django-htmx-autocomplete-0.8.3/autocomplete/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/static/autocomplete/css/autocomplete.css` & `django-htmx-autocomplete-0.8.3/autocomplete/static/autocomplete/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/static/autocomplete/js/autocomplete.js` & `django-htmx-autocomplete-0.8.3/autocomplete/static/autocomplete/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/ac_container.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/ac_container.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/chip.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/chip.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/component.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/component.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/head.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/head.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/indicator-icon.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/indicator-icon.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/item.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/item.html`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,15 @@
     onclick="return phac_aspc_autocomplete_item_click_handler(event)"
     href="#"
     hx-put="{% url route_name method='toggle' %}"
     hx-params="{{ name }},name,item,component_id"
     hx-include="#{{ component_id }}"
     hx-vals='{"name": "{{ name|escapejs }}", "component_id": "{{ component_id|escapejs }}", "item": "{{ item.value|escapejs }}"}'
     hx-swap="outerHTML"
-    {% if swap_oob %}
-    hx-swap-oob="outerHTML:#{{ component_id }}__item__{{ item.value|make_id }}"
-    {% endif %}
+   {% if swap_oob %} hx-swap-oob="outerHTML:#{{ component_id }}__item__{{ item.value|make_id }}" {% else %} hx-target="this" {% endif %}
 >
     {{ item.label|search_highlight:search }}
 </a>
 
 {% if toggle is not None %}
     <div id="{{ component_id }}" hx-swap-oob="true">
         {% include "./values.html" %}
@@ -70,8 +68,8 @@
             {% endif %}
         {% endfor %}
     {% endif %}
     <script data-componentid="{{ component_id }}">
         phac_aspc_autocomplete_trigger_change(document.currentScript.dataset.componentid + '__container');
     </script>
 
-{% endif %}
+{% endif %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% load autocomplete %}
 % if swap_oob %} hx-swap-oob="outerHTML:#{{ component_id }}__item__{
-{ item.value|make_id }}" {% endif %} > {{ item.label|search_highlight:search }}
+{ item.value|make_id }}" {% else %} hx-target="this" {% endif %} > {
+{ item.label|search_highlight:search }}
  {% if toggle is not None %}
 {% include "./values.html" %}
 {% if toggle|length > 0 %} {% for item in toggle %} {% with item=item.label %}
 {% use_string "item_selected" custom_strings %} {% endwith %} {% endfor %} {%
 else %} {% use_string "nothing_selected" custom_strings %} {% endif %}
 {% if multiselect %} {% include "./ac_container.html" with
 selected_items=toggle %}
```

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/item_list.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/item_list.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/scripts.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/scripts.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templates/autocomplete/textinput.html` & `django-htmx-autocomplete-0.8.3/autocomplete/templates/autocomplete/textinput.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/templatetags/autocomplete.py` & `django-htmx-autocomplete-0.8.3/autocomplete/templatetags/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/test_autocomplete.py` & `django-htmx-autocomplete-0.8.3/autocomplete/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/autocomplete/widgets.py` & `django-htmx-autocomplete-0.8.3/autocomplete/widgets.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/django_htmx_autocomplete.egg-info/PKG-INFO` & `django-htmx-autocomplete-0.8.3/django_htmx_autocomplete.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-autocomplete
-Version: 0.8.2
+Version: 0.8.3
 Summary: A Django autocomplete component powered by htmx
 Home-page: https://github.com/PHACDataHub/django-htmx-autocomplete
 Author: Luc Belliveau
 Author-email: luc.belliveau@canada.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.8.2 Summary: A
+Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.8.3 Summary: A
 Django autocomplete component powered by htmx Home-page: https://github.com/
 PHACDataHub/django-htmx-autocomplete Author: Luc Belliveau Author-email:
 luc.belliveau@canada.ca License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `django-htmx-autocomplete-0.8.2/django_htmx_autocomplete.egg-info/SOURCES.txt` & `django-htmx-autocomplete-0.8.3/django_htmx_autocomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.8.2/setup.cfg` & `django-htmx-autocomplete-0.8.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-htmx-autocomplete
-version = 0.8.2
+version = 0.8.3
 description = A Django autocomplete component powered by htmx
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PHACDataHub/django-htmx-autocomplete
 author = Luc Belliveau
 author_email = luc.belliveau@canada.ca
 license = MIT
```

### Comparing `django-htmx-autocomplete-0.8.2/setup.py` & `django-htmx-autocomplete-0.8.3/setup.py`

 * *Files identical despite different names*

