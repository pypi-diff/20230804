# Comparing `tmp/sphinx_rtd_theme-1.2.2rc1.tar.gz` & `tmp/sphinx_rtd_theme-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_rtd_theme-1.2.2rc1.tar", last modified: Wed Jun  7 12:48:22 2023, max compression
+gzip compressed data, was "sphinx_rtd_theme-1.3.0rc1.tar", last modified: Fri Aug  4 00:29:01 2023, max compression
```

## Comparing `sphinx_rtd_theme-1.2.2rc1.tar` & `sphinx_rtd_theme-1.3.0rc1.tar`

### file list

```diff
@@ -1,154 +1,155 @@
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.119685 sphinx_rtd_theme-1.2.2rc1/
--rw-rw-r--   0 balder    (1000) balder    (1000)    11379 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/Apache-License-2.0.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)     1119 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/LICENSE
--rw-rw-r--   0 balder    (1000) balder    (1000)      576 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/MANIFEST.in
--rw-rw-r--   0 balder    (1000) balder    (1000)     4438 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/OFL-License.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)     4185 2023-06-07 12:48:22.119685 sphinx_rtd_theme-1.2.2rc1/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     2742 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/README.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)      338 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/babel.cfg
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.099684 sphinx_rtd_theme-1.2.2rc1/bin/
--rwxrwxr-x   0 balder    (1000) balder    (1000)      853 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/bin/preinstall.js
--rw-rw-r--   0 balder    (1000) balder    (1000)     2949 2023-06-07 12:48:22.119685 sphinx_rtd_theme-1.2.2rc1/setup.cfg
--rw-rw-r--   0 balder    (1000) balder    (1000)     2111 2023-06-07 12:41:28.000000 sphinx_rtd_theme-1.2.2rc1/setup.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.099684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/
--rw-r--r--   0 balder    (1000) balder    (1000)     3480 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)     4277 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2915 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/footer.html
--rw-r--r--   0 balder    (1000) balder    (1000)     9716 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/layout.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2514 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5820 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2087 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4023 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)      457 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4912 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2567 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5094 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2380 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4828 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2693 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5018 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2522 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5050 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)      575 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)      842 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)      501 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)      765 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2703 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5824 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2750 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5711 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2549 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5505 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2339 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4257 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2354 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5038 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2780 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5830 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     3449 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     6468 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po
--rw-r--r--   0 balder    (1000) balder    (1000)     4633 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sphinx.pot
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2132 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4353 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2117 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4142 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2511 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5523 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)      506 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)      769 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po
--rw-r--r--   0 balder    (1000) balder    (1000)     1759 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/search.html
--rw-r--r--   0 balder    (1000) balder    (1000)      405 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/searchbox.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/
--rw-r--r--   0 balder    (1000) balder    (1000)     3229 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/badge_only.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.111684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/
--rw-r--r--   0 balder    (1000) balder    (1000)    87624 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    67312 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)    86288 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    66444 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   165742 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 balder    (1000) balder    (1000)   444379 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 balder    (1000) balder    (1000)   165548 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 balder    (1000) balder    (1000)    98024 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    77160 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   323344 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   193308 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   309728 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   184912 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   328412 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   195704 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   309192 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   182708 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   135314 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/theme.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.111684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/
--rw-r--r--   0 balder    (1000) balder    (1000)      934 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/badge_only.js
--rw-r--r--   0 balder    (1000) balder    (1000)     4370 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 balder    (1000) balder    (1000)     2734 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/html5shiv.min.js
--rw-r--r--   0 balder    (1000) balder    (1000)     5023 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/theme.js
--rw-r--r--   0 balder    (1000) balder    (1000)      407 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/theme.conf
--rw-r--r--   0 balder    (1000) balder    (1000)     1247 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/versions.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/
--rw-rw-r--   0 balder    (1000) balder    (1000)     4185 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     4199 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)       57 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/entry_points.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-01-13 09:47:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/not-zip-safe
--rw-rw-r--   0 balder    (1000) balder    (1000)      124 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/requires.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)       17 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/top_level.txt
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.115684 sphinx_rtd_theme-1.2.2rc1/tests/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/__init__.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.099684 sphinx_rtd_theme-1.2.2rc1/tests/roots/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.115684 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/
--rw-rw-r--   0 balder    (1000) balder    (1000)        8 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/bar.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       31 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/foo.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)       85 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/index.rst
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.115684 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-empty/
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-empty/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-empty/index.rst
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.115684 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-missing-toctree/
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-missing-toctree/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       42 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-missing-toctree/index.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)     3159 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/test_builders.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1770 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/util.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.325750 sphinx_rtd_theme-1.3.0rc1/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11379 2018-09-26 18:18:21.000000 sphinx_rtd_theme-1.3.0rc1/Apache-License-2.0.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1119 2018-04-05 19:52:21.000000 sphinx_rtd_theme-1.3.0rc1/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      576 2021-03-12 20:59:52.000000 sphinx_rtd_theme-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4438 2018-09-26 18:18:21.000000 sphinx_rtd_theme-1.3.0rc1/OFL-License.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4786 2023-08-04 00:29:01.325750 sphinx_rtd_theme-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2742 2021-10-20 22:54:41.000000 sphinx_rtd_theme-1.3.0rc1/README.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      338 2019-10-18 21:08:25.000000 sphinx_rtd_theme-1.3.0rc1/babel.cfg
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.219083 sphinx_rtd_theme-1.3.0rc1/bin/
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)      853 2019-10-18 21:08:25.000000 sphinx_rtd_theme-1.3.0rc1/bin/preinstall.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1337 2023-08-04 00:27:48.000000 sphinx_rtd_theme-1.3.0rc1/package.json
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2949 2023-08-04 00:29:01.355750 sphinx_rtd_theme-1.3.0rc1/setup.cfg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2111 2023-08-04 00:27:48.000000 sphinx_rtd_theme-1.3.0rc1/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.222416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3480 2023-08-04 00:27:48.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4277 2022-12-14 00:34:41.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2915 2022-05-26 19:44:31.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/footer.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9716 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/layout.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.225750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/da/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.229083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2514 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5820 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/de/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.229083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2087 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4023 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/en/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.232416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      457 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4912 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/es/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.232416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2567 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5094 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/et/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.235750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2380 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4828 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fa_IR/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.235750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2693 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5018 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fr/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.239083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2522 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5050 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hr/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.239083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      575 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      842 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.205750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hu/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.242416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      501 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      765 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/it/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.242416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2703 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5824 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/lt/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.245750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2750 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5711 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/nl/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.245750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2549 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5505 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pl/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.249083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2339 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4257 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.249083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2354 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5038 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt_BR/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.252416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2780 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5830 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/ru/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.252416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3449 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6468 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4633 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/sphinx.pot
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/sv/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.252416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2132 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4353 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/tr/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.255750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2117 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4142 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.209083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_CN/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.255750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2511 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5523 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.212416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_TW/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.259083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      506 2023-02-07 20:54:04.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      769 2023-08-04 00:27:42.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1759 2021-08-03 22:51:48.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/search.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      405 2022-12-14 00:34:41.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/searchbox.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.212416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.259083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3229 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/badge_only.css
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.312416 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    87624 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    67312 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    86288 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    66444 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   165742 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   444379 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   165548 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    98024 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    77160 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   323344 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   193308 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   309728 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   184912 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   328412 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   195704 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   309192 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   182708 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   135314 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/theme.css
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.319083 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      934 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/badge_only.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4370 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2734 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/html5shiv.min.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5023 2023-08-04 00:24:45.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/theme.js
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      407 2021-03-12 20:59:52.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/theme.conf
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1247 2021-03-12 20:59:52.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/versions.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.225750 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4786 2023-08-04 00:29:00.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4212 2023-08-04 00:29:01.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-08-04 00:29:00.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       58 2023-08-04 00:29:00.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2018-04-05 19:55:59.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      124 2023-08-04 00:29:00.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       17 2023-08-04 00:29:00.000000 sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/top_level.txt
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.319083 sphinx_rtd_theme-1.3.0rc1/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.212416 sphinx_rtd_theme-1.3.0rc1/tests/roots/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.322417 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-basic/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        8 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-basic/bar.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       76 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-basic/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       31 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-basic/foo.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       85 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-basic/index.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.325750 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-empty/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       76 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-empty/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       76 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-empty/index.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-08-04 00:29:01.325750 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-missing-toctree/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       76 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-missing-toctree/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       42 2018-03-30 00:05:39.000000 sphinx_rtd_theme-1.3.0rc1/tests/roots/test-missing-toctree/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3159 2021-08-03 22:51:48.000000 sphinx_rtd_theme-1.3.0rc1/tests/test_builders.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1770 2021-08-03 22:51:48.000000 sphinx_rtd_theme-1.3.0rc1/tests/util.py
```

### Comparing `sphinx_rtd_theme-1.2.2rc1/Apache-License-2.0.txt` & `sphinx_rtd_theme-1.3.0rc1/Apache-License-2.0.txt`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/LICENSE` & `sphinx_rtd_theme-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/MANIFEST.in` & `sphinx_rtd_theme-1.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/OFL-License.txt` & `sphinx_rtd_theme-1.3.0rc1/OFL-License.txt`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/PKG-INFO` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,94 @@
 Metadata-Version: 2.1
-Name: sphinx_rtd_theme
-Version: 1.2.2rc1
+Name: sphinx-rtd-theme
+Version: 1.3.0rc1
 Summary: Read the Docs theme for Sphinx
 Home-page: https://github.com/readthedocs/sphinx_rtd_theme
 Author: Dave Snider, Read the Docs, Inc. & contributors
 Author-email: dev@readthedocs.org
 License: MIT
 Project-URL: Homepage, https://sphinx-rtd-theme.readthedocs.io/
 Project-URL: Source Code, https://github.com/readthedocs/sphinx_rtd_theme
 Project-URL: Issue Tracker, https://github.com/readthedocs/sphinx_rtd_theme/issues
+Description: **************************
+        Read the Docs Sphinx Theme
+        **************************
+        
+        .. image:: https://img.shields.io/pypi/v/sphinx_rtd_theme.svg
+           :target: https://pypi.python.org/pypi/sphinx_rtd_theme
+           :alt: Pypi Version
+        .. image:: https://circleci.com/gh/readthedocs/sphinx_rtd_theme.svg?style=svg
+           :alt: Build Status
+           :target: https://circleci.com/gh/readthedocs/sphinx_rtd_theme
+        .. image:: https://img.shields.io/pypi/l/sphinx_rtd_theme.svg
+           :target: https://pypi.python.org/pypi/sphinx_rtd_theme/
+           :alt: License
+        .. image:: https://readthedocs.org/projects/sphinx-rtd-theme/badge/?version=latest
+          :target: http://sphinx-rtd-theme.readthedocs.io/en/latest/?badge=latest
+          :alt: Documentation Status
+        
+        This Sphinx_ theme was designed to provide a great reader experience for
+        documentation users on both desktop and mobile devices. This theme is used
+        primarily on `Read the Docs`_ but can work with any Sphinx project. You can find
+        a working demo of the theme in the `theme documentation`_
+        
+        .. _Sphinx: http://www.sphinx-doc.org
+        .. _Read the Docs: http://www.readthedocs.org
+        .. _theme documentation: https://sphinx-rtd-theme.readthedocs.io/en/stable/
+        
+        Installation
+        ============
+        
+        This theme is distributed on PyPI_ and can be installed with ``pip``:
+        
+        .. code:: console
+        
+           $ pip install sphinx-rtd-theme
+        
+        To use the theme in your Sphinx project, you will need to edit
+        your ``conf.py`` file's ``html_theme`` setting:
+        
+        .. code:: python
+        
+            html_theme = "sphinx_rtd_theme"
+        
+        .. admonition:: See also:
+        
+            `Supported browsers`_
+                Officially supported and tested browser/operating system combinations
+        
+            `Supported dependencies`_
+                Supported versions of Python, Sphinx, and other dependencies.
+        
+            `Example documentation`_
+                A full example of this theme output, with localized strings enabled.
+        
+        .. _PyPI: https://pypi.python.org/pypi/sphinx_rtd_theme
+        .. _Supported browsers: https://sphinx-rtd-theme.readthedocs.io/en/stable/development.html#supported-browsers
+        .. _Supported dependencies: https://sphinx-rtd-theme.readthedocs.io/en/stable/development.html#supported-dependencies
+        .. _Example documentation:  https://sphinx-rtd-theme.readthedocs.io/en/stable/
+        
+        Configuration
+        =============
+        
+        This theme is highly customizable on both the page level and on a global level.
+        To see all the possible configuration options, read the documentation on
+        `configuring the theme`_.
+        
+        .. _configuring the theme: https://sphinx-rtd-theme.readthedocs.io/en/stable/configuring.html
+        
+        Contributing
+        ============
+        
+        If you would like to help modify or translate the theme, you'll find more
+        information on contributing in our `contributing guide`_.
+        
+        .. _contributing guide: https://sphinx-rtd-theme.readthedocs.io/en/stable/contributing.html
+        
+Platform: UNKNOWN
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -25,83 +101,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
 Provides-Extra: dev
-License-File: LICENSE
-
-**************************
-Read the Docs Sphinx Theme
-**************************
-
-.. image:: https://img.shields.io/pypi/v/sphinx_rtd_theme.svg
-   :target: https://pypi.python.org/pypi/sphinx_rtd_theme
-   :alt: Pypi Version
-.. image:: https://circleci.com/gh/readthedocs/sphinx_rtd_theme.svg?style=svg
-   :alt: Build Status
-   :target: https://circleci.com/gh/readthedocs/sphinx_rtd_theme
-.. image:: https://img.shields.io/pypi/l/sphinx_rtd_theme.svg
-   :target: https://pypi.python.org/pypi/sphinx_rtd_theme/
-   :alt: License
-.. image:: https://readthedocs.org/projects/sphinx-rtd-theme/badge/?version=latest
-  :target: http://sphinx-rtd-theme.readthedocs.io/en/latest/?badge=latest
-  :alt: Documentation Status
-
-This Sphinx_ theme was designed to provide a great reader experience for
-documentation users on both desktop and mobile devices. This theme is used
-primarily on `Read the Docs`_ but can work with any Sphinx project. You can find
-a working demo of the theme in the `theme documentation`_
-
-.. _Sphinx: http://www.sphinx-doc.org
-.. _Read the Docs: http://www.readthedocs.org
-.. _theme documentation: https://sphinx-rtd-theme.readthedocs.io/en/stable/
-
-Installation
-============
-
-This theme is distributed on PyPI_ and can be installed with ``pip``:
-
-.. code:: console
-
-   $ pip install sphinx-rtd-theme
-
-To use the theme in your Sphinx project, you will need to edit
-your ``conf.py`` file's ``html_theme`` setting:
-
-.. code:: python
-
-    html_theme = "sphinx_rtd_theme"
-
-.. admonition:: See also:
-
-    `Supported browsers`_
-        Officially supported and tested browser/operating system combinations
-
-    `Supported dependencies`_
-        Supported versions of Python, Sphinx, and other dependencies.
-
-    `Example documentation`_
-        A full example of this theme output, with localized strings enabled.
-
-.. _PyPI: https://pypi.python.org/pypi/sphinx_rtd_theme
-.. _Supported browsers: https://sphinx-rtd-theme.readthedocs.io/en/stable/development.html#supported-browsers
-.. _Supported dependencies: https://sphinx-rtd-theme.readthedocs.io/en/stable/development.html#supported-dependencies
-.. _Example documentation:  https://sphinx-rtd-theme.readthedocs.io/en/stable/
-
-Configuration
-=============
-
-This theme is highly customizable on both the page level and on a global level.
-To see all the possible configuration options, read the documentation on
-`configuring the theme`_.
-
-.. _configuring the theme: https://sphinx-rtd-theme.readthedocs.io/en/stable/configuring.html
-
-Contributing
-============
-
-If you would like to help modify or translate the theme, you'll find more
-information on contributing in our `contributing guide`_.
-
-.. _contributing guide: https://sphinx-rtd-theme.readthedocs.io/en/stable/contributing.html
```

