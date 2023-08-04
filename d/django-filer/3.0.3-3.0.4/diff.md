# Comparing `tmp/django-filer-3.0.3.tar.gz` & `tmp/django-filer-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-filer-3.0.3.tar", last modified: Fri Jul 21 13:47:02 2023, max compression
+gzip compressed data, was "django-filer-3.0.4.tar", last modified: Fri Aug  4 18:35:27 2023, max compression
```

## Comparing `django-filer-3.0.3.tar` & `django-filer-3.0.4.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-21 13:46:52.000000 django-filer-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-21 13:46:52.000000 django-filer-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-21 13:47:02.489183 django-filer-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-21 13:46:52.000000 django-filer-3.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.449180 django-filer-3.0.3/django_filer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.449180 django-filer-3.0.3/filer/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.449180 django-filer-3.0.3/filer/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/clipboardadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/fileadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    57077 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/folderadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/imageadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/admin/patched/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/patched/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/permissionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/thumbnailoptionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/contrib/django_cms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/contrib/django_cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/contrib/django_cms/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/multistorage_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31052 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30552 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36871 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37978 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31970 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31106 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36774 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    39279 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36970 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30439 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37572 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30912 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35169 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30709 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37766 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    41615 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30834 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/vi_VN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    38041 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/zh-Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30452 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/commands/filer_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/commands/generate_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/commands/import_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.469181 django-filer-3.0.3/filer/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0002_auto_20150606_2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0003_thumbnailoption.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0004_auto_20160328_1434.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0005_auto_20160623_1425.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0006_auto_20160623_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0007_auto_20161016_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0008_auto_20171117_1313.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0009_auto_20171220_1635.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0010_auto_20180414_2058.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0011_auto_20190418_0137.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0012_file_mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0013_image_width_height_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0014_folder_permission_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0017_image__transparent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.469181 django-filer-3.0.3/filer/models/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/clipboardmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/filemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/foldermodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/imagemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/thumbnailoptionmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/virtualitems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.469181 django-filer-3.0.3/filer/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.469181 django-filer-3.0.3/filer/server/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/xsendfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/main_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/thumbnails_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/static/filer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.473182 django-filer-3.0.3/filer/static/filer/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/admin_filer.cms.icons.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    91187 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/admin_filer.css
--rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/admin_filer.fa.icons.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/admin_folderpermissions.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.473182 django-filer-3.0.3/filer/static/filer/css/maps/
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.cms.icons.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    87138 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    65841 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.fa.icons.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.icons.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.473182 django-filer-3.0.3/filer/static/filer/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.477182 django-filer-3.0.3/filer/static/filer/fonts/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/expand.svg
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/move-to-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/remove-selection.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/select.svg
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/th-large.svg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/th-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.477182 django-filer-3.0.3/filer/static/filer/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/cloud-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-zip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/folder-dropdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/folder-root.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/folder-unfiled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/folder.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.481182 django-filer-3.0.3/filer/static/filer/img/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/button-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/close.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/icon_changelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/icon_deletelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/loading_animation.gif
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/nav-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/select_item-hover.gif
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/select_item.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/upload_button.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.481182 django-filer-3.0.3/filer/static/filer/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.481182 django-filer-3.0.3/filer/static/filer/js/addons/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/copy-move-files.js
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/dropdown-menu.js
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/dropzone.init.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/filer_popup_response.js
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/focal-point.js
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/popup_handling.js
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/table-dropzone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/toggler.js
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/tooltip.js
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/upload-button.js
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/static/filer/js/libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/class.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/dropzone.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/fileuploader.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/jquery.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/mediator.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/delete_selected_files_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/dismiss_popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/file/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/file/popup_response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/folder/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/choose_copy_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/choose_images_resize_options.html
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/choose_move_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/choose_rename_format.html
--rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/directory_listing.html
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/directory_table_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/directory_thumbnail_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/list_type_switcher.html
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/new_folder_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/image/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/templatetags/file_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/clipboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/tools/detail_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/tools/search_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/filer/templates/admin/filer/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/widgets/admin_file.html
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/widgets/admin_folder.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templatetags/filer_admin_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templatetags/filer_image_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templatetags/filer_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/thumbnail_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/filer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/filer_easy_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/generate_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/model_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/pil_exif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/recursive_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 13:47:02.489183 django-filer-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-21 13:46:52.000000 django-filer-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.552956 django-filer-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-04 18:35:12.000000 django-filer-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-04 18:35:12.000000 django-filer-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-08-04 18:35:27.552956 django-filer-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-04 18:35:12.000000 django-filer-3.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.508953 django-filer-3.0.4/django_filer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-08-04 18:35:27.000000 django-filer-3.0.4/django_filer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-08-04 18:35:27.000000 django-filer-3.0.4/django_filer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:35:27.000000 django-filer-3.0.4/django_filer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:35:27.000000 django-filer-3.0.4/django_filer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-04 18:35:27.000000 django-filer-3.0.4/django_filer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 18:35:27.000000 django-filer-3.0.4/django_filer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.508953 django-filer-3.0.4/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.508953 django-filer-3.0.4/filer/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/clipboardadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/fileadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57077 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/folderadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/imageadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.508953 django-filer-3.0.4/filer/admin/patched/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/patched/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/permissionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/thumbnailoptionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.508953 django-filer-3.0.4/filer/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.512953 django-filer-3.0.4/filer/contrib/django_cms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/contrib/django_cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/contrib/django_cms/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.512953 django-filer-3.0.4/filer/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/fields/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/fields/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/fields/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/fields/multistorage_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.512953 django-filer-3.0.4/filer/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.492952 django-filer-3.0.4/filer/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.512953 django-filer-3.0.4/filer/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31124 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.492952 django-filer-3.0.4/filer/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.512953 django-filer-3.0.4/filer/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.492952 django-filer-3.0.4/filer/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.512953 django-filer-3.0.4/filer/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37042 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.512953 django-filer-3.0.4/filer/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37178 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.512953 django-filer-3.0.4/filer/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    39624 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36803 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    39587 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32039 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34611 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31181 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36936 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    39882 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31737 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37078 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36072 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.516954 django-filer-3.0.4/filer/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37190 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37673 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.496952 django-filer-3.0.4/filer/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30522 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37749 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30987 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/lt_LT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    38931 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/nl_NL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/nn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35248 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37787 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.520954 django-filer-3.0.4/filer/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30781 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37955 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    41750 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30906 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33090 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    38200 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30507 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/zh-Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/zh-Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/zh-Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/zh-Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30521 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.500953 django-filer-3.0.4/filer/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30522 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.524954 django-filer-3.0.4/filer/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.528954 django-filer-3.0.4/filer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/management/commands/filer_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/management/commands/generate_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/management/commands/import_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.528954 django-filer-3.0.4/filer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0002_auto_20150606_2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0003_thumbnailoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0004_auto_20160328_1434.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0005_auto_20160623_1425.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0006_auto_20160623_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0007_auto_20161016_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0008_auto_20171117_1313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0009_auto_20171220_1635.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0010_auto_20180414_2058.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0011_auto_20190418_0137.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0012_file_mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0013_image_width_height_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0014_folder_permission_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/0017_image__transparent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.532955 django-filer-3.0.4/filer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/clipboardmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/filemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/foldermodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/imagemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/thumbnailoptionmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/models/virtualitems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.532955 django-filer-3.0.4/filer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.532955 django-filer-3.0.4/filer/server/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/backends/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/backends/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/backends/xsendfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/main_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/thumbnails_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.504953 django-filer-3.0.4/filer/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.504953 django-filer-3.0.4/filer/static/filer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.532955 django-filer-3.0.4/filer/static/filer/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/css/admin_filer.cms.icons.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91187 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/css/admin_filer.css
+-rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/css/admin_filer.fa.icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/css/admin_folderpermissions.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.532955 django-filer-3.0.4/filer/static/filer/css/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/css/maps/admin_filer.cms.icons.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    87138 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/css/maps/admin_filer.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    65841 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/css/maps/admin_filer.fa.icons.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/css/maps/admin_filer.icons.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.536955 django-filer-3.0.4/filer/static/filer/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.540955 django-filer-3.0.4/filer/static/filer/fonts/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/move-to-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/remove-selection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/select.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/th-large.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/th-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/fonts/src/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.540955 django-filer-3.0.4/filer/static/filer/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/cloud-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/file-zip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/folder-dropdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/folder-root.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/folder-unfiled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/icons/folder.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.540955 django-filer-3.0.4/filer/static/filer/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/button-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/close.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/icon_changelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/icon_deletelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/loading_animation.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/nav-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/select_item-hover.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/select_item.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/img/upload_button.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.540955 django-filer-3.0.4/filer/static/filer/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.544955 django-filer-3.0.4/filer/static/filer/js/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/copy-move-files.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/dropdown-menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/dropzone.init.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/filer_popup_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/focal-point.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/popup_handling.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/table-dropzone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/toggler.js
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/tooltip.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/upload-button.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/addons/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.544955 django-filer-3.0.4/filer/static/filer/js/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/libs/class.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/libs/dropzone.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/libs/fileuploader.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/libs/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/libs/jquery.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/libs/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/static/filer/js/libs/mediator.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.504953 django-filer-3.0.4/filer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.504953 django-filer-3.0.4/filer/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.548956 django-filer-3.0.4/filer/templates/admin/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/delete_selected_files_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/dismiss_popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.548956 django-filer-3.0.4/filer/templates/admin/filer/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/file/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/file/popup_response.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.548956 django-filer-3.0.4/filer/templates/admin/filer/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/choose_copy_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/choose_images_resize_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/choose_move_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/choose_rename_format.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/directory_listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/directory_table_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/directory_thumbnail_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/list_type_switcher.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/folder/new_folder_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.548956 django-filer-3.0.4/filer/templates/admin/filer/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/image/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.548956 django-filer-3.0.4/filer/templates/admin/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/templatetags/file_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.548956 django-filer-3.0.4/filer/templates/admin/filer/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.548956 django-filer-3.0.4/filer/templates/admin/filer/tools/clipboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/tools/clipboard/clipboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/tools/detail_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/tools/search_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.548956 django-filer-3.0.4/filer/templates/admin/filer/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/widgets/admin_file.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templates/admin/filer/widgets/admin_folder.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.552956 django-filer-3.0.4/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templatetags/filer_admin_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templatetags/filer_image_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/templatetags/filer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/thumbnail_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:27.552956 django-filer-3.0.4/filer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/filer_easy_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/generate_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/model_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/pil_exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/recursive_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/utils/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-04 18:35:12.000000 django-filer-3.0.4/filer/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-04 18:35:27.552956 django-filer-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-04 18:35:12.000000 django-filer-3.0.4/setup.py
```

### Comparing `django-filer-3.0.3/LICENSE` & `django-filer-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/PKG-INFO` & `django-filer-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.0.3
+Version: 3.0.4
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `django-filer-3.0.3/README.rst` & `django-filer-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/django_filer.egg-info/PKG-INFO` & `django-filer-3.0.4/django_filer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.0.3
+Version: 3.0.4
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `django-filer-3.0.3/django_filer.egg-info/SOURCES.txt` & `django-filer-3.0.4/django_filer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/__init__.py` & `django-filer-3.0.4/filer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,10 +9,8 @@
  5. git push
  6. Assure that all tests pass on https://github.com/django-cms/django-filer/actions
  7. Create a new release on github. Create the new tag against the latest master commit and auto generate
     the release notes https://github.com/django-cms/django-filer/releases/new
  8. Publish the release and it will automatically release to pypi
 """
 
-__version__ = '3.0.3'
-
-default_app_config = 'filer.apps.FilerConfig'
+__version__ = '3.0.4'
```

### Comparing `django-filer-3.0.3/filer/admin/__init__.py` & `django-filer-3.0.4/filer/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/admin/clipboardadmin.py` & `django-filer-3.0.4/filer/admin/clipboardadmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         data = {
             'thumbnail': thumbnail,
             'alt_text': '',
             'label': str(file_obj),
             'file_id': file_obj.pk,
         }
         # prepare preview thumbnail
-        if type(file_obj) == Image:
+        if isinstance(file_obj, Image):
             thumbnail_180_options = {
                 'size': (180, 180),
                 'crop': True,
                 'upscale': True,
             }
             thumbnail_180 = file_obj.file.get_thumbnail(
                 thumbnail_180_options)
```

### Comparing `django-filer-3.0.3/filer/admin/fileadmin.py` & `django-filer-3.0.4/filer/admin/fileadmin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from django import forms
 from django.contrib.admin.utils import unquote
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.http import Http404, HttpResponse, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.urls import path, reverse
 from django.utils.safestring import mark_safe
+from django.utils.timezone import now
 from django.utils.translation import gettext as _
 
 from easy_thumbnails.exceptions import InvalidImageFormatError
 from easy_thumbnails.files import get_thumbnailer
+from easy_thumbnails.models import Thumbnail as EasyThumbnail
 from easy_thumbnails.options import ThumbnailOptions
 
 from .. import settings
 from ..models import BaseImage, File
 from ..settings import DEFERRED_THUMBNAIL_SIZES
 from .permissions import PrimitivePermissionAwareModelAdmin
 from .tools import AdminContext, admin_url_params_encoded, popup_status
@@ -176,13 +178,15 @@
         if not isinstance(file, BaseImage):
             raise Http404()
 
         try:
             thumbnailer = get_thumbnailer(file)
             thumbnail_options = ThumbnailOptions({'size': (size, size), "crop": True})
             thumbnail = thumbnailer.get_thumbnail(thumbnail_options, generate=True)
+            # Touch thumbnail to allow it to be prefetched for directory listing
+            EasyThumbnail.objects.filter(name=thumbnail.name).update(modified=now())
             return HttpResponseRedirect(thumbnail.url)
         except InvalidImageFormatError:
             return HttpResponseRedirect(staticfiles_storage.url('filer/icons/file-missing.svg'))
 
 
 FileAdmin.fieldsets = FileAdmin.build_fieldsets()
```

### Comparing `django-filer-3.0.3/filer/admin/folderadmin.py` & `django-filer-3.0.4/filer/admin/folderadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/admin/forms.py` & `django-filer-3.0.4/filer/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/admin/imageadmin.py` & `django-filer-3.0.4/filer/admin/imageadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/admin/patched/admin_utils.py` & `django-filer-3.0.4/filer/admin/patched/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/admin/permissionadmin.py` & `django-filer-3.0.4/filer/admin/permissionadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/admin/permissions.py` & `django-filer-3.0.4/filer/admin/permissions.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/admin/tools.py` & `django-filer-3.0.4/filer/admin/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/admin/views.py` & `django-filer-3.0.4/filer/admin/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/apps.py` & `django-filer-3.0.4/filer/apps.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/contrib/django_cms/cms_toolbars.py` & `django-filer-3.0.4/filer/contrib/django_cms/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/fields/file.py` & `django-filer-3.0.4/filer/fields/file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/fields/folder.py` & `django-filer-3.0.4/filer/fields/folder.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/fields/multistorage_file.py` & `django-filer-3.0.4/filer/fields/multistorage_file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/sk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Arabic (http://app.transifex.com/divio/django-filer/language/ar/)\n"
+"Language-Team: Slovak (http://app.transifex.com/divio/django-filer/language/"
+"sk/)\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ar\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -52,16 +51,14 @@
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
-msgstr[4] ""
-msgstr[5] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -245,27 +242,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -287,15 +284,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -317,15 +314,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -340,152 +337,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -522,27 +533,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -579,24 +587,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -641,38 +649,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -698,15 +706,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -739,31 +747,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -782,71 +790,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -881,28 +889,24 @@
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
-msgstr[4] ""
-msgstr[5] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
-msgstr[4] ""
-msgstr[5] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -939,21 +943,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1007,20 +1009,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1032,16 +1032,14 @@
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
-msgstr[4] ""
-msgstr[5] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1081,16 +1079,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1138,15 +1135,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1207,12 +1203,10 @@
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
 #~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
 #~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
 #~ msgstr[3] "15c0f2d28d6dab1af1f6d94906beb627_pl_3"
-#~ msgstr[4] "15c0f2d28d6dab1af1f6d94906beb627_pl_4"
-#~ msgstr[5] "15c0f2d28d6dab1af1f6d94906beb627_pl_5"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.3/filer/locale/bg/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Bulgarian (http://app.transifex.com/divio/django-filer/language/bg/)\n"
+"Language-Team: Lithuanian (Lithuania) (http://app.transifex.com/divio/django-"
+"filer/language/lt_LT/)\n"
+"Language: lt_LT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: bg\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
+"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
+"1 : n % 1 != 0 ? 2: 3);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -50,14 +50,16 @@
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -241,27 +243,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -283,15 +285,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -313,15 +315,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -336,152 +338,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -518,27 +534,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -575,24 +588,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -637,38 +650,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -694,15 +707,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -735,31 +748,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -778,71 +791,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -875,22 +888,26 @@
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -927,21 +944,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -995,20 +1010,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1018,14 +1031,16 @@
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1065,16 +1080,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1122,15 +1136,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1189,10 +1202,12 @@
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
 #~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
+#~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
+#~ msgstr[3] "15c0f2d28d6dab1af1f6d94906beb627_pl_3"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/ca/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Roger Pons <rogerpons@gmail.com>, 2013-2014,2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Roger Pons <rogerpons@gmail.com>, 2013-2014,2016\n"
-"Language-Team: Catalan (http://app.transifex.com/divio/django-filer/language/ca/)\n"
+"Language-Team: Catalan (http://app.transifex.com/divio/django-filer/language/"
+"ca/)\n"
+"Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Avançat"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "URL canònica"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Cal seleccionar els elements en ordre per tal de realitzar accions sobre ells. No s'ha modificat cap element."
+msgstr ""
+"Cal seleccionar els elements en ordre per tal de realitzar accions sobre "
+"ells. No s'ha modificat cap element."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s seleccionat"
 msgstr[1] "Tots %(total_count)s seleccionats"
@@ -124,15 +124,16 @@
 msgstr "Ja existeixen carpetes amb els noms %s a la destinació seleccionada"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "S'han mogut %(count)d fitxers i/o carpetes a la carpeta '%(destination)s'"
+msgstr ""
+"S'han mogut %(count)d fitxers i/o carpetes a la carpeta '%(destination)s'"
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Moure fitxers i/o carpetes"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -149,15 +150,16 @@
 msgstr "Canviar el nom a fitxers"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "S'han copiat %(count)d fitxeres i/o carpetes a la carpeta '%(destination)s'."
+msgstr ""
+"S'han copiat %(count)d fitxeres i/o carpetes a la carpeta '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copiar fitxers i/o carpetes"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -181,15 +183,17 @@
 msgstr "Sufix que serà afegit als noms de fitxer dels fitxers copiats"
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "El sufix ha de ser una part de nom de fitxer vàlida, simple i en minúscules, com ara \"%(valid)s\"."
+msgstr ""
+"El sufix ha de ser una part de nom de fitxer vàlida, simple i en minúscules, "
+"com ara \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Format de renombrat amb valor de clau \"%(key)s\" desconegut."
 
 #: admin/forms.py:54
@@ -242,27 +246,27 @@
 msgstr "La ubicació del subjecte està fora de la imatge."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "La teva entrada: \"{subject_location}\"."
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Ja existeix una carpeta amb aquest nom."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -284,15 +288,15 @@
 msgid "image"
 msgstr "imatge"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "imatges"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "usuari"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "fitxers"
 
@@ -314,15 +318,15 @@
 msgstr "element del portapapers"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "elements del portapapers"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "carpeta"
 
 #: models/filemodels.py:81
@@ -337,152 +341,168 @@
 msgid "has all mandatory data"
 msgstr "té totes les dades obligatòries"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "nom de fitxer original"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nom"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "descripció"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "propietari"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "pujat a"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "modificat a"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Permisos desactivats"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Desactiveu tots els permisos d'aquest fitxer. Aquest serà accessible de forma pública per a tothom."
+msgstr ""
+"Desactiveu tots els permisos d'aquest fitxer. Aquest serà accessible de "
+"forma pública per a tothom."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "creat a"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Carpeta"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Carpetes"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "tots els elements"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "només aquest element"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "aquest elements i els seus fills"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "permetre"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "denegar"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tipus"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "group"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "tothom"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "pot llegir"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "pot editar"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "pot afegir fills"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "permís de carpeta"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "permisos de carpeta"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data agafada"
 
@@ -519,27 +539,24 @@
 msgid "Unsorted Uploads"
 msgstr "Pujades sense ordre"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "fitxer als que els falten metadades"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "arrel"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Executar l'acció seleccionada"
 
@@ -547,15 +564,16 @@
 msgid "Go"
 msgstr "Anar"
 
 #: templates/admin/filer/actions.html:14
 #: templates/admin/filer/folder/directory_table_list.html:232
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 msgid "Click here to select the objects across all pages"
-msgstr "Cliqueu aquí per seleccionar els objectes a través de totes les pàgines"
+msgstr ""
+"Cliqueu aquí per seleccionar els objectes a través de totes les pàgines"
 
 #: templates/admin/filer/actions.html:14
 #, python-format
 msgid "Select all %(total_count)s files and/or folders"
 msgstr "Seleccionar tots els %(total_count)s fitixers i/o carpetes"
 
 #: templates/admin/filer/actions.html:16
@@ -576,50 +594,57 @@
 msgstr "Inici"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Tornar a l'aplicació Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Tornar a la carpeta arrel"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Tornar a la carpeta '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplicats"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Esborrar els fitxers seleccionats provocarà l'esborrar d'objectes relacionats, però el teu compte no té permisos per esborrar els següents tipus d'objectes:"
+msgstr ""
+"Esborrar els fitxers seleccionats provocarà l'esborrar d'objectes "
+"relacionats, però el teu compte no té permisos per esborrar els següents "
+"tipus d'objectes:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Esborrer els fitxers i/o carpetes seleccionades provocarà l'esborrat dels següents objectes protegits relacionats:"
+msgstr ""
+"Esborrer els fitxers i/o carpetes seleccionades provocarà l'esborrat dels "
+"següents objectes protegits relacionats:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Segur que voleu esborrar els fitxers i/o carpetes seleccionades? Els següents objectes i els seus elements relacionats seran esborrats:"
+msgstr ""
+"Segur que voleu esborrar els fitxers i/o carpetes seleccionades? Els "
+"següents objectes i els seus elements relacionats seran esborrats:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "No, porta'm enrere."
 
@@ -638,38 +663,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Veure al lloc"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Tornar a"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "pàgina principal d'administració"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Icona de la carpeta"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr "Sense permisos per copiar tots els fitxers i/o carpetes seleccionats."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -686,164 +711,182 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "No hi ha fitxers i/o carpetes disponibles."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Els següents fitxers i/o carpetes seran copiats a una carpeta de destí (mantenint la seva estructura d'arbre):"
+msgstr ""
+"Els següents fitxers i/o carpetes seran copiats a una carpeta de destí "
+"(mantenint la seva estructura d'arbre):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Carpeta de destí:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Copiar"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "No està permès copiar fitxers a la mateixa carpeta"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "El vostre compte no té permisos per redimensionar totes les imatges seleccionades."
+msgstr ""
+"El vostre compte no té permisos per redimensionar totes les imatges "
+"seleccionades."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "No hi ha imatges disponibles per redimensionar."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Les següents imatges seran redimensionades:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Trieu una opció de miniatura existent o especifiqueu paràmetres de redimensionat:"
+msgstr ""
+"Trieu una opció de miniatura existent o especifiqueu paràmetres de "
+"redimensionat:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Trieu els paràmetres de redimensionat:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Avís: les imatges seran redimensionades al mateix lloc i les originals es perdran. Considereu realitzar abans una còpia d'aquestes per mantenir els originals."
+msgstr ""
+"Avís: les imatges seran redimensionades al mateix lloc i les originals es "
+"perdran. Considereu realitzar abans una còpia d'aquestes per mantenir els "
+"originals."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Redimensionar"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "El vostre compte no té permisos per moure tots els fitxers i/o carpetes seleccionats."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"El vostre compte no té permisos per moure tots els fitxers i/o carpetes "
+"seleccionats."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "No hi ha fitxers i/o carpetes disponibles per moure."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Els següents fitxers i/o carpetes seran moguts a una carpeta de destí (mantenint la seva estructura d'arbre):"
+msgstr ""
+"Els següents fitxers i/o carpetes seran moguts a una carpeta de destí "
+"(mantenint la seva estructura d'arbre):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Moure"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "No està permès moure fitxers a la mateixa carpeta"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "El vostre compte no té permisos per canviar el nom de tots els fitxers seleccionats."
+msgstr ""
+"El vostre compte no té permisos per canviar el nom de tots els fitxers "
+"seleccionats."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "No hi ha fitxers per canviar el nom disponibles."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "En canviarà el nom dels següents fitxers (seguiran estant a les seves carpetes i mantindran el seu nom de fitxers original, només serà modificat el nom que es mostrarà):"
+msgstr ""
+"En canviarà el nom dels següents fitxers (seguiran estant a les seves "
+"carpetes i mantindran el seu nom de fitxers original, només serà modificat "
+"el nom que es mostrarà):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Canviar el nom"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Tornar a la carpeta pare"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Modificar els detalls de la carpeta actual"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Modificar"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Cliqueu aquí per cercar la frase introduïda"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Cercar"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Tancar"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limitar"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Marqueu per limitar la cercar a la carpeta actual"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Limitar la cerca a la carpeta actual"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Esborrar"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Afegir una Carpeta nova"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Carpeta nova"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Pujar Arxius"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Cal que abans seleccioneu una carpeta"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Nom"
 
@@ -928,21 +971,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "activat"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Esborrar fitxer"
 
@@ -996,20 +1037,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Seleccionar tots/es %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Afegir nou"
@@ -1066,16 +1105,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipus"
 
@@ -1123,15 +1161,14 @@
 msgstr "Cercar"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Escollir Fitxer"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Jakub Dorňák <jakub.dornak@misli.cz>, 2020
 # Mirek Simek <miroslav.simek@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Jakub Dorňák <jakub.dornak@misli.cz>, 2020\n"
-"Language-Team: Czech (http://app.transifex.com/divio/django-filer/language/cs/)\n"
+"Language-Team: Czech (http://app.transifex.com/divio/django-filer/language/"
+"cs/)\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: cs\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Pokročilé"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "kanonický odkaz"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -127,15 +126,17 @@
 msgstr "Složky pojmenované %s již v cílové složce existují"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Vybrané soubory a/nebo složky (%(count)d) byly přesunuty do složky '%(destination)s'."
+msgstr ""
+"Vybrané soubory a/nebo složky (%(count)d) byly přesunuty do složky "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Přesunout soubory a/nebo složky"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -152,15 +153,17 @@
 msgstr "Přejmenovat soubory"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Soubory a/nebo složky (%(count)d) byly zkopírovány do složky '%(destination)s'."
+msgstr ""
+"Soubory a/nebo složky (%(count)d) byly zkopírovány do složky "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopírovat soubory a/nebo složky"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -184,15 +187,17 @@
 msgstr "Koncovka, která bude přidána ke jménům kopírovaných souborů."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Koncovka by měla být jednoduchá součást názvu souboru malými písmeny, například \"%(valid)s\"."
+msgstr ""
+"Koncovka by měla být jednoduchá součást názvu souboru malými písmeny, "
+"například \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Neznámý formát klíče pro přejmenování \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -218,15 +223,17 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "zvětšit"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr "Musíte vybrat předdefinované volby náhledu nebo nastavit jednotlivé parametry."
+msgstr ""
+"Musíte vybrat předdefinované volby náhledu nebo nastavit jednotlivé "
+"parametry."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Parametry pro změny velikosti musí být vybrány."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -245,27 +252,27 @@
 msgstr "Zadaná pozice objektu je mimo obrázek. "
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Vaše zadání: \"{subject_location}\". "
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Složka s tímto názvem již existuje."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Správce souborů"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -287,15 +294,15 @@
 msgid "image"
 msgstr "obrázek"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "obrázky"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "uživatel"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "soubory"
 
@@ -317,15 +324,15 @@
 msgstr "položka schránky"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "položky schránky"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "složka"
 
 #: models/filemodels.py:81
@@ -340,152 +347,168 @@
 msgid "has all mandatory data"
 msgstr "má všechna povinná data"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "původní název souboru"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "název"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "popis"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "vlastník"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "nahráno"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "změněno"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Oprávnění neaktivní"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Deaktivovat veškerá oprávnění pro tento soubor. Soubor bude komukoli veřejně dostupný."
+msgstr ""
+"Deaktivovat veškerá oprávnění pro tento soubor. Soubor bude komukoli veřejně "
+"dostupný."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "vytvořeno"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Složka"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Složky"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "všechny položky"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "pouze tato položka"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "tato položka včetně všech potomků"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "povolit"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "zakázat"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "typ"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "skupina"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "kdokoli"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "smí číst"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "smí upravit"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "smí přidávat potomky"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "oprávnění složky"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "oprávnění složky"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "datum pořízení"
 
@@ -522,27 +545,24 @@
 msgid "Unsorted Uploads"
 msgstr "Nezařazené"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "soubory s chybějícími informacemi"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "kořenová složka"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Provést vybranou operaci"
 
@@ -579,50 +599,57 @@
 msgstr "Hlavní stránka"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Přejít zpět do Správce souborů"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Přejít zpět do kořenové složky"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Přejít zpět do složky '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplicity"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Smazání vybraných souborů a/nebo složek bude mít za následek smazání všech přidružených objektů, nicméně ke smazání následujících objektů nemáte oprávnění:"
+msgstr ""
+"Smazání vybraných souborů a/nebo složek bude mít za následek smazání všech "
+"přidružených objektů, nicméně ke smazání následujících objektů nemáte "
+"oprávnění:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Smazání vybraných souborů a/nebo složek bude mít za následek smazání následujících přidružených objektů:"
+msgstr ""
+"Smazání vybraných souborů a/nebo složek bude mít za následek smazání "
+"následujících přidružených objektů:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Opravdu chcete smazat vybrané soubory a složky? Všechny následující objekty budou smazány:"
+msgstr ""
+"Opravdu chcete smazat vybrané soubory a složky? Všechny následující objekty "
+"budou smazány:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Ne, chci zpátky"
 
@@ -641,38 +668,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Zobrazit na webu"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Vrátit se do"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "hlavní stránka administrace"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Ikona složky"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr "Nemáte oprávnění kopírovat vybrané soubory a/nebo složky."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -689,24 +716,26 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Žádné soubory ani složky není možno kopírovat."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Následující soubory a/nebo složky budou zkopírovány do cílové slžoky (jejich stromová struktura bude zachována):"
+msgstr ""
+"Následující soubory a/nebo složky budou zkopírovány do cílové slžoky (jejich "
+"stromová struktura bude zachována):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Cílová složka:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopírovat"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Není možné kopírovat soubory do stejné složky"
 
@@ -721,49 +750,55 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Následujícím obrázkům bude změněna velikost:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Vyberte existující volby náhledu nebo zadejte parametry změny velikosti:"
+msgstr ""
+"Vyberte existující volby náhledu nebo zadejte parametry změny velikosti:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Vyberte parametry změny velikosti:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Varování: Bude změněna velikost obrázků a původní obrázky budou přepsány. Pokud chcete zachovat obrázky v původní velikosti, nejdříve vytvořte jejich kopie."
+msgstr ""
+"Varování: Bude změněna velikost obrázků a původní obrázky budou přepsány. "
+"Pokud chcete zachovat obrázky v původní velikosti, nejdříve vytvořte jejich "
+"kopie."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Změnit velikost"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr "Nemáte oprávnění k přesunu vybraných souborů nebo složek."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Žádné soubory k přesunutí."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Následující soubory a/nebo složky budou přesunyty do cílové složky (jejich stromová struktura bude zachována)"
+msgstr ""
+"Následující soubory a/nebo složky budou přesunyty do cílové složky (jejich "
+"stromová struktura bude zachována)"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Přesunout"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Není možné přesouvat soubory do stejné složky"
 
@@ -776,77 +811,78 @@
 msgid "There are no files available to rename."
 msgstr "Žádné soubory k přejmenování."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Následující soubory budou přejmenovány (změněno bude pouze zobrazované jméno)"
+msgstr ""
+"Následující soubory budou přejmenovány (změněno bude pouze zobrazované jméno)"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Přejmenovat"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Přejít zpět do nadřazené složky"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Upravit aktuální složku"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Upravit"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Klikněte sem pro vyhledání zadaného výrazu"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Hledat"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Zavřít"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Omezit"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Zaškrtněte pro omezení hledání na aktuální složku"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Omezit hledání na aktuální složku"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Smazat"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Přidá novou složku"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Nová složka"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Nahrát soubory"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Nejdříve musíte vybrat složku"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Název"
 
@@ -935,21 +971,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "aktivní"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Kanonický odkaz '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Stáhnout '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Smazat soubor"
 
@@ -1003,20 +1037,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Vybrat všechny (%(total_count)s)"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Přidat"
@@ -1075,16 +1107,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Typ"
 
@@ -1132,15 +1163,14 @@
 msgstr "Vyhledat"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Vybrat soubor"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/de/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/de/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Mitja Martini <mitja.martini@t-online.de>, 2012
 # Peter Wischer <peter.wischer@lwl.org>, 2018
 # Stefan Foulis <stefan.foulis@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Fabian Braun <fsbraun@gmx.de>, 2023\n"
 "Language-Team: German (http://app.transifex.com/divio/django-filer/language/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de\n"
@@ -37,19 +37,19 @@
 msgstr "Ich kann den Zielordner nicht finden. Bitter lade die Seite neu und versuche es noch einmal."
 
 #: admin/clipboardadmin.py:19
 msgid ""
 "Can't use this folder, Permission Denied. Please select another folder."
 msgstr "Zugriff auf diesen Ordner verweigert. Bitte wähle einen anderen Ordner."
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Fortgeschritten"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "Kanonische URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -248,27 +248,27 @@
 msgstr "Angegebene Position des Hauptinhalts liegt außerhalb des Bildes."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Deine Eingabe: \"{subject_location}\". "
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr "Wer"
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr "Was"
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Dieser Ordnername wird bereits verwendet."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -290,15 +290,15 @@
 msgid "image"
 msgstr "Bild"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "Bilder"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "Benutzer"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "Dateien"
 
@@ -320,15 +320,15 @@
 msgstr "Eintrag der Zwischenablage"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "Einträge der Zwischenablage"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "Ordner"
 
 #: models/filemodels.py:81
@@ -343,151 +343,168 @@
 msgid "has all mandatory data"
 msgstr "hat alle Pflichtinhalte"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "ursprünglicher Dateiname"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "Name"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "Beschreibung"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "Besitzer"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "Hochgeladen am"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "Verändert am"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Berechtigungen deaktiviert"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr "Zugriffskontrolle für diese Datei deaktivieren. Die Datei wird für jeden öffentlich zugreifbar sein."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr "Übergeordneter Ordner"
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "Angelegt am"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Ordner"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Ordner"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "alle Einträge"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "nur dieser Eintrag"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "dieser Eintrag und alle darunter liegenden Einträge"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr "vererben"
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "erlauben"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "verbieten"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "Typ"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "Gruppe"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "Jeder"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "kann lesen"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "kann ändern"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "kann Kinder hinzufügen"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "Ordnerberechtigung"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "Ordnerberechtigungen"
 
-#: models/foldermodels.py:359
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr "Für den Typ \"Alle Einträge\" kann kein Ordner ausgewählt werden. "
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr "Für alle Typen außer \"Alle Einträge\" muss ein Ordner ausgewählt werden."
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr "Zusammen mit \"Jeder\" kann kein Benutzer oder eine Gruppe ausgewählt werden."
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr "Mindestens ein Eintrag muss gewählt werden: \"Benutzer\", \"Gruppe\" oder \"Jeder\"."
+
+#: models/foldermodels.py:360
 #| msgid "Folders"
 msgid "All Folders"
 msgstr "Alle Ordner"
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr "Logischer Pfad"
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr "Nutzer: {user}"
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr "Gruppe: {group}"
 
-#: models/foldermodels.py:374
+#: models/foldermodels.py:375
 #| msgid "everybody"
 msgid "Everybody"
 msgstr "Jede(r)"
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr "Edit"
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr "Lesen"
 
-#: models/foldermodels.py:389
+#: models/foldermodels.py:390
 #| msgid "can add children"
 msgid "Add children"
 msgstr "Unterordner hinzufügen"
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "Aufgenommen am"
@@ -525,18 +542,16 @@
 msgid "Unsorted Uploads"
 msgstr "Nicht sortierte Uploads"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "Dateien mit fehlenden Metadaten"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "Start"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr "Tabellenansicht"
 
@@ -582,24 +597,24 @@
 msgstr "Startseite"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Zur Filer App zurück gehen"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Zum Root Ordner zurück gehen"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Zum Ordner '%(folder_name)s' zurück gehen"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplikate"
@@ -644,25 +659,25 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Auf der Website ansehen"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Gehe zurück zu"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "Admin Startseite"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
@@ -701,15 +716,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Zielordner"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopieren"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Es ist nicht erlaubt Dateien in den selben Ordner zu kopieren"
 
@@ -758,15 +773,15 @@
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr "Die folgenden Dateien und/oder Ordner werden in ein Zielordner verschoben (unter Beibehaltung ihrer Ordnerstruktur):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Verschieben"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Es ist nicht erlaubt Dateien in den selben Ordner zu verschieben"
 
@@ -785,71 +800,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr "Die folgenden Dateien werden umbenannt (sie bleiben in ihren Ordnern und behalten ihren originalen Dateinamen, nur dier angezeigte Dateiname wird geändert):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Umbenennen"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Gehe zurück zum übergeordneten Ordner"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Details des aktuellen Ordners ändern"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Ändern"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Hier klicken, um nach dem eingegebenen Text zu suchen"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Suchen"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Schliessen"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limit"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Aktivieren, um die Suche auf den aktuellen Ordner zu beschränken"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Suche auf aktuellen Ordner beschränken"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Löschen"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Fügt einen neuen Ordner hinzu"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Neuer Ordner"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Dateien hochladen"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Du musst zuerst einen Ordner auswählen"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Name"
 
@@ -1072,15 +1087,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr "Vergrößern"
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
+#: templatetags/filer_admin_tags.py:107
 #| msgid "file missing"
 msgid "File is missing"
 msgstr "Datei fehlt"
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Typ"
```

### Comparing `django-filer-3.0.3/filer/locale/en/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/en/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/en/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2016-06-17 14:16+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
 "Language-Team: English (http://www.transifex.com/divio/django-filer/language/"
 "en/)\n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -31,19 +31,19 @@
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
 msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Advanced"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "canonical URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -250,27 +250,27 @@
 msgstr "Subject location is outside of the image. "
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Your input: \"{subject_location}\". "
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Folder with this name already exists."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -292,15 +292,15 @@
 msgid "image"
 msgstr "image"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "images"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "user"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "files"
 
@@ -322,15 +322,15 @@
 msgstr "clipboard item"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "clipboard items"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "folder"
 
 #: models/filemodels.py:81
@@ -345,32 +345,32 @@
 msgid "has all mandatory data"
 msgstr "has all mandatory data"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "original filename"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "name"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "description"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "owner"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "uploaded at"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "modified at"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Permissions disabled"
 
@@ -378,122 +378,139 @@
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "created at"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Folder"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Folders"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "all items"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "this item only"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "this item and all children"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "allow"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "deny"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "type"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "group"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "everybody"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "can read"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "can edit"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "can add children"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "folder permission"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "folder permissions"
 
-#: models/foldermodels.py:359
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 #, fuzzy
 #| msgid "Folders"
 msgid "All Folders"
 msgstr "Folders"
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
+#: models/foldermodels.py:375
 #, fuzzy
 #| msgid "everybody"
 msgid "Everybody"
 msgstr "everybody"
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
+#: models/foldermodels.py:390
 #, fuzzy
 #| msgid "can add children"
 msgid "Add children"
 msgstr "can add children"
 
 #: models/imagemodels.py:18
 msgid "date taken"
@@ -532,18 +549,16 @@
 msgid "Unsorted Uploads"
 msgstr "Unsorted Uploads"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "files with missing metadata"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "root"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
@@ -590,24 +605,24 @@
 msgstr "Home"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Go back to Filer app"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Go back to root folder"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Go back to '%(folder_name)s' folder"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplicates"
@@ -659,25 +674,25 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "View on site"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Go back to"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "admin homepage"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
@@ -720,15 +735,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Destination folder:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Copy"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "It is not allowed to copy files into same folder"
 
@@ -784,15 +799,15 @@
 "(retaining their tree structure):"
 msgstr ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Move"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "It is not allowed to move files into same folder"
 
@@ -814,71 +829,71 @@
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Rename"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Go back to the parent folder"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Change current folder details"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Change"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Click here to run search for entered phrase"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Search"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Close"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limit"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Check it to limit the search to current folder"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Limit the search to current folder"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Delete"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Adds a new Folder"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "New Folder"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Upload Files"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "You have to select a folder first"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Name"
 
@@ -1103,15 +1118,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
+#: templatetags/filer_admin_tags.py:107
 #, fuzzy
 #| msgid "file missing"
 msgid "File is missing"
 msgstr "file missing"
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
```

### Comparing `django-filer-3.0.3/filer/locale/es/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/es/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Luis Zárate <luisza@visualcon.net>, 2019\n"
+"Last-Translator: Biel Frontera, 2023\n"
 "Language-Team: Spanish (http://app.transifex.com/divio/django-filer/language/"
 "es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
@@ -33,33 +33,52 @@
 
 msgid "0 of %(cnt)s selected"
 msgstr "0 de %(cnt)s seleccionados"
 
 msgid "Action"
 msgstr "Acción"
 
+msgid "Add children"
+msgstr "Añadir hijos"
+
 msgid "Add new"
 msgstr "Añadir nuevo"
 
 msgid "Adds a new Folder"
 msgstr "Añade una nueva Carpeta"
 
 msgid "Advanced"
 msgstr "Avanzado"
 
+msgid "All Folders"
+msgstr "Todas las carpetas"
+
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
 msgstr ""
 "¿Estás seguro de que quieres borrar los archivos y/o carpetas seleccionados? "
 "Los siguientes objetos y sus elementos relacionados serán borrados:"
 
 msgid "Are you sure?"
 msgstr "¿Estás seguro?"
 
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr "Al menos se debe seleccionar un usuario, un grupo o \"todos\"."
+
+msgid "Can't find folder to upload. Please refresh and try again"
+msgstr ""
+"No se ha encontrado la carpeta donde guardar el fichero. Por favor, refresca "
+"la página y vuelve a probar."
+
+msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgstr ""
+"No se puede utilizar esta carpeta: permiso denegado. Por favor, selecciona "
+"otra carpeta."
+
 msgid "Cannot delete files and/or folders"
 msgstr "No es posible eliminar ficheros y/o directorios"
 
 msgid "Canonical url '%(item_label)s'"
 msgstr "Url canónica '%(item_label)s'"
 
 msgid "Change"
@@ -79,14 +98,17 @@
 
 msgid "Check it to limit the search to current folder"
 msgstr "Comprueba el límite de búsqueda en la carpeta actual"
 
 msgid "Choose File"
 msgstr "Selecciona el archivo"
 
+msgid "Choose Folder"
+msgstr "Escoge una carpeta"
+
 msgid "Choose an existing thumbnail option or enter resize parameters:"
 msgstr ""
 "Elige una opción de miniatura existente o introduce parámetros para el "
 "cambio de tamaño:"
 
 msgid "Choose resize parameters:"
 msgstr "Elegir parámetros para el cambio de tamaño:"
@@ -162,44 +184,93 @@
 
 msgid "Disable permissions for selected files"
 msgstr "Deshabilitar permisos para los archivos seleccionados."
 
 msgid "Django site admin"
 msgstr "Sitio administrativo de Django"
 
+msgid "Download"
+msgstr "Descarga"
+
 msgid "Download '%(item_label)s'"
 msgstr "Descargar '%(item_label)s'"
 
 msgid "Drop files here or use the \"Upload Files\" button"
 msgstr "Suelta los archivos aquí o usa el botón \"Subir archivos\""
 
 msgid "Drop your file to upload into:"
 msgstr "Suelta el archivo a subir dentro:"
 
 msgid "Duplicates"
 msgstr "Duplicados"
 
+msgid "Edit"
+msgstr "Editar"
+
 msgid "Empty Clipboard"
 msgstr "Portapapeles vacío"
 
 msgid "Enable permissions for selected files"
 msgstr "Habilitar permisos para los archivos seleccionados."
 
+msgid "Everybody"
+msgstr "Todos"
+
+msgid "Expand"
+msgstr "Expande"
+
+msgid "File \"{file_name}\": HTML upload denied by site security policy"
+msgstr ""
+"Fichero \"{file_name}\": carga de HTML denegada por políticas de seguridad "
+"del sitio web"
+
+msgid ""
+"File \"{file_name}\": Rejected due to potential cross site scripting "
+"vulnerability"
+msgstr ""
+"Fichero \"{file_name}\": rechazado por posible vulnerabilidad XSS (Cross-"
+"site scripting)"
+
+msgid "File \"{file_name}\": Upload denied by site security policy"
+msgstr ""
+"Fichero \"{file_name}\": carga denegada por políticas de seguridad del sitio "
+"web"
+
+msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
+msgstr ""
+"Fichero \"{file_name}\": carga del tipo {file_type} denegada por políticas "
+"de seguridad del sitio web"
+
+msgid "File is missing"
+msgstr "Fichero no encontrado"
+
 msgid "File-size"
 msgstr "Tamaño del archivo"
 
 msgid "Filer"
 msgstr "Filer"
 
+msgid "Files"
+msgstr "Ficheros"
+
 msgid "Folder"
 msgstr "Carpeta"
 
 msgid "Folder Icon"
 msgstr "Icono de la Carpeta"
 
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+"La carpeta no se puede seleccionar con el tipo \"todos los elementos\"."
+
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+"La carpeta se tiene que seleccionar cuando el tipo no es \"todos los "
+"elementos\"."
+
 msgid "Folder with this name already exists."
 msgstr "Ya existe un directorio con este nombre."
 
 msgid "Folders"
 msgstr "Carpetas"
 
 msgid "Folders with names %s already exist at the selected destination"
@@ -222,14 +293,17 @@
 
 msgid "Go back to root folder"
 msgstr "Volver a la carpeta raíz"
 
 msgid "Go back to the parent folder"
 msgstr "Volver a la carpeta padre"
 
+msgid "Group: {group}"
+msgstr "Grupo: {group}"
+
 msgid "History"
 msgstr "Histórico"
 
 msgid "Home"
 msgstr "Inicio"
 
 msgid "Invalid rename format: %(error)s."
@@ -256,14 +330,17 @@
 
 msgid "Limit the search to current folder"
 msgstr "Limitar busqueda a la carpeta actual"
 
 msgid "Location of the main subject of the scene. Format: \"x,y\"."
 msgstr "Ubicación del tema principal en la escena. Formato \"x,y\""
 
+msgid "Logical Path"
+msgstr "Path lógico"
+
 msgid "Lookup"
 msgstr "Buscar"
 
 msgid "Media library"
 msgstr "Biblioteca multimedia"
 
 msgid "Modified"
@@ -313,14 +390,17 @@
 
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] "Por favor, corrige el error indicado abajo."
 msgstr[1] "Por favor, corrige los errores indicados abajo."
 msgstr[2] "Por favor, corrige los errores indicados abajo."
 
+msgid "Read"
+msgstr "Leer"
+
 msgid "Remove file"
 msgstr "Eliminar archivo"
 
 msgid "Remove folder"
 msgstr "Eliminar carpeta"
 
 msgid "Rename"
@@ -346,23 +426,32 @@
 
 msgid "Save"
 msgstr "Guardar"
 
 msgid "Search"
 msgstr "Buscar"
 
+msgid "Select all"
+msgstr "Selecciona todas"
+
 msgid "Select all %(total_count)s"
 msgstr "Seleccionar todo %(total_count)s"
 
 msgid "Select all %(total_count)s files and/or folders"
 msgstr "Seleccionar los %(total_count)s archivos y/o carpetas"
 
 msgid "Select this file"
 msgstr "Seleccionar este archivo"
 
+msgid "Show table view"
+msgstr "Muestra la vista de tabla"
+
+msgid "Show thumbnail view"
+msgstr "Muestra la vista de miniaturas"
+
 msgid "Size"
 msgstr "Tamaño"
 
 msgid "Subject location"
 msgstr "Localización del sujeto."
 
 msgid "Subject location is outside of the image. "
@@ -476,28 +565,43 @@
 
 msgid "Upload canceled!"
 msgstr "Subida cancelada!"
 
 msgid "Upload success!"
 msgstr "Subida exitosa!"
 
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr "Usuario y grupo no se pueden seleccionar a la vez con \"todos\"."
+
+msgid "User: {user}"
+msgstr "Usuario: {user}"
+
 msgid "View on site"
 msgstr "Ver en la página"
 
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
 msgstr ""
 "Aviso: se cambiará el tamaño de las imágenes en el mismo sitio y los "
 "originales se perderán. Considera realizar una copia de aquellas para "
 "conservar los originales."
 
+msgid "What"
+msgstr "Qué"
+
+msgid "Who"
+msgstr "Quién"
+
 msgid "Yes, I&#39;m sure"
 msgstr "Sí, estoy seguro"
 
+msgid "You do not have permission to upload files."
+msgstr "No tienes autorización para subir ficheros. "
+
 msgid "You have to select a folder first"
 msgstr "Tiene que seleccionar primero una carpeta"
 
 msgid ""
 "Your account doesn't have permissions to copy all of the selected files and/"
 "or folders."
 msgstr ""
@@ -518,14 +622,20 @@
 
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
 msgstr ""
 "Tu cuenta no tiene permisos para cambiar el tamaño de todas las imágenes "
 "seleccionadas."
 
+msgid "Your browser does not support audio."
+msgstr "El navegador no soporta audio."
+
+msgid "Your browser does not support video."
+msgstr "El navegador no soporta vídeo."
+
 msgid "Your input: \"{subject_location}\". "
 msgstr "Tu entrada: \"{subject_location}\"."
 
 msgid "admin homepage"
 msgstr "página de inicio de la administración"
 
 msgid "all items"
@@ -638,14 +748,17 @@
 
 msgid "image"
 msgstr "imagen"
 
 msgid "images"
 msgstr "imágenes"
 
+msgid "inherit"
+msgstr "hereda"
+
 msgid "modified at"
 msgstr "modificado el"
 
 msgid "must always publish author credit"
 msgstr "siempre debes dar crédito al autor"
 
 msgid "must always publish copyright"
@@ -665,14 +778,17 @@
 
 msgid "original filename"
 msgstr "nombre del archivo original"
 
 msgid "owner"
 msgstr "propietario"
 
+msgid "parent"
+msgstr "Padre"
+
 msgid "previous"
 msgstr "anterior"
 
 msgid "root"
 msgstr "raíz"
 
 msgid "sha1"
```

### Comparing `django-filer-3.0.3/filer/locale/es/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Translators:
 # Translators:
+# Biel Frontera, 2023
 # Cristian Acevedo <arucar17@gmail.com>, 2016
 # David <d.diazp@gmail.com>, 2015
 # Jason Gass Martinez <jason.tra@jason-pc.tk>, 2016
 # Luis Zárate <luisza@visualcon.net>, 2019
 # Manuel E. Gutierrez <manuel.gutierrez@etecsa.cu>, 2013,2015
 # Manuel E. Gutierrez <manuel.gutierrez@etecsa.cu>, 2013
 # Pablo, 2015
 # Pablo, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Luis Zárate <luisza@visualcon.net>, 2019\n"
+"Last-Translator: Biel Frontera, 2023\n"
 "Language-Team: Spanish (http://app.transifex.com/divio/django-filer/language/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
 #| msgid ""
 #| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
-msgstr ""
+msgstr "No tienes autorización para subir ficheros. "
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
-msgstr ""
+msgstr "No se ha encontrado la carpeta donde guardar el fichero. Por favor, refresca la página y vuelve a probar."
 
 #: admin/clipboardadmin.py:19
 msgid ""
 "Can't use this folder, Permission Denied. Please select another folder."
-msgstr ""
+msgstr "No se puede utilizar esta carpeta: permiso denegado. Por favor, selecciona otra carpeta."
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Avanzado"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "URL canónica"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -250,27 +251,27 @@
 msgstr "La ubicación del tema está fuera de la imagen"
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Tu entrada: \"{subject_location}\"."
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
-msgstr ""
+msgstr "Quién"
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
-msgstr ""
+msgstr "Qué"
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Ya existe un directorio con este nombre."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -292,15 +293,15 @@
 msgid "image"
 msgstr "imagen"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "imágenes"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "usuario"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "archivos"
 
@@ -322,15 +323,15 @@
 msgstr "elemento del portapapeles"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "elementos del portapapeles"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "carpeta"
 
 #: models/filemodels.py:81
@@ -345,154 +346,171 @@
 msgid "has all mandatory data"
 msgstr "tiene todos los datos obligatorios"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "nombre del archivo original"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nombre"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "descripción"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "propietario"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "subido a"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "modificado el"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Permisos desactivados"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr "Desactiva cualquier comprobación de permiso para este archivo. El archivo será accesible públicamente para todos."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
-msgstr ""
+msgstr "Padre"
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "creado el"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Carpeta"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Carpetas"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "todos los elementos"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "sólo este elemento"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "este elemento y todos los hijos"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
-msgstr ""
+msgstr "hereda"
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "permitir"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "denegar"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tipo"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "grupo"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "todos"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "puede leer"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "puede editar"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "puede añadir hijos"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "permiso de la carpeta"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "permisos de la carpeta"
 
-#: models/foldermodels.py:359
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr "La carpeta no se puede seleccionar con el tipo \"todos los elementos\"."
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr "La carpeta se tiene que seleccionar cuando el tipo no es \"todos los elementos\"."
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr "Usuario y grupo no se pueden seleccionar a la vez con \"todos\"."
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr "Al menos se debe seleccionar un usuario, un grupo o \"todos\"."
+
+#: models/foldermodels.py:360
 #| msgid "Folders"
 msgid "All Folders"
-msgstr ""
+msgstr "Todas las carpetas"
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
-msgstr ""
+msgstr "Path lógico"
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
-msgstr ""
+msgstr "Usuario: {user}"
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
-msgstr ""
+msgstr "Grupo: {group}"
 
-#: models/foldermodels.py:374
+#: models/foldermodels.py:375
 #| msgid "everybody"
 msgid "Everybody"
-msgstr ""
+msgstr "Todos"
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
-msgstr ""
+msgstr "Editar"
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
-msgstr ""
+msgstr "Leer"
 
-#: models/foldermodels.py:389
+#: models/foldermodels.py:390
 #| msgid "can add children"
 msgid "Add children"
-msgstr ""
+msgstr "Añadir hijos"
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "fecha"
 
 #: models/imagemodels.py:25
 msgid "author"
@@ -527,29 +545,27 @@
 msgid "Unsorted Uploads"
 msgstr "Subidas desordenadas"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "archivos con metadatos perdidos"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "raíz"
 
 #: settings.py:273
 msgid "Show table view"
-msgstr ""
+msgstr "Muestra la vista de tabla"
 
 #: settings.py:278
 #| msgid "thumbnail option"
 msgid "Show thumbnail view"
-msgstr ""
+msgstr "Muestra la vista de miniaturas"
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Ejecutar la acción seleccionada"
 
 #: templates/admin/filer/actions.html:5
 msgid "Go"
@@ -584,24 +600,24 @@
 msgstr "Inicio"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Volver a la app Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Volver a la carpeta raíz"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Volver a la carpeta '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplicados"
@@ -646,25 +662,25 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Ver en la página"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Volver a"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "página de inicio de la administración"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
@@ -703,15 +719,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Carpeta de destino:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Copiar"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "No está permitido copiar los archivos dentro de la misma carpeta"
 
@@ -760,15 +776,15 @@
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr "Los siguientes archivos y/o directorios serán movidos a una carpeta de destino (manteniendo su estructura de árbol):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Mover"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "No está permitido mover los archivos dentro de la misma carpeta"
 
@@ -787,71 +803,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr "Los siguientes archivos serán renombrados (se quedarán en sus carpetas y mantendrán su nombre original, solo los nombres mostrados serán cambiados):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Cambiar el nombre"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Volver a la carpeta padre"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Cambiar los detalles de la carpeta actual"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Cambiar"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Haz clic para correr la búsqueda del texto ingresado"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Buscar"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Cerrar"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limite"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Comprueba el límite de búsqueda en la carpeta actual"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Limitar busqueda a la carpeta actual"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Borrar"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Añade una nueva Carpeta"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Carpeta Nueva"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Subir archivos."
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Tiene que seleccionar primero una carpeta"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Nombre"
 
@@ -1008,20 +1024,20 @@
 msgid "Select all %(total_count)s"
 msgstr "Seleccionar todo %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
 #| msgid "Select this file"
 msgid "Select all"
-msgstr ""
+msgstr "Selecciona todas"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
 #| msgid "Filer"
 msgid "Files"
-msgstr ""
+msgstr "Ficheros"
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Añadir nuevo"
 
 #: templates/admin/filer/folder/new_folder_form.html:4
@@ -1037,19 +1053,19 @@
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr "Guardar"
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
-msgstr ""
+msgstr "El navegador no soporta audio."
 
 #: templates/admin/filer/templatetags/file_icon.html:14
 msgid "Your browser does not support video."
-msgstr ""
+msgstr "El navegador no soporta vídeo."
 
 #: templates/admin/filer/tools/clipboard/clipboard.html:9
 msgid "Clipboard"
 msgstr "Portapapeles"
 
 #: templates/admin/filer/tools/clipboard/clipboard.html:21
 msgid "Paste all items here"
@@ -1069,26 +1085,26 @@
 
 #: templates/admin/filer/tools/clipboard/clipboard_item_rows.html:16
 msgid "upload failed"
 msgstr "fallo en la subida"
 
 #: templates/admin/filer/tools/detail_info.html:11
 msgid "Download"
-msgstr ""
+msgstr "Descarga"
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
-msgstr ""
+msgstr "Expande"
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
+#: templatetags/filer_admin_tags.py:107
 #| msgid "file missing"
 msgid "File is missing"
-msgstr ""
+msgstr "Fichero no encontrado"
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipo"
 
 #: templates/admin/filer/tools/detail_info.html:37
 msgid "File-size"
@@ -1136,37 +1152,37 @@
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Selecciona el archivo"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
 #| msgid "Choose File"
 msgid "Choose Folder"
-msgstr ""
+msgstr "Escoge una carpeta"
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
-msgstr ""
+msgstr "Fichero \"{file_name}\": carga denegada por políticas de seguridad del sitio web"
 
 #: validation.py:22
 #, python-brace-format
 msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
-msgstr ""
+msgstr "Fichero \"{file_name}\": carga del tipo {file_type} denegada por políticas de seguridad del sitio web"
 
 #: validation.py:33
 #, python-brace-format
 msgid "File \"{file_name}\": HTML upload denied by site security policy"
-msgstr ""
+msgstr "Fichero \"{file_name}\": carga de HTML denegada por políticas de seguridad del sitio web"
 
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
-msgstr ""
+msgstr "Fichero \"{file_name}\": rechazado por posible vulnerabilidad XSS (Cross-site scripting)"
 
 #~ msgid "Open file"
 #~ msgstr "Open file"
 
 #~ msgid "Full size preview"
 #~ msgstr "Full size preview"
```

### Comparing `django-filer-3.0.3/filer/locale/et/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/et/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/et/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Johan Viirok, 2022
 # Martin <martinpajuste@gmail.com>, 2016
 # Rivo Zängov <eraser@eraser.ee>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Johan Viirok, 2022\n"
-"Language-Team: Estonian (http://app.transifex.com/divio/django-filer/language/et/)\n"
+"Language-Team: Estonian (http://app.transifex.com/divio/django-filer/"
+"language/et/)\n"
+"Language: et\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -244,27 +242,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -286,15 +284,15 @@
 msgid "image"
 msgstr "pilt"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "pildid"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "kasutaja"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "failid"
 
@@ -316,15 +314,15 @@
 msgstr "lõikelaua kirje"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "lõikelaua kirjed"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "kaust"
 
 #: models/filemodels.py:81
@@ -339,152 +337,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "algne failinimi"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nimi"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "kirjeldus"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "omanik"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "üles laaditud"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "muudetud"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "loodud"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Kaust"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Kaustad"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "kõik kirjed"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "ainult see kirje"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "see kirje ja kõik alamkirjed"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "luba"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "keeldu"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tüüp"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "grupp"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "kõik"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "saab lugeda"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "saab mutua"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "kausta õigus"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "kausta õigused"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -521,27 +533,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -578,24 +587,24 @@
 msgstr "Koduleht"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Tagasi peakausta"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplikaadid"
@@ -640,38 +649,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Vaata saidil"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Mine tagasi"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "admini koduleht"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Kausta ikoon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -697,15 +706,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopeeri"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -738,31 +747,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Muuda suurust"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Liiguta"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -781,71 +790,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Nimeta ümber"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Mine tagasi peamisesse kausta"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Muuda"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Otsi"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Sulge"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Kustuta"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Lisab uue kausta"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Uus kaust"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Nimi"
 
@@ -930,21 +939,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "sisse lülitatud"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Lae alla '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Eemalda fail"
 
@@ -998,20 +1005,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Vali kõik %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Lisa uus"
@@ -1068,16 +1073,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tüüp"
 
@@ -1125,15 +1129,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Vali fail"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/eu/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Ales Zabala Alava <shagi@gisa-elkartea.org>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Ales Zabala Alava <shagi@gisa-elkartea.org>, 2013\n"
-"Language-Team: Basque (http://app.transifex.com/divio/django-filer/language/eu/)\n"
+"Language-Team: Basque (http://app.transifex.com/divio/django-filer/language/"
+"eu/)\n"
+"Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: eu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Aurreratua"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Elementuak hautatu behar dira beraiekin zeozer egiteko. Ez da elementurik aldatu."
+msgstr ""
+"Elementuak hautatu behar dira beraiekin zeozer egiteko. Ez da elementurik "
+"aldatu."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "bat haututa"
 msgstr[1] "%(total_count)s hautatuta"
@@ -124,15 +124,16 @@
 msgstr ""
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d fitxategi eta/edo karpeta '%(destination)s' karpetara mugituta."
+msgstr ""
+"%(count)d fitxategi eta/edo karpeta '%(destination)s' karpetara mugituta."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Fitxategi eta/edo karpetak mugitu"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -149,15 +150,16 @@
 msgstr "Fitxategiak berrizendatu"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d fitxategi eta/edo karpeta %(destination)s karpetara kopiatuta."
+msgstr ""
+"%(count)d fitxategi eta/edo karpeta %(destination)s karpetara kopiatuta."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Fitxategi eta/edo karpetak kopiatu"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -181,15 +183,17 @@
 msgstr "Kopiatutako fitxategiei gehituko zaien atzizkia."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Atzizkia baliozko, sinple eta letra xehetan dagoen fitxategi izen zatia izan beharko luke, \"%(valid)s\" bezala."
+msgstr ""
+"Atzizkia baliozko, sinple eta letra xehetan dagoen fitxategi izen zatia izan "
+"beharko luke, \"%(valid)s\" bezala."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Berrizendatze formatuko gako balio ezezaguna \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -215,15 +219,16 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "handitu"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr "Argazkitxo aukerak edo tamaina aldatzeko parametroak zehaztu behar dira."
+msgstr ""
+"Argazkitxo aukerak edo tamaina aldatzeko parametroak zehaztu behar dira."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Tamaina aldatzeko parametroak zehaztu behar dira."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -242,27 +247,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Izen honetako karpeta badago."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -284,15 +289,15 @@
 msgid "image"
 msgstr "irudia"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "irudiak"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "erabiltzailea"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "fitxategiak"
 
@@ -314,15 +319,15 @@
 msgstr "arbeleko elementua"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "arbeleko elementuak"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "karpeta"
 
 #: models/filemodels.py:81
@@ -337,152 +342,166 @@
 msgid "has all mandatory data"
 msgstr "beharrezko datu guztiak ditu"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "jatorrizko fitxategi izena"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "izena"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "deskribapena"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "jaea"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "noiz igota"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "noiz aldatua"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Baimenak ezgaituta"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "noiz sortua"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Karpeta"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Karpetak"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "elementu guztiak"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "elementu hau bakarrik"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "elementu hau eta bere semeak"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "mota"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "taldea"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "edonor"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "irakurri dezake"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "editatu dezake"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "semeak gehitu ditzake"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "karpeta baimena"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "karpeta baimenak"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "sortze data"
 
@@ -519,27 +538,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "metadatuak faltan dituzten fitxategiak"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "erroa"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Hautatutako ekintza abiarazi"
 
@@ -576,24 +592,24 @@
 msgstr "Etxea"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Filer aplikaziora itzuli"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Erro karpetara itzuli"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "'%(folder_name)s karpetara itzuli'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -611,15 +627,17 @@
 "following protected related objects:"
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Ziur hautatutako fitxategi eta/edo karpetak ezabatu nahi dituzula? Ondoko objektu eta erlazionatutako elementu guztiak ezabatuko lirateke:"
+msgstr ""
+"Ziur hautatutako fitxategi eta/edo karpetak ezabatu nahi dituzula? Ondoko "
+"objektu eta erlazionatutako elementu guztiak ezabatuko lirateke:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -638,38 +656,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Webgunean ikusi"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Itzuli hona:"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "kudeaketa hasiera"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Karpeta ikonoa"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -695,15 +713,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Helburuko karpeta:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopiatu"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -718,49 +736,54 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Ondoko irudien tamaina aldatuko da:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Argazkitxo aukera bat hautatu edo tamaina aldatzeko parametroak ezarri:"
+msgstr ""
+"Argazkitxo aukera bat hautatu edo tamaina aldatzeko parametroak ezarri:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Tamaina aldatzeko parametroak aukeratu:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Kontuz: Irudien tamaina aldatzean jatorrizkoak galduko dira. Lehenbizi jatorrizkoen kopia egin zenezake."
+msgstr ""
+"Kontuz: Irudien tamaina aldatzean jatorrizkoak galduko dira. Lehenbizi "
+"jatorrizkoen kopia egin zenezake."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Tamaina aldatu"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Zure kontuak ez du hautatutako fitxategi eta/edo karpeta guztiak mugitzeko baimenik."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Zure kontuak ez du hautatutako fitxategi eta/edo karpeta guztiak mugitzeko "
+"baimenik."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Ez dago mugitu daitekeen fitxategi edo/eta karpetarik."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Mugitu"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -779,71 +802,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Berrizendatu"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Karpeta gurasora joan"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Uneko karpetaren xehetasunak aldatu"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Aldatu"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Bilatu"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Ezabatu"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Karpeta berri bat sortzen du"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Karpeta berria"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Izena"
 
@@ -928,21 +951,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "gaituta"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -996,20 +1017,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Berria gehitu"
@@ -1066,16 +1085,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1123,15 +1141,14 @@
 msgstr "Bilatu"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,87 +1,83 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
-# Fariman Ghaedi <farimanghaedi@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Fariman Ghaedi <farimanghaedi@gmail.com>, 2019\n"
-"Language-Team: Persian (http://app.transifex.com/divio/django-filer/language/fa/)\n"
+"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
+"Language-Team: Japanese (http://app.transifex.com/divio/django-filer/"
+"language/ja/)\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fa\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
-msgstr "پیشرفته"
+msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
-msgstr "آدرس کانونی"
+msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "برای اینکه بتوانید روی آیتم ها اقداماتی انجام دهید ابتدا باید آیتم ها را انتخاب کنید. هیچ آیتمی تغییر نکرد."
+msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
-msgstr[1] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
 #, python-format
 msgid "0 of %(cnt)s selected"
 msgstr ""
 
 #: admin/folderadmin.py:600
 msgid "No action selected."
-msgstr "هیچ اقدامی انتخاب نشده است."
+msgstr ""
 
 #: admin/folderadmin.py:652
 #, python-format
 msgid "Successfully moved %(count)d files to clipboard."
 msgstr ""
 
 #: admin/folderadmin.py:657
 msgid "Move selected files to clipboard"
-msgstr "انتقال فایل های انتخاب شده به کلیپ برد"
+msgstr ""
 
 #: admin/folderadmin.py:697
 #, python-format
 msgid "Successfully disabled permissions for %(count)d files."
 msgstr ""
 
 #: admin/folderadmin.py:699
@@ -104,23 +100,23 @@
 
 #: admin/folderadmin.py:782
 msgid "Cannot delete files and/or folders"
 msgstr ""
 
 #: admin/folderadmin.py:784
 msgid "Are you sure?"
-msgstr "آیا مطمئن هستید؟"
+msgstr ""
 
 #: admin/folderadmin.py:790
 msgid "Delete files and/or folders"
-msgstr "پاک کردن فایل ها و/یا پوشه ها"
+msgstr ""
 
 #: admin/folderadmin.py:811
 msgid "Delete selected files and/or folders"
-msgstr "پاک کردن فایل ها و/یا پوشه های انتخاب شده"
+msgstr ""
 
 #: admin/folderadmin.py:918
 #, python-format
 msgid "Folders with names %s already exist at the selected destination"
 msgstr ""
 
 #: admin/folderadmin.py:922
@@ -242,27 +238,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -284,15 +280,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -314,15 +310,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -337,152 +333,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -519,27 +529,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -576,24 +583,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -638,38 +645,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -695,15 +702,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -736,31 +743,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -779,71 +786,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -875,23 +882,21 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
-msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
-msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -928,21 +933,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -996,20 +999,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1018,15 +1019,14 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
-msgstr[1] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1066,16 +1066,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1123,15 +1122,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1189,11 +1187,10 @@
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
-#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/fi/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Niklas Jerva <niklas.jerva@gmail.com>, 2016
 # Teemu Gratschev <teemu.gratschev@gmail.com>, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Teemu Gratschev <teemu.gratschev@gmail.com>, 2022\n"
-"Language-Team: Finnish (http://app.transifex.com/divio/django-filer/language/fi/)\n"
+"Language-Team: Finnish (http://app.transifex.com/divio/django-filer/language/"
+"fi/)\n"
+"Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Edistyneet asetukset"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "sääntöjenmukainen URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Toiminnon suorittamiseksi pitää valita kohteita. Yhtäänkohdetta ei ole valittu."
+msgstr ""
+"Toiminnon suorittamiseksi pitää valita kohteita. Yhtäänkohdetta ei ole "
+"valittu."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s valittu"
 msgstr[1] "Kaikki %(total_count)s valittu"
@@ -125,15 +125,16 @@
 msgstr "%s niminen kansio on jo valitussa kohteessa"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d tiedostoa ja/tai kansiota siirretty kansioon '%(destination)s'."
+msgstr ""
+"%(count)d tiedostoa ja/tai kansiota siirretty kansioon '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Siirrä tiedostot ja/tai kansiot"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -150,15 +151,16 @@
 msgstr "Nimeä tiedostot uudelleen"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d tiedostoa ja/tai kansiota kopioitu kansioon '%(destination)s'."
+msgstr ""
+"%(count)d tiedostoa ja/tai kansiota kopioitu kansioon '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopioi tiedostot ja/tai kansiot"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -182,15 +184,17 @@
 msgstr "Pääte, joka lisätään kopioitujen tiedostojen nimiin."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Päätteen tulee olla käypä, yksinkertainen ja pienellä kirjoitettu osa tiedostonimeä, esim. \"%(valid)s\"."
+msgstr ""
+"Päätteen tulee olla käypä, yksinkertainen ja pienellä kirjoitettu osa "
+"tiedostonimeä, esim. \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Tuntematon uudelleennimeämisarvo \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -243,27 +247,27 @@
 msgstr "Kohteen sijainti kuvan ulkopuolella."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Syöttösi: \"{subject_location}\"."
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Saman niminen kansio on jo olemassa."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -285,15 +289,15 @@
 msgid "image"
 msgstr "kuva"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "kuvat"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "käyttäjä"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "tiedostot"
 
@@ -315,15 +319,15 @@
 msgstr "leikepöydän kohde"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "leikepöydän kohteet"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "kansio"
 
 #: models/filemodels.py:81
@@ -338,152 +342,168 @@
 msgid "has all mandatory data"
 msgstr "sisältää kaikki pakolliset tiedot"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "alkuperäinen tiedostonimi"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nimi"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "kuvaus"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "omistaja"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "ladattu"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "muokattu"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Käyttöoikeudet pois käytöstä"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Poista käyttöoikeuksien tarkistus tältä tiedostolta. Tiedosto näkyy julkisena kaikille."
+msgstr ""
+"Poista käyttöoikeuksien tarkistus tältä tiedostolta. Tiedosto näkyy "
+"julkisena kaikille."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "luotu"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Kansio"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Kansiot"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "kaikki kohteet"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "vain tämä kohde"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "tämä kohde ja kaikki lapset"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "salli"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "kiellä"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tyyppi"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "ryhmä"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "kaikki"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "saa lukea"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "saa muokata"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "saa lisätä lapsia"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "kansion käyttöoikeus"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "kansion käyttöoikeudet"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "päivämäärä"
 
@@ -520,27 +540,24 @@
 msgid "Unsorted Uploads"
 msgstr "Järjestelemättömät lataukset"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "tiedostot ilman metadataa"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "juuri"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Suorita valittu toiminto"
 
@@ -577,50 +594,57 @@
 msgstr "Etusivu"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Palaa Fileriin"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Palaa juurikansioon"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Palaa kansioon '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Kaksoiskappaleet"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Valittujen tiedostojen ja/tai kansioiden poistaminen vaatii liittyvien objektien poistamista, mutta käyttöoikeutesi eivät riitäseuraavien objektityyppien poistamiseen:"
+msgstr ""
+"Valittujen tiedostojen ja/tai kansioiden poistaminen vaatii liittyvien "
+"objektien poistamista, mutta käyttöoikeutesi eivät riitäseuraavien "
+"objektityyppien poistamiseen:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Valittujen tiedostojen ja/tai kansioiden poistaminen vaatisi seuraavien suojattujen liittyvien objektien poistamista:"
+msgstr ""
+"Valittujen tiedostojen ja/tai kansioiden poistaminen vaatisi seuraavien "
+"suojattujen liittyvien objektien poistamista:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Oletko varma, että haluat poistaa valitut tiedostot ja/tai kansiot? Kaikki seuraavat objektit ja niihin liittyvät kohteet poistetaan:"
+msgstr ""
+"Oletko varma, että haluat poistaa valitut tiedostot ja/tai kansiot? Kaikki "
+"seuraavat objektit ja niihin liittyvät kohteet poistetaan:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Ei, vie minut takaisin"
 
@@ -639,39 +663,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Näytä sivustolla"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Palaa kohteeseen"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "hallinnan etusivu"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Kansion kuvake"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen ja/tai kansioidenkopioimiseen."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen ja/tai "
+"kansioidenkopioimiseen."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -687,35 +713,38 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Kopioitavia tiedostoja ja/tai kansioita ei ole saatavilla."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Seuraavat tiedostot ja/tai kansiot kopioidaan kohdekansioon (säilyttäen puurakenteen):"
+msgstr ""
+"Seuraavat tiedostot ja/tai kansiot kopioidaan kohdekansioon (säilyttäen "
+"puurakenteen):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Kohdekansio:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopioi"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Tiedostojen kopiointi samaan kansioon ei ole sallittu"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Käyttöoikeutesi eivät riitä kaikkien valittujen kuvien koon muuttamiseen."
+msgstr ""
+"Käyttöoikeutesi eivät riitä kaikkien valittujen kuvien koon muuttamiseen."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Kuvia, joiden kokoa voisi muuttaa ei ole saatavilla."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
@@ -729,122 +758,133 @@
 msgid "Choose resize parameters:"
 msgstr "Valitse kokoparametrit:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Varoitus: Kuvien kokoa muuttaessa alkuperäiset versiot menetetään. On hyvä idea tehdä kuvista ensin kopiot alkuperäisten säilyttämiseksi."
+msgstr ""
+"Varoitus: Kuvien kokoa muuttaessa alkuperäiset versiot menetetään. On hyvä "
+"idea tehdä kuvista ensin kopiot alkuperäisten säilyttämiseksi."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Muuta kokoa"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen ja/tai kansioidensiirtämiseen."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen ja/tai "
+"kansioidensiirtämiseen."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Siirrettäviä tiedostoja ja/tai kansioita ei ole saatavilla."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Seuraavat tiedostot ja/tai kansiot siirretään kohdekansioon (säilyttäen niiden puurakenne):"
+msgstr ""
+"Seuraavat tiedostot ja/tai kansiot siirretään kohdekansioon (säilyttäen "
+"niiden puurakenne):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Siirrä"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Tiedostojen siirto samaan kansioon ei ole sallittua"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen uudelleennimeämiseen."
+msgstr ""
+"Käyttöoikeutesi eivät riitä kaikkien valittujen tiedostojen "
+"uudelleennimeämiseen."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Uudelleennimettäviä tiedostoja ei ole saatavilla."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Seuraavat tiedostot uudelleennimetään (ne pysyvät kansioissaan ja alkuperäiset tiedostonimet säilytetään, vain näytettävä tiedostonimi muutetaan):"
+msgstr ""
+"Seuraavat tiedostot uudelleennimetään (ne pysyvät kansioissaan ja "
+"alkuperäiset tiedostonimet säilytetään, vain näytettävä tiedostonimi "
+"muutetaan):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Uudelleennimeä"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Palaa ylempään kansioon"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Muuta nykyisen kansion tietoja"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Muuta"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Valitse suorittaaksesi haun annetulla hakusanalla"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Hae"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Sulje"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Raja"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Valitse rajoittaaksesi haun nykyiseen kansioon"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Rajoita haku nykyiseen kansioon"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Poista"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Lisää uusi kansio"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Uusi kansio"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Lataa tiedostoja"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Sinun tulee valita kansio ensin"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Nimi"
 
@@ -929,21 +969,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "käytössä"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Canonical-osoite '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Lataa '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Poista tiedosto"
 
@@ -997,20 +1035,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Valitse kaikki %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Lisää uusi"
@@ -1067,16 +1103,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tyyppi"
 
@@ -1124,15 +1159,14 @@
 msgstr "Haku"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Valitse tiedosto"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/fr/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -58,14 +58,19 @@
 msgstr ""
 "Voulez-vous vraiment supprimer les fichiers et/ou dossiers sélectionnés ? "
 "Tous les objets suivants et leurs éléments liés seront supprimés :"
 
 msgid "Are you sure?"
 msgstr "Êtes-vous sûr(e) ?"
 
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+"Au moins une option parmi un utilisateur, un groupe, ou \"tout le monde\" "
+"doit être sélectionnée."
+
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr "Dossier d'hébergement introuvable, rafraîchissez la page et réessayez."
 
 msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 "Utilisation du dossier impossible : Permissions insuffisantes. Sélectionnez "
 "un autre dossier."
@@ -249,14 +254,23 @@
 
 msgid "Folder"
 msgstr "Dossier"
 
 msgid "Folder Icon"
 msgstr "Icône du dossier"
 
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+"Le dossier ne peut pas être sélectionné avec le type \"tous les éléments\"."
+
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+"Un dossier doit être sélectionné lorsque le type n'est pas \"tous les "
+"éléments\"."
+
 msgid "Folder with this name already exists."
 msgstr "Il existe déjà un dossier avec ce nom."
 
 msgid "Folders"
 msgstr "Dossiers"
 
 msgid "Folders with names %s already exist at the selected destination"
@@ -550,14 +564,19 @@
 
 msgid "Upload canceled!"
 msgstr "Téléversement annulé !"
 
 msgid "Upload success!"
 msgstr "Téléversement réussi !"
 
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+"Un utilisateur ou un groupe ne peuvent être sélectionnés lorsque \"tout le "
+"monde\" est également sélectionné."
+
 msgid "User: {user}"
 msgstr "Utilisateur : {user}"
 
 msgid "View on site"
 msgstr "Voir sur le site"
 
 msgid ""
```

### Comparing `django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Assma Buifruri <assma.buifruri@hotmail.com>, 2017
 # Bertrand Bordage <bordage.bertrand@gmail.com>, 2012-2013
 # Sylvain Chiron <chironsylvain@orange.fr>, 2016
 # Corentin Bettiol, 2023
 # Jason Gass Martinez <jason.tra@jason-pc.tk>, 2016
 # Marion Balensi <kitsunesama@laposte.net>, 2012
 # Nicolas PASCAL <np.pascal@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Corentin Bettiol, 2023\n"
-"Language-Team: French (http://app.transifex.com/divio/django-filer/language/fr/)\n"
+"Language-Team: French (http://app.transifex.com/divio/django-filer/language/"
+"fr/)\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fr\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
+"1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr "Vous n'avez pas la permission d'héberger des fichiers."
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr "Dossier d'hébergement introuvable, rafraîchissez la page et réessayez."
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
-msgstr "Utilisation du dossier impossible : Permissions insuffisantes. Sélectionnez un autre dossier."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
+msgstr ""
+"Utilisation du dossier impossible : Permissions insuffisantes. Sélectionnez "
+"un autre dossier."
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Avancé"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "URL canonique"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Des éléments doivent être sélectionnés pour effectuer les actions. Aucun élément n'a été modifié."
+msgstr ""
+"Des éléments doivent être sélectionnés pour effectuer les actions. Aucun "
+"élément n'a été modifié."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s sélectionné"
 msgstr[1] "Tous les %(total_count)s sélectionnés"
@@ -131,15 +134,17 @@
 msgstr "Des dossiers nommés %s existent déjà dans la destination sélectionnée"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d fichiers et/ou dossiers déplacés avec succès vers le dossier « %(destination)s »."
+msgstr ""
+"%(count)d fichiers et/ou dossiers déplacés avec succès vers le dossier "
+"« %(destination)s »."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Déplacer les fichiers et/ou dossiers"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -156,15 +161,17 @@
 msgstr "Renommer les fichiers"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d fichiers et/dossiers copiés avec succès dans le dossier « %(destination)s »."
+msgstr ""
+"%(count)d fichiers et/dossiers copiés avec succès dans le dossier "
+"« %(destination)s »."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copier les fichiers et/ou dossiers"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -188,15 +195,17 @@
 msgstr "Suffixe qui sera ajouté au nom des fichiers copiés."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Le suffixe doit être une partie de nom de fichier valide, simple et en minuscules, comme « %(valid)s »."
+msgstr ""
+"Le suffixe doit être une partie de nom de fichier valide, simple et en "
+"minuscules, comme « %(valid)s »."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "La clé de formatage « %(key)s » est inconnue."
 
 #: admin/forms.py:54
@@ -222,15 +231,17 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "agrandir"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr "Une option de miniature ou des paramètres de dimensionnement doivent être choisis."
+msgstr ""
+"Une option de miniature ou des paramètres de dimensionnement doivent être "
+"choisis."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Des paramètres de dimensionnement doivent être choisis."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -249,27 +260,27 @@
 msgstr "L'emplacement du sujet est en dehors de l'image."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Votre entrée : « {subject_location} »."
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr "Qui"
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr "Quoi"
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Il existe déjà un dossier avec ce nom."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -291,15 +302,15 @@
 msgid "image"
 msgstr "image"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "images"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "utilisateur"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "fichiers"
 
@@ -321,15 +332,15 @@
 msgstr "élément du presse-papiers"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "éléments du presse-papiers"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "dossier"
 
 #: models/filemodels.py:81
@@ -344,152 +355,168 @@
 msgid "has all mandatory data"
 msgstr "possède toutes les données nécessaires"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "nom de fichier originel"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nom"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "description"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "propriétaire"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "téléversé le"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "modifié le"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Permissions désactivées"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Désactiver la vérification des permissions pour ce fichier. Le fichier sera publiquement accessible à tout le monde."
+msgstr ""
+"Désactiver la vérification des permissions pour ce fichier. Le fichier sera "
+"publiquement accessible à tout le monde."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr "parent"
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "créé le"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Dossier"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Dossiers"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "tous les éléments"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "cet élément seulement"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "cet élément et ses enfants"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr "hériter"
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "autoriser"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "refuser"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "type"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "groupe"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "tous"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "peut lire"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "peut éditer"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "peut ajouter un enfant"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "permission du dossier"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "permissions du dossier"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr "Le dossier ne peut pas être sélectionné avec le type \"tous les éléments\"."
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr "Un dossier doit être sélectionné lorsque le type n'est pas \"tous les éléments\"."
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr "Un utilisateur ou un groupe ne peuvent être sélectionnés lorsque \"tout le monde\" est également sélectionné."
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr "Au moins une option parmi un utilisateur, un groupe, ou \"tout le monde\" doit être sélectionnée."
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr "Tous les dossiers"
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr "Chemin logique"
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr "Utilisateur : {user}"
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr "Groupe : {group}"
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr "Tout le monde"
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr "Modifier"
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr "Lire"
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr "Ajouter un sous-dossier"
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "date de prise de vue"
 
@@ -526,27 +553,24 @@
 msgid "Unsorted Uploads"
 msgstr "Téléversements non triés"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "fichiers avec des métadonnées manquantes"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "racine"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr "Voir la vue en liste"
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr "Voir la vue avec des miniatures"
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Exécuter l'action sélectionnée"
 
@@ -583,50 +607,57 @@
 msgstr "Accueil"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Revenir à l'application Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Revenir au dossier racine"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Revenir au dossier « %(folder_name)s »"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplicatas"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Supprimer les fichiers et/ou dossiers sélectionnés devrait provoquer la suppression des objets liés, mais votre compte n'a pas les permissions nécessaires pour supprimer les types d'objets suivants :"
+msgstr ""
+"Supprimer les fichiers et/ou dossiers sélectionnés devrait provoquer la "
+"suppression des objets liés, mais votre compte n'a pas les permissions "
+"nécessaires pour supprimer les types d'objets suivants :"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Supprimer les fichiers et/ou dossiers provoquera la suppression des objets liés protégés suivants :"
+msgstr ""
+"Supprimer les fichiers et/ou dossiers provoquera la suppression des objets "
+"liés protégés suivants :"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Voulez-vous vraiment supprimer les fichiers et/ou dossiers sélectionnés ? Tous les objets suivants et leurs éléments liés seront supprimés :"
+msgstr ""
+"Voulez-vous vraiment supprimer les fichiers et/ou dossiers sélectionnés ? "
+"Tous les objets suivants et leurs éléments liés seront supprimés :"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Non, faites-moi revenir"
 
@@ -645,39 +676,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Voir sur le site"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Retourner à"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "page d'accueil de l'administrateur"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Icône du dossier"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Votre compte n'a pas les permissions nécessaires pour copier tous les fichiers et/ou dossiers sélectionnés."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Votre compte n'a pas les permissions nécessaires pour copier tous les "
+"fichiers et/ou dossiers sélectionnés."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -693,164 +726,182 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Aucun fichier ou dossier n'est disponible à copier."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Les fichiers et/ou dossiers suivants seront copiés vers un dossier de destination (en conservant leur arborescence) :"
+msgstr ""
+"Les fichiers et/ou dossiers suivants seront copiés vers un dossier de "
+"destination (en conservant leur arborescence) :"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Dossier de destination :"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Copier"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Il est impossible de copier des fichiers dans le même dossier"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Votre compte na pas les permissions nécessaires pour redimensionner toutes les images sélectionnées."
+msgstr ""
+"Votre compte na pas les permissions nécessaires pour redimensionner toutes "
+"les images sélectionnées."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Il n'y a aucune image disponible à redimensionner."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Les images suivantes seront redimensionnées :"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Choisissez une option de miniature existante ou entrez des paramètres de redimensionnement :"
+msgstr ""
+"Choisissez une option de miniature existante ou entrez des paramètres de "
+"redimensionnement :"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Choisissez des paramètres de redimensionnement :"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Avertissement : Les images seront redimensionnées en place et les originales seront perdues. Faites-en éventuellement une copie préalable afin de les conserver."
+msgstr ""
+"Avertissement : Les images seront redimensionnées en place et les originales "
+"seront perdues. Faites-en éventuellement une copie préalable afin de les "
+"conserver."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Redimensionner"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Votre compte n'a pas les permissions nécessaires pour déplacer tous les fichiers et/ou dossiers sélectionnés."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Votre compte n'a pas les permissions nécessaires pour déplacer tous les "
+"fichiers et/ou dossiers sélectionnés."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Il n'y a pas de fichiers et/ou dossiers disponibles à déplacer."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Les fichiers et/ou dossiers suivants seront déplacés vers un dossier de destination (en conservant leur arborescence) :"
+msgstr ""
+"Les fichiers et/ou dossiers suivants seront déplacés vers un dossier de "
+"destination (en conservant leur arborescence) :"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Déplacer"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Il est impossible de déplacer des fichiers dans le même dossier"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "Votre compte n'a pas les permissions nécessaires pour renommer tous les fichiers sélectionnés."
+msgstr ""
+"Votre compte n'a pas les permissions nécessaires pour renommer tous les "
+"fichiers sélectionnés."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Il n'y a pas de fichiers disponibles à renommer."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Les fichiers suivants seront renommés (ils resteront dans leurs dossiers et conserveront leur nom de fichier d'origine ; seul le nom affiché sera changé) :"
+msgstr ""
+"Les fichiers suivants seront renommés (ils resteront dans leurs dossiers et "
+"conserveront leur nom de fichier d'origine ; seul le nom affiché sera "
+"changé) :"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Renommer"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Retourner au dossier parent"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Modifier les détails du dossier actuel"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Modifier"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Cliquez ici pour lancer la recherche pour la phrase saisie"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Rechercher"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Fermer"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limite"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Cochez pour limiter la recherche au dossier actuel"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Limiter la recherche au dossier actuel"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Supprimer"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Ajoute un nouveau dossier"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Nouveau dossier"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Téléverser des fichiers"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Vous devez d'abord sélectionner un dossier"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Nom"
 
@@ -937,32 +988,31 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "activé"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "url canonique '%(item_label)s' "
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Télécharger '%(item_label)s' "
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Supprimer le fichier"
 
 #: templates/admin/filer/folder/directory_table_list.html:160
 #: templates/admin/filer/folder/directory_thumbnail_list.html:138
 msgid "Drop files here or use the \"Upload Files\" button"
-msgstr "Déposez des fichiers ici ou utilisez le bouton « Téléverser des fichiers »"
+msgstr ""
+"Déposez des fichiers ici ou utilisez le bouton « Téléverser des fichiers »"
 
 #: templates/admin/filer/folder/directory_table_list.html:175
 #: templates/admin/filer/folder/directory_thumbnail_list.html:153
 msgid "Drop your file to upload into:"
 msgstr "Déposez votre fichier à téléverser dans :"
 
 #: templates/admin/filer/folder/directory_table_list.html:185
@@ -1005,20 +1055,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Sélectionner les %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr "Tout sélectionner"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr "Fichiers"
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Ajouter un nouveau"
@@ -1076,16 +1124,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr "Agrandir"
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr "Le fichier est manquant"
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Type"
 
@@ -1133,39 +1180,46 @@
 msgstr "Recherche"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Sélectionner un fichier"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr "Choisissez un dossier"
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
-msgstr "Fichier \"{file_name}\" : Hébergement refusé par la politique de sécurité du site"
+msgstr ""
+"Fichier \"{file_name}\" : Hébergement refusé par la politique de sécurité du "
+"site"
 
 #: validation.py:22
 #, python-brace-format
 msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
-msgstr "Fichier \"{file_name}\" : hébergement de {file_type} refusé par la politique de sécurité du site"
+msgstr ""
+"Fichier \"{file_name}\" : hébergement de {file_type} refusé par la politique "
+"de sécurité du site"
 
 #: validation.py:33
 #, python-brace-format
 msgid "File \"{file_name}\": HTML upload denied by site security policy"
-msgstr "Fichier \"{file_name}\" : hébergement HTML refusé par la politique de sécurité du site"
+msgstr ""
+"Fichier \"{file_name}\" : hébergement HTML refusé par la politique de "
+"sécurité du site"
 
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
-msgstr "Fichier \"{file_name}\" : Rejeté à cause d'une potentielle vulnérabilité de cross-site scripting"
+msgstr ""
+"Fichier \"{file_name}\" : Rejeté à cause d'une potentielle vulnérabilité de "
+"cross-site scripting"
 
 #~ msgid "Open file"
 #~ msgstr "Open file"
 
 #~ msgid "Full size preview"
 #~ msgstr "Full size preview"
```

### Comparing `django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/gl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Pablo, 2015
 # Pablo, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Pablo, 2015\n"
-"Language-Team: Galician (http://app.transifex.com/divio/django-filer/language/gl/)\n"
+"Language-Team: Galician (http://app.transifex.com/divio/django-filer/"
+"language/gl/)\n"
+"Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Avanzado"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -243,27 +241,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -285,15 +283,15 @@
 msgid "image"
 msgstr "imaxe"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "imaxes"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "usuario"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "arquivos"
 
@@ -315,15 +313,15 @@
 msgstr "elemento do portapapeis"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "elementos do portapapeis"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "carpeta"
 
 #: models/filemodels.py:81
@@ -338,152 +336,166 @@
 msgid "has all mandatory data"
 msgstr "ten todos os datos obrigatorios"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "nome do arquivo orixinal"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nome"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "descrición"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "propietario"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "subido a"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "modificado o"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Permisos desactivados"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "creado o"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Carpeta"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Carpetas"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "todos os elementos"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "só este elemento"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "este elemento e todos os fillos"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tipo"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "grupo"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "todos"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "pode ler"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "pode editar"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "pode engadir fillos"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "permiso da carpeta"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "permisos da carpeta"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data"
 
@@ -520,27 +532,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -577,24 +586,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -639,38 +648,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -696,15 +705,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -737,31 +746,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -780,71 +789,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -929,21 +938,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -997,20 +1004,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1067,16 +1072,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1124,15 +1128,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/he/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/he/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/he/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Hebrew (http://app.transifex.com/divio/django-filer/language/he/)\n"
+"Language-Team: Hebrew (http://app.transifex.com/divio/django-filer/language/"
+"he/)\n"
+"Language: he\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: he\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % 1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
+"1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "מתקדם"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -243,27 +242,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "תיקיה בשם זה כבר קיימת."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -285,15 +284,15 @@
 msgid "image"
 msgstr "תמונה"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "תמונות"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "משתמש"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "קבצים"
 
@@ -315,15 +314,15 @@
 msgstr "פריט לוח"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "פריטי לוח"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "תיקיה"
 
 #: models/filemodels.py:81
@@ -338,152 +337,166 @@
 msgid "has all mandatory data"
 msgstr "כל המידע הנחוץ קיים"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "שם קובץ מקורי"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "שם"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "תיאור"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "בעלים"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "הועלה ב-"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "שונה ב-"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "הרשאות בוטלו"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "נוצר ב-"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "תיקיה"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "תיקיות"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "כל הפריטים"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "פריט זה בלבד"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "פריט זה וכל ילדיו"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "סוג"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "קבוצה"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "כל אחד"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "רשאי לקרוא"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "רשאי לערוך"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "רשאי להוסיף ילדים"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "הרשאת תיקיה"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "הרשאות תיקיה"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "תאריך צילום"
 
@@ -520,27 +533,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "קבצים עם מטה נתונים חסרים"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "שורש"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "הרץ את הפעולה הבחורה"
 
@@ -577,50 +587,56 @@
 msgstr "בית"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "חזור לאפליקציית Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "חזור לתיקיית השורש"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "חזור לתיקיה '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "עבור מחיקת הקבצים ו/או התיקיות הבחורים יש צורך למחוק אובייקטים מקושרים, אך לחשבונך אין הרשאות למחוק אובייקטים מהסוגים הבאים:"
+msgstr ""
+"עבור מחיקת הקבצים ו/או התיקיות הבחורים יש צורך למחוק אובייקטים מקושרים, אך "
+"לחשבונך אין הרשאות למחוק אובייקטים מהסוגים הבאים:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "עבור מחיקת הקבצים ו/או התיקיות הבחורים יש צורך למחוק את האובייקטים המוגנים הבאים:"
+msgstr ""
+"עבור מחיקת הקבצים ו/או התיקיות הבחורים יש צורך למחוק את האובייקטים המוגנים "
+"הבאים:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "האם את/ה בטוח/ה שברצונך למחוק את הקבצים ו/או התיקיות הבחורים? כל הפריטים המקושרים יימחקו:"
+msgstr ""
+"האם את/ה בטוח/ה שברצונך למחוק את הקבצים ו/או התיקיות הבחורים? כל הפריטים "
+"המקושרים יימחקו:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -639,38 +655,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "צפה בתוך האתר"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "חזור ל-"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "דף הניהול הראשי"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "צלמית תיקייה"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr "לחשבונך אין רשות להעתיק את כל הקבצים ו/או התיקיות הבחורים."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -687,24 +703,25 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "אין קבצים ו/או תיקיות זמינים להעתקה."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "הקבצים ו/או התיקיות הבאים יועתקו לתיקיית יעד (תוך שמירה על מבנה העץ שלהם):"
+msgstr ""
+"הקבצים ו/או התיקיות הבאים יועתקו לתיקיית יעד (תוך שמירה על מבנה העץ שלהם):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "תיקיית יעד:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "העתק"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -729,39 +746,42 @@
 msgid "Choose resize parameters:"
 msgstr "בחר פרמטרי שינוי גודל:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "הזהרה: התמונות ישונה גודלן במקום והמקוריות יאבדו. אולי ראשית עשה/י העתק שלהם כדי לשמור על המקויות."
+msgstr ""
+"הזהרה: התמונות ישונה גודלן במקום והמקוריות יאבדו. אולי ראשית עשה/י העתק שלהם "
+"כדי לשמור על המקויות."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "שנה גודל"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr "לחשבונך אין רשות להעביר את כל הקבצים ו/או התיקיות הבחורים."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "אין קבצים ו/או תיקיות זמינים להעברה."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "הקבצים ו/או התיקיות הבאים יועברו לתיקיית יעד (תוך שמירה על מבנה העץ שלהם):"
+msgstr ""
+"הקבצים ו/או התיקיות הבאים יועברו לתיקיית יעד (תוך שמירה על מבנה העץ שלהם):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "העבר"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -774,77 +794,79 @@
 msgid "There are no files available to rename."
 msgstr "אין קבצים זמינים לשינוי שמם."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "הקבצים הבאים ישונו שמותיהם (הם יישארו בתיקיות הנוכחיות שלהם ושמם המקורי יישאר - רק שמות התצוגה שלהם ישונו):"
+msgstr ""
+"הקבצים הבאים ישונו שמותיהם (הם יישארו בתיקיות הנוכחיות שלהם ושמם המקורי "
+"יישאר - רק שמות התצוגה שלהם ישונו):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "שנה שם"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "חזור לתיקיה ההורה"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "שנה פרטי תיקיה נוכחית"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "שנה"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "חיפוש"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "מחק"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "מוסיף תיקיה חדשה"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "תיקיה חדשה"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "שם"
 
@@ -933,21 +955,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "מאופשר"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1001,20 +1021,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "הוסף חדש"
@@ -1073,16 +1091,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1130,15 +1147,14 @@
 msgstr "חיפוש"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/hr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Aleks Acimovic, 2022
 # Damir <damir.arbula@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Aleks Acimovic, 2022\n"
-"Language-Team: Croatian (http://app.transifex.com/divio/django-filer/language/hr/)\n"
+"Language-Team: Croatian (http://app.transifex.com/divio/django-filer/"
+"language/hr/)\n"
+"Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: hr\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Napredno"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Stavke moraju biti odabrane kako bi se obavila akcija. Nijedna stavka nije promijenjena."
+msgstr ""
+"Stavke moraju biti odabrane kako bi se obavila akcija. Nijedna stavka nije "
+"promijenjena."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s odabrana"
 msgstr[1] "%(total_count)s odabrano"
@@ -126,15 +127,17 @@
 msgstr ""
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Uspješno premješteno %(count)d datoteka i/ili direktorija u direktorij '%(destination)s'."
+msgstr ""
+"Uspješno premješteno %(count)d datoteka i/ili direktorija u direktorij "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Premjesti datoteke i/ili direktorije"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -151,15 +154,17 @@
 msgstr "Preimenuj datoteke"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Uspješno kopirano %(count)d datoteka i/ili direktorija u direktorij '%(destination)s'."
+msgstr ""
+"Uspješno kopirano %(count)d datoteka i/ili direktorija u direktorij "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopiraj datoteke i/ili direktorije"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -183,15 +188,16 @@
 msgstr "Sufiks koji će biti dodan imenima kopiranih datoteka."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Sufiks treba biti jednostavan i upisan malim slovima poput \"%(valid)s\"."
+msgstr ""
+"Sufiks treba biti jednostavan i upisan malim slovima poput \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Nepoznata vrijednost formata ključa za preimenovanje \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -217,15 +223,16 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "povećaj veličinu"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr "Opcija sličica ili parametri za promjenu veličine moraju biti izabrani."
+msgstr ""
+"Opcija sličica ili parametri za promjenu veličine moraju biti izabrani."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Parametri za promjenu veličine moraju biti izabrani."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -244,27 +251,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Direktorij s ovim imenom već postoji."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -286,15 +293,15 @@
 msgid "image"
 msgstr "slika"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "slike"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "korisnik"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "datoteke"
 
@@ -316,15 +323,15 @@
 msgstr "stavka spremnika"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "stavke spremnika"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "direktorij"
 
 #: models/filemodels.py:81
@@ -339,152 +346,166 @@
 msgid "has all mandatory data"
 msgstr "sadrži sve obavezne podatke"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "originalno ime datoteke"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "ime"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "opis"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "vlasnik"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "postavljeno"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "modificirano"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Ovlasti onemogućene"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "kerirano"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Direktorij"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Direktoriji"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "sve stavke"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "samo ova stavka"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "ova stavka i sva djeca"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tip"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "grupa"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "svi"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "mogu čitati"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "mogu uređivati"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "mogu dodavati djecu"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "ovlast direktorija"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "ovlasti direktorija"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "datum nastanka"
 
@@ -521,27 +542,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "datoteke s nedostajućim metapodacima"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "korijenski"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Pokreni odabranu akciju"
 
@@ -578,50 +596,56 @@
 msgstr "Početna"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Povratak na Filer aplikaciju"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Povratak na korijenski direktorij"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Povratak na direktorij '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Brisanje odabranih objekata bi rezultiralo brisanjem povezanih objekata, ali Vaš korisnički račun nema ovlasti za brisanje slijedećih tipova objekata:"
+msgstr ""
+"Brisanje odabranih objekata bi rezultiralo brisanjem povezanih objekata, ali "
+"Vaš korisnički račun nema ovlasti za brisanje slijedećih tipova objekata:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Brisanje odabranih datoteka i/ili direktorija bi zahtijevalo brisanje slijedećih zaštičenih povezanih objekata:"
+msgstr ""
+"Brisanje odabranih datoteka i/ili direktorija bi zahtijevalo brisanje "
+"slijedećih zaštičenih povezanih objekata:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Jeste li sigurni kako želite obrisati odabrane datoteke i/ili direktorije? Svi navedeni objekti i s njima povezane stavke biti će obrisani:"
+msgstr ""
+"Jeste li sigurni kako želite obrisati odabrane datoteke i/ili direktorije? "
+"Svi navedeni objekti i s njima povezane stavke biti će obrisani:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -640,39 +664,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Pogledaj na stranicama"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Idi natrag na"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "početna stranica administracije"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Ikona direktorija"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Vaš korisnički račun nema ovlasti za kopiranje odabranih datoteka i/ili direktorija."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Vaš korisnički račun nema ovlasti za kopiranje odabranih datoteka i/ili "
+"direktorija."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -688,164 +714,179 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Nema dostupnih datoteka i/ili direktorija za kopiranje."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Slijedeće datoteke i/ili direktoriji biti će kopirani u odredišni direktorij (zadržavajući postojeću strukturu):"
+msgstr ""
+"Slijedeće datoteke i/ili direktoriji biti će kopirani u odredišni direktorij "
+"(zadržavajući postojeću strukturu):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Odredišni direktorij"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopiraj"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Vaš korisnički račun nema ovlasti za promjenu veličina odabranih slika."
+msgstr ""
+"Vaš korisnički račun nema ovlasti za promjenu veličina odabranih slika."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Nema dostupnih slika kojima bi se promijenila veličina."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Slijedećim slikama biti će promijenjena veličina:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Izaberite postojeću opciju sličica ili unesite parametre za promjenu veličine:"
+msgstr ""
+"Izaberite postojeću opciju sličica ili unesite parametre za promjenu "
+"veličine:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Odaberite parametre za promjenu veličine:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Pažnja: Slikama će biti promijenjena veličina, a originali će biti prepisani sa slikama s novom veličinom. Preporuča se prvo kopirati originalne slike prije promjene veličine."
+msgstr ""
+"Pažnja: Slikama će biti promijenjena veličina, a originali će biti prepisani "
+"sa slikama s novom veličinom. Preporuča se prvo kopirati originalne slike "
+"prije promjene veličine."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Promjeni veličinu"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Vaš korisnički račun nema ovlasti za premještaj svih odabranih datoteka i/ili direktorija."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Vaš korisnički račun nema ovlasti za premještaj svih odabranih datoteka i/"
+"ili direktorija."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Nema dostupnih datoteka i/ili direktorija za premještaj."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Slijedeće datoteke i/ili direktoriji biti će premješteni u odredišni direktorij (zadržavajući postojeću strukturu):"
+msgstr ""
+"Slijedeće datoteke i/ili direktoriji biti će premješteni u odredišni "
+"direktorij (zadržavajući postojeću strukturu):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Premjesti"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "Vaš korisnički račun nema ovlasti za preimenovanje svih odabranih datoteka."
+msgstr ""
+"Vaš korisnički račun nema ovlasti za preimenovanje svih odabranih datoteka."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Nema dostupnih datoteka i/ili direktorija za preimenovanje."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Slijedeće datoteke če biti preimenovane (ostati će u svojim direktorijima i zadržati ime datoteke, samo će prikazano ime biti promijenjeno):"
+msgstr ""
+"Slijedeće datoteke če biti preimenovane (ostati će u svojim direktorijima i "
+"zadržati ime datoteke, samo će prikazano ime biti promijenjeno):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Preimenuj"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Vrati se u nadređeni direktorij"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Promijeni detalje trenutnog direktorija"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Promijeni"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Traži"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Obriši"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Dodaje novi direktorij"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Novi direktorij"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Ime"
 
@@ -932,21 +973,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "omogućeno"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1000,20 +1039,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Dodaj novi"
@@ -1071,16 +1108,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1128,15 +1164,14 @@
 msgstr "Pregled"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/hu/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Istvan Farkas <istvan.farkas@gmail.com>, 2016-2017
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Istvan Farkas <istvan.farkas@gmail.com>, 2016-2017\n"
-"Language-Team: Hungarian (http://app.transifex.com/divio/django-filer/language/hu/)\n"
+"Language-Team: Hungarian (http://app.transifex.com/divio/django-filer/"
+"language/hu/)\n"
+"Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Haladó"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "egyedi URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Az akciók végrehajtásához egy vagy több elemet ki kell választani. Egyetlen elem sem változott."
+msgstr ""
+"Az akciók végrehajtásához egy vagy több elemet ki kell választani. Egyetlen "
+"elem sem változott."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s kiválasztva"
 msgstr[1] "Mind (%(total_count)s) kiválasztva"
@@ -124,15 +124,17 @@
 msgstr "A kiválasztott helyen már létezik %s nevű mappa"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d fájl és/vagy mappa sikeresen átmozgatva ebbe a mappába: %(destination)s"
+msgstr ""
+"%(count)d fájl és/vagy mappa sikeresen átmozgatva ebbe a mappába: "
+"%(destination)s"
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Fájlok és/vagy mappák mozgatása"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -149,15 +151,17 @@
 msgstr "Fájlok átnevezése"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d fájl és/vagy mappa sikeresen átmásolva ebbe a mappába: %(destination)s"
+msgstr ""
+"%(count)d fájl és/vagy mappa sikeresen átmásolva ebbe a mappába: "
+"%(destination)s"
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Fájlok és/vagy mappák másolása"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -181,15 +185,17 @@
 msgstr "Utótag, amely a másolt fájlok nevéhez lesz hozzáadva."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Az utótag lehetőleg egyszerű, kisbetűs fájlnév részlet legyen, például \"%(valid)s\"."
+msgstr ""
+"Az utótag lehetőleg egyszerű, kisbetűs fájlnév részlet legyen, például "
+"\"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Ismeretlen átnevezés formázási szó: \"%(key)s\" "
 
 #: admin/forms.py:54
@@ -215,15 +221,16 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "felméretezés"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr "Előnézeti kép beállítást vagy átméretezési paramétert kötelező kiválasztani."
+msgstr ""
+"Előnézeti kép beállítást vagy átméretezési paramétert kötelező kiválasztani."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Átméretezési paramétert kötelező kiválasztani."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -242,27 +249,27 @@
 msgstr "A fókusz helye kívül esik a képen."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "A beírt érték: \"{subject_location}\"."
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Már létezik ilyen nevű mappa."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Fájlkezelő"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -284,15 +291,15 @@
 msgid "image"
 msgstr "kép"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "képek"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "felhasználó"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "fájlok"
 
@@ -314,15 +321,15 @@
 msgstr "vágólap elem"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "vágólap elemek"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "mappa"
 
 #: models/filemodels.py:81
@@ -337,152 +344,168 @@
 msgid "has all mandatory data"
 msgstr "fontos adatok kitöltve"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "eredeti fájlnév"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "név"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "leírás"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "tulajdonos"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "feltöltés ideje"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "módosítás ideje"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Jogosultságok kikapcsolva"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Jogosultságok ellenőrzésének kikapcsolása ennél a fájlnál. Ezt a fájlt bárki letöltheti."
+msgstr ""
+"Jogosultságok ellenőrzésének kikapcsolása ennél a fájlnál. Ezt a fájlt bárki "
+"letöltheti."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "létrehozás ideje"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Mappa"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Mappák"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "minden elem"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "csak ez az elem"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "csak ez az elem, és az alá tartozók"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "engedélyez"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "letilt"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "típus"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "csoport"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "mindenki"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "olvashatja"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "szerkesztheti"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "hozzáadhat gyermekelemet"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "mappa jogosultság"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "mappa jogosultságok"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "fotózás dátuma"
 
@@ -519,27 +542,24 @@
 msgid "Unsorted Uploads"
 msgstr "Kategorizálatlan feltöltések"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "fájlok hiányzó meta adatokkal"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "gyökér"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Kiválasztott akció végrehajtása"
 
@@ -576,50 +596,57 @@
 msgstr "Nyitólap"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Vissza a fájlkezelőbe"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Vissza a gyökérmappába"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Vissza a(z)  '%(folder_name)s'  mappába"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplikátumok"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "A kiválasztott fájlok és mappák törlése csatlakozó elemek törlésével is járna, viszont a jelenlegi fiók nem rendelkezik a megfelelő jogosultságokkal a következő objektum típusok törléséhez:"
+msgstr ""
+"A kiválasztott fájlok és mappák törlése csatlakozó elemek törlésével is "
+"járna, viszont a jelenlegi fiók nem rendelkezik a megfelelő jogosultságokkal "
+"a következő objektum típusok törléséhez:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "A kiválasztott fájlok és mappák törlése azzal járna, hogy a következő kapcsolt elemek is törlődnek:"
+msgstr ""
+"A kiválasztott fájlok és mappák törlése azzal járna, hogy a következő "
+"kapcsolt elemek is törlődnek:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Biztosan törli a kiválasztott fájlokat és/vagy mappákat? A következő objektumok, és a hozzájuk kapcsolt elemek is törlődni fognak:"
+msgstr ""
+"Biztosan törli a kiválasztott fájlokat és/vagy mappákat? A következő "
+"objektumok, és a hozzájuk kapcsolt elemek is törlődni fognak:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Nem, mégsem"
 
@@ -638,39 +665,40 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Megtekintés az oldalon"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Vissza ide:"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "adminisztrációs felület"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Mappa Ikon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Nincs jogosultsága az összes kiválasztott fájl és/vagy mappa másolásához."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Nincs jogosultsága az összes kiválasztott fájl és/vagy mappa másolásához."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -686,24 +714,26 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Nincsenek másolható fájlok és/vagy könyvtárak"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "A következő fájlok és/vagy mappák lesznek a célkönyvtárba másolva (megtartva a szerkezetüket):"
+msgstr ""
+"A következő fájlok és/vagy mappák lesznek a célkönyvtárba másolva (megtartva "
+"a szerkezetüket):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Cél mappa:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Másol"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Nem lehet fájlokat a saját könyvtárukba másolni"
 
@@ -718,49 +748,56 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "A következő képek lesznek átméretezve:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Válasszon ki egy meglévő előnézeti kép beállítást, vagy írja be az átméretezési paramétereket:"
+msgstr ""
+"Válasszon ki egy meglévő előnézeti kép beállítást, vagy írja be az "
+"átméretezési paramétereket:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Válasszon átméretezési paramétereket:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Figyelem: a képek helyben lesznek átméretezve, felülírva az eredetieket. Ha meg szeretné őrizni az eredeti képeket, előbb másolja át őket."
+msgstr ""
+"Figyelem: a képek helyben lesznek átméretezve, felülírva az eredetieket. Ha "
+"meg szeretné őrizni az eredeti képeket, előbb másolja át őket."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Átméretezés"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Nincs jogosultsága az összes kiválasztott fájl és/vagy mappa mozgatásához."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Nincs jogosultsága az összes kiválasztott fájl és/vagy mappa mozgatásához."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Nincsenek mozgatható fájlok és/vagy mappák."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "A következő fájlok és/vagy mappák lesznek átmozgatva a cél mappába (megtartva a szerkezetüket):"
+msgstr ""
+"A következő fájlok és/vagy mappák lesznek átmozgatva a cél mappába "
+"(megtartva a szerkezetüket):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Mozgatás"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Nem lehet fájlokat az eredeti mappájukba mozgatni"
 
@@ -773,77 +810,79 @@
 msgid "There are no files available to rename."
 msgstr "Nincsenek átnevezhető fájlok."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "A következő fájlok lesznek átnevezve (a mappában maradnak, és az eredeti fájlnév megmarad, csak a megjelenített név változik):"
+msgstr ""
+"A következő fájlok lesznek átnevezve (a mappában maradnak, és az eredeti "
+"fájlnév megmarad, csak a megjelenített név változik):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Átnevezés"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Vissza a szülőmappába"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Jelenlegi mappa beállításai"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Szerkeszt"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Kattintson ide a beírt szó kereséséhez"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Keresés"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Bezár"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Korlátozás"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Kattintsa be, hogy a keresést a jelenlegi mappára korlátozza"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Keresés korlátozása a jelenlegi mappára"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Törlés"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Új mappát hoz létre"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Új mappa"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Fájlok feltöltése"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Először válasszon mappát"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Név"
 
@@ -928,32 +967,31 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "engedélyezve"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "'%(item_label)s' letöltése"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Fájl eltávolítása"
 
 #: templates/admin/filer/folder/directory_table_list.html:160
 #: templates/admin/filer/folder/directory_thumbnail_list.html:138
 msgid "Drop files here or use the \"Upload Files\" button"
-msgstr "Egérrel dobjon ide fájlokat, vagy használja a \"Fájlok feltöltése\" gombot"
+msgstr ""
+"Egérrel dobjon ide fájlokat, vagy használja a \"Fájlok feltöltése\" gombot"
 
 #: templates/admin/filer/folder/directory_table_list.html:175
 #: templates/admin/filer/folder/directory_thumbnail_list.html:153
 msgid "Drop your file to upload into:"
 msgstr "Egérre dobja ide a fájl, hogy feltöltse ebbe a mappába:"
 
 #: templates/admin/filer/folder/directory_table_list.html:185
@@ -996,20 +1034,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Összes (%(total_count)s) kiválasztása"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Új"
@@ -1066,16 +1102,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Típus"
 
@@ -1123,15 +1158,14 @@
 msgstr "Keresés"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Fájl kiválasztása"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/it/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/it/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/it/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # yakky <i.spalletti@nephila.it>, 2012
 # yakky <i.spalletti@nephila.it>, 2013,2015-2018
 # yakky <i.spalletti@nephila.it>, 2012
 # yakky <i.spalletti@nephila.it>, 2012-2013,2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: yakky <i.spalletti@nephila.it>, 2013,2015-2018\n"
-"Language-Team: Italian (http://app.transifex.com/divio/django-filer/language/it/)\n"
+"Language-Team: Italian (http://app.transifex.com/divio/django-filer/language/"
+"it/)\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: it\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
+"1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Avanzato"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "URL standard"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Gli elementi devono essere selezionati in modo da eseguire azioni su di essi. Nessun elemento è stato modificato."
+msgstr ""
+"Gli elementi devono essere selezionati in modo da eseguire azioni su di "
+"essi. Nessun elemento è stato modificato."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] " %(total_count)s elemento selezionato"
 msgstr[1] "Tutti e %(total_count)s selezionati"
@@ -128,15 +129,17 @@
 msgstr "Esistono altre cartelle chiamate %s nella destinazione selezionata"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d file e/o le cartelle spostati con successo nella cartella '%(destination)s'."
+msgstr ""
+"%(count)d file e/o le cartelle spostati con successo nella cartella "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Sposta i file e/o le cartelle"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -153,15 +156,17 @@
 msgstr "Rinomina file"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d file e/o cartelle copiati con successo nella cartella '%(destination)s '."
+msgstr ""
+"%(count)d file e/o cartelle copiati con successo nella cartella "
+"'%(destination)s '."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copia i file e/o le cartelle"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -185,15 +190,17 @@
 msgstr "Suffisso che sarà aggiunto al nome dei file copiati."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Il suffisso deve essere una sezione del nome del file valida, semplice e minuscola, come \"%(valid)s\"."
+msgstr ""
+"Il suffisso deve essere una sezione del nome del file valida, semplice e "
+"minuscola, come \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Valore del formato di rinomina non valido \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -219,15 +226,17 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "ingrandisci"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr "Devi selezionare l'opzione anteprima immagine o i parametri di ridimensionamento."
+msgstr ""
+"Devi selezionare l'opzione anteprima immagine o i parametri di "
+"ridimensionamento."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Seleziona le opzioni di ridimensionamento."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -246,27 +255,27 @@
 msgstr "La posizione del soggetto è esterna all'immagine."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Valore fornito: \"{subject_location}\""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Esiste già una cartella con questo nome."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -288,15 +297,15 @@
 msgid "image"
 msgstr "immagine"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "immagini"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "utente"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "file"
 
@@ -318,15 +327,15 @@
 msgstr "elemento degli appunti"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "elementi degli appunti"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "cartella"
 
 #: models/filemodels.py:81
@@ -341,152 +350,168 @@
 msgid "has all mandatory data"
 msgstr "ha tutti i dati obbligatori"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "nome del file originale"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nome"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "descrizione"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "proprietario"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "caricato il"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "modificato il"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Permessi disabilitati"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Disabilita ogni controllo dei permessi per questo file. Il file sarà accessibile da chiunque"
+msgstr ""
+"Disabilita ogni controllo dei permessi per questo file. Il file sarà "
+"accessibile da chiunque"
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "creato il"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Cartella"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Cartelle"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "tutti gli elementi"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "solo questo elemento"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "questo elemento e tutti i figli"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "permetti"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "nega"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tipo"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "gruppo"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "tutti"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "può leggere"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "può modificare"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "può aggiungere figli"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "permessi cartella"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "permessi cartella"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data di creazione"
 
@@ -523,27 +548,24 @@
 msgid "Unsorted Uploads"
 msgstr "File non archiviati"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "file con metadati mancanti"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "cartella principale"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Esegui l'azione selezionata"
 
@@ -580,50 +602,57 @@
 msgstr "Pagina iniziale"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Torna all'app Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Torna alla cartella principale"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Torna alla  cartella ' %(folder_name)s '"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplicati"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Cancellare i file selezionati e/o cartelle comporta l'eliminazione degli oggetti correlati, ma il tuo account non dispone dell'autorizzazione per eliminare i seguenti tipi di oggetti:"
+msgstr ""
+"Cancellare i file selezionati e/o cartelle comporta l'eliminazione degli "
+"oggetti correlati, ma il tuo account non dispone dell'autorizzazione per "
+"eliminare i seguenti tipi di oggetti:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Cancellare i file selezionati e/o cartelle richiede eliminazione dei seguenti oggetti protetti correlati:"
+msgstr ""
+"Cancellare i file selezionati e/o cartelle richiede eliminazione dei "
+"seguenti oggetti protetti correlati:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Sei sicuro di voler cancellare i file selezionati e/o le cartelle? Tutti gli oggetti seguenti e quelli correlati verranno cancellati:"
+msgstr ""
+"Sei sicuro di voler cancellare i file selezionati e/o le cartelle? Tutti gli "
+"oggetti seguenti e quelli correlati verranno cancellati:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "No, torna indietro"
 
@@ -642,39 +671,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Vedi sul sito"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Torna a"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "Pagina iniziale admin"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Icona della cartella"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Il tuo account non dispone delle autorizzazioni per copiare tutti i file e/o cartelle selezionati."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Il tuo account non dispone delle autorizzazioni per copiare tutti i file e/o "
+"cartelle selezionati."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -690,164 +721,181 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Non ci sono file e/o le cartelle disponibili per la copia."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "I seguenti file e/o cartelle verranno copiati in una cartella di destinazione (mantenendo la loro struttura ad albero):"
+msgstr ""
+"I seguenti file e/o cartelle verranno copiati in una cartella di "
+"destinazione (mantenendo la loro struttura ad albero):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Cartella di destinazione:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Copia"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Non è autorizzato a copiare file nella stessa cartella"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Il tuo account non dispone delle autorizzazioni per ridimensionare tutte le immagini selezionate."
+msgstr ""
+"Il tuo account non dispone delle autorizzazioni per ridimensionare tutte le "
+"immagini selezionate."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Non ci sono immagini disponibili da ridimensionare."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Le seguenti immagini verranno ridimensionate:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Scegli un'opzione miniatura esistente o immetti i parametri di ridimensionamento:"
+msgstr ""
+"Scegli un'opzione miniatura esistente o immetti i parametri di "
+"ridimensionamento:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Scegli i parametri di ridimensionamento:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Attenzione: Le immagini verranno ridimensionate ora e le immagini originali andranno perse. Forse è meglio fare una copia per mantenere i file originali."
+msgstr ""
+"Attenzione: Le immagini verranno ridimensionate ora e le immagini originali "
+"andranno perse. Forse è meglio fare una copia per mantenere i file originali."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Ridimensiona"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Il tuo account non dispone delle autorizzazioni per spostare tutti i file e/o cartelle selezionati."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Il tuo account non dispone delle autorizzazioni per spostare tutti i file e/"
+"o cartelle selezionati."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Non ci sono file e/o cartelle a disponibili per lo spostamento."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "I seguenti file e/o cartelle verranno spostati in una cartella di destinazione (mantenendo la loro struttura ad albero):"
+msgstr ""
+"I seguenti file e/o cartelle verranno spostati in una cartella di "
+"destinazione (mantenendo la loro struttura ad albero):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Sposta"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Non è autorizzato a spostare file nella stessa cartella"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "Il tuo account non dispone delle autorizzazioni per rinominare tutti i file selezionati."
+msgstr ""
+"Il tuo account non dispone delle autorizzazioni per rinominare tutti i file "
+"selezionati."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Non ci sono file disponibili da rinominare."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "I file seguenti saranno rinominati (rimarranno nelle rispettive cartelle e manterranno il nome del file originario, solo il nome visualizzato sarà modificato):"
+msgstr ""
+"I file seguenti saranno rinominati (rimarranno nelle rispettive cartelle e "
+"manterranno il nome del file originario, solo il nome visualizzato sarà "
+"modificato):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Rinomina"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Torna alla cartella superiore"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Modifica i dettagli della cartella corrente"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Modifica"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Clicca qui per eseguire la ricerca della frase inserita"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Cerca"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Chiudi"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limita"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Seleziona per limitare la ricerca alla cartella corrente"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Limita la ricerca alla cartella corrente"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Cancella"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Aggiungi una nuova cartella"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Nuova cartella"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Carica file"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "E' necessario selezionare prima una cartella"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Nome"
 
@@ -934,21 +982,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "abilitato"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "URL canonico '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Download '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Cancella file"
 
@@ -1002,20 +1048,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Seleziona tutti %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Aggiungi nuovo"
@@ -1073,16 +1117,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipo"
 
@@ -1130,15 +1173,14 @@
 msgstr "Consultazione"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Seleziona file"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/ja/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Japanese (http://app.transifex.com/divio/django-filer/language/ja/)\n"
+"Language-Team: Japanese (Japan) (http://app.transifex.com/divio/django-filer/"
+"language/ja_JP/)\n"
+"Language: ja_JP\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -240,27 +238,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -282,15 +280,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -312,15 +310,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -335,152 +333,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -517,27 +529,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -574,24 +583,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -636,38 +645,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -693,15 +702,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -734,31 +743,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -777,71 +786,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -924,21 +933,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -992,20 +999,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1061,16 +1066,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1118,15 +1122,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/ja_JP/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/zh/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Japanese (Japan) (http://app.transifex.com/divio/django-filer/language/ja_JP/)\n"
+"Language-Team: Chinese (http://app.transifex.com/divio/django-filer/language/"
+"zh/)\n"
+"Language: zh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ja_JP\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -240,27 +238,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -282,15 +280,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -312,15 +310,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -335,152 +333,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -517,27 +529,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -574,24 +583,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -636,38 +645,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -693,15 +702,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -734,31 +743,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -777,71 +786,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -924,21 +933,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -992,20 +999,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1061,16 +1066,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1118,15 +1122,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/lt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Matas Dailyda <matas@dailyda.com>, 2015-2018
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Matas Dailyda <matas@dailyda.com>, 2015-2018\n"
-"Language-Team: Lithuanian (http://app.transifex.com/divio/django-filer/language/lt/)\n"
+"Language-Team: Lithuanian (http://app.transifex.com/divio/django-filer/"
+"language/lt/)\n"
+"Language: lt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: lt\n"
-"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
+"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
+"1 : n % 1 != 0 ? 2: 3);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Išplėstinės funkcijos"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "kanoninis URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Objektai turi būti pasirinkti, kad su jais būtų galima atlikti veiksmus. Jokie objektai nebuvo pakeisti."
+msgstr ""
+"Objektai turi būti pasirinkti, kad su jais būtų galima atlikti veiksmus. "
+"Jokie objektai nebuvo pakeisti."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "pasirinkta %(total_count)s"
 msgstr[1] "pasirinkta %(total_count)s"
@@ -119,22 +121,25 @@
 #: admin/folderadmin.py:811
 msgid "Delete selected files and/or folders"
 msgstr "Pašalinti pasirinktus failus ir / ar aplankus"
 
 #: admin/folderadmin.py:918
 #, python-format
 msgid "Folders with names %s already exist at the selected destination"
-msgstr "Aplankai su %s pavadinimais jau egzistuoja pasirinktoje paskirties vietoje."
+msgstr ""
+"Aplankai su %s pavadinimais jau egzistuoja pasirinktoje paskirties vietoje."
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Sėkmingai perkelti %(count)d failai ir / ar aplankai į aplanką '%(destination)s'."
+msgstr ""
+"Sėkmingai perkelti %(count)d failai ir / ar aplankai į aplanką "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Perkelti failus ir / ar aplankus"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -151,15 +156,17 @@
 msgstr "Pervardinti failus"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Sėkmingai nukopijuoti %(count)d failai ir / ar aplankai į aplanką '%(destination)s'."
+msgstr ""
+"Sėkmingai nukopijuoti %(count)d failai ir / ar aplankai į aplanką "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopijuoti failus ir / ar aplankus"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -183,15 +190,17 @@
 msgstr "Priesaga kuri bus pridėta prie nukopijuotų failų pavadinimų."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Priesaga turi būti paprasta ir taisyklinga bylos pavadinimo dalis pvz.  \"%(valid)s\"."
+msgstr ""
+"Priesaga turi būti paprasta ir taisyklinga bylos pavadinimo dalis pvz.  "
+"\"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Nežinomas pervardinimo formato reikšmės raktažodis \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -217,15 +226,16 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "išdidinti"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr "Miniatiūros nustatymas arba dydžio keitimo parametrai turi būti pasirinkti."
+msgstr ""
+"Miniatiūros nustatymas arba dydžio keitimo parametrai turi būti pasirinkti."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Turi būti pasirinkti dydžio keitimo parametrai."
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -244,27 +254,27 @@
 msgstr "Subjekto vieta yra už paveikslėlio."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Jūsų įvestis: \"{subject_location}\". "
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Aplankas su tokiu pavadinimu jau egzistuoja."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer'is"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -286,15 +296,15 @@
 msgid "image"
 msgstr "paveikslėlis"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "paveikslėliai"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "vartotojas"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "failai"
 
@@ -316,15 +326,15 @@
 msgstr "iškarpinės objektas"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "iškarpinės objektai"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "aplankas"
 
 #: models/filemodels.py:81
@@ -339,152 +349,168 @@
 msgid "has all mandatory data"
 msgstr "turi visus privalomus duomenis"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "originalus failo pavadinimas"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "pavadinimas"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "apibūdinimas"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "savininkas"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "įkelta"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "pakeista"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Leidimai išjungti"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Įšjungti bet kokius leidimų tikrinimus šiai bylai. Byla bus viešai pasiekiama bet kam."
+msgstr ""
+"Įšjungti bet kokius leidimų tikrinimus šiai bylai. Byla bus viešai "
+"pasiekiama bet kam."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "sukurta"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Aplankas"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Aplankai"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "visi objektai"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "tik šį objektą"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "šį objektą ir visus vidinius"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "leisti"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "neleisti"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tipas"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "grupė"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "visi"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "gali skaityti"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "gali redaguoti"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "gali pridėti vidinius"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "aplanko leidimas"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "aplanko leidimai"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "paimta data"
 
@@ -521,27 +547,24 @@
 msgid "Unsorted Uploads"
 msgstr "Nerūšiuotos įkeltos bylos"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "failai su trūkstamais meta duomenimis"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "pradinis"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Vykdyti pasirinktą veiksmą"
 
@@ -578,50 +601,56 @@
 msgstr "Pradinis"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Grįžti į Failer'io apklikaciją"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Grįžti į pradinį aplanką"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Grįžti į '%(folder_name)s' aplanką"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Dublikatai"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Pasirintų failų ir / ar aplankų šalinimas pašalintų susijusius objektus, tačiau jūsų vartotojas neturi leidimo šalinti šių objektų tipų:"
+msgstr ""
+"Pasirintų failų ir / ar aplankų šalinimas pašalintų susijusius objektus, "
+"tačiau jūsų vartotojas neturi leidimo šalinti šių objektų tipų:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Pasirinktų failų ir / ar aplankų šalinimas reikalautų pašalinti šiuos apsaugotus susijusius objektus:"
+msgstr ""
+"Pasirinktų failų ir / ar aplankų šalinimas reikalautų pašalinti šiuos "
+"apsaugotus susijusius objektus:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Ar tikrai norite pašalinti pasirinktus failus ir / ar aplankus? Visi susiję objektai bus pašalinti:"
+msgstr ""
+"Ar tikrai norite pašalinti pasirinktus failus ir / ar aplankus? Visi susiję "
+"objektai bus pašalinti:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Ne, grįžti atgal"
 
@@ -640,39 +669,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Žiūrėti puslapyje"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Grįžti į"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "administravimo pradinis puslapis"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Aplanko piktograma"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Jūsų vartotojas neturi leidimų kopijuoti visus pasirinktus failus ir / ar aplankus."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Jūsų vartotojas neturi leidimų kopijuoti visus pasirinktus failus ir / ar "
+"aplankus."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -688,81 +719,93 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Nėra jokiu failų ir / ar aplankų kopijavimui."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Šie failai ir / ar aplankai bus nukopijuoti į paskirtą aplanką (išlaikant jų medžio struktūrą):"
+msgstr ""
+"Šie failai ir / ar aplankai bus nukopijuoti į paskirtą aplanką (išlaikant jų "
+"medžio struktūrą):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Paskyrimo aplankas:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopijuoti"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Neleidžiama kopijuoti bylų į tą patį aplanką"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Jūsų vartotojas neturi leidimų keisti dydžius visiems pasirinktiems paveikslėliams."
+msgstr ""
+"Jūsų vartotojas neturi leidimų keisti dydžius visiems pasirinktiems "
+"paveikslėliams."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Nėra jokiu paveikslėlių dydžio keitimui."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Šių paveikslėlių dydis bus pakeistas:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Pasirinkite esamą miniatiūros nustatymą, arba įveskite dydžio keitimo parametrus:"
+msgstr ""
+"Pasirinkite esamą miniatiūros nustatymą, arba įveskite dydžio keitimo "
+"parametrus:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Pasirinkite dydžio keitimo parametrus:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Įspėjimas: Paveikslėlių dydžiai bus pakeisti vietoje, ir originalas bus pašalintas. Patartina atsikopijuoti paveikslėlį, kad nedingtų originalas."
+msgstr ""
+"Įspėjimas: Paveikslėlių dydžiai bus pakeisti vietoje, ir originalas bus "
+"pašalintas. Patartina atsikopijuoti paveikslėlį, kad nedingtų originalas."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Pakeisti dydį"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Jūsų vartotojas neturi leidimų perkelti visus pasirinktus failus ir / ar aplankus."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Jūsų vartotojas neturi leidimų perkelti visus pasirinktus failus ir / ar "
+"aplankus."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Nėra jokiu failų ir / ar aplankų perkelimui."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Šie failai ir / ar aplankai bus perkelti į paskirtą aplanką (išlaikant jų medžio struktūrą):"
+msgstr ""
+"Šie failai ir / ar aplankai bus perkelti į paskirtą aplanką (išlaikant jų "
+"medžio struktūrą):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Perkelti"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Neleidžiama perkelti bylų į tą patį aplanką"
 
@@ -775,77 +818,79 @@
 msgid "There are no files available to rename."
 msgstr "Nėra jokių failų pervardinimui."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Šie failai bus pervardinti (jie liks savo aplankuose ir pasiliks savo originalius pavadinimus, pasikeis tik atvaizduojamas failo pavadinimas):"
+msgstr ""
+"Šie failai bus pervardinti (jie liks savo aplankuose ir pasiliks savo "
+"originalius pavadinimus, pasikeis tik atvaizduojamas failo pavadinimas):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Pervardinti"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Grįžti į pirminį aplanką"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Keisti dabartinio aplanko detales"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Keisti"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Spausti čia kad būtų paleista paieška visai frazei"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Ieškoti"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Uždaryti"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limitas"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Pažymėti, kad paieška būtų apribota tik dabartiniame aplanke"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Apriboti paieška tik dabartiniame aplanke"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Pašalinti"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Sukuria naują aplanką"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Naujas aplankas"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "įkelti bylas"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Pirma turite pasirinkti aplanką"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Pavadinimas"
 
@@ -934,21 +979,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "įjungta"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Kanoninis url '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Parsisiųsti '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Pašalinti bylą"
 
@@ -1002,20 +1045,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Pasirinkti visus %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Pridėti naują"
@@ -1074,16 +1115,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipas"
 
@@ -1131,15 +1171,14 @@
 msgstr "Informacijos ieškojimas"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Pasirinkti bylą"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/ar/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Lithuanian (Lithuania) (http://app.transifex.com/divio/django-filer/language/lt_LT/)\n"
+"Language-Team: Arabic (http://app.transifex.com/divio/django-filer/language/"
+"ar/)\n"
+"Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: lt_LT\n"
-"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
+"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -52,14 +51,16 @@
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
+msgstr[4] ""
+msgstr[5] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -243,27 +244,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -285,15 +286,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -315,15 +316,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -338,152 +339,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -520,27 +535,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -577,24 +589,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -639,38 +651,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -696,15 +708,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -737,31 +749,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -780,71 +792,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -879,24 +891,28 @@
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
+msgstr[4] ""
+msgstr[5] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
+msgstr[4] ""
+msgstr[5] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -933,21 +949,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1001,20 +1015,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1026,14 +1038,16 @@
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
+msgstr[4] ""
+msgstr[5] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1073,16 +1087,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1130,15 +1143,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1199,10 +1211,12 @@
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
 #~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
 #~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
 #~ msgstr[3] "15c0f2d28d6dab1af1f6d94906beb627_pl_3"
+#~ msgstr[4] "15c0f2d28d6dab1af1f6d94906beb627_pl_4"
+#~ msgstr[5] "15c0f2d28d6dab1af1f6d94906beb627_pl_5"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/nb/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Eirik Krogstad <eirikkr@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Eirik Krogstad <eirikkr@gmail.com>, 2013\n"
-"Language-Team: Norwegian Bokmål (http://app.transifex.com/divio/django-filer/language/nb/)\n"
+"Language-Team: Norwegian Bokmål (http://app.transifex.com/divio/django-filer/"
+"language/nb/)\n"
+"Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Avansert"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Du må velge noen elementer for å utføre handlinger på dem. Ingen elementer er endret."
+msgstr ""
+"Du må velge noen elementer for å utføre handlinger på dem. Ingen elementer "
+"er endret."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s valgt"
 msgstr[1] "Alle %(total_count)s valgt"
@@ -124,15 +124,16 @@
 msgstr ""
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Flyttet %(count)d filer og/eller mapper til mappen \"%(destination)s\"."
+msgstr ""
+"Flyttet %(count)d filer og/eller mapper til mappen \"%(destination)s\"."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Flytt filer og/eller mapper"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -149,15 +150,16 @@
 msgstr "Endre navn på filer"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Kopierte %(count)d filer og/eller mapper til mappen \"%(destination)s\"."
+msgstr ""
+"Kopierte %(count)d filer og/eller mapper til mappen \"%(destination)s\"."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopier filer og/eller mapper"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -181,15 +183,17 @@
 msgstr "Endelse som vil tilføyes filnavn på kopierte filer."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Endelse bør være en gyldig, enkel del av filnavnet med små bokstaver, som \"%(valid)s\"."
+msgstr ""
+"Endelse bør være en gyldig, enkel del av filnavnet med små bokstaver, som "
+"\"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Ugyldig nøkkel \"%(key)s\" for endring av navn."
 
 #: admin/forms.py:54
@@ -242,27 +246,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "En mappe med dette navnet eksisterer allerede."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -284,15 +288,15 @@
 msgid "image"
 msgstr "bilde"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "bilder"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "bruker"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "filer"
 
@@ -314,15 +318,15 @@
 msgstr "element på utklippstavle"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "elementer på utklippstavle"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "mappe"
 
 #: models/filemodels.py:81
@@ -337,152 +341,166 @@
 msgid "has all mandatory data"
 msgstr "har alle påkrevde data"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "originalt filnavn"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "navn"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "beskrivelse"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "eier"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "lastet opp"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "endret"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Tillatelser er deaktivert"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "opprettet"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Mappe"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Mapper"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "alle elementer"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "kun dette elementet"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "dette elementet og alle underliggende nivå"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "type"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "gruppe"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "alle"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "kan lese"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "kan redigere"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "kan legge til undernivåer"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "tillatelse for mappe"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "tillatelser for mappe"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "dato bildet ble tatt"
 
@@ -519,27 +537,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "filer med manglende metadata"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "rot"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Utfør den valgte handlingen"
 
@@ -576,50 +591,57 @@
 msgstr "Hjem"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Gå tilbake til Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Gå tilbake til rotmappen"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Gå tilbake til mappen \"%(folder_name)s\""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Å slette de valgte filene og/eller mappene ville resultere i sletting av relaterte objekter, men din konto har ikke tillatelse til å slette objekter av følgende typer:"
+msgstr ""
+"Å slette de valgte filene og/eller mappene ville resultere i sletting av "
+"relaterte objekter, men din konto har ikke tillatelse til å slette objekter "
+"av følgende typer:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Å slette de valgte filene og/eller mappene ville kreve å slette følgende beskyttede relaterte objekter:"
+msgstr ""
+"Å slette de valgte filene og/eller mappene ville kreve å slette følgende "
+"beskyttede relaterte objekter:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Er du sikker på at du vil slette de valgte filene og/eller mappene? Alle de følgende objektene og deres relaterte elementer vil bli slettet:"
+msgstr ""
+"Er du sikker på at du vil slette de valgte filene og/eller mappene? Alle de "
+"følgende objektene og deres relaterte elementer vil bli slettet:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -638,39 +660,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Se på nettstedet"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Gå tilbake til"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "administrasjonssiden"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Mappeikon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Din konto har ikke tillatelse til å kopiere alle de valgte filene og/eller mappene."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Din konto har ikke tillatelse til å kopiere alle de valgte filene og/eller "
+"mappene."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -686,164 +710,178 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Det er ingen filer og/eller mapper å kopiere."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "De følgende filene og/eller mappene vil bli kopiert til en målmappe (mappestruktur vil beholdes):"
+msgstr ""
+"De følgende filene og/eller mappene vil bli kopiert til en målmappe "
+"(mappestruktur vil beholdes):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Målmappe:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopier"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Din konto har ikke tillatelse til å endre størrelse på alle valgte bilder."
+msgstr ""
+"Din konto har ikke tillatelse til å endre størrelse på alle valgte bilder."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Det er ingen bilder å endre størrelse på."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "De følgende bildene vil få endret størrelse:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Velg et eksisterende miniatyrbildevalg eller skriv inn parametre for endring av størrelse:"
+msgstr ""
+"Velg et eksisterende miniatyrbildevalg eller skriv inn parametre for endring "
+"av størrelse:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Velg parametre for endring av størrelse:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Advarsel: Bilder vil få sin størrelse endret, og originalene vil gå tapt. Det kan være ønskelig å først gjøre en kopi for å beholde originalene."
+msgstr ""
+"Advarsel: Bilder vil få sin størrelse endret, og originalene vil gå tapt. "
+"Det kan være ønskelig å først gjøre en kopi for å beholde originalene."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Endre størrelse"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Din konto har ikke tillatelse til å flytte alle de valgte filene og/eller mappene."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Din konto har ikke tillatelse til å flytte alle de valgte filene og/eller "
+"mappene."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Det er ingen filer og/eller mapper å flytte."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "De følgende filene og/eller mappene vil bli flyttet til en målmappe (mappestruktur vil beholdes):"
+msgstr ""
+"De følgende filene og/eller mappene vil bli flyttet til en målmappe "
+"(mappestruktur vil beholdes):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Flytt"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "Din konto har ikke tillatelse til å endre navn på alle de valgte filene."
+msgstr ""
+"Din konto har ikke tillatelse til å endre navn på alle de valgte filene."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Det er ingen filer å endre navn på."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "De følgende filene vil få endret navn (de vil forbli på samme sted og beholde originalt filnavn, bare visningsnavn vil endres):"
+msgstr ""
+"De følgende filene vil få endret navn (de vil forbli på samme sted og "
+"beholde originalt filnavn, bare visningsnavn vil endres):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Endre navn"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Gå tilbake til overordnet nivå"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Endre detaljer for gjeldende mappe"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Endre"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Søk"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Slett"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Legger til en ny mappe"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Ny mappe"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Navn"
 
@@ -928,21 +966,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "aktivert"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -996,20 +1032,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Legg til ny"
@@ -1066,16 +1100,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1123,15 +1156,14 @@
 msgstr "Slå opp"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Edwin Janssen, 2023\n"
+"Last-Translator: Stefan van den Eertwegh <stefan@corebyte.nl>, 2023\n"
 "Language-Team: Dutch (Netherlands) (http://app.transifex.com/divio/django-"
 "filer/language/nl_NL/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nl_NL\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -55,14 +55,18 @@
 "Weet je zeker dat je de geselecteerde bestanden en/of folders wilt "
 "verwijderen? Alle volgende objecten en gerelateerde items zullen worden "
 "verwijderd: "
 
 msgid "Are you sure?"
 msgstr "Weet je het zeker?"
 
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+"Ten minste één gebruiker, groep of \"iedereen\" moet worden geselecteerd."
+
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 "Kan map niet vinden om te uploaden. Herlaad de pagina en probeer het opnieuw."
 
 msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr "Kan deze map niet gebruiken, rechten geweigerd. Kies een andere map."
 
@@ -242,14 +246,20 @@
 
 msgid "Folder"
 msgstr "Map"
 
 msgid "Folder Icon"
 msgstr "Map icoon"
 
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr "Map kan niet geselecteerd worden met type \"alle items\"."
+
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr "Map moet geselecteerd worden wanneer type niet \"alle items\" is."
+
 msgid "Folder with this name already exists."
 msgstr "Er bestaat al een map met deze naam."
 
 msgid "Folders"
 msgstr "Mappen"
 
 msgid "Folders with names %s already exist at the selected destination"
@@ -541,14 +551,18 @@
 
 msgid "Upload canceled!"
 msgstr "Upload geannuleerd!"
 
 msgid "Upload success!"
 msgstr "Upload succesvol!"
 
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+"Gebruiker of groep kan niet geselecteerd worden samen met \"iedereen\"."
+
 msgid "User: {user}"
 msgstr "Gebruiker:{user}"
 
 msgid "View on site"
 msgstr "Bekijk op site"
 
 msgid ""
```

### Comparing `django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Alexander Schoemaker <alexander.schoemaker@gmail.com>, 2012
 # Alexander Schoemaker <alexander.schoemaker@gmail.com>, 2012
 # Edwin Janssen, 2023
 # Evelijn Saaltink <evelijnsaaltink@gmail.com>, 2017
 # Jeroen, 2018
 # Maikel Wever, 2013
 # Maikel Wever, 2013
+# Stefan van den Eertwegh <stefan@corebyte.nl>, 2023
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Edwin Janssen, 2023\n"
+"Last-Translator: Stefan van den Eertwegh <stefan@corebyte.nl>, 2023\n"
 "Language-Team: Dutch (Netherlands) (http://app.transifex.com/divio/django-filer/language/nl_NL/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: nl_NL\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr "Je hebt geen rechten om bestanden te uploaden."
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
-msgstr "Kan map niet vinden om te uploaden. Herlaad de pagina en probeer het opnieuw."
+msgstr ""
+"Kan map niet vinden om te uploaden. Herlaad de pagina en probeer het opnieuw."
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr "Kan deze map niet gebruiken, rechten geweigerd. Kies een andere map."
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Geavanceerd"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "canonieke URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "De actie kan niet worden uitgevoerd omdat er zijn geen items geselecteerd."
+msgstr ""
+"De actie kan niet worden uitgevoerd omdat er zijn geen items geselecteerd."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s geselecteerd"
 msgstr[1] "Alle %(total_count)s geselecteerd"
@@ -130,15 +129,17 @@
 msgstr "Er bestaan al mappen met de namen %s op de geselecteerde bestemming"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d bestanden en of mappen zijn succesvol verplaatst naar map '%(destination)s'."
+msgstr ""
+"%(count)d bestanden en of mappen zijn succesvol verplaatst naar map "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Verplaats bestanden en/of mappen"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -155,15 +156,17 @@
 msgstr "Hernoem bestanden"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d bestanden en/of mappen zijn succesvol gekopieerd naar map '%(destination)s'."
+msgstr ""
+"%(count)d bestanden en/of mappen zijn succesvol gekopieerd naar map "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopieer bestanden en/of mappen"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -180,22 +183,25 @@
 
 #: admin/folderadmin.py:1292
 msgid "Resize selected images"
 msgstr "Afmetingen aanpassen van geselecteerde afbeeldingen"
 
 #: admin/forms.py:24
 msgid "Suffix which will be appended to filenames of copied files."
-msgstr "Achtervoegsel wordt toegevoegd aan bestandsnaam van gekopieerde bestanden"
+msgstr ""
+"Achtervoegsel wordt toegevoegd aan bestandsnaam van gekopieerde bestanden"
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Achtervoegsel moet een geldige waarde zijn in kleine letters, bv. \"%(valid)s\"."
+msgstr ""
+"Achtervoegsel moet een geldige waarde zijn in kleine letters, bv. "
+"\"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Type \"%(key)s\" voor het hernoemen van bestandsnamen is ongeldig."
 
 #: admin/forms.py:54
@@ -248,27 +254,27 @@
 msgstr "Locatie van het onderwerp bevindt zich buiten de afbeelding."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Je invoer: \"{subject_location}\"."
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr "Wie"
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr "Wat"
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Er bestaat al een map met deze naam."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Bestandsbeheer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -290,15 +296,15 @@
 msgid "image"
 msgstr "afbeelding"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "afbeeldingen"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "gebruiker"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "bestanden"
 
@@ -320,15 +326,15 @@
 msgstr "klembord item"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "klembord items"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "map"
 
 #: models/filemodels.py:81
@@ -343,152 +349,168 @@
 msgid "has all mandatory data"
 msgstr "heeft allen verplichte eigenschappen"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "oorspronkelijke bestandsnaam"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "naam"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "omschrijving"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "eigenaar"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "geüpload op"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "gewijzigd op"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Toegangsrechten uitgeschakeld"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Schakel controle op toegangsrechten uit voor dit bestand. Het bestand zal publiek toegankelijk zijn voor iedereen"
+msgstr ""
+"Schakel controle op toegangsrechten uit voor dit bestand. Het bestand zal "
+"publiek toegankelijk zijn voor iedereen"
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr "ouder"
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "aangemaakt op"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Map"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Mappen"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "alle items"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "alleen dit item"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "dit item en alle onderliggende items"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr "overerven"
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "toestaan"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "afwijzen"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "type"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "groep"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "iedereen"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "mag lezen"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "mag wijzigen"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "mag onderliggende items toevoegen"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "toegangsrecht folder"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "toegangsrechten folder"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr "Map kan niet geselecteerd worden met type \"alle items\"."
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr "Map moet geselecteerd worden wanneer type niet \"alle items\" is."
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr "Gebruiker of groep kan niet geselecteerd worden samen met \"iedereen\"."
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr "Ten minste één gebruiker, groep of \"iedereen\" moet worden geselecteerd."
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr "Alle Mappen"
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr "Logisch Pad"
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr "Gebruiker:{user}"
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr "Groep: {group}"
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr "Iedereen"
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr "Bewerken"
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr "Lezen"
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr "Toevoegen kinderen"
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "datum"
 
@@ -525,27 +547,24 @@
 msgid "Unsorted Uploads"
 msgstr "Ongesorteerde uploads"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "bestanden met ontbrekende meta gegevens"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "hoofdmap"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr "Toon tabel weergave"
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr "Toon thumbnail weergave"
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Geselecteerde actie uitvoeren"
 
@@ -582,50 +601,58 @@
 msgstr "Home"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Ga terug naar Bestandsbeheer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Ga terug naar de hoofdmap"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Ga terug naar map '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplicaten"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Het verwijderen van de geselecteerde bestanden en/of mappen resulteert in het verwijderen van gerelateerde objecten. Je hebt echter geen toegangsrechten voor het verwijderen van de volgende objecttypes:"
+msgstr ""
+"Het verwijderen van de geselecteerde bestanden en/of mappen resulteert in "
+"het verwijderen van gerelateerde objecten. Je hebt echter geen "
+"toegangsrechten voor het verwijderen van de volgende objecttypes:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Het verwijderen van de geselecteerde bestanden en/of mappen leidt tot het verwijderen van de volgende beschermde gerelateerde objecten:"
+msgstr ""
+"Het verwijderen van de geselecteerde bestanden en/of mappen leidt tot het "
+"verwijderen van de volgende beschermde gerelateerde objecten:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Weet je zeker dat je de geselecteerde bestanden en/of folders wilt verwijderen? Alle volgende objecten en gerelateerde items zullen worden verwijderd: "
+msgstr ""
+"Weet je zeker dat je de geselecteerde bestanden en/of folders wilt "
+"verwijderen? Alle volgende objecten en gerelateerde items zullen worden "
+"verwijderd: "
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Nee, ga terug"
 
@@ -644,39 +671,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Bekijk op site"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Ga terug naar"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "admin homepage"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Map icoon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Je account heeft geen toegangsrechten voor het kopiëren van de geselecteerde bestanden en/of mappen"
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Je account heeft geen toegangsrechten voor het kopiëren van de geselecteerde "
+"bestanden en/of mappen"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -692,39 +721,44 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Er zijn geen bestanden en/of mappen beschikbaar om te kopiëren."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "De volgende bestanden en/of mappen zullen worden gekopieerd naar een bestemmingsmap (structuur blijft behouden):"
+msgstr ""
+"De volgende bestanden en/of mappen zullen worden gekopieerd naar een "
+"bestemmingsmap (structuur blijft behouden):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Bestemmingsmap:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopiëren"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Het is niet toegestaan om bestanden naar dezelfde map te kopiëren"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Je account heeft geen toegangsrechten om afmetingen van alle geselecteerde afbeeldingen aan te passen."
+msgstr ""
+"Je account heeft geen toegangsrechten om afmetingen van alle geselecteerde "
+"afbeeldingen aan te passen."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
-msgstr "Er zijn geen afbeeldingen beschikbaar voor het aanpassen van afmetingen."
+msgstr ""
+"Er zijn geen afbeeldingen beschikbaar voor het aanpassen van afmetingen."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "De afmetingen van de volgende afbeeldingen zullen worden aangepast:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
@@ -734,122 +768,134 @@
 msgid "Choose resize parameters:"
 msgstr "Selecteer afmetingsopties:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Waarschuwing: bestaande afmetingen van afbeeldingen zullen worden aangepast. Oorspronkelijke bestanden zullen verloren gaan. Maak eventueel eerst een kopie om de oorspronkelijke bestanden te behouden."
+msgstr ""
+"Waarschuwing: bestaande afmetingen van afbeeldingen zullen worden aangepast. "
+"Oorspronkelijke bestanden zullen verloren gaan. Maak eventueel eerst een "
+"kopie om de oorspronkelijke bestanden te behouden."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Afmetingen aanpassen"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Je account heeft geen toegangsrechten om alle geselecteerde bestanden en/of mappen te verplaatsen."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Je account heeft geen toegangsrechten om alle geselecteerde bestanden en/of "
+"mappen te verplaatsen."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Er zijn geen bestanden en/of mappen beschikbaar om te verplaatsen."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "De volgende bestanden en/of mappen zullen worden verplaatst naar een bestemmingsmap (huidige mapstructuur blijft behouden): "
+msgstr ""
+"De volgende bestanden en/of mappen zullen worden verplaatst naar een "
+"bestemmingsmap (huidige mapstructuur blijft behouden): "
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Verplaatsen"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Het is niet toegestaan om bestanden naar dezelfde map te verplaatsen"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "Je account heeft onvoldoende toegangsrechten om alle geselecteerde bestanden te hernoemen."
+msgstr ""
+"Je account heeft onvoldoende toegangsrechten om alle geselecteerde bestanden "
+"te hernoemen."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Er zijn geen bestanden beschikbaar om te hernoemen."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "De volgende bestanden zullen worden hernoemd (de oorspronkelijke mapstructuur en bestandsnamen blijven behouden, alleen de weergave zal worden gewijzigd):"
+msgstr ""
+"De volgende bestanden zullen worden hernoemd (de oorspronkelijke "
+"mapstructuur en bestandsnamen blijven behouden, alleen de weergave zal "
+"worden gewijzigd):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Hernoemen"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Ga terug naar de bovenliggende folder"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Wijzig eigenschappen van huidige map"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Wijzigen"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Klik hier om een zoekopdracht te doen voor de ingevoerde woorden"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Zoeken"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Sluiten"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limiteren"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Vink het aan om de zoekopdracht te beperken tot de huidige map"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Zoekopdracht beperken tot huidige map"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Verwijderen"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Voegt een nieuwe map toe"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Nieuwe map"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Bestanden uploaden"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Je moet eerst een map selecteren"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Naam"
 
@@ -934,21 +980,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "ingeschakeld"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Gebruikelijke url '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Download '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Verwijder bestand"
 
@@ -1002,20 +1046,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Selecteer alle %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr "Alles selecteren"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr "Bestanden"
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Toevoegen nieuwe"
@@ -1072,16 +1114,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr "Uitvouwen"
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr "Bestand ontbreekt"
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Type"
 
@@ -1129,39 +1170,46 @@
 msgstr "Opzoeken"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Kies bestand"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr "Kies Map"
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
-msgstr "Bestand \"{file_name}\": Upload geweigerd door het beveiligingsbeleid van de site"
+msgstr ""
+"Bestand \"{file_name}\": Upload geweigerd door het beveiligingsbeleid van de "
+"site"
 
 #: validation.py:22
 #, python-brace-format
 msgid "File \"{file_name}\": {file_type} upload denied by site security policy"
-msgstr "Bestand \"{file_name}\": {file_type} upload geweigerd door het beveiligingsbeleid van de site"
+msgstr ""
+"Bestand \"{file_name}\": {file_type} upload geweigerd door het "
+"beveiligingsbeleid van de site"
 
 #: validation.py:33
 #, python-brace-format
 msgid "File \"{file_name}\": HTML upload denied by site security policy"
-msgstr "Bestand \"{file_name}\": HTML upload geweigerd door het beveiligingsbeleid van de site"
+msgstr ""
+"Bestand \"{file_name}\": HTML upload geweigerd door het beveiligingsbeleid "
+"van de site"
 
 #: validation.py:71
 #, python-brace-format
 msgid ""
 "File \"{file_name}\": Rejected due to potential cross site scripting "
 "vulnerability"
-msgstr "Bestand \"{file_name}\": Afgewezen wegens mogelijke kwetsbaarheid voor cross-site scripting"
+msgstr ""
+"Bestand \"{file_name}\": Afgewezen wegens mogelijke kwetsbaarheid voor cross-"
+"site scripting"
 
 #~ msgid "Open file"
 #~ msgstr "Open file"
 
 #~ msgid "Full size preview"
 #~ msgstr "Full size preview"
```

### Comparing `django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/nn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/nn/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Eirik Krogstad <eirikkr@gmail.com>, 2013
 # Eirik Krogstad <eirikkr@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Eirik Krogstad <eirikkr@gmail.com>, 2013\n"
-"Language-Team: Norwegian Nynorsk (http://app.transifex.com/divio/django-filer/language/nn/)\n"
+"Language-Team: Norwegian Nynorsk (http://app.transifex.com/divio/django-"
+"filer/language/nn/)\n"
+"Language: nn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: nn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Avansert"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Element må vere vald for å utføre handlingar på dei. Ingen element vart endra."
+msgstr ""
+"Element må vere vald for å utføre handlingar på dei. Ingen element vart "
+"endra."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s vald"
 msgstr[1] "Alle %(total_count)s vald"
@@ -150,15 +150,16 @@
 msgstr "Endre namn på filer"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Kopierte %(count)d filer og/eller mapper til mappa \"%(destination)s\"."
+msgstr ""
+"Kopierte %(count)d filer og/eller mapper til mappa \"%(destination)s\"."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Kopier filer og/eller mapper"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -182,15 +183,17 @@
 msgstr "Ending som vert tilføyd filnamn på kopierte filer."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Ending bør vere ein gyldig, enkel del av filnamnet med små bokstavar, som \"%(valid)s\"."
+msgstr ""
+"Ending bør vere ein gyldig, enkel del av filnamnet med små bokstavar, som "
+"\"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Ugyldig nykel \"%(key)s\" for endring av namn."
 
 #: admin/forms.py:54
@@ -243,27 +246,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Ein mappe med dette namnet eksisterer allereie."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -285,15 +288,15 @@
 msgid "image"
 msgstr "bilete"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "bilete"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "brukar"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "filer"
 
@@ -315,15 +318,15 @@
 msgstr "element på utklippstavle"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "element på utklippstavle"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "mappe"
 
 #: models/filemodels.py:81
@@ -338,152 +341,166 @@
 msgid "has all mandatory data"
 msgstr "har alle påkravde data"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "originalt filnamn"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "namn"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "beskriving"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "eigar"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "lasta opp"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "endra"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Løyve er deaktivert"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "oppretta"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Mappe"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Mapper"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "alle element"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "berre dette elementet"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "dette elementet og alle underliggjande nivå"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "type"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "gruppe"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "alle"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "kan lese"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "kan redigere"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "kan leggje til undernivå"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "løyve for mappe"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "løyve for mappe"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "dato biletet vert tatt"
 
@@ -520,27 +537,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "filer med manglande metadata"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "rot"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Utfør den valde handlinga"
 
@@ -577,50 +591,57 @@
 msgstr "Heim"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Gå tilbake til Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Gå tilbake til rotmappa"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Gå tilbake til mappa \"%(folder_name)s\""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Å slette dei valde filene og/eller mappene ville resultere i sletting av relaterte objekt, men din konto har ikkje løyve til å slette objekt av følgjande typer:"
+msgstr ""
+"Å slette dei valde filene og/eller mappene ville resultere i sletting av "
+"relaterte objekt, men din konto har ikkje løyve til å slette objekt av "
+"følgjande typer:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Å slette dei valde filene og/eller mappene ville kreve å slette følgjande beskytta relaterte objekt:"
+msgstr ""
+"Å slette dei valde filene og/eller mappene ville kreve å slette følgjande "
+"beskytta relaterte objekt:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Er du sikker på at du vil slette dei valde filene og/eller mappene? Alle dei følgjande objekta og deira relaterte element vil verte sletta:"
+msgstr ""
+"Er du sikker på at du vil slette dei valde filene og/eller mappene? Alle dei "
+"følgjande objekta og deira relaterte element vil verte sletta:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr ""
 
@@ -639,39 +660,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Se på nettstaden"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Gå tilbake til"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "administrasjonssida"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Mappeikon"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Din konto har ikkje løyve til å kopiere alle dei valde filene og/eller mappene."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Din konto har ikkje løyve til å kopiere alle dei valde filene og/eller "
+"mappene."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -687,24 +710,26 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Det er ingen filer og/eller mapper å kopiere."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Dei følgjande filene og/eller mappene vil verte kopiert til ein målmappe (mappestruktur vil behaldes):"
+msgstr ""
+"Dei følgjande filene og/eller mappene vil verte kopiert til ein målmappe "
+"(mappestruktur vil behaldes):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Målmappe:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Kopier"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -719,49 +744,56 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Dei følgjande bileta vil få endra storleik:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Vel eit eksisterande miniatyrbileteval eller skriv inn parametrar for endring av storleik:"
+msgstr ""
+"Vel eit eksisterande miniatyrbileteval eller skriv inn parametrar for "
+"endring av storleik:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Vel parametrar for endring av storleik:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Åtvaring: Bileta vil få sin storleik endra, og originalane vil gå tapt. Det kan være ønskjeleg å først gjere ein kopi for å behalde originalane."
+msgstr ""
+"Åtvaring: Bileta vil få sin storleik endra, og originalane vil gå tapt. Det "
+"kan være ønskjeleg å først gjere ein kopi for å behalde originalane."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Endre storleik"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Din konto har ikke løyve til å flytte alle dei valde filene og/eller mappene."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Din konto har ikke løyve til å flytte alle dei valde filene og/eller mappene."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Det er ingen filer og/eller mapper å flytte."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Dei følgjande filene og/eller mappene vil verte flytta til ein målmappe (mappestruktur vil behaldes):"
+msgstr ""
+"Dei følgjande filene og/eller mappene vil verte flytta til ein målmappe "
+"(mappestruktur vil behaldes):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Flytt"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -774,77 +806,79 @@
 msgid "There are no files available to rename."
 msgstr "Det er ingen filer å endre namn på."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Dei følgjande filene vil få endra namn (dei vil framleis vere på samme stad og behalde originalt filnamn, berre visningsnamn vil verte endra):"
+msgstr ""
+"Dei følgjande filene vil få endra namn (dei vil framleis vere på samme stad "
+"og behalde originalt filnamn, berre visningsnamn vil verte endra):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Endre namn"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Gå tilbake til overordna nivå"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Endre detaljar for gjeldande mappe"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Endre"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Søk"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Slett"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Legg til ein ny mappe"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Ny mappe"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Namn"
 
@@ -929,21 +963,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "aktivert"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -997,20 +1029,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Legg til ny"
@@ -1067,16 +1097,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1124,15 +1153,14 @@
 msgstr "Slå opp"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/pl/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # crunchorn <crunchorn@prokonto.pl>, 2010
 # Grzegorz Biały <grzegorz@elcodo.pl>, 2017
 # Mateusz Marzantowicz <mmarzantowicz@osdf.com.pl>, 2013
 # Piotr Wojcik <pwwpww@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Grzegorz Biały <grzegorz@elcodo.pl>, 2017\n"
-"Language-Team: Polish (http://app.transifex.com/divio/django-filer/language/pl/)\n"
+"Language-Team: Polish (http://app.transifex.com/divio/django-filer/language/"
+"pl/)\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pl\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
+"(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
+"n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Zaawansowane"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "kanoniczny URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Należy zaznaczyć elementy aby wykonań na nich jakąś akcję. Nie zaznaczono żadnych elementów."
+msgstr ""
+"Należy zaznaczyć elementy aby wykonań na nich jakąś akcję. Nie zaznaczono "
+"żadnych elementów."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "zaznaczono %(total_count)s"
 msgstr[1] "zaznaczono %(total_count)s"
@@ -129,15 +131,16 @@
 msgstr "Katalogi z nazwami %s już istnieją w podanej lokacji"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Pomyślnie przeniesiono %(count)d plików i/lub katalogów do '%(destination)s'."
+msgstr ""
+"Pomyślnie przeniesiono %(count)d plików i/lub katalogów do '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Przenieś pliki i/lub katalogi"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -154,15 +157,16 @@
 msgstr "Zmień nazwy plików"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Pomyślnie skopiowano %(count)d plików i/lub katalogów di '%(destination)s'."
+msgstr ""
+"Pomyślnie skopiowano %(count)d plików i/lub katalogów di '%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Skopiuj pliki i/lub katalogi"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -186,15 +190,17 @@
 msgstr "Przyrostek, który zostanie dodany do nazw skopiowanych plików."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Przyrostek powinien być poprawną, prostą, składającą się z małych liter częścią nazwy pliku, np. \"%(valid)s\""
+msgstr ""
+"Przyrostek powinien być poprawną, prostą, składającą się z małych liter "
+"częścią nazwy pliku, np. \"%(valid)s\""
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Nieznany format klucza \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -247,27 +253,27 @@
 msgstr "Współrzędne obiektu znajdują się poza obrazem."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Twój wpis: \"{subject_location}\"."
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Katalog o podanej nazwie już istnieje."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -289,15 +295,15 @@
 msgid "image"
 msgstr "obraz"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "obrazy"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "użytkownik"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "pliki"
 
@@ -319,15 +325,15 @@
 msgstr "element schowka"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "elementy schowka"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "katalog"
 
 #: models/filemodels.py:81
@@ -342,152 +348,168 @@
 msgid "has all mandatory data"
 msgstr "posiada wszystkie potrzebne dane"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "oryginalna nazwa pliku"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nazwa"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "opis"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "właściciel"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "zaktualizowano"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "zmieniono"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Uprawnienia wyłączone"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Wyłącz jakiekolwiek sprawdzanie uprawnień dla tego pliku. Plik będzie dostępny publicznie dla wszystkich."
+msgstr ""
+"Wyłącz jakiekolwiek sprawdzanie uprawnień dla tego pliku. Plik będzie "
+"dostępny publicznie dla wszystkich."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "utworzono"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Katalog"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Katalogi"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "wszystkie elementy"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "tylko ten element"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "ten katalog i wszystkie podrzędne"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "zezwól"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "zabroń"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "typ"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "grupa"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "wszyscy"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "może wyświetlić"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "może edytować"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "może dodawać elementy podrzędne"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "uprawnienie katalogu"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "uprawnienia katalogu"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data wykonania"
 
@@ -524,27 +546,24 @@
 msgid "Unsorted Uploads"
 msgstr "Nieuporządkowane Przesłane"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "pliki z brakującymi metadanymi"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "Katalog główny"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Wykonaj wybraną akcję"
 
@@ -581,50 +600,57 @@
 msgstr "Początek"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Wróć do aplikacji Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Wróć do katalogu głównego"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Przejdź do katalogu '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplikaty"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Usunięcie zaznaczonych plików i/lub katalogów spowoduje usunięcie powiązanych obiektów, niestety Twoje konto nie posiada uprawnień do usunięcia następujących typów obiektów:"
+msgstr ""
+"Usunięcie zaznaczonych plików i/lub katalogów spowoduje usunięcie "
+"powiązanych obiektów, niestety Twoje konto nie posiada uprawnień do "
+"usunięcia następujących typów obiektów:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Usunięcie zaznaczonych plików i/lub katalogów wymaga usunięcia następujących chronionych obiektów powiązanych:"
+msgstr ""
+"Usunięcie zaznaczonych plików i/lub katalogów wymaga usunięcia następujących "
+"chronionych obiektów powiązanych:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Czy na pewno chcesz usunąć zaznaczone pliki i/lub katalogi? Następujące obiekty oraz powiązane z nimi elementy zostaną usunięte:"
+msgstr ""
+"Czy na pewno chcesz usunąć zaznaczone pliki i/lub katalogi? Następujące "
+"obiekty oraz powiązane z nimi elementy zostaną usunięte:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Nie, wróć"
 
@@ -643,39 +669,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Zobacz na stronie"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Wróć do"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "panelu administracyjnego"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Ikona katalogu"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Twoje konto nie ma uprawnień do skopiowania wszystkich zaznaczonych plików i/lub katalogów."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Twoje konto nie ma uprawnień do skopiowania wszystkich zaznaczonych plików i/"
+"lub katalogów."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -691,164 +719,180 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Brak dostępnych plików i/lub katalogów do skopiowania."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Następujące pliki i/lub katalogi zostaną skopiowane do katalogu docelowego (z zachowaniem ich struktury):"
+msgstr ""
+"Następujące pliki i/lub katalogi zostaną skopiowane do katalogu docelowego "
+"(z zachowaniem ich struktury):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Katalog docelowy:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Skopiuj"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Nie można kopiować plików to tego samego folderu"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Twoje konto nie ma uprawnień do zmiany rozmiaru wszystkich zaznaczonych obrazów."
+msgstr ""
+"Twoje konto nie ma uprawnień do zmiany rozmiaru wszystkich zaznaczonych "
+"obrazów."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Brak dostępnych obrazów do zmiany ich rozmiaru."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Następujące obrazy będą miały zmieniony rozmiar:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Wybierz istniejącą opcje miniatury albo wprowadź parametry zmiany rozmiaru:"
+msgstr ""
+"Wybierz istniejącą opcje miniatury albo wprowadź parametry zmiany rozmiaru:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Wybierz parametry zmiany rozmiaru:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Uwaga: Rozmiary obrazów zostanie zmienione w miejscu a oryginały zostaną utracone. W celu zachowania oryginałów, najpierw wykonaj ich kopię."
+msgstr ""
+"Uwaga: Rozmiary obrazów zostanie zmienione w miejscu a oryginały zostaną "
+"utracone. W celu zachowania oryginałów, najpierw wykonaj ich kopię."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Zmień rozmiar"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Twoje konto nie ma uprawnień do przeniesienia wszystkich zaznaczonych plików i/lub katalogów."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Twoje konto nie ma uprawnień do przeniesienia wszystkich zaznaczonych plików "
+"i/lub katalogów."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Brak plików i/lub folderów do przeniesienia."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Następujące pliki i/lub katalogi zostaną przeniesione do katalogu docelowego (z zachowaniem ich struktury):"
+msgstr ""
+"Następujące pliki i/lub katalogi zostaną przeniesione do katalogu docelowego "
+"(z zachowaniem ich struktury):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Przenieś"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Nie można przenieść plików do tego samego folderu"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "Twoje konto nie posiada uprawnień do zmiany nazwy wszystkich zaznaczonych plików."
+msgstr ""
+"Twoje konto nie posiada uprawnień do zmiany nazwy wszystkich zaznaczonych "
+"plików."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Brak dostępnych plików do zmiany nazwy."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Następujące pliki będą miały zmienioną nazwę (pliki pozostaną w swoich katalogach i zachowają oryginalne nazwy, zmieni się jedynie ich wyświetlana nazwa):"
+msgstr ""
+"Następujące pliki będą miały zmienioną nazwę (pliki pozostaną w swoich "
+"katalogach i zachowają oryginalne nazwy, zmieni się jedynie ich wyświetlana "
+"nazwa):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Zmień nazwę"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Wróć do katalogu nadrzędnego"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Zmień dane aktualnie wyświetlanego katalogu"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Zmień"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Kliknij tutaj aby szukać daną frazę"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Szukaj"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Zamknij"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limit"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Zaznacz, by ograniczyć szukanie do bieżącego folderu"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Ogranicz szukanie do bieżącego folderu"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Usuń"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Dodaje nowy katalog"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Nowy katalog"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Wyślij Pliki"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Musisz najpierw wybrać katalog"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Nazwa"
 
@@ -937,21 +981,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "włączony"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Kanoniczny url '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Pobierz '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Usuń plik"
 
@@ -1005,20 +1047,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Wybierz wszystkie %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Dodaj nowy"
@@ -1077,16 +1117,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Typ"
 
@@ -1134,15 +1173,14 @@
 msgstr "Wyszukaj"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Wybierz plik"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/pt/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/pt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Portuguese (http://app.transifex.com/divio/django-filer/language/pt/)\n"
+"Language-Team: Portuguese (http://app.transifex.com/divio/django-filer/"
+"language/pt/)\n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
+"1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -242,27 +241,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -284,15 +283,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -314,15 +313,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -337,152 +336,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -519,27 +532,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -576,24 +586,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -638,38 +648,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -695,15 +705,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -736,31 +746,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -779,71 +789,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -930,21 +940,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -998,20 +1006,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1069,16 +1075,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1126,15 +1131,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Claudio Rogerio Carvalho Filho <excriptbrasil@gmail.com>, 2017
 # Julio Lucchese <juliorieger@gmail.com>, 2018
 # Rodrigo <rprior@infranology.com.br>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Julio Lucchese <juliorieger@gmail.com>, 2018\n"
-"Language-Team: Portuguese (Brazil) (http://app.transifex.com/divio/django-filer/language/pt_BR/)\n"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/divio/django-"
+"filer/language/pt_BR/)\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt_BR\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
+"1000000 == 0 ? 1 : 2;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Avançado"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "URL canônico"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "itens precisam ser selecionar para que a ação seja executada. Nenhuma alteração foi efetuada."
+msgstr ""
+"itens precisam ser selecionar para que a ação seja executada. Nenhuma "
+"alteração foi efetuada."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s selecionado"
 msgstr[1] "Todos %(total_count)s selecionados"
@@ -127,15 +128,17 @@
 msgstr "Pastas com os nomes %s s já existem no local selecionado"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d arquivo(s) e/ou pasta(s) foram movidos para a pasta '%(destination)s' com sucesso."
+msgstr ""
+"%(count)d arquivo(s) e/ou pasta(s) foram movidos para a pasta "
+"'%(destination)s' com sucesso."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Mover arquivo(s) e/ou pasta(s)"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -152,15 +155,17 @@
 msgstr "Renomear arquivos"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d arquivo(s) e/ou pasta(s) foram copiados para o pasta '%(destination)s' com sucesso."
+msgstr ""
+"%(count)d arquivo(s) e/ou pasta(s) foram copiados para o pasta "
+"'%(destination)s' com sucesso."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Copiar arquivo(s) e/ou pasta(s)"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -184,20 +189,24 @@
 msgstr "Sufixo que será anexado aos nomes dos arquivos copiados"
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "O sufixo precisa ser válido, simples e com letras minúsculas para o nome de um arquivo, como por exemplo: \"%(valid)s\"."
+msgstr ""
+"O sufixo precisa ser válido, simples e com letras minúsculas para o nome de "
+"um arquivo, como por exemplo: \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
-msgstr "A chave de valor \"%(key)s\" utilizada para renomear o arquivo é desconhecida."
+msgstr ""
+"A chave de valor \"%(key)s\" utilizada para renomear o arquivo é "
+"desconhecida."
 
 #: admin/forms.py:54
 #, python-format
 msgid "Invalid rename format: %(error)s."
 msgstr "Formato inválido para renomear: %(error)s."
 
 #: admin/forms.py:64 models/thumbnailoptionmodels.py:37
@@ -218,15 +227,16 @@
 
 #: admin/forms.py:70 models/thumbnailoptionmodels.py:30
 msgid "upscale"
 msgstr "aumentar"
 
 #: admin/forms.py:75
 msgid "Thumbnail option or resize parameters must be choosen."
-msgstr "Escolher entre as opções de miniaturas ou parâmetros de redimensionamento."
+msgstr ""
+"Escolher entre as opções de miniaturas ou parâmetros de redimensionamento."
 
 #: admin/forms.py:77
 msgid "Resize parameters must be choosen."
 msgstr "Os parâmetros de redimensionamento precisam ser escolhidos"
 
 #: admin/imageadmin.py:18 admin/imageadmin.py:105
 msgid "Subject location"
@@ -245,27 +255,27 @@
 msgstr "A localização do assunto está fora da imagem."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Sua entrada: \"{subject_location}\". "
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Já existe uma pasta com esse nome."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -287,15 +297,15 @@
 msgid "image"
 msgstr "imagem"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "imagens"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "usuário"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "arquivos"
 
@@ -317,15 +327,15 @@
 msgstr "item da área de transferência"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "itens da área de transferência"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "pasta"
 
 #: models/filemodels.py:81
@@ -340,152 +350,168 @@
 msgid "has all mandatory data"
 msgstr "possui todos os dados necessários"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "nome original do arquivo"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "nome"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "descrição"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "Proprietário"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "enviado em"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "modificado em"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Permissões desabilitadas"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Desative qualquer verificação de permissão para este arquivo. O arquivo estará acessível ao público para que qualquer possa acessar."
+msgstr ""
+"Desative qualquer verificação de permissão para este arquivo. O arquivo "
+"estará acessível ao público para que qualquer possa acessar."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "criado em"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Pasta"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Pastas"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "todos os itens"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "este item somente"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "este item e todos subjacentes"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "permitir"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "negar"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tipo"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "grupo"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "todos"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "pode ler"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "pode editar"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "pode adicionar filhos"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "permissão de pasta"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "permissões de pasta"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "data de tomada"
 
@@ -522,27 +548,24 @@
 msgid "Unsorted Uploads"
 msgstr "Uploads não classificados"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "arquivos com falta de metadados"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "raiz"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Executar a ação selecionada"
 
@@ -579,50 +602,58 @@
 msgstr "Início"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Voltar para Filer app"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Volte à pasta raiz"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Volte para a pasta '%(folder_name)s'"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Duplicados"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Remover os arquivo(s) e/ou pasta(s) selecionados resultará na remoção de objetos relacionados, mas sua conta não tem permissão para remover os seguintes tipos de objetos:"
+msgstr ""
+"Remover os arquivo(s) e/ou pasta(s) selecionados resultará na remoção de "
+"objetos relacionados, mas sua conta não tem permissão para remover os "
+"seguintes tipos de objetos:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Remover os arquivo(s) e/ou pasta(s) selecionados, requer remover os seguites objetos protegidos relacionados:"
+msgstr ""
+"Remover os arquivo(s) e/ou pasta(s) selecionados, requer remover os seguites "
+"objetos protegidos relacionados:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Você tem certeza que deseja remover os arquivo(s) e/ou pasta(s) selecionados? Todos os seguintes objetos e itens relacionados serão removidos: "
+msgstr ""
+"Você tem certeza que deseja remover os arquivo(s) e/ou pasta(s) "
+"selecionados? Todos os seguintes objetos e itens relacionados serão "
+"removidos: "
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Não, me leve de volta"
 
@@ -641,39 +672,41 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Ver no site"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Voltar para"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "página inicial de administração"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Ícone da Pasta"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Sua conta não possui permissão para copiar todos os arquivo(s) e/ou pasta(s) selecionados."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Sua conta não possui permissão para copiar todos os arquivo(s) e/ou pasta(s) "
+"selecionados."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -689,164 +722,180 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Não existem arquivo(s) e/ou pasta(s) disponíveis para copiar."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Os arquivo(s) e/ou pasta(s) serão copiados para a pasta de destino (mantendo a estrutura de diretórios):"
+msgstr ""
+"Os arquivo(s) e/ou pasta(s) serão copiados para a pasta de destino (mantendo "
+"a estrutura de diretórios):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Pasta de destino:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Copiar"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Não é permitido copiar arquivos para a mesma pasta"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Sua conta não possui permissão para redimensionar todas as imagens selecionadas."
+msgstr ""
+"Sua conta não possui permissão para redimensionar todas as imagens "
+"selecionadas."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Não existem imagens disponíveis para redimensionar."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "As seguintes imagens serão redimensionadas:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Selecionar uma opção de miniatura ou digitar os parâmetros de redimensionamento:"
+msgstr ""
+"Selecionar uma opção de miniatura ou digitar os parâmetros de "
+"redimensionamento:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Selecionar os parâmetros de redimensionamento:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Cuidado: as imagens serão redimensionadas no mesmo local e os originais serão perdidos. Uma sugestão seria fazer uma cópia para guardar os originais."
+msgstr ""
+"Cuidado: as imagens serão redimensionadas no mesmo local e os originais "
+"serão perdidos. Uma sugestão seria fazer uma cópia para guardar os originais."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Redimensionar"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Sua conta não possui permissão para mover todos os arquivo(s) e/ou pasta(s) selecionados."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Sua conta não possui permissão para mover todos os arquivo(s) e/ou pasta(s) "
+"selecionados."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Não existem arquivo(s) e/ou pasta(s) disponíveis para mover."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Os arquivo(s) e/ou pasta(s) serão movidos para a pasta de destino (mantendo a estrutura de diretórios):"
+msgstr ""
+"Os arquivo(s) e/ou pasta(s) serão movidos para a pasta de destino (mantendo "
+"a estrutura de diretórios):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Mover"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Não é permitido mover arquivos na mesma pasta"
 
 #: templates/admin/filer/folder/choose_rename_format.html:15
 msgid ""
 "Your account doesn't have permissions to rename all of the selected files."
-msgstr "Sua conta não possui permissão para renomear todos os arquivos selecionados."
+msgstr ""
+"Sua conta não possui permissão para renomear todos os arquivos selecionados."
 
 #: templates/admin/filer/folder/choose_rename_format.html:18
 msgid "There are no files available to rename."
 msgstr "Não existem arquivos disponíveis para renomear."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Os seguintes arquivos serão renomeados (estes arquivos serão mantidos em suas pastas e os nomes originais serão mantidos, apenas o nome de apresentação será alterado):"
+msgstr ""
+"Os seguintes arquivos serão renomeados (estes arquivos serão mantidos em "
+"suas pastas e os nomes originais serão mantidos, apenas o nome de "
+"apresentação será alterado):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Renomear"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Volte para a pasta pai"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Alterar os detalhes da pasta atual"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Alterar"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Clique aqui para pesquisar pela frase inserida"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Pesquisar"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Fechar"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Limite"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Marque para limitar a pesquisa na pasta atual"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Limitar a pesquisa na pasta atual"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Remover"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Adiciona uma nova pasta"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Nova Pasta"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Enviar arquivos"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Você precisa selecionar a pasta primeiro"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Nome"
 
@@ -933,21 +982,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "habilitado"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "URL Canônico '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Baixar '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Remover arquivo"
 
@@ -1001,20 +1048,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Selecione todos %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Adicionar novo"
@@ -1072,16 +1117,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tipo"
 
@@ -1129,15 +1173,14 @@
 msgstr "Pesquisar"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Alterar Arquivo"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Alexander Naydenko <an@zeppelinen.com>, 2020
 # Oleg Fish <okfish@yandex.ru>, 2017
 # Pavel <neoascetic@gmail.com>, 2012
 # Pavel <neoascetic@gmail.com>, 2012
 # Vladimir Puzakov <vppuzakov@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Alexander Naydenko <an@zeppelinen.com>, 2020\n"
-"Language-Team: Russian (http://app.transifex.com/divio/django-filer/language/ru/)\n"
+"Language-Team: Russian (http://app.transifex.com/divio/django-filer/language/"
+"ru/)\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ru\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Дополнительно"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "канонический URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Для выполнения действий нужно выбрать хотя бы один объект. Не произведено никаких изменений."
+msgstr ""
+"Для выполнения действий нужно выбрать хотя бы один объект. Не произведено "
+"никаких изменений."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "%(total_count)s выбран"
 msgstr[1] "%(total_count)s выбрано"
@@ -187,15 +189,17 @@
 msgstr "Окончание, которое будет добавлено к именам скопированных файлов."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Окончание должно быть правильной, простой и в нижнем регистре частью имени файла, например \"%(valid)s\"."
+msgstr ""
+"Окончание должно быть правильной, простой и в нижнем регистре частью имени "
+"файла, например \"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Неизвестный ключ форматирования \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -248,27 +252,27 @@
 msgstr "Расположение объекта указано за пределами изображения."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Вы ввели: \"{subject_location}\". "
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Папка с таким именем уже существует"
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -290,15 +294,15 @@
 msgid "image"
 msgstr "изображение"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "изображения"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "пользователь"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "файлы"
 
@@ -320,15 +324,15 @@
 msgstr "элемент буфера обмена"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "элементы буфера обмена"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "папка"
 
 #: models/filemodels.py:81
@@ -343,152 +347,168 @@
 msgid "has all mandatory data"
 msgstr "это обязательные данные"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "оригинальное имя файла"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "имя"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "описание"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "владелец"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "загружено"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "изменено"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Разрешения отключены"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Отменить все проверки разрешений для этого файла. Файл будет доступен публично для каждого."
+msgstr ""
+"Отменить все проверки разрешений для этого файла. Файл будет доступен "
+"публично для каждого."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "создан"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Папка"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Папки"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "все элементы"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "только этот элемент"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "этот элемент и потомки"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "разрешить"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "запретить"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "тип"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "группа"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "все"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "могут читать"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "могут редактировать"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "могут добавлять потомков"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "разрешение папки"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "разрешения папки"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "дата создания"
 
@@ -525,27 +545,24 @@
 msgid "Unsorted Uploads"
 msgstr "Несортированные загрузки"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "файлы с отсутсвующими метаданными"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "корень"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Выполнить выбранное действие"
 
@@ -582,50 +599,56 @@
 msgstr "Домой"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Вернуться на главную Filer'а"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Вернуться в корневую папку"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Вернуться в папку \"%(folder_name)s\""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Дубликаты"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Удаление выбранных файлов/папок приведет к удалению связанных объектов, но у вас нет прав удалять следующие объекты:"
+msgstr ""
+"Удаление выбранных файлов/папок приведет к удалению связанных объектов, но у "
+"вас нет прав удалять следующие объекты:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Удаление выбранных файлов/папок потребует удаления следующих защищенных связанных объектов:"
+msgstr ""
+"Удаление выбранных файлов/папок потребует удаления следующих защищенных "
+"связанных объектов:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Вы уверены, что хотите удалить выбранные файлы/папки? Следующие объекты вместе со связанными объектами будут удалены:"
+msgstr ""
+"Вы уверены, что хотите удалить выбранные файлы/папки? Следующие объекты "
+"вместе со связанными объектами будут удалены:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Нет, пустите меня обратно"
 
@@ -644,38 +667,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Посмотреть на сайте"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Вернуться к"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "главная страница администрирования"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Иконка папки"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr "У вас нет прав на копирование выбранных файлов/папок"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -692,24 +715,26 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Нет файлов для копирования."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Эти файлы/папки будут скопированы в целевую папку (с сохранением иерархичности):"
+msgstr ""
+"Эти файлы/папки будут скопированы в целевую папку (с сохранением "
+"иерархичности):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Целевая папка:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Копировать"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Копирование файлов в ту же самую папку запрещено"
 
@@ -734,39 +759,43 @@
 msgid "Choose resize parameters:"
 msgstr "Выбрите параметры изменения размеров:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Внимание: изображения будут изменены в размерах с заменой оригиналов. Возможно, лучше будет сперва сделать копии."
+msgstr ""
+"Внимание: изображения будут изменены в размерах с заменой оригиналов. "
+"Возможно, лучше будет сперва сделать копии."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Изменить размеры"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr "Вы не имеете прав для перемещения выбранных файлов/папок."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Нет файлов/папок для перемещения."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Следующие файлы/папки будут перемещены в целевую папку (сохраняя иерархичность):"
+msgstr ""
+"Следующие файлы/папки будут перемещены в целевую папку (сохраняя "
+"иерархичность):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Переместить"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Перемещение файлов в ту же самую папку запрещено"
 
@@ -779,77 +808,79 @@
 msgid "There are no files available to rename."
 msgstr "Нет файлов для переименовывания."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Эти файлы будут переименованы (они остануться в их папках и сохранят имена оригинальных файлов, только отображаемое имя измениться):"
+msgstr ""
+"Эти файлы будут переименованы (они остануться в их папках и сохранят имена "
+"оригинальных файлов, только отображаемое имя измениться):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Переименовать"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Возвратиться к родительской папке"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Изменить текущую папку"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Изменить"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Нажмите здесь для поиска по введенной фразе"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Поиск"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Закрыть"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Ограничить"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Отметьте, чтобы ограничить поиск текущей папкой"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Ограничить поиск текущей папкой"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Удалить"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Добавляет новую папку"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Новая папка"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Загрузить файлы"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Сначала надо выбрать папку"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Имя"
 
@@ -938,21 +969,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "включены"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Канонический URL '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Скачать '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Удалить файл"
 
@@ -1006,20 +1035,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Выбрать все %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Добавить новую"
@@ -1078,16 +1105,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Тип"
 
@@ -1135,15 +1161,14 @@
 msgstr "Выбрать"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Выбрать файл"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,60 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Slovak (http://app.transifex.com/divio/django-filer/language/sk/)\n"
+"Language-Team: Chinese (Taiwan) (http://app.transifex.com/divio/django-filer/"
+"language/zh_TW/)\n"
+"Language: zh_TW\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
 msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -243,27 +238,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -285,15 +280,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -315,15 +310,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -338,152 +333,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -520,27 +529,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -577,24 +583,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -639,38 +645,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -696,15 +702,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -737,31 +743,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -780,71 +786,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -876,27 +882,21 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -933,21 +933,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -1001,20 +999,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1023,17 +1019,14 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1073,16 +1066,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1130,15 +1122,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1196,13 +1187,10 @@
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
-#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
-#~ msgstr[2] "15c0f2d28d6dab1af1f6d94906beb627_pl_2"
-#~ msgstr[3] "15c0f2d28d6dab1af1f6d94906beb627_pl_3"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/tr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Cihad GÜNDOĞDU <cihadgundogdu@gmail.com>, 2013,2015-2016
 # Cihad GÜNDOĞDU <cihadgundogdu@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Cihad GÜNDOĞDU <cihadgundogdu@gmail.com>, 2013,2015-2016\n"
-"Language-Team: Turkish (http://app.transifex.com/divio/django-filer/language/tr/)\n"
+"Language-Team: Turkish (http://app.transifex.com/divio/django-filer/language/"
+"tr/)\n"
+"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Gelişmiş"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "standart URL"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -125,15 +123,16 @@
 msgstr "%s isimli klasörler seçili hedefte var."
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d adet dosya/klasör başarıyla '%(destination)s' klasörüne taşındı"
+msgstr ""
+"%(count)d adet dosya/klasör başarıyla '%(destination)s' klasörüne taşındı"
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Dosya veya klasörleri taşı"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -150,15 +149,16 @@
 msgstr "Dosyaları yeniden adlandır"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "%(count)d adet dosya veya klasör '%(destination)s' klasörüne kopyalandı"
+msgstr ""
+"%(count)d adet dosya veya klasör '%(destination)s' klasörüne kopyalandı"
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Dosya veya klasörleri kopyala"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -243,27 +243,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Bu isimde dizin zaten var"
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -285,15 +285,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "kullanıcı"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "dosyalar"
 
@@ -315,15 +315,15 @@
 msgstr "arabellek nesnesi"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "klasör"
 
 #: models/filemodels.py:81
@@ -338,152 +338,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "orjinal dosya adı"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "isim"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "açıklama"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "sahib"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "yüklendi"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "düzenlendi"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Yetkiler pasifleştirildi"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "tüm elemanlar"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "sadece bu eleman"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "bu eleman ve alt elemanlar"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "izin ver"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "engelle"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "tip"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "grup"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "herkes"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "okuyabilir"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "düzenleyebilir"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "alt eleman ekleyebilir"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "dizin yetki"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "dizin yetkileri"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -520,27 +534,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "kök"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Seçili aksiyonu çalışıtır"
 
@@ -577,24 +588,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -639,38 +650,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -696,15 +707,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -737,31 +748,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -780,71 +791,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Yeniden adlandır"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Ara"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Geçerli klasörün aramalarını sınırla"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Sil"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Yeni Klasör Ekle"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Yeni Klasör"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Dosyaları Yükle"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Önce bir klasör seçmelisin"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "İsim"
 
@@ -929,21 +940,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "aktif"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Dosyayı kaldır"
 
@@ -997,20 +1006,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "%(total_count)s Tümünü seç"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Yeni ekle"
@@ -1067,16 +1074,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Tip"
 
@@ -1124,15 +1130,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Dosya Seç"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/vi_VN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 # Duong Vu Hong <duong.vuhong.uet@gmail.com>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Duong Vu Hong <duong.vuhong.uet@gmail.com>, 2021\n"
-"Language-Team: Vietnamese (Viet Nam) (http://app.transifex.com/divio/django-filer/language/vi_VN/)\n"
+"Language-Team: Vietnamese (Viet Nam) (http://app.transifex.com/divio/django-"
+"filer/language/vi_VN/)\n"
+"Language: vi_VN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: vi_VN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr "Nâng Cao"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr "URL hợp chuẩn"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
-msgstr "Những item được chọn để thực hiện hành động trên đó. Không có item nào bị thay đổi."
+msgstr ""
+"Những item được chọn để thực hiện hành động trên đó. Không có item nào bị "
+"thay đổi."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] "Tất cả %(total_count)s được chọn"
 
@@ -123,15 +123,16 @@
 msgstr "Các thư mục với tên %s đã tồn tại ở vị trí đã chọn"
 
 #: admin/folderadmin.py:922
 #, python-format
 msgid ""
 "Successfully moved %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Đã di chuyển %(count)d tệp và/hoặc thư mục tới thư mục '%(destination)s'."
+msgstr ""
+"Đã di chuyển %(count)d tệp và/hoặc thư mục tới thư mục '%(destination)s'."
 
 #: admin/folderadmin.py:930 admin/folderadmin.py:932
 msgid "Move files and/or folders"
 msgstr "Di chuyển tệp và/hoặc thư mục"
 
 #: admin/folderadmin.py:947
 msgid "Move selected files and/or folders"
@@ -148,15 +149,17 @@
 msgstr "Đổi tên tệp"
 
 #: admin/folderadmin.py:1125
 #, python-format
 msgid ""
 "Successfully copied %(count)d files and/or folders to folder "
 "'%(destination)s'."
-msgstr "Đã thành công sao chép %(count)d tệp và/hoặc thư mục tới thư mục '%(destination)s'."
+msgstr ""
+"Đã thành công sao chép %(count)d tệp và/hoặc thư mục tới thư mục "
+"'%(destination)s'."
 
 #: admin/folderadmin.py:1143 admin/folderadmin.py:1145
 msgid "Copy files and/or folders"
 msgstr "Sao chép tệp và/hoặc thư mục"
 
 #: admin/folderadmin.py:1162
 msgid "Copy selected files and/or folders"
@@ -180,15 +183,17 @@
 msgstr "Hậu tố sẽ được nối vào tên của tệp đã sao chép."
 
 #: admin/forms.py:31
 #, python-format
 msgid ""
 "Suffix should be a valid, simple and lowercase filename part, like "
 "\"%(valid)s\"."
-msgstr "Hậu tố phải là một phần tên tệp hợp lệ, đơn giản và chữ thường, như \"%(valid)s\"."
+msgstr ""
+"Hậu tố phải là một phần tên tệp hợp lệ, đơn giản và chữ thường, như "
+"\"%(valid)s\"."
 
 #: admin/forms.py:52
 #, python-format
 msgid "Unknown rename format value key \"%(key)s\"."
 msgstr "Không biết định dạng đổi tên của khóa giá trị \"%(key)s\"."
 
 #: admin/forms.py:54
@@ -241,27 +246,27 @@
 msgstr "Vị trí chủ đề ở bên ngoài hình ảnh."
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr "Đầu vào của bạn: \"{subject_location}\"."
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr "Thư mục với tên này đã tồn tại."
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr "Filer"
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -283,15 +288,15 @@
 msgid "image"
 msgstr "hình ảnh"
 
 #: models/abstract.py:79
 msgid "images"
 msgstr "những hình ảnh"
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr "người dùng"
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr "những tệp"
 
@@ -313,15 +318,15 @@
 msgstr "item bảng tạm"
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr "items bảng tạm"
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr "thư mục"
 
 #: models/filemodels.py:81
@@ -336,152 +341,168 @@
 msgid "has all mandatory data"
 msgstr "có tất cả dữ liệu ủy thác"
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr "tên tệp gốc"
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr "tên"
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr "mô tả"
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr "người sở hữu"
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr "đã tải lên tại"
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr "đã chỉnh sửa tại"
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr "Quyền bị vô hiệu hóa"
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
-msgstr "Vô hiệu hóa bất kỳ quyền kiểm tra cho tệp này. Tệp sẽ truy cập được bởi bất kỳ ai."
+msgstr ""
+"Vô hiệu hóa bất kỳ quyền kiểm tra cho tệp này. Tệp sẽ truy cập được bởi bất "
+"kỳ ai."
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr "đã tạo tại"
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr "Thư mục"
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr "Những thư mục"
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr "tất cả đồ"
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr "chỉ đồ này"
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr "đồ này và tất cả các con"
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr "cho phép"
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr "không cho phép"
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr "kiểu"
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr "nhóm"
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr "tất cả mọi người"
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr "có thể đọc"
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr "có thể tùy chỉnh"
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr "có thể thêm con"
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr "quyền thư mục"
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr "những quyền thư mục"
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr "ngày nắm giữ"
 
@@ -518,27 +539,24 @@
 msgid "Unsorted Uploads"
 msgstr "Những tải lên chưa sắp xếp"
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr "những tệp với metadata bị mất"
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr "gốc"
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr "Chạy hành dộng đã chọn"
 
@@ -575,50 +593,56 @@
 msgstr "Trang chủ"
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr "Trở lại ứng dụng Filer"
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr "Trở lại thư mục gốc"
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr "Trở lại '%(folder_name)s' thư mục"
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr "Lặp"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:11
 msgid ""
 "Deleting the selected files and/or folders would result in deleting related "
 "objects, but your account doesn't have permission to delete the following "
 "types of objects:"
-msgstr "Xóa tệp và/hoặc thưc mục đã chọn sẽ dẫn đến xóa đối tượng liên quan, nhưng tài khoản của bạn không có quyền xóa những loại của các đối tượng:"
+msgstr ""
+"Xóa tệp và/hoặc thưc mục đã chọn sẽ dẫn đến xóa đối tượng liên quan, nhưng "
+"tài khoản của bạn không có quyền xóa những loại của các đối tượng:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:19
 msgid ""
 "Deleting the selected files and/or folders would require deleting the "
 "following protected related objects:"
-msgstr "Xóa tệp và/hoặc thư mục đã chọn sẽ yêu cầu xóa những đối tượng liên quan được bảo vệ sau:"
+msgstr ""
+"Xóa tệp và/hoặc thư mục đã chọn sẽ yêu cầu xóa những đối tượng liên quan "
+"được bảo vệ sau:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:27
 msgid ""
 "Are you sure you want to delete the selected files and/or folders? All of "
 "the following objects and their related items will be deleted:"
-msgstr "Bạn có chắc muốn xóa tệp và/hoặc thư mục đã chọn? Tất cả những đối tượng và những thứ liên quan đến chúng sẽ bị xóa:"
+msgstr ""
+"Bạn có chắc muốn xóa tệp và/hoặc thư mục đã chọn? Tất cả những đối tượng và "
+"những thứ liên quan đến chúng sẽ bị xóa:"
 
 #: templates/admin/filer/delete_selected_files_confirmation.html:46
 #: templates/admin/filer/folder/choose_copy_destination.html:64
 #: templates/admin/filer/folder/choose_move_destination.html:72
 msgid "No, take me back"
 msgstr "Không, đưa tôi quay lại"
 
@@ -637,39 +661,40 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr "Xem trong trang"
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr "Quay lại"
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr "trang chủ người quản trị"
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr "Biểu tượng thư mục"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
-msgstr "Tài khoản của bạn không có quyền để sao chép tất cả tệp và thư mục được chọn."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
+msgstr ""
+"Tài khoản của bạn không có quyền để sao chép tất cả tệp và thư mục được chọn."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
 #: templates/admin/filer/folder/choose_move_destination.html:49
@@ -685,81 +710,93 @@
 msgid "There are no files and/or folders available to copy."
 msgstr "Không có tệp và/hoặc thư mục để sao chép."
 
 #: templates/admin/filer/folder/choose_copy_destination.html:40
 msgid ""
 "The following files and/or folders will be copied to a destination folder "
 "(retaining their tree structure):"
-msgstr "Những tệp và thư mục sau sẽ được sao chép tới một thư mục đích (giữ cấu trúc cây thư mục):"
+msgstr ""
+"Những tệp và thư mục sau sẽ được sao chép tới một thư mục đích (giữ cấu trúc "
+"cây thư mục):"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr "Thư mục đích:"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr "Sao chép"
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr "Không cho phép sao chép tệp tới cùng thư mục"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:15
 msgid ""
 "Your account doesn't have permissions to resize all of the selected images."
-msgstr "Tài khoản của bạn không có quyền để thay đổi kích thước của tất cả hình ảnh đã chọn."
+msgstr ""
+"Tài khoản của bạn không có quyền để thay đổi kích thước của tất cả hình ảnh "
+"đã chọn."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:18
 msgid "There are no images available to resize."
 msgstr "Không có hình ảnh để thay dổi kích thước"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:20
 msgid "The following images will be resized:"
 msgstr "Hình ảnh dưới đay sẽ bị thay đổi kích thước:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:33
 msgid "Choose an existing thumbnail option or enter resize parameters:"
-msgstr "Chọn một tùy chọn của thumbnail đang tồn tại hoặc nhập tham số thay đổi kích thước:"
+msgstr ""
+"Chọn một tùy chọn của thumbnail đang tồn tại hoặc nhập tham số thay đổi kích "
+"thước:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:35
 msgid "Choose resize parameters:"
 msgstr "Chọn tham số thay dổi kích thước:"
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:38
 msgid ""
 "Warning: Images will be resized in-place and originals will be lost. Maybe "
 "first make a copy of them to retain the originals."
-msgstr "Cảnh bảo: Hình ảnh sẽ bị thay đổi tại chỗ và ảnh gốc sẽ bị mất. Có thể tạo một sao chép của chúng để giữ lại hình ảnh gốc."
+msgstr ""
+"Cảnh bảo: Hình ảnh sẽ bị thay đổi tại chỗ và ảnh gốc sẽ bị mất. Có thể tạo "
+"một sao chép của chúng để giữ lại hình ảnh gốc."
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr "Thay đổi kích thước"
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
-msgstr "Tài khoản của bạn không có quyền để di chuyển tất cả các tệp và thư mục đã chọn."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
+msgstr ""
+"Tài khoản của bạn không có quyền để di chuyển tất cả các tệp và thư mục đã "
+"chọn."
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr "Không có tệp và/hoặc thư mục để di chuyển."
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
-msgstr "Tệp và thư mục dưới đây sẽ được chuyển tới thư mục đích (giữ nguyên cấu trúc cây thư mục):"
+msgstr ""
+"Tệp và thư mục dưới đây sẽ được chuyển tới thư mục đích (giữ nguyên cấu trúc "
+"cây thư mục):"
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr "Di chuyển"
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr "Không cho phép di chuyển tệp vào cùng thư mục"
 
@@ -772,77 +809,79 @@
 msgid "There are no files available to rename."
 msgstr "Không có tệp để đổi tên."
 
 #: templates/admin/filer/folder/choose_rename_format.html:20
 msgid ""
 "The following files will be renamed (they will stay in their folders and "
 "keep original filename, only displayed filename will be changed):"
-msgstr "Tệp dưới đây sẽ bị đổi tên (chúng vẫn ở trong thư mục của chúng và giữ tên gốc, chỉ tên hiển thị sẽ bị thay đổi):"
+msgstr ""
+"Tệp dưới đây sẽ bị đổi tên (chúng vẫn ở trong thư mục của chúng và giữ tên "
+"gốc, chỉ tên hiển thị sẽ bị thay đổi):"
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr "Đổi tên"
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr "Trở lại thư mục cha"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr "Thay đổi thông tin chi tiết thư mục hiện tại"
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr "Thay đổi"
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr "Bấm vào đây để chạy tìm kiếm cho đoạn văn đã nhập"
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr "Tìm kiếm"
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr "Đóng"
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr "Giới hạn"
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr "Chọn để giới hạn tìm kiếm cho thư mục hiện tại"
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr "Giới hạn tìm kiếm cho thư mục hiện tại"
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr "Xóa"
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr "Thêm một thư mục mới"
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr "Thư mục mới"
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr "Tải tệp lên"
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr "Bạn đầu tiên phải chọn một thư mục"
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr "Tên"
 
@@ -925,21 +964,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr "đã kích hoạt"
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr "Url hợp chuẩn '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr "Tải '%(item_label)s'"
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr "Xóa tệp"
 
@@ -993,20 +1030,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr "Chọn tất cả %(total_count)s"
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr "Thêm mới"
@@ -1062,16 +1097,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr "Kiểu"
 
@@ -1119,15 +1153,14 @@
 msgstr "Tìm kiếm"
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr "Chọn tệp"
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/zh/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Chinese (http://app.transifex.com/divio/django-filer/language/zh/)\n"
+"Language-Team: Chinese (China) (http://app.transifex.com/divio/django-filer/"
+"language/zh_CN/)\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
@@ -240,27 +238,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -282,15 +280,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -312,15 +310,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -335,152 +333,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -517,27 +529,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -574,24 +583,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -636,38 +645,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -693,15 +702,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -734,31 +743,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -777,71 +786,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -924,21 +933,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -992,20 +999,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1061,16 +1066,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1118,15 +1122,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
```

### Comparing `django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/django.mo` & `django-filer-3.0.4/filer/locale/zh-Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/zh-Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/locale/zh_CN/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/bg/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
 "Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Chinese (China) (http://app.transifex.com/divio/django-filer/language/zh_CN/)\n"
+"Language-Team: Bulgarian (http://app.transifex.com/divio/django-filer/"
+"language/bg/)\n"
+"Language: bg\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_CN\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
 msgstr ""
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
 msgstr ""
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
 msgstr ""
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
+msgstr[1] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
@@ -240,27 +239,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -282,15 +281,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -312,15 +311,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -335,152 +334,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -517,27 +530,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -574,24 +584,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -636,38 +646,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -693,15 +703,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -734,31 +744,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -777,71 +787,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -873,21 +883,23 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -924,21 +936,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -992,20 +1002,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1014,14 +1022,15 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1061,16 +1070,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1118,15 +1126,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1184,10 +1191,11 @@
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
+#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

### Comparing `django-filer-3.0.3/filer/locale/zh_TW/LC_MESSAGES/django.po` & `django-filer-3.0.4/filer/locale/fa/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Translators:
 # Translators:
+# Fariman Ghaedi <farimanghaedi@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django Filer\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 19:25+0200\n"
+"POT-Creation-Date: 2023-07-31 22:21+0200\n"
 "PO-Revision-Date: 2012-07-13 15:50+0000\n"
-"Last-Translator: Angelo Dini <finalangeljp@hotmail.com>\n"
-"Language-Team: Chinese (Taiwan) (http://app.transifex.com/divio/django-filer/language/zh_TW/)\n"
+"Last-Translator: Fariman Ghaedi <farimanghaedi@gmail.com>, 2019\n"
+"Language-Team: Persian (http://app.transifex.com/divio/django-filer/language/"
+"fa/)\n"
+"Language: fa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: admin/clipboardadmin.py:16
-#| msgid ""
-#| "ccount doesn't have permissions to rename all of the selected files."
 msgid "You do not have permission to upload files."
 msgstr ""
 
 #: admin/clipboardadmin.py:17
 msgid "Can't find folder to upload. Please refresh and try again"
 msgstr ""
 
 #: admin/clipboardadmin.py:19
-msgid ""
-"Can't use this folder, Permission Denied. Please select another folder."
+msgid "Can't use this folder, Permission Denied. Please select another folder."
 msgstr ""
 
-#: admin/fileadmin.py:45
+#: admin/fileadmin.py:47
 msgid "Advanced"
-msgstr ""
+msgstr "پیشرفته"
 
-#: admin/fileadmin.py:160
+#: admin/fileadmin.py:162
 msgid "canonical URL"
-msgstr ""
+msgstr "آدرس کانونی"
 
 #: admin/folderadmin.py:399 admin/folderadmin.py:570
 msgid ""
 "Items must be selected in order to perform actions on them. No items have "
 "been changed."
 msgstr ""
+"برای اینکه بتوانید روی آیتم ها اقداماتی انجام دهید ابتدا باید آیتم ها را "
+"انتخاب کنید. هیچ آیتمی تغییر نکرد."
 
 #: admin/folderadmin.py:422
 #, python-format
 msgid "%(total_count)s selected"
 msgid_plural "All %(total_count)s selected"
 msgstr[0] ""
+msgstr[1] ""
 
 #: admin/folderadmin.py:448
 #, python-format
 msgid "Directory listing for %(folder_name)s"
 msgstr ""
 
 #: admin/folderadmin.py:463
 #, python-format
 msgid "0 of %(cnt)s selected"
 msgstr ""
 
 #: admin/folderadmin.py:600
 msgid "No action selected."
-msgstr ""
+msgstr "هیچ اقدامی انتخاب نشده است."
 
 #: admin/folderadmin.py:652
 #, python-format
 msgid "Successfully moved %(count)d files to clipboard."
 msgstr ""
 
 #: admin/folderadmin.py:657
 msgid "Move selected files to clipboard"
-msgstr ""
+msgstr "انتقال فایل های انتخاب شده به کلیپ برد"
 
 #: admin/folderadmin.py:697
 #, python-format
 msgid "Successfully disabled permissions for %(count)d files."
 msgstr ""
 
 #: admin/folderadmin.py:699
@@ -102,23 +104,23 @@
 
 #: admin/folderadmin.py:782
 msgid "Cannot delete files and/or folders"
 msgstr ""
 
 #: admin/folderadmin.py:784
 msgid "Are you sure?"
-msgstr ""
+msgstr "آیا مطمئن هستید؟"
 
 #: admin/folderadmin.py:790
 msgid "Delete files and/or folders"
-msgstr ""
+msgstr "پاک کردن فایل ها و/یا پوشه ها"
 
 #: admin/folderadmin.py:811
 msgid "Delete selected files and/or folders"
-msgstr ""
+msgstr "پاک کردن فایل ها و/یا پوشه های انتخاب شده"
 
 #: admin/folderadmin.py:918
 #, python-format
 msgid "Folders with names %s already exist at the selected destination"
 msgstr ""
 
 #: admin/folderadmin.py:922
@@ -240,27 +242,27 @@
 msgstr ""
 
 #: admin/imageadmin.py:74
 #, python-brace-format
 msgid "Your input: \"{subject_location}\". "
 msgstr ""
 
-#: admin/permissionadmin.py:10 models/foldermodels.py:379
+#: admin/permissionadmin.py:10 models/foldermodels.py:380
 msgid "Who"
 msgstr ""
 
-#: admin/permissionadmin.py:11 models/foldermodels.py:400
+#: admin/permissionadmin.py:11 models/foldermodels.py:401
 msgid "What"
 msgstr ""
 
 #: admin/views.py:55
 msgid "Folder with this name already exists."
 msgstr ""
 
-#: apps.py:9 templates/admin/filer/breadcrumbs.html:5
+#: apps.py:11 templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/directory_listing.html:33
 msgid "Filer"
 msgstr ""
 
 #: contrib/django_cms/cms_toolbars.py:44
 msgid "Media library"
@@ -282,15 +284,15 @@
 msgid "image"
 msgstr ""
 
 #: models/abstract.py:79
 msgid "images"
 msgstr ""
 
-#: models/clipboardmodels.py:11 models/foldermodels.py:288
+#: models/clipboardmodels.py:11 models/foldermodels.py:289
 msgid "user"
 msgstr ""
 
 #: models/clipboardmodels.py:17 models/filemodels.py:157
 msgid "files"
 msgstr ""
 
@@ -312,15 +314,15 @@
 msgstr ""
 
 #: models/clipboardmodels.py:57
 msgid "clipboard items"
 msgstr ""
 
 #: models/filemodels.py:66 templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 #: templates/admin/filer/tools/clipboard/clipboard.html:27
 msgid "folder"
 msgstr ""
 
 #: models/filemodels.py:81
@@ -335,152 +337,166 @@
 msgid "has all mandatory data"
 msgstr ""
 
 #: models/filemodels.py:100
 msgid "original filename"
 msgstr ""
 
-#: models/filemodels.py:110 models/foldermodels.py:101
+#: models/filemodels.py:110 models/foldermodels.py:102
 #: models/thumbnailoptionmodels.py:10
 msgid "name"
 msgstr ""
 
 #: models/filemodels.py:116
 msgid "description"
 msgstr ""
 
-#: models/filemodels.py:125 models/foldermodels.py:107
+#: models/filemodels.py:125 models/foldermodels.py:108
 msgid "owner"
 msgstr ""
 
-#: models/filemodels.py:129 models/foldermodels.py:115
+#: models/filemodels.py:129 models/foldermodels.py:116
 msgid "uploaded at"
 msgstr ""
 
-#: models/filemodels.py:134 models/foldermodels.py:125
+#: models/filemodels.py:134 models/foldermodels.py:126
 msgid "modified at"
 msgstr ""
 
 #: models/filemodels.py:140
 msgid "Permissions disabled"
 msgstr ""
 
 #: models/filemodels.py:141
 msgid ""
 "Disable any permission checking for this file. File will be publicly "
 "accessible to anyone."
 msgstr ""
 
-#: models/foldermodels.py:93
+#: models/foldermodels.py:94
 msgid "parent"
 msgstr ""
 
-#: models/foldermodels.py:120
+#: models/foldermodels.py:121
 msgid "created at"
 msgstr ""
 
-#: models/foldermodels.py:135
+#: models/foldermodels.py:136 templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Folder"
 msgstr ""
 
-#: models/foldermodels.py:136
+#: models/foldermodels.py:137
 #: templates/admin/filer/folder/directory_thumbnail_list.html:12
 msgid "Folders"
 msgstr ""
 
-#: models/foldermodels.py:259
+#: models/foldermodels.py:260
 msgid "all items"
 msgstr ""
 
-#: models/foldermodels.py:260
+#: models/foldermodels.py:261
 msgid "this item only"
 msgstr ""
 
-#: models/foldermodels.py:261
+#: models/foldermodels.py:262
 msgid "this item and all children"
 msgstr ""
 
-#: models/foldermodels.py:265
+#: models/foldermodels.py:266
 msgid "inherit"
 msgstr ""
 
-#: models/foldermodels.py:266
+#: models/foldermodels.py:267
 msgid "allow"
 msgstr ""
 
-#: models/foldermodels.py:267
+#: models/foldermodels.py:268
 msgid "deny"
 msgstr ""
 
-#: models/foldermodels.py:279
+#: models/foldermodels.py:280
 msgid "type"
 msgstr ""
 
-#: models/foldermodels.py:296
+#: models/foldermodels.py:297
 msgid "group"
 msgstr ""
 
-#: models/foldermodels.py:303
+#: models/foldermodels.py:304
 msgid "everybody"
 msgstr ""
 
-#: models/foldermodels.py:308
+#: models/foldermodels.py:309
 msgid "can read"
 msgstr ""
 
-#: models/foldermodels.py:316
+#: models/foldermodels.py:317
 msgid "can edit"
 msgstr ""
 
-#: models/foldermodels.py:324
+#: models/foldermodels.py:325
 msgid "can add children"
 msgstr ""
 
-#: models/foldermodels.py:332
+#: models/foldermodels.py:333
 msgid "folder permission"
 msgstr ""
 
-#: models/foldermodels.py:333
+#: models/foldermodels.py:334
 msgid "folder permissions"
 msgstr ""
 
-#: models/foldermodels.py:359
-#| msgid "Folders"
+#: models/foldermodels.py:348
+msgid "Folder cannot be selected with type \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:350
+msgid "Folder has to be selected when type is not \"all items\"."
+msgstr ""
+
+#: models/foldermodels.py:352
+msgid "User or group cannot be selected together with \"everybody\"."
+msgstr ""
+
+#: models/foldermodels.py:354
+msgid "At least one of user, group, or \"everybody\" has to be selected."
+msgstr ""
+
+#: models/foldermodels.py:360
 msgid "All Folders"
 msgstr ""
 
-#: models/foldermodels.py:361
+#: models/foldermodels.py:362
 msgid "Logical Path"
 msgstr ""
 
-#: models/foldermodels.py:370
+#: models/foldermodels.py:371
 #, python-brace-format
 msgid "User: {user}"
 msgstr ""
 
-#: models/foldermodels.py:372
+#: models/foldermodels.py:373
 #, python-brace-format
 msgid "Group: {group}"
 msgstr ""
 
-#: models/foldermodels.py:374
-#| msgid "everybody"
+#: models/foldermodels.py:375
 msgid "Everybody"
 msgstr ""
 
-#: models/foldermodels.py:387 templates/admin/filer/widgets/admin_file.html:45
+#: models/foldermodels.py:388 templates/admin/filer/widgets/admin_file.html:45
 msgid "Edit"
 msgstr ""
 
-#: models/foldermodels.py:388
+#: models/foldermodels.py:389
 msgid "Read"
 msgstr ""
 
-#: models/foldermodels.py:389
-#| msgid "can add children"
+#: models/foldermodels.py:390
 msgid "Add children"
 msgstr ""
 
 #: models/imagemodels.py:18
 msgid "date taken"
 msgstr ""
 
@@ -517,27 +533,24 @@
 msgid "Unsorted Uploads"
 msgstr ""
 
 #: models/virtualitems.py:73
 msgid "files with missing metadata"
 msgstr ""
 
-#: models/virtualitems.py:87 templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:37
-#: templates/admin/filer/folder/directory_listing.html:104
+#: models/virtualitems.py:87 templates/admin/filer/folder/change_form.html:8
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "root"
 msgstr ""
 
 #: settings.py:273
 msgid "Show table view"
 msgstr ""
 
 #: settings.py:278
-#| msgid "thumbnail option"
 msgid "Show thumbnail view"
 msgstr ""
 
 #: templates/admin/filer/actions.html:5
 msgid "Run the selected action"
 msgstr ""
 
@@ -574,24 +587,24 @@
 msgstr ""
 
 #: templates/admin/filer/breadcrumbs.html:5
 #: templates/admin/filer/folder/directory_listing.html:32
 msgid "Go back to Filer app"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:7
-#: templates/admin/filer/folder/directory_listing.html:37
+#: templates/admin/filer/breadcrumbs.html:6
+#: templates/admin/filer/folder/directory_listing.html:35
 msgid "Go back to root folder"
 msgstr ""
 
-#: templates/admin/filer/breadcrumbs.html:10
-#: templates/admin/filer/breadcrumbs.html:20
+#: templates/admin/filer/breadcrumbs.html:8
+#: templates/admin/filer/breadcrumbs.html:18
 #: templates/admin/filer/folder/change_form.html:10
-#: templates/admin/filer/folder/directory_listing.html:42
-#: templates/admin/filer/folder/directory_listing.html:49
+#: templates/admin/filer/folder/directory_listing.html:39
+#: templates/admin/filer/folder/directory_listing.html:47
 #, python-format
 msgid "Go back to '%(folder_name)s' folder"
 msgstr ""
 
 #: templates/admin/filer/change_form.html:26
 msgid "Duplicates"
 msgstr ""
@@ -636,38 +649,38 @@
 #: templates/admin/filer/image/change_form.html:37
 msgid "View on site"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 #: templates/admin/filer/folder/change_form.html:7
 #: templates/admin/filer/folder/change_form.html:8
-#: templates/admin/filer/folder/directory_listing.html:104
+#: templates/admin/filer/folder/directory_listing.html:102
 msgid "Go back to"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:6
 msgid "admin homepage"
 msgstr ""
 
 #: templates/admin/filer/folder/change_form.html:37
-#: templates/admin/filer/folder/directory_listing.html:97
-#: templates/admin/filer/folder/directory_listing.html:105
+#: templates/admin/filer/folder/directory_listing.html:95
+#: templates/admin/filer/folder/directory_listing.html:103
 #: templates/admin/filer/folder/directory_table_list.html:29
 #: templates/admin/filer/folder/directory_table_list.html:59
 #: templates/admin/filer/folder/directory_table_list.html:178
 #: templates/admin/filer/folder/directory_thumbnail_list.html:27
 #: templates/admin/filer/folder/directory_thumbnail_list.html:61
 #: templates/admin/filer/folder/directory_thumbnail_list.html:156
 msgid "Folder Icon"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:23
 msgid ""
-"Your account doesn't have permissions to copy all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to copy all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:25
 #: templates/admin/filer/folder/choose_copy_destination.html:31
 #: templates/admin/filer/folder/choose_copy_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:37
 #: templates/admin/filer/folder/choose_move_destination.html:43
@@ -693,15 +706,15 @@
 #: templates/admin/filer/folder/choose_copy_destination.html:54
 #: templates/admin/filer/folder/choose_move_destination.html:64
 msgid "Destination folder:"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:65
 #: templates/admin/filer/folder/choose_copy_destination.html:68
-#: templates/admin/filer/folder/directory_listing.html:180
+#: templates/admin/filer/folder/directory_listing.html:178
 msgid "Copy"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_copy_destination.html:67
 msgid "It is not allowed to copy files into same folder"
 msgstr ""
 
@@ -734,31 +747,31 @@
 
 #: templates/admin/filer/folder/choose_images_resize_options.html:41
 msgid "Resize"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:35
 msgid ""
-"Your account doesn't have permissions to move all of the selected files "
-"and/or folders."
+"Your account doesn't have permissions to move all of the selected files and/"
+"or folders."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:47
 msgid "There are no files and/or folders available to move."
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:52
 msgid ""
 "The following files and/or folders will be moved to a destination folder "
 "(retaining their tree structure):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:73
 #: templates/admin/filer/folder/choose_move_destination.html:76
-#: templates/admin/filer/folder/directory_listing.html:183
+#: templates/admin/filer/folder/directory_listing.html:181
 msgid "Move"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_move_destination.html:75
 msgid "It is not allowed to move files into same folder"
 msgstr ""
 
@@ -777,71 +790,71 @@
 "keep original filename, only displayed filename will be changed):"
 msgstr ""
 
 #: templates/admin/filer/folder/choose_rename_format.html:59
 msgid "Rename"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:96
+#: templates/admin/filer/folder/directory_listing.html:94
 msgid "Go back to the parent folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change current folder details"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:133
+#: templates/admin/filer/folder/directory_listing.html:131
 msgid "Change"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:143
+#: templates/admin/filer/folder/directory_listing.html:141
 msgid "Click here to run search for entered phrase"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:146
+#: templates/admin/filer/folder/directory_listing.html:144
 msgid "Search"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:153
+#: templates/admin/filer/folder/directory_listing.html:151
 msgid "Close"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:155
+#: templates/admin/filer/folder/directory_listing.html:153
 msgid "Limit"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:160
+#: templates/admin/filer/folder/directory_listing.html:158
 msgid "Check it to limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:161
+#: templates/admin/filer/folder/directory_listing.html:159
 msgid "Limit the search to current folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:177
+#: templates/admin/filer/folder/directory_listing.html:175
 msgid "Delete"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:205
+#: templates/admin/filer/folder/directory_listing.html:203
 msgid "Adds a new Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:208
+#: templates/admin/filer/folder/directory_listing.html:206
 msgid "New Folder"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:213
-#: templates/admin/filer/folder/directory_listing.html:220
-#: templates/admin/filer/folder/directory_listing.html:223
-#: templates/admin/filer/folder/directory_listing.html:230
-#: templates/admin/filer/folder/directory_listing.html:237
+#: templates/admin/filer/folder/directory_listing.html:211
+#: templates/admin/filer/folder/directory_listing.html:218
+#: templates/admin/filer/folder/directory_listing.html:221
+#: templates/admin/filer/folder/directory_listing.html:228
+#: templates/admin/filer/folder/directory_listing.html:235
 msgid "Upload Files"
 msgstr ""
 
-#: templates/admin/filer/folder/directory_listing.html:235
+#: templates/admin/filer/folder/directory_listing.html:233
 msgid "You have to select a folder first"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:16
 msgid "Name"
 msgstr ""
 
@@ -873,21 +886,23 @@
 
 #: templates/admin/filer/folder/directory_table_list.html:76
 #: templates/admin/filer/tools/search_form.html:5
 #, python-format
 msgid "%(counter)s folder"
 msgid_plural "%(counter)s folders"
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:77
 #: templates/admin/filer/tools/search_form.html:6
 #, python-format
 msgid "%(counter)s file"
 msgid_plural "%(counter)s files"
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/directory_table_list.html:83
 msgid "Change folder details"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:84
 msgid "Remove folder"
@@ -924,21 +939,19 @@
 #: templates/admin/filer/folder/directory_table_list.html:131
 #: templates/admin/filer/folder/directory_thumbnail_list.html:130
 msgid "enabled"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:144
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Canonical url '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:148
 #, python-format
-#| msgid "Change '%(item_label)s' details"
 msgid "Download '%(item_label)s'"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_table_list.html:152
 msgid "Remove file"
 msgstr ""
 
@@ -992,20 +1005,18 @@
 #: templates/admin/filer/folder/directory_thumbnail_list.html:210
 #, python-format
 msgid "Select all %(total_count)s"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:15
 #: templates/admin/filer/folder/directory_thumbnail_list.html:80
-#| msgid "Select this file"
 msgid "Select all"
 msgstr ""
 
 #: templates/admin/filer/folder/directory_thumbnail_list.html:77
-#| msgid "Filer"
 msgid "Files"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:4
 #: templates/admin/filer/folder/new_folder_form.html:7
 msgid "Add new"
 msgstr ""
@@ -1014,14 +1025,15 @@
 msgid "Django site admin"
 msgstr ""
 
 #: templates/admin/filer/folder/new_folder_form.html:15
 msgid "Please correct the error below."
 msgid_plural "Please correct the errors below."
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/admin/filer/folder/new_folder_form.html:30
 msgid "Save"
 msgstr ""
 
 #: templates/admin/filer/templatetags/file_icon.html:9
 msgid "Your browser does not support audio."
@@ -1061,16 +1073,15 @@
 
 #: templates/admin/filer/tools/detail_info.html:15
 msgid "Expand"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:20
 #: templates/admin/filer/widgets/admin_file.html:32
-#: templatetags/filer_admin_tags.py:101
-#| msgid "file missing"
+#: templatetags/filer_admin_tags.py:107
 msgid "File is missing"
 msgstr ""
 
 #: templates/admin/filer/tools/detail_info.html:29
 msgid "Type"
 msgstr ""
 
@@ -1118,15 +1129,14 @@
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_file.html:51
 msgid "Choose File"
 msgstr ""
 
 #: templates/admin/filer/widgets/admin_folder.html:16
-#| msgid "Choose File"
 msgid "Choose Folder"
 msgstr ""
 
 #: validation.py:19
 #, python-brace-format
 msgid "File \"{file_name}\": Upload denied by site security policy"
 msgstr ""
@@ -1184,10 +1194,11 @@
 #~ msgid ""
 #~ "\n"
 #~ "            %(counter)s file"
 #~ msgid_plural ""
 #~ "%(counter)s files\n"
 #~ "        "
 #~ msgstr[0] "15c0f2d28d6dab1af1f6d94906beb627_pl_0"
+#~ msgstr[1] "15c0f2d28d6dab1af1f6d94906beb627_pl_1"
 
 #~ msgid "Upload File"
 #~ msgstr "Upload File"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-filer-3.0.3/filer/management/commands/filer_check.py` & `django-filer-3.0.4/filer/management/commands/filer_check.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/management/commands/generate_thumbnails.py` & `django-filer-3.0.4/filer/management/commands/generate_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/management/commands/import_files.py` & `django-filer-3.0.4/filer/management/commands/import_files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0001_initial.py` & `django-filer-3.0.4/filer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0002_auto_20150606_2003.py` & `django-filer-3.0.4/filer/migrations/0002_auto_20150606_2003.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0003_thumbnailoption.py` & `django-filer-3.0.4/filer/migrations/0003_thumbnailoption.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0005_auto_20160623_1425.py` & `django-filer-3.0.4/filer/migrations/0005_auto_20160623_1425.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0006_auto_20160623_1627.py` & `django-filer-3.0.4/filer/migrations/0006_auto_20160623_1627.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0008_auto_20171117_1313.py` & `django-filer-3.0.4/filer/migrations/0008_auto_20171117_1313.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0010_auto_20180414_2058.py` & `django-filer-3.0.4/filer/migrations/0010_auto_20180414_2058.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0011_auto_20190418_0137.py` & `django-filer-3.0.4/filer/migrations/0011_auto_20190418_0137.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0012_file_mime_type.py` & `django-filer-3.0.4/filer/migrations/0012_file_mime_type.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0013_image_width_height_to_float.py` & `django-filer-3.0.4/filer/migrations/0013_image_width_height_to_float.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0014_folder_permission_choices.py` & `django-filer-3.0.4/filer/migrations/0014_folder_permission_choices.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py` & `django-filer-3.0.4/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py` & `django-filer-3.0.4/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/models/abstract.py` & `django-filer-3.0.4/filer/models/abstract.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/models/clipboardmodels.py` & `django-filer-3.0.4/filer/models/clipboardmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/models/filemodels.py` & `django-filer-3.0.4/filer/models/filemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/models/foldermodels.py` & `django-filer-3.0.4/filer/models/foldermodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.contrib.auth import models as auth_models
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.db.models import Q
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.html import format_html, format_html_join
+from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
 
 from .. import settings as filer_settings
 from . import mixins
 
 
 class FolderPermissionManager(models.Manager):
@@ -340,27 +341,27 @@
 
     def __repr__(self):
         return f'<{self.__class__.__name__}(pk={self.pk}): folder="{self.pretty_logical_path}", ' \
                'who="{self.who}", what="{self.what}">'
 
     def clean(self):
         if self.type == self.ALL and self.folder:
-            raise ValidationError('Folder cannot be selected with type "all items".')
+            raise ValidationError(_('Folder cannot be selected with type "all items".'))
         if self.type != self.ALL and not self.folder:
-            raise ValidationError('Folder has to be selected when type is not "all items".')
+            raise ValidationError(_('Folder has to be selected when type is not "all items".'))
         if self.everybody and (self.user or self.group):
-            raise ValidationError('User or group cannot be selected together with "everybody".')
+            raise ValidationError(_('User or group cannot be selected together with "everybody".'))
         if not self.user and not self.group and not self.everybody:
-            raise ValidationError('At least one of user, group, or "everybody" has to be selected.')
+            raise ValidationError(_('At least one of user, group, or "everybody" has to be selected.'))
 
     @cached_property
     def pretty_logical_path(self):
         if self.folder:
             return self.folder.pretty_logical_path
-        return _("All Folders")
+        return gettext("All Folders")
 
     pretty_logical_path.short_description = _("Logical Path")
 
     @cached_property
     def who(self):
         """
         Returns a human readable string of *who* can interact with a given folder