### Comparing `sphinx_rtd_theme-1.2.2rc1/README.rst` & `sphinx_rtd_theme-1.3.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/bin/preinstall.js` & `sphinx_rtd_theme-1.3.0rc1/bin/preinstall.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/setup.cfg` & `sphinx_rtd_theme-1.3.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.2rc1
+current_version = 1.3.0rc1
 commit = false
 tag = false
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)((?P<release>[a-z]+)(?P<dev>\d+))?
 serialize = 
 	{major}.{minor}.{patch}{release}{dev}
 	{major}.{minor}.{patch}
 
@@ -41,15 +41,15 @@
 
 [options]
 include_package_data = True
 zip_safe = False
 packages = sphinx_rtd_theme
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 install_requires = 
-	sphinx >=1.6,<7
+	sphinx >=1.6,<8
 	docutils <0.19
 	sphinxcontrib-jquery >=4,<5
 tests_require = 
 	pytest
 
 [options.extras_require]
 dev =
```

### Comparing `sphinx_rtd_theme-1.2.2rc1/setup.py` & `sphinx_rtd_theme-1.3.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def run(self):
         subprocess.run(['tx', 'push', '--source'], check=True)
         subprocess.run(['tx', 'pull', '--mode', 'onlyreviewed', '-f', '-a'], check=True)
 
 
 setup(
-    version='1.2.2rc1',
+    version='1.3.0rc1',
     cmdclass={
         'update_translations': UpdateTranslationsCommand,
         'transifex': TransifexCommand,
         'build_assets': WebpackBuildCommand,
         'watch': WebpackDevelopCommand,
     },
 )
```

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/__init__.py` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sys import version_info as python_version
 
 from sphinx import version_info as sphinx_version
 from sphinx.locale import _
 from sphinx.util.logging import getLogger
 
 
-__version__ = '1.2.2rc1'
+__version__ = '1.3.0rc1'
 __version_full__ = __version__
 
 logger = getLogger(__name__)
 
 
 def get_html_theme_path():
     """Return list of HTML theme paths."""
```

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/breadcrumbs.html` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/footer.html` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/layout.html` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sphinx.pot` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/sphinx.pot`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/search.html` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/badge_only.css` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/theme.css` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/badge_only.js` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/html5shiv.min.js` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/theme.js` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/versions.html` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/PKG-INFO` & `sphinx_rtd_theme-1.3.0rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,94 @@
 Metadata-Version: 2.1
-Name: sphinx-rtd-theme
-Version: 1.2.2rc1
+Name: sphinx_rtd_theme
+Version: 1.3.0rc1
 Summary: Read the Docs theme for Sphinx
 Home-page: https://github.com/readthedocs/sphinx_rtd_theme
 Author: Dave Snider, Read the Docs, Inc. & contributors
 Author-email: dev@readthedocs.org
 License: MIT
 Project-URL: Homepage, https://sphinx-rtd-theme.readthedocs.io/
 Project-URL: Source Code, https://github.com/readthedocs/sphinx_rtd_theme
 Project-URL: Issue Tracker, https://github.com/readthedocs/sphinx_rtd_theme/issues
+Description: **************************
+        Read the Docs Sphinx Theme
+        **************************
+        
+        .. image:: https://img.shields.io/pypi/v/sphinx_rtd_theme.svg
+           :target: https://pypi.python.org/pypi/sphinx_rtd_theme
+           :alt: Pypi Version
+        .. image:: https://circleci.com/gh/readthedocs/sphinx_rtd_theme.svg?style=svg
+           :alt: Build Status
+           :target: https://circleci.com/gh/readthedocs/sphinx_rtd_theme
+        .. image:: https://img.shields.io/pypi/l/sphinx_rtd_theme.svg
+           :target: https://pypi.python.org/pypi/sphinx_rtd_theme/
+           :alt: License
+        .. image:: https://readthedocs.org/projects/sphinx-rtd-theme/badge/?version=latest
+          :target: http://sphinx-rtd-theme.readthedocs.io/en/latest/?badge=latest
+          :alt: Documentation Status
+        
+        This Sphinx_ theme was designed to provide a great reader experience for
+        documentation users on both desktop and mobile devices. This theme is used
+        primarily on `Read the Docs`_ but can work with any Sphinx project. You can find
+        a working demo of the theme in the `theme documentation`_
+        
+        .. _Sphinx: http://www.sphinx-doc.org
+        .. _Read the Docs: http://www.readthedocs.org
+        .. _theme documentation: https://sphinx-rtd-theme.readthedocs.io/en/stable/
+        
+        Installation
+        ============
+        
+        This theme is distributed on PyPI_ and can be installed with ``pip``:
+        
+        .. code:: console
+        
+           $ pip install sphinx-rtd-theme
+        
+        To use the theme in your Sphinx project, you will need to edit
+        your ``conf.py`` file's ``html_theme`` setting:
+        
+        .. code:: python
+        
+            html_theme = "sphinx_rtd_theme"
+        
+        .. admonition:: See also:
+        
+            `Supported browsers`_
+                Officially supported and tested browser/operating system combinations
+        
+            `Supported dependencies`_
+                Supported versions of Python, Sphinx, and other dependencies.
+        
+            `Example documentation`_
+                A full example of this theme output, with localized strings enabled.
+        
+        .. _PyPI: https://pypi.python.org/pypi/sphinx_rtd_theme
+        .. _Supported browsers: https://sphinx-rtd-theme.readthedocs.io/en/stable/development.html#supported-browsers
+        .. _Supported dependencies: https://sphinx-rtd-theme.readthedocs.io/en/stable/development.html#supported-dependencies
+        .. _Example documentation:  https://sphinx-rtd-theme.readthedocs.io/en/stable/
+        
+        Configuration
+        =============
+        
+        This theme is highly customizable on both the page level and on a global level.
+        To see all the possible configuration options, read the documentation on
+        `configuring the theme`_.
+        
+        .. _configuring the theme: https://sphinx-rtd-theme.readthedocs.io/en/stable/configuring.html
+        
+        Contributing
+        ============
+        
+        If you would like to help modify or translate the theme, you'll find more
+        information on contributing in our `contributing guide`_.
+        
+        .. _contributing guide: https://sphinx-rtd-theme.readthedocs.io/en/stable/contributing.html
+        
+Platform: UNKNOWN
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -25,83 +101,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
 Provides-Extra: dev
-License-File: LICENSE
-
-**************************
-Read the Docs Sphinx Theme
-**************************
-
-.. image:: https://img.shields.io/pypi/v/sphinx_rtd_theme.svg
-   :target: https://pypi.python.org/pypi/sphinx_rtd_theme
-   :alt: Pypi Version
-.. image:: https://circleci.com/gh/readthedocs/sphinx_rtd_theme.svg?style=svg
-   :alt: Build Status
-   :target: https://circleci.com/gh/readthedocs/sphinx_rtd_theme
-.. image:: https://img.shields.io/pypi/l/sphinx_rtd_theme.svg
-   :target: https://pypi.python.org/pypi/sphinx_rtd_theme/
-   :alt: License
-.. image:: https://readthedocs.org/projects/sphinx-rtd-theme/badge/?version=latest
-  :target: http://sphinx-rtd-theme.readthedocs.io/en/latest/?badge=latest
-  :alt: Documentation Status
-
-This Sphinx_ theme was designed to provide a great reader experience for
-documentation users on both desktop and mobile devices. This theme is used
-primarily on `Read the Docs`_ but can work with any Sphinx project. You can find
-a working demo of the theme in the `theme documentation`_
-
-.. _Sphinx: http://www.sphinx-doc.org
-.. _Read the Docs: http://www.readthedocs.org
-.. _theme documentation: https://sphinx-rtd-theme.readthedocs.io/en/stable/
-
-Installation
-============
-
-This theme is distributed on PyPI_ and can be installed with ``pip``:
-
-.. code:: console
-
-   $ pip install sphinx-rtd-theme
-
-To use the theme in your Sphinx project, you will need to edit
-your ``conf.py`` file's ``html_theme`` setting:
-
-.. code:: python
-
-    html_theme = "sphinx_rtd_theme"
-
-.. admonition:: See also:
-
-    `Supported browsers`_
-        Officially supported and tested browser/operating system combinations
-
-    `Supported dependencies`_
-        Supported versions of Python, Sphinx, and other dependencies.
-
-    `Example documentation`_
-        A full example of this theme output, with localized strings enabled.
-
-.. _PyPI: https://pypi.python.org/pypi/sphinx_rtd_theme
-.. _Supported browsers: https://sphinx-rtd-theme.readthedocs.io/en/stable/development.html#supported-browsers
-.. _Supported dependencies: https://sphinx-rtd-theme.readthedocs.io/en/stable/development.html#supported-dependencies
-.. _Example documentation:  https://sphinx-rtd-theme.readthedocs.io/en/stable/
-
-Configuration
-=============
-
-This theme is highly customizable on both the page level and on a global level.
-To see all the possible configuration options, read the documentation on
-`configuring the theme`_.
-
-.. _configuring the theme: https://sphinx-rtd-theme.readthedocs.io/en/stable/configuring.html
-
-Contributing
-============
-
-If you would like to help modify or translate the theme, you'll find more
-information on contributing in our `contributing guide`_.
-
-.. _contributing guide: https://sphinx-rtd-theme.readthedocs.io/en/stable/contributing.html
```

### Comparing `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/SOURCES.txt` & `sphinx_rtd_theme-1.3.0rc1/sphinx_rtd_theme.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Apache-License-2.0.txt
 LICENSE
 MANIFEST.in
 OFL-License.txt
 README.rst
 babel.cfg
+package.json
 setup.cfg
 setup.py
 bin/preinstall.js
 sphinx_rtd_theme/__init__.py
 sphinx_rtd_theme/breadcrumbs.html
 sphinx_rtd_theme/footer.html
 sphinx_rtd_theme/layout.html
```

### Comparing `sphinx_rtd_theme-1.2.2rc1/tests/test_builders.py` & `sphinx_rtd_theme-1.3.0rc1/tests/test_builders.py`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2rc1/tests/util.py` & `sphinx_rtd_theme-1.3.0rc1/tests/util.py`

 * *Files identical despite different names*