```

### Comparing `django-filer-3.0.3/filer/models/imagemodels.py` & `django-filer-3.0.4/filer/models/imagemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/models/mixins.py` & `django-filer-3.0.4/filer/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/models/thumbnailoptionmodels.py` & `django-filer-3.0.4/filer/models/thumbnailoptionmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/models/tools.py` & `django-filer-3.0.4/filer/models/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/models/virtualitems.py` & `django-filer-3.0.4/filer/models/virtualitems.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/server/backends/base.py` & `django-filer-3.0.4/filer/server/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/server/backends/default.py` & `django-filer-3.0.4/filer/server/backends/default.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/server/backends/nginx.py` & `django-filer-3.0.4/filer/server/backends/nginx.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/server/backends/xsendfile.py` & `django-filer-3.0.4/filer/server/backends/xsendfile.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/server/views.py` & `django-filer-3.0.4/filer/server/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/settings.py` & `django-filer-3.0.4/filer/settings.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/css/admin_filer.cms.icons.css` & `django-filer-3.0.4/filer/static/filer/css/admin_filer.cms.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/css/admin_filer.css` & `django-filer-3.0.4/filer/static/filer/css/admin_filer.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/css/admin_filer.fa.icons.css` & `django-filer-3.0.4/filer/static/filer/css/admin_filer.fa.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.cms.icons.css.map` & `django-filer-3.0.4/filer/static/filer/css/maps/admin_filer.cms.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.css.map` & `django-filer-3.0.4/filer/static/filer/css/maps/admin_filer.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.fa.icons.css.map` & `django-filer-3.0.4/filer/static/filer/css/maps/admin_filer.fa.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.icons.css.map` & `django-filer-3.0.4/filer/static/filer/css/maps/admin_filer.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/FontAwesome.otf` & `django-filer-3.0.4/filer/static/filer/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.eot` & `django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.svg` & `django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.ttf` & `django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.woff` & `django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.woff2` & `django-filer-3.0.4/filer/static/filer/fonts/django-filer-iconfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.eot` & `django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.svg` & `django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.ttf` & `django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.woff` & `django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.woff2` & `django-filer-3.0.4/filer/static/filer/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/src/arrow-down.svg` & `django-filer-3.0.4/filer/static/filer/fonts/src/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/src/link.svg` & `django-filer-3.0.4/filer/static/filer/fonts/src/link.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/src/move-to-folder.svg` & `django-filer-3.0.4/filer/static/filer/fonts/src/move-to-folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/src/th-list.svg` & `django-filer-3.0.4/filer/static/filer/fonts/src/th-list.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/fonts/src/upload.svg` & `django-filer-3.0.4/filer/static/filer/fonts/src/upload.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/cloud-up.svg` & `django-filer-3.0.4/filer/static/filer/icons/cloud-up.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-audio.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-empty.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-font.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-missing.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-pdf.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-picture.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-unknown.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-video.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/file-zip.svg` & `django-filer-3.0.4/filer/static/filer/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/folder-dropdown.svg` & `django-filer-3.0.4/filer/static/filer/icons/folder-dropdown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/folder-root.svg` & `django-filer-3.0.4/filer/static/filer/icons/folder-root.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/folder-unfiled.svg` & `django-filer-3.0.4/filer/static/filer/icons/folder-unfiled.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/icons/folder.svg` & `django-filer-3.0.4/filer/static/filer/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/img/icon_changelink.gif` & `django-filer-3.0.4/filer/static/filer/img/icon_changelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/img/icon_deletelink.gif` & `django-filer-3.0.4/filer/static/filer/img/icon_deletelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/img/loading_animation.gif` & `django-filer-3.0.4/filer/static/filer/img/loading_animation.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/img/upload_button.png` & `django-filer-3.0.4/filer/static/filer/img/upload_button.png`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/copy-move-files.js` & `django-filer-3.0.4/filer/static/filer/js/addons/copy-move-files.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/dropdown-menu.js` & `django-filer-3.0.4/filer/static/filer/js/addons/dropdown-menu.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/dropzone.init.js` & `django-filer-3.0.4/filer/static/filer/js/addons/dropzone.init.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/filer_popup_response.js` & `django-filer-3.0.4/filer/static/filer/js/addons/filer_popup_response.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/focal-point.js` & `django-filer-3.0.4/filer/static/filer/js/addons/focal-point.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/popup_handling.js` & `django-filer-3.0.4/filer/static/filer/js/addons/popup_handling.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/table-dropzone.js` & `django-filer-3.0.4/filer/static/filer/js/addons/table-dropzone.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/toggler.js` & `django-filer-3.0.4/filer/static/filer/js/addons/toggler.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/tooltip.js` & `django-filer-3.0.4/filer/static/filer/js/addons/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/upload-button.js` & `django-filer-3.0.4/filer/static/filer/js/addons/upload-button.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/addons/widget.js` & `django-filer-3.0.4/filer/static/filer/js/addons/widget.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/base.js` & `django-filer-3.0.4/filer/static/filer/js/base.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/libs/class.min.js` & `django-filer-3.0.4/filer/static/filer/js/libs/class.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/libs/dropzone.min.js` & `django-filer-3.0.4/filer/static/filer/js/libs/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/libs/fileuploader.min.js` & `django-filer-3.0.4/filer/static/filer/js/libs/fileuploader.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/libs/jquery-ui.min.js` & `django-filer-3.0.4/filer/static/filer/js/libs/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/libs/jquery.cookie.min.js` & `django-filer-3.0.4/filer/static/filer/js/libs/jquery.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/libs/jquery.min.js` & `django-filer-3.0.4/filer/static/filer/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/static/filer/js/libs/mediator.min.js` & `django-filer-3.0.4/filer/static/filer/js/libs/mediator.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/storage.py` & `django-filer-3.0.4/filer/storage.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/actions.html` & `django-filer-3.0.4/filer/templates/admin/filer/actions.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/base_site.html` & `django-filer-3.0.4/filer/templates/admin/filer/base_site.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/breadcrumbs.html` & `django-filer-3.0.4/filer/templates/admin/filer/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/change_form.html` & `django-filer-3.0.4/filer/templates/admin/filer/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/delete_selected_files_confirmation.html` & `django-filer-3.0.4/filer/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/file/change_form.html` & `django-filer-3.0.4/filer/templates/admin/filer/file/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/change_form.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/choose_copy_destination.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/choose_copy_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/choose_images_resize_options.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/choose_images_resize_options.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/choose_move_destination.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/choose_move_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/choose_rename_format.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/choose_rename_format.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/directory_listing.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/directory_listing.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/directory_table_list.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/directory_table_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/directory_thumbnail_list.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/directory_thumbnail_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/folder/new_folder_form.html` & `django-filer-3.0.4/filer/templates/admin/filer/folder/new_folder_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/image/change_form.html` & `django-filer-3.0.4/filer/templates/admin/filer/image/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/templatetags/file_icon.html` & `django-filer-3.0.4/filer/templates/admin/filer/templatetags/file_icon.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/clipboard.html` & `django-filer-3.0.4/filer/templates/admin/filer/tools/clipboard/clipboard.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html` & `django-filer-3.0.4/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/tools/detail_info.html` & `django-filer-3.0.4/filer/templates/admin/filer/tools/detail_info.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/tools/search_form.html` & `django-filer-3.0.4/filer/templates/admin/filer/tools/search_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/widgets/admin_file.html` & `django-filer-3.0.4/filer/templates/admin/filer/widgets/admin_file.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templates/admin/filer/widgets/admin_folder.html` & `django-filer-3.0.4/filer/templates/admin/filer/widgets/admin_folder.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templatetags/filer_admin_tags.py` & `django-filer-3.0.4/filer/templatetags/filer_admin_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templatetags/filer_image_tags.py` & `django-filer-3.0.4/filer/templatetags/filer_image_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/templatetags/filer_tags.py` & `django-filer-3.0.4/filer/templatetags/filer_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/thumbnail_processors.py` & `django-filer-3.0.4/filer/thumbnail_processors.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/utils/compatibility.py` & `django-filer-3.0.4/filer/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/utils/filer_easy_thumbnails.py` & `django-filer-3.0.4/filer/utils/filer_easy_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/utils/files.py` & `django-filer-3.0.4/filer/utils/files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/utils/generate_filename.py` & `django-filer-3.0.4/filer/utils/generate_filename.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/utils/loader.py` & `django-filer-3.0.4/filer/utils/loader.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/utils/pil_exif.py` & `django-filer-3.0.4/filer/utils/pil_exif.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/utils/recursive_dictionary.py` & `django-filer-3.0.4/filer/utils/recursive_dictionary.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/utils/zip.py` & `django-filer-3.0.4/filer/utils/zip.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/filer/validation.py` & `django-filer-3.0.4/filer/validation.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/setup.cfg` & `django-filer-3.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.3/setup.py` & `django-filer-3.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 from filer import __version__
 
 
 REQUIREMENTS = [
-    'django>=2.2,<5',
+    'django>=3.2,<5',
     'django-polymorphic',
     'easy-thumbnails[svg]',
 ]
 
 
 EXTRA_REQUIREMENTS = {
     "heif": [
```

