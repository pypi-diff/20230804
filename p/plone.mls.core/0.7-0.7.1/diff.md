# Comparing `tmp/plone.mls.core-0.7.tar.gz` & `tmp/plone.mls.core-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.mls.core-0.7.tar", last modified: Tue Dec 12 13:00:06 2017, max compression
+gzip compressed data, was "dist/plone.mls.core-0.7.1.tar", last modified: Fri Aug  4 08:55:51 2023, max compression
```

## Comparing `plone.mls.core-0.7.tar` & `plone.mls.core-0.7.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/
--rw-r--r--   0 thomas     (501) staff       (20)     1950 2017-12-12 13:00:05.000000 plone.mls.core-0.7/CHANGES.rst
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/docs/
--rw-r--r--   0 thomas     (501) staff       (20)     1282 2017-12-12 13:00:05.000000 plone.mls.core-0.7/docs/INSTALL.txt
--rw-r--r--   0 thomas     (501) staff       (20)    17987 2017-12-12 13:00:05.000000 plone.mls.core-0.7/docs/LICENSE.GPL
--rw-r--r--   0 thomas     (501) staff       (20)      749 2017-12-12 13:00:05.000000 plone.mls.core-0.7/docs/LICENSE.txt
--rw-r--r--   0 thomas     (501) staff       (20)       79 2017-12-12 13:00:05.000000 plone.mls.core-0.7/MANIFEST.in
--rw-r--r--   0 thomas     (501) staff       (20)     4156 2017-12-12 13:00:06.000000 plone.mls.core-0.7/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      211 2017-12-12 13:00:05.000000 plone.mls.core-0.7/README.rst
--rw-r--r--   0 thomas     (501) staff       (20)      427 2017-12-12 13:00:06.000000 plone.mls.core-0.7/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)     1977 2017-12-12 13:00:05.000000 plone.mls.core-0.7/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/
--rw-r--r--   0 thomas     (501) staff       (20)       80 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/
--rw-r--r--   0 thomas     (501) staff       (20)       80 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/
--rw-r--r--   0 thomas     (501) staff       (20)       71 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     2269 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/api.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/browser/
--rw-r--r--   0 thomas     (501) staff       (20)       69 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/browser/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     1595 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/browser/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)      929 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/browser/controlpanel.py
--rw-r--r--   0 thomas     (501) staff       (20)      229 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/browser/interfaces.py
--rw-r--r--   0 thomas     (501) staff       (20)     3693 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/browser/localconfig.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/browser/resources/
--rw-r--r--   0 thomas     (501) staff       (20)      889 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/browser/resources/icon.png
--rw-r--r--   0 thomas     (501) staff       (20)      411 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/browser/resources/plone_mls_core.js
--rw-r--r--   0 thomas     (501) staff       (20)      454 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/config.py
--rw-r--r--   0 thomas     (501) staff       (20)     1221 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)      164 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/i18n.py
--rw-r--r--   0 thomas     (501) staff       (20)     1204 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/interfaces.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ar/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ar/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     3983 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ar/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/cmn/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/cmn/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     3907 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/cmn/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/de/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/de/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     4984 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/de/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/en/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/en/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     3696 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/en/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/es/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/es/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     5002 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/es/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/et/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/et/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     3902 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/et/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/fr/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/fr/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     5026 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/fr/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/it/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/it/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     4843 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/it/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ja/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ja/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     4326 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ja/LC_MESSAGES/plone.mls.core.po
--rw-r--r--   0 thomas     (501) staff       (20)      491 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/manual.pot
--rw-r--r--   0 thomas     (501) staff       (20)     3801 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/plone.mls.core.pot
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/pt/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/pt/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     4884 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/pt/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ru/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ru/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     5594 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/ru/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/vi/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/vi/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     3897 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/vi/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/vi_VN/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/vi_VN/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     3914 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/vi_VN/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/zh/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/zh/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     4121 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/zh/LC_MESSAGES/plone.mls.core.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/zh_TW/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)     3909 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/locales/zh_TW/LC_MESSAGES/plone.mls.core.po
--rw-r--r--   0 thomas     (501) staff       (20)      462 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/migration.py
--rw-r--r--   0 thomas     (501) staff       (20)     4250 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/navigation.py
--rw-r--r--   0 thomas     (501) staff       (20)      248 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/permissions.zcml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/base/
--rw-r--r--   0 thomas     (501) staff       (20)      167 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/base/metadata.xml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone4/
--rw-r--r--   0 thomas     (501) staff       (20)     2705 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone4/actions.xml
--rw-r--r--   0 thomas     (501) staff       (20)      151 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone4/browserlayer.xml
--rw-r--r--   0 thomas     (501) staff       (20)      237 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone4/jsregistry.xml
--rw-r--r--   0 thomas     (501) staff       (20)      171 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone4/metadata.xml
--rw-r--r--   0 thomas     (501) staff       (20)      109 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone4/registry.xml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone5/
--rw-r--r--   0 thomas     (501) staff       (20)     2705 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone5/actions.xml
--rw-r--r--   0 thomas     (501) staff       (20)      151 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone5/browserlayer.xml
--rw-r--r--   0 thomas     (501) staff       (20)      171 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone5/metadata.xml
--rw-r--r--   0 thomas     (501) staff       (20)      109 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/plone5/registry.xml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/uninstall-base/
--rw-r--r--   0 thomas     (501) staff       (20)      317 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/uninstall-base/import_steps.xml
--rw-r--r--   0 thomas     (501) staff       (20)       51 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/uninstall-base/plone.mls.core_uninstall.txt
--rw-r--r--   0 thomas     (501) staff       (20)      299 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/uninstall-base/registry.xml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/uninstall-plone4/
--rw-r--r--   0 thomas     (501) staff       (20)      170 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/uninstall-plone4/metadata.xml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/uninstall-plone5/
--rw-r--r--   0 thomas     (501) staff       (20)      170 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles/uninstall-plone5/metadata.xml
--rw-r--r--   0 thomas     (501) staff       (20)     2740 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/profiles.zcml
--rw-r--r--   0 thomas     (501) staff       (20)     1050 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/setuphandlers.py
--rw-r--r--   0 thomas     (501) staff       (20)      877 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/testing.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone/mls/core/tests/
--rw-r--r--   0 thomas     (501) staff       (20)       71 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/tests/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     1634 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/tests/test_controlpanel.py
--rw-r--r--   0 thomas     (501) staff       (20)     1702 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/tests/test_registry.py
--rw-r--r--   0 thomas     (501) staff       (20)     1063 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/tests/test_setup.py
--rw-r--r--   0 thomas     (501) staff       (20)     2620 2017-12-12 13:00:05.000000 plone.mls.core-0.7/src/plone/mls/core/utils.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)        1 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       82 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/entry_points.txt
--rw-r--r--   0 thomas     (501) staff       (20)       16 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/namespace_packages.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/not-zip-safe
--rw-r--r--   0 thomas     (501) staff       (20)     4156 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      137 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)     3159 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        6 2017-12-12 13:00:06.000000 plone.mls.core-0.7/src/plone.mls.core.egg-info/top_level.txt
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/
+-rw-r--r--   0 zach       (501) staff       (20)     4346 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)       79 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/MANIFEST.in
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/docs/
+-rw-r--r--   0 zach       (501) staff       (20)    17987 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/docs/LICENSE.GPL
+-rw-r--r--   0 zach       (501) staff       (20)     1282 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/docs/INSTALL.txt
+-rw-r--r--   0 zach       (501) staff       (20)      749 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/docs/LICENSE.txt
+-rw-r--r--   0 zach       (501) staff       (20)     1979 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/setup.py
+-rw-r--r--   0 zach       (501) staff       (20)      427 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/setup.cfg
+-rw-r--r--   0 zach       (501) staff       (20)      211 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/README.rst
+-rw-r--r--   0 zach       (501) staff       (20)     2103 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/CHANGES.rst
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/
+-rw-r--r--   0 zach       (501) staff       (20)     4346 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (501) staff       (20)       16 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 zach       (501) staff       (20)     3159 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (501) staff       (20)       82 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/entry_points.txt
+-rw-r--r--   0 zach       (501) staff       (20)      137 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/requires.txt
+-rw-r--r--   0 zach       (501) staff       (20)        6 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/top_level.txt
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone.mls.core.egg-info/dependency_links.txt
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/
+-rw-r--r--   0 zach       (501) staff       (20)       80 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/__init__.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/
+-rw-r--r--   0 zach       (501) staff       (20)     1764 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/interfaces.py
+-rw-r--r--   0 zach       (501) staff       (20)     1221 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/configure.zcml
+-rw-r--r--   0 zach       (501) staff       (20)      454 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/config.py
+-rw-r--r--   0 zach       (501) staff       (20)     2740 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles.zcml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/vi/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     3825 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/vi/LC_MESSAGES/plone.mls.core.po
+-rw-r--r--   0 zach       (501) staff       (20)     3801 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/plone.mls.core.pot
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ja/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     4289 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ja/LC_MESSAGES/plone.mls.core.po
+-rw-r--r--   0 zach       (501) staff       (20)      491 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/manual.pot
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/it/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/it/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     4879 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/it/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/zh_TW/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     3837 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/zh_TW/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ru/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     5680 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ru/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/cmn/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/cmn/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     3835 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/cmn/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/pt/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     4994 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/pt/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/zh/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/zh/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     4110 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/zh/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ar/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     3911 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/ar/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/de/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/de/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     4973 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/de/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/fr/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     5017 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/fr/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/es/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/es/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     4989 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/es/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/et/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/et/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     3830 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/et/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/en/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/en/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     3696 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/en/LC_MESSAGES/plone.mls.core.po
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/vi_VN/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 zach       (501) staff       (20)     3842 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/locales/vi_VN/LC_MESSAGES/plone.mls.core.po
+-rw-r--r--   0 zach       (501) staff       (20)      248 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/permissions.zcml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/tests/
+-rw-r--r--   0 zach       (501) staff       (20)     1702 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/tests/test_registry.py
+-rw-r--r--   0 zach       (501) staff       (20)     1063 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/tests/test_setup.py
+-rw-r--r--   0 zach       (501) staff       (20)       71 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/tests/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     1634 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/tests/test_controlpanel.py
+-rw-r--r--   0 zach       (501) staff       (20)      143 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     1146 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/setuphandlers.py
+-rw-r--r--   0 zach       (501) staff       (20)     2270 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/api.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/
+-rw-r--r--   0 zach       (501) staff       (20)      229 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/interfaces.py
+-rw-r--r--   0 zach       (501) staff       (20)     1595 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/configure.zcml
+-rw-r--r--   0 zach       (501) staff       (20)     3691 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/localconfig.py
+-rw-r--r--   0 zach       (501) staff       (20)      930 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/controlpanel.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/resources/
+-rw-r--r--   0 zach       (501) staff       (20)      889 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/resources/icon.png
+-rw-r--r--   0 zach       (501) staff       (20)      411 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/resources/plone_mls_core.js
+-rw-r--r--   0 zach       (501) staff       (20)       69 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/browser/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     2620 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/utils.py
+-rw-r--r--   0 zach       (501) staff       (20)      164 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/i18n.py
+-rw-r--r--   0 zach       (501) staff       (20)     4250 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/navigation.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/uninstall-base/
+-rw-r--r--   0 zach       (501) staff       (20)      317 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/uninstall-base/import_steps.xml
+-rw-r--r--   0 zach       (501) staff       (20)       51 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/uninstall-base/plone.mls.core_uninstall.txt
+-rw-r--r--   0 zach       (501) staff       (20)      299 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/uninstall-base/registry.xml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/uninstall-plone5/
+-rw-r--r--   0 zach       (501) staff       (20)      170 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/uninstall-plone5/metadata.xml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/uninstall-plone4/
+-rw-r--r--   0 zach       (501) staff       (20)      170 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/uninstall-plone4/metadata.xml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone5/
+-rw-r--r--   0 zach       (501) staff       (20)     2705 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone5/actions.xml
+-rw-r--r--   0 zach       (501) staff       (20)      109 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone5/registry.xml
+-rw-r--r--   0 zach       (501) staff       (20)      151 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone5/browserlayer.xml
+-rw-r--r--   0 zach       (501) staff       (20)      171 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone5/metadata.xml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone4/
+-rw-r--r--   0 zach       (501) staff       (20)     2705 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone4/actions.xml
+-rw-r--r--   0 zach       (501) staff       (20)      237 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone4/jsregistry.xml
+-rw-r--r--   0 zach       (501) staff       (20)      109 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone4/registry.xml
+-rw-r--r--   0 zach       (501) staff       (20)      151 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone4/browserlayer.xml
+-rw-r--r--   0 zach       (501) staff       (20)      171 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone4/metadata.xml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-08-04 08:55:51.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/base/
+-rw-r--r--   0 zach       (501) staff       (20)      167 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/profiles/base/metadata.xml
+-rw-r--r--   0 zach       (501) staff       (20)      877 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/testing.py
+-rw-r--r--   0 zach       (501) staff       (20)      462 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/core/migration.py
+-rw-r--r--   0 zach       (501) staff       (20)       80 2023-08-04 08:55:50.000000 plone.mls.core-0.7.1/src/plone/mls/__init__.py
```

### Comparing `plone.mls.core-0.7/CHANGES.rst` & `plone.mls.core-0.7.1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.7.1 (2023-08-04)
+------------------
+
+- Add a new optional setting for an override email address which would be used as the sender for all inquiries.
+
+
 0.7 (2017-12-12)
 ----------------
 
 - Add dependency to ps.plone.mls.
 - Remove controlpanel settings from GS profiles (now handled by ps.plone.mls).
```

### Comparing `plone.mls.core-0.7/docs/INSTALL.txt` & `plone.mls.core-0.7.1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/docs/LICENSE.GPL` & `plone.mls.core-0.7.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/docs/LICENSE.txt` & `plone.mls.core-0.7.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/PKG-INFO` & `plone.mls.core-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: plone.mls.core
-Version: 0.7
+Version: 0.7.1
 Summary: Plone support for the Propertyshelf MLS.
 Home-page: https://github.com/propertyshelf/plone.mls.core
 Author: Propertyshelf, Inc.
 Author-email: development@propertyshelf.com
 License: GPL
 Download-URL: http://pypi.python.org/pypi/plone.mls.core
-Description-Content-Type: UNKNOWN
 Description: Introduction
         ============
         
         .. image:: https://travis-ci.org/propertyshelf/plone.mls.core.png?branch=master
            :target: http://travis-ci.org/propertyshelf/plone.mls.core
         
         Plone support for the Propertyshelf MLS.
         
         Changelog
         =========
         
+        0.7.1 (2023-08-04)
+        ------------------
+        
+        - Add a new optional setting for an override email address which would be used as the sender for all inquiries.
+        
+        
         0.7 (2017-12-12)
         ----------------
         
         - Add dependency to ps.plone.mls.
         - Remove controlpanel settings from GS profiles (now handled by ps.plone.mls).
         
         
@@ -144,7 +149,8 @@
 Classifier: Framework :: Plone :: 5.0
 Classifier: Framework :: Plone :: 5.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
+Provides-Extra: test
```

### Comparing `plone.mls.core-0.7/setup.py` & `plone.mls.core-0.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """Setup for plone.mls.core package."""
 
 from setuptools import setup, find_packages
 
-version = '0.7'
+version = '0.7.1'
 description = "Plone support for the Propertyshelf MLS."
 long_description = ('\n'.join([
     open('README.rst').read(),
     open('CHANGES.rst').read(),
 ]))
 
 install_requires = [
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/api.py` & `plone.mls.core-0.7.1/src/plone/mls/core/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,11 +62,11 @@
         try:
             registry_settings = registry.forInterface(IMLSSettings)  # noqa
         except KeyError:
             logger.warning('Global MLS settings not available.')
         else:
             settings = dict([
                 (a, getattr(registry_settings, a)) for a in
-                registry_settings.__schema__]
+                registry_settings.__schema__],
             )
             logger.debug('Returning global MLS settings.')
     return settings
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/browser/configure.zcml` & `plone.mls.core-0.7.1/src/plone/mls/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/browser/controlpanel.py` & `plone.mls.core-0.7.1/src/plone/mls/core/browser/controlpanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """Global/default MLS Settings Form."""
 
     schema = IMLSSettings
     label = _(u'Propertyshelf MLS Settings')
     description = _(
         u'This MLS configuration will be used as the default for this '
         u'Plone site. You can add more MLS configurations by activating '
-        u'the local MLS settings on any content item within the site.'
+        u'the local MLS settings on any content item within the site.',
     )
 
     def updateFields(self):
         super(MLSSettingsEditForm, self).updateFields()
 
     def updateWidgets(self):
         super(MLSSettingsEditForm, self).updateWidgets()
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/browser/localconfig.py` & `plone.mls.core-0.7.1/src/plone/mls/core/browser/localconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class LocalMLSSettings(form.Form):
     """Local MLS Settings Form."""
 
     fields = field.Fields(IMLSSettings)
     label = _(u'Local Propertyshelf MLS Settings')
     description = _(
         u'This MLS configuration will be used for this content item and all '
-        u'possible child elements.'
+        u'possible child elements.',
     )
 
     def getContent(self):
         """Get the annotations with the local MLS config."""
         annotations = IAnnotations(self.context)
         return annotations.get(
             CONFIGURATION_KEY,
@@ -81,23 +81,23 @@
     def __call__(self):
         """Perform the toggle."""
         msg_type = 'info'
 
         if ILocalMLSSettings.providedBy(self.context):
             # Deactivate local MLS settings.
             noLongerProvides(self.context, ILocalMLSSettings)
-            self.context.reindexObject(idxs=['object_provides', ])
+            self.context.reindexObject(idxs=['object_provides'])
             msg = _(u'Local MLS settings deactivated.')
         elif IPossibleLocalMLSSettings.providedBy(self.context):
             alsoProvides(self.context, ILocalMLSSettings)
-            self.context.reindexObject(idxs=['object_provides', ])
+            self.context.reindexObject(idxs=['object_provides'])
             msg = _(u'Local MLS settings activated.')
         else:
             msg = _(
                 u'The local MLS settings don\'t work with this '
                 u'content type. Add \'IPossibleLocalMLSSettings\' to the '
-                u'provided interfaces to enable this feature.'
+                u'provided interfaces to enable this feature.',
             )
             msg_type = 'error'
 
         self.context.plone_utils.addPortalMessage(msg, msg_type)
         self.request.response.redirect(self.context.absolute_url())
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/browser/resources/icon.png` & `plone.mls.core-0.7.1/src/plone/mls/core/browser/resources/icon.png`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/configure.zcml` & `plone.mls.core-0.7.1/src/plone/mls/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/ar/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/zh/LC_MESSAGES/plone.mls.core.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
+# Translators:
+# Thomas Massmann <thomas.massmann@it-spir.it>, 2020
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Arabic (http://www.transifex.com/propertyshelf/MLS_Plone/language/ar/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>, 2020\n"
+"Language-Team: Chinese (https://www.transifex.com/propertyshelf/teams/13797/zh/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
-"Language: ar\n"
+"Language: zh\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "Preferred-Encodings: utf-8 latin1\n"
 
 #: plone/mls/core/profiles.zcml:56
 msgid "A Plone 4 uninstall profile for plone.mls.core."
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:66
@@ -34,19 +37,19 @@
 #: plone/mls/core/profiles/plone4/actions.xml
 #: plone/mls/core/profiles/plone5/actions.xml
 msgid "Activate the local MLS configuration."
 msgstr ""
 
 #: plone/mls/core/interfaces.py:34
 msgid "Agency ID"
-msgstr ""
+msgstr "房仲公司編碼"
 
 #: plone/mls/core/browser/localconfig.py:52
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
 #: plone/mls/core/profiles/plone4/actions.xml
 #: plone/mls/core/profiles/plone5/actions.xml
 msgid "Deactivate local MLS settings"
 msgstr ""
 
 #: plone/mls/core/profiles/plone4/actions.xml
@@ -69,24 +72,24 @@
 
 #: plone/mls/core/browser/localconfig.py:27
 msgid "Local Propertyshelf MLS Settings"
 msgstr ""
 
 #: plone/mls/core/interfaces.py:22
 msgid "MLS API Key"
-msgstr ""
+msgstr "房地產物件搜尋系統API鎖"
 
 #: plone/mls/core/profiles/plone4/controlpanel.xml
 #: plone/mls/core/profiles/plone5/controlpanel.xml
 msgid "MLS Base Settings"
 msgstr ""
 
 #: plone/mls/core/interfaces.py:28
 msgid "MLS URL"
-msgstr ""
+msgstr "房地產物件系統URL網址"
 
 #: plone/mls/core/profiles/plone4/actions.xml
 #: plone/mls/core/profiles/plone5/actions.xml
 msgid "Manage the local MLS settings."
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:27
@@ -95,19 +98,19 @@
 
 #: plone/mls/core/profiles.zcml:37
 msgid "Plone 5 support for the Propertyshelf MLS."
 msgstr ""
 
 #: plone/mls/core/browser/controlpanel.py:16
 msgid "Propertyshelf MLS Settings"
-msgstr ""
+msgstr "Propertyshelf 房地產物件搜尋系統(MLS)設定"
 
 #: plone/mls/core/browser/localconfig.py:41
 msgid "Save"
-msgstr ""
+msgstr "保存"
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
 "The local MLS settings don't work with this content type. Add "
 "'IPossibleLocalMLSSettings' to the provided interfaces to enable this "
 "feature."
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/cmn/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/ar/LC_MESSAGES/plone.mls.core.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Chinese (Mandarin) (http://www.transifex.com/propertyshelf/MLS_Plone/language/cmn/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Language-Team: Arabic (https://www.transifex.com/propertyshelf/teams/13797/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
-"Language: cmn\n"
+"Language: ar\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "Preferred-Encodings: utf-8 latin1\n"
 
 #: plone/mls/core/profiles.zcml:56
 msgid "A Plone 4 uninstall profile for plone.mls.core."
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:66
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/de/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/de/LC_MESSAGES/plone.mls.core.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
-# Thomas Massmann <thomas.massmann@it-spir.it>, 2012
-# Thomas Massmann <thomas.massmann@it-spir.it>, 2014
+# Translators:
+# Thomas Massmann <thomas.massmann@it-spir.it>, 2020
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: German (http://www.transifex.com/propertyshelf/MLS_Plone/language/de/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>, 2020\n"
+"Language-Team: German (https://www.transifex.com/propertyshelf/teams/13797/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
 "Language: de\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
@@ -108,28 +109,36 @@
 msgstr "Speichern"
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
 "The local MLS settings don't work with this content type. Add "
 "'IPossibleLocalMLSSettings' to the provided interfaces to enable this "
 "feature."
-msgstr "Die lokale MLS-Konfiguration konnte für diesen Inhaltstyp nicht aktiviert werden. Fügen Sie 'IPossibleLocalMLSSettings' zu den unterstützten Interfaces hinzu um dieses Feature zu aktivieren."
+msgstr ""
+"Die lokale MLS-Konfiguration konnte für diesen Inhaltstyp nicht aktiviert "
+"werden. Fügen Sie 'IPossibleLocalMLSSettings' zu den unterstützten "
+"Interfaces hinzu um dieses Feature zu aktivieren."
 
 #: plone/mls/core/browser/controlpanel.py:17
 msgid ""
 "This MLS configuration will be used as the default for this Plone site. You "
 "can add more MLS configurations by activating the local MLS settings on any "
 "content item within the site."
-msgstr "Diese MLS-Konfiguration wird standardmäßig für diese Plone Site verwendet. Es können weitere MLS-Konfigurationen hinzugefügt werden, indem für die jeweiligen Inhaltselemente die lokale Konfiguration aktiviert wird."
+msgstr ""
+"Diese MLS-Konfiguration wird standardmäßig für diese Plone Site verwendet. "
+"Es können weitere MLS-Konfigurationen hinzugefügt werden, indem für die "
+"jeweiligen Inhaltselemente die lokale Konfiguration aktiviert wird."
 
 #: plone/mls/core/browser/localconfig.py:28
 msgid ""
 "This MLS configuration will be used for this content item and all possible "
 "child elements."
-msgstr "Diese MLS-Konfiguration wird hier und in allen möglichen Unterelementen verwendet."
+msgstr ""
+"Diese MLS-Konfiguration wird hier und in allen möglichen Unterelementen "
+"verwendet."
 
 #: plone/mls/core/profiles.zcml:27
 msgid "plone.mls.core"
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:56
 msgid "plone.mls.core - uninstall"
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/en/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/en/LC_MESSAGES/plone.mls.core.po`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/es/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/es/LC_MESSAGES/plone.mls.core.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
-# Juan Salazar <juancarlos@propertyshelf.com>, 2012
-# Thomas Massmann <thomas.massmann@it-spir.it>, 2014
-# Valeria Garcia <valeriassimsou@gmail.com>, 2014
+# Translators:
+# Thomas Massmann <thomas.massmann@it-spir.it>, 2020
+# Valeria Garcia <valeriassimsou@gmail.com>, 2020
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Spanish (http://www.transifex.com/propertyshelf/MLS_Plone/language/es/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Last-Translator: Valeria Garcia <valeriassimsou@gmail.com>, 2020\n"
+"Language-Team: Spanish (https://www.transifex.com/propertyshelf/teams/13797/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
 "Language: es\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
@@ -109,28 +110,36 @@
 msgstr "Guardar"
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
 "The local MLS settings don't work with this content type. Add "
 "'IPossibleLocalMLSSettings' to the provided interfaces to enable this "
 "feature."
-msgstr "Los ajustes locales del MLS no funcionan con este tipo de contenido. Añadir 'IPossibleLocalMLSSettings' a las interfaces proporcionadas para activar esta función."
+msgstr ""
+"Los ajustes locales del MLS no funcionan con este tipo de contenido. Añadir "
+"'IPossibleLocalMLSSettings' a las interfaces proporcionadas para activar "
+"esta función."
 
 #: plone/mls/core/browser/controlpanel.py:17
 msgid ""
 "This MLS configuration will be used as the default for this Plone site. You "
 "can add more MLS configurations by activating the local MLS settings on any "
 "content item within the site."
-msgstr "Esta configuración MLS se utilizará como valor predeterminado para este sitio Plone. Puede añadir más conjuntos MLS activando la configuración local del MLS en cualquier tema dentro del sitio."
+msgstr ""
+"Esta configuración MLS se utilizará como valor predeterminado para este "
+"sitio Plone. Puede añadir más conjuntos MLS activando la configuración local"
+" del MLS en cualquier tema dentro del sitio."
 
 #: plone/mls/core/browser/localconfig.py:28
 msgid ""
 "This MLS configuration will be used for this content item and all possible "
 "child elements."
-msgstr "Esta configuración MLS será utilizado para este elemento de contenido y todos los posibles elementos secundarios."
+msgstr ""
+"Esta configuración MLS será utilizado para este elemento de contenido y "
+"todos los posibles elementos secundarios."
 
 #: plone/mls/core/profiles.zcml:27
 msgid "plone.mls.core"
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:56
 msgid "plone.mls.core - uninstall"
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/et/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/vi/LC_MESSAGES/plone.mls.core.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Estonian (http://www.transifex.com/propertyshelf/MLS_Plone/language/et/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Language-Team: Vietnamese (https://www.transifex.com/propertyshelf/teams/13797/vi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
-"Language: et\n"
+"Language: vi\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "Preferred-Encodings: utf-8 latin1\n"
 
 #: plone/mls/core/profiles.zcml:56
 msgid "A Plone 4 uninstall profile for plone.mls.core."
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:66
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/fr/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/fr/LC_MESSAGES/plone.mls.core.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
-# Anna-Lya Masson <masson@monde-immo.fr>, 2015
-# claudia.aubin <inactive+claudia.aubin@transifex.com>, 2014
-# Claudia Oberbeck <c.oberbeck@gmx.de>, 2013
-# Thomas Massmann <thomas.massmann@it-spir.it>, 2014
+# Translators:
+# Thomas Massmann <thomas.massmann@it-spir.it>, 2020
+# claudia.aubin <inactive+claudia.aubin@transifex.com>, 2020
+# Anna-Lya Masson <masson@monde-immo.fr>, 2020
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: French (http://www.transifex.com/propertyshelf/MLS_Plone/language/fr/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Last-Translator: Anna-Lya Masson <masson@monde-immo.fr>, 2020\n"
+"Language-Team: French (https://www.transifex.com/propertyshelf/teams/13797/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
 "Language: fr\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
@@ -110,28 +111,36 @@
 msgstr "Enregistrer"
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
 "The local MLS settings don't work with this content type. Add "
 "'IPossibleLocalMLSSettings' to the provided interfaces to enable this "
 "feature."
-msgstr "Les paramètres du MLS local ne fonctionnent pas avec ce type de contenu. Ajouter 'IPossibleLocalMLSSettings' aux interfaces fournies pour activer cette fonction."
+msgstr ""
+"Les paramètres du MLS local ne fonctionnent pas avec ce type de contenu. "
+"Ajouter 'IPossibleLocalMLSSettings' aux interfaces fournies pour activer "
+"cette fonction."
 
 #: plone/mls/core/browser/controlpanel.py:17
 msgid ""
 "This MLS configuration will be used as the default for this Plone site. You "
 "can add more MLS configurations by activating the local MLS settings on any "
 "content item within the site."
-msgstr "Cette configuration MLS sera utilisé comme valeur par défaut pour ce site Plone. Vous pouvez ajouter plus de configurations MLS en activant les paramètres du MLS local sur n'importe quel item à même le site."
+msgstr ""
+"Cette configuration MLS sera utilisé comme valeur par défaut pour ce site "
+"Plone. Vous pouvez ajouter plus de configurations MLS en activant les "
+"paramètres du MLS local sur n'importe quel item à même le site."
 
 #: plone/mls/core/browser/localconfig.py:28
 msgid ""
 "This MLS configuration will be used for this content item and all possible "
 "child elements."
-msgstr "Cette configuration MLS sera utilisée pour ce contenu et pour tous les sous éléments possible."
+msgstr ""
+"Cette configuration MLS sera utilisée pour ce contenu et pour tous les sous "
+"éléments possible."
 
 #: plone/mls/core/profiles.zcml:27
 msgid "plone.mls.core"
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:56
 msgid "plone.mls.core - uninstall"
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/it/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/it/LC_MESSAGES/plone.mls.core.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
-# Athanassios <a.karaiannis@gmail.com>, 2015
+# Translators:
+# Zach Cashero <zach@propertyshelf.com>, 2020
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Italian (http://www.transifex.com/propertyshelf/MLS_Plone/language/it/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Last-Translator: Zach Cashero <zach@propertyshelf.com>, 2020\n"
+"Language-Team: Italian (https://www.transifex.com/propertyshelf/teams/13797/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
 "Language: it\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
@@ -107,28 +109,36 @@
 msgstr "Salva"
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
 "The local MLS settings don't work with this content type. Add "
 "'IPossibleLocalMLSSettings' to the provided interfaces to enable this "
 "feature."
-msgstr "Le impostazioni del MLS locale non funzionano con questa tipologia di contenuto. Aggiungere 'IPossibleLocalMLSSettings' alle interfacce fornite per abilitare questa possibilità."
+msgstr ""
+"Le impostazioni del MLS locale non funzionano con questa tipologia di "
+"contenuto. Aggiungere 'IPossibleLocalMLSSettings' alle interfacce fornite "
+"per abilitare questa possibilità."
 
 #: plone/mls/core/browser/controlpanel.py:17
 msgid ""
 "This MLS configuration will be used as the default for this Plone site. You "
 "can add more MLS configurations by activating the local MLS settings on any "
 "content item within the site."
-msgstr "Questa configurazione MLS sarà usata come predefinita per questo sito Plone. E' possibile aggiungere più configurazioni MLS attivando le impostazioni del MLS locale su ogni elemento contenuto nel sito."
+msgstr ""
+"Questa configurazione MLS sarà usata come predefinita per questo sito Plone."
+" E' possibile aggiungere più configurazioni MLS attivando le impostazioni "
+"del MLS locale su ogni elemento contenuto nel sito."
 
 #: plone/mls/core/browser/localconfig.py:28
 msgid ""
 "This MLS configuration will be used for this content item and all possible "
 "child elements."
-msgstr "Questa configurazione MLS sarà usata per questo elemento del contenuto e per tutti gli elementi derivanti."
+msgstr ""
+"Questa configurazione MLS sarà usata per questo elemento del contenuto e per"
+" tutti gli elementi derivanti."
 
 #: plone/mls/core/profiles.zcml:27
 msgid "plone.mls.core"
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:56
 msgid "plone.mls.core - uninstall"
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/ja/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/ja/LC_MESSAGES/plone.mls.core.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
-# BryanAllen <bryan@propertyshelf.com>, 2013-2014
-# BryanAllen <bryan@propertyshelf.com>, 2012
-# Thomas Massmann <thomas.massmann@it-spir.it>, 2014
+# Translators:
+# Thomas Massmann <thomas.massmann@it-spir.it>, 2020
+# BryanAllen <bryan@propertyshelf.com>, 2020
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Japanese (http://www.transifex.com/propertyshelf/MLS_Plone/language/ja/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Last-Translator: BryanAllen <bryan@propertyshelf.com>, 2020\n"
+"Language-Team: Japanese (https://www.transifex.com/propertyshelf/teams/13797/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
 "Language: ja\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
@@ -109,15 +110,16 @@
 msgstr " セーブ"
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
 "The local MLS settings don't work with this content type. Add "
 "'IPossibleLocalMLSSettings' to the provided interfaces to enable this "
 "feature."
-msgstr "このMLS 設定: コンテンツタイプわ機能しない. 追加の 'IPossibleLocalMLSSettings'提供されたインターフェース"
+msgstr ""
+"このMLS 設定: コンテンツタイプわ機能しない. 追加の 'IPossibleLocalMLSSettings'提供されたインターフェース"
 
 #: plone/mls/core/browser/controlpanel.py:17
 msgid ""
 "This MLS configuration will be used as the default for this Plone site. You "
 "can add more MLS configurations by activating the local MLS settings on any "
 "content item within the site."
 msgstr ""
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/plone.mls.core.pot` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/plone.mls.core.pot`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/pt/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/pt/LC_MESSAGES/plone.mls.core.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
-# Valeria Garcia <valeriassimsou@gmail.com>, 2014
+# Translators:
+# Thomas Massmann <thomas.massmann@it-spir.it>, 2020
+# Valeria Garcia <valeriassimsou@gmail.com>, 2020
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Portuguese (http://www.transifex.com/propertyshelf/MLS_Plone/language/pt/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Last-Translator: Valeria Garcia <valeriassimsou@gmail.com>, 2020\n"
+"Language-Team: Portuguese (https://www.transifex.com/propertyshelf/teams/13797/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
 "Language: pt\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
@@ -35,15 +38,15 @@
 #: plone/mls/core/profiles/plone4/actions.xml
 #: plone/mls/core/profiles/plone5/actions.xml
 msgid "Activate the local MLS configuration."
 msgstr "Ativar as Configurações SLM Locais"
 
 #: plone/mls/core/interfaces.py:34
 msgid "Agency ID"
-msgstr "Indentidade do Agente"
+msgstr "Número de Indentificação da Agência"
 
 #: plone/mls/core/browser/localconfig.py:52
 msgid "Cancel"
 msgstr "Cancelar"
 
 #: plone/mls/core/profiles/plone4/actions.xml
 #: plone/mls/core/profiles/plone5/actions.xml
@@ -107,28 +110,36 @@
 msgstr "Salvar"
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
 "The local MLS settings don't work with this content type. Add "
 "'IPossibleLocalMLSSettings' to the provided interfaces to enable this "
 "feature."
-msgstr "As configurações locais so SLM não funcionão com este tipo de conteúdo. Adicione 'Possiveis Configurações SLM Locais' as interfaces fornecidas para ativar essa característica. "
+msgstr ""
+"As configurações locais so SLM não funcionão com este tipo de conteúdo. "
+"Adicione 'Possiveis Configurações SLM Locais' as interfaces fornecidas para "
+"ativar essa característica. "
 
 #: plone/mls/core/browser/controlpanel.py:17
 msgid ""
 "This MLS configuration will be used as the default for this Plone site. You "
 "can add more MLS configurations by activating the local MLS settings on any "
 "content item within the site."
-msgstr "Esta configuração SLM será utilizado como padrão para este site Plone. Você pode adicionar mais configurações SLM ativando as configurações locais SLM em qualquer item de conteúdo no site."
+msgstr ""
+"Esta configuração SLM será utilizado como padrão para este site Plone. Você "
+"pode adicionar mais configurações SLM ativando as configurações locais SLM "
+"em qualquer item de conteúdo no site."
 
 #: plone/mls/core/browser/localconfig.py:28
 msgid ""
 "This MLS configuration will be used for this content item and all possible "
 "child elements."
-msgstr "Esta configuração SLM será usado para este conteúdo e todos os possíveis elementos filhos."
+msgstr ""
+"Esta configuração SLM será usado para este conteúdo e todos os possíveis "
+"elementos filhos."
 
 #: plone/mls/core/profiles.zcml:27
 msgid "plone.mls.core"
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:56
 msgid "plone.mls.core - uninstall"
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/ru/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/ru/LC_MESSAGES/plone.mls.core.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
-# Olga Plavidal <oplavidal@gmail.com>, 2014
+# Translators:
+# Thomas Massmann <thomas.massmann@it-spir.it>, 2020
+# Olga Plavidal <oplavidal@gmail.com>, 2020
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Russian (http://www.transifex.com/propertyshelf/MLS_Plone/language/ru/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Last-Translator: Olga Plavidal <oplavidal@gmail.com>, 2020\n"
+"Language-Team: Russian (https://www.transifex.com/propertyshelf/teams/13797/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
 "Language: ru\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
@@ -107,28 +110,36 @@
 msgstr "Сохранить"
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
 "The local MLS settings don't work with this content type. Add "
 "'IPossibleLocalMLSSettings' to the provided interfaces to enable this "
 "feature."
-msgstr "Местные настройки MLS не работают с этим типом контента. Добавить \"IPossibleLocalMLSSettings\" в список предоставляемых интерфейсов для включения этой функции."
+msgstr ""
+"Местные настройки MLS не работают с этим типом контента. Добавить "
+"\"IPossibleLocalMLSSettings\" в список предоставляемых интерфейсов для "
+"включения этой функции."
 
 #: plone/mls/core/browser/controlpanel.py:17
 msgid ""
 "This MLS configuration will be used as the default for this Plone site. You "
 "can add more MLS configurations by activating the local MLS settings on any "
 "content item within the site."
-msgstr "Эта конфигурация MLS будет использоваться как дефолт для этого сайта Plone. Вы можете добавить несколько конфигураций MLS, активизируя локальные параметры MLS на любую тему в рамках сайта."
+msgstr ""
+"Эта конфигурация MLS будет использоваться как дефолт для этого сайта Plone. "
+"Вы можете добавить несколько конфигураций MLS, активизируя локальные "
+"параметры MLS на любую тему в рамках сайта."
 
 #: plone/mls/core/browser/localconfig.py:28
 msgid ""
 "This MLS configuration will be used for this content item and all possible "
 "child elements."
-msgstr "Эта конфигурация MLS будет использоваться для этого элемента контента и всех возможных дочерних элементов."
+msgstr ""
+"Эта конфигурация MLS будет использоваться для этого элемента контента и всех"
+" возможных дочерних элементов."
 
 #: plone/mls/core/profiles.zcml:27
 msgid "plone.mls.core"
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:56
 msgid "plone.mls.core - uninstall"
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/vi/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/zh_TW/LC_MESSAGES/plone.mls.core.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Vietnamese (http://www.transifex.com/propertyshelf/MLS_Plone/language/vi/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Language-Team: Chinese (Taiwan) (https://www.transifex.com/propertyshelf/teams/13797/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
-"Language: vi\n"
+"Language: zh_TW\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "Preferred-Encodings: utf-8 latin1\n"
 
 #: plone/mls/core/profiles.zcml:56
 msgid "A Plone 4 uninstall profile for plone.mls.core."
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/vi_VN/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/vi_VN/LC_MESSAGES/plone.mls.core.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Vietnamese (Viet Nam) (http://www.transifex.com/propertyshelf/MLS_Plone/language/vi_VN/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Language-Team: Vietnamese (Viet Nam) (https://www.transifex.com/propertyshelf/teams/13797/vi_VN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
 "Language: vi_VN\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/zh/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/cmn/LC_MESSAGES/plone.mls.core.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
-# yuhaha <meiyu@propertyshelf.com>, 2012
-# Thomas Massmann <thomas.massmann@it-spir.it>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Chinese (http://www.transifex.com/propertyshelf/MLS_Plone/language/zh/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Language-Team: Chinese (Mandarin) (https://www.transifex.com/propertyshelf/teams/13797/cmn/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
-"Language: zh\n"
+"Language: cmn\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "Preferred-Encodings: utf-8 latin1\n"
 
 #: plone/mls/core/profiles.zcml:56
 msgid "A Plone 4 uninstall profile for plone.mls.core."
@@ -36,15 +33,15 @@
 #: plone/mls/core/profiles/plone4/actions.xml
 #: plone/mls/core/profiles/plone5/actions.xml
 msgid "Activate the local MLS configuration."
 msgstr ""
 
 #: plone/mls/core/interfaces.py:34
 msgid "Agency ID"
-msgstr "房仲公司編碼"
+msgstr ""
 
 #: plone/mls/core/browser/localconfig.py:52
 msgid "Cancel"
 msgstr ""
 
 #: plone/mls/core/profiles/plone4/actions.xml
 #: plone/mls/core/profiles/plone5/actions.xml
@@ -71,24 +68,24 @@
 
 #: plone/mls/core/browser/localconfig.py:27
 msgid "Local Propertyshelf MLS Settings"
 msgstr ""
 
 #: plone/mls/core/interfaces.py:22
 msgid "MLS API Key"
-msgstr "房地產物件搜尋系統API鎖"
+msgstr ""
 
 #: plone/mls/core/profiles/plone4/controlpanel.xml
 #: plone/mls/core/profiles/plone5/controlpanel.xml
 msgid "MLS Base Settings"
 msgstr ""
 
 #: plone/mls/core/interfaces.py:28
 msgid "MLS URL"
-msgstr "房地產物件系統URL網址"
+msgstr ""
 
 #: plone/mls/core/profiles/plone4/actions.xml
 #: plone/mls/core/profiles/plone5/actions.xml
 msgid "Manage the local MLS settings."
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:27
@@ -97,15 +94,15 @@
 
 #: plone/mls/core/profiles.zcml:37
 msgid "Plone 5 support for the Propertyshelf MLS."
 msgstr ""
 
 #: plone/mls/core/browser/controlpanel.py:16
 msgid "Propertyshelf MLS Settings"
-msgstr "Propertyshelf 房地產物件搜尋系統(MLS)設定"
+msgstr ""
 
 #: plone/mls/core/browser/localconfig.py:41
 msgid "Save"
 msgstr ""
 
 #: plone/mls/core/browser/localconfig.py:98
 msgid ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/locales/zh_TW/LC_MESSAGES/plone.mls.core.po` & `plone.mls.core-0.7.1/src/plone/mls/core/locales/et/LC_MESSAGES/plone.mls.core.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: MLS Plone Components\n"
 "POT-Creation-Date: 2017-08-21 10:09+0000\n"
-"PO-Revision-Date: 2017-08-21 10:10+0000\n"
-"Last-Translator: Thomas Massmann <thomas.massmann@it-spir.it>\n"
-"Language-Team: Chinese (Taiwan) (http://www.transifex.com/propertyshelf/MLS_Plone/language/zh_TW/)\n"
+"PO-Revision-Date: 2020-05-14 16:28+0000\n"
+"Language-Team: Estonian (https://www.transifex.com/propertyshelf/teams/13797/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Domain: plone.mls.core\n"
-"Language: zh_TW\n"
+"Language: et\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "Preferred-Encodings: utf-8 latin1\n"
 
 #: plone/mls/core/profiles.zcml:56
 msgid "A Plone 4 uninstall profile for plone.mls.core."
 msgstr ""
 
 #: plone/mls/core/profiles.zcml:66
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/navigation.py` & `plone.mls.core-0.7.1/src/plone/mls/core/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/profiles/plone4/actions.xml` & `plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone5/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/profiles/plone5/actions.xml` & `plone.mls.core-0.7.1/src/plone/mls/core/profiles/plone4/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/profiles.zcml` & `plone.mls.core-0.7.1/src/plone/mls/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/setuphandlers.py` & `plone.mls.core-0.7.1/src/plone/mls/core/setuphandlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """Additional setup steps."""
 
 from logging import getLogger
 from plone.browserlayer import utils as layerutils
+from plone.mls.core import PLONE_4
 from plone.mls.core.browser.interfaces import IMLSSpecific
 from Products.CMFPlone.interfaces import INonInstallable
 from zope.interface import implementer
 
 
 logger = getLogger('plone.mls.core')
 
@@ -23,13 +24,17 @@
 
 
 @implementer(INonInstallable)
 class HiddenProfiles(object):
 
     def getNonInstallableProfiles(self):
         """Hide uninstall profile from site-creation and quickinstaller."""
-        return [
-            'plone.mls.core:default',
+        items = [
             'plone.mls.core:install-base',
             'plone.mls.core:uninstall',
             'plone.mls.core:uninstall-base',
         ]
+
+        if not PLONE_4:
+            items.append('plone.mls.core:default')
+
+        return items
```

### Comparing `plone.mls.core-0.7/src/plone/mls/core/testing.py` & `plone.mls.core-0.7.1/src/plone/mls/core/testing.py`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/tests/test_controlpanel.py` & `plone.mls.core-0.7.1/src/plone/mls/core/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/tests/test_registry.py` & `plone.mls.core-0.7.1/src/plone/mls/core/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/tests/test_setup.py` & `plone.mls.core-0.7.1/src/plone/mls/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone/mls/core/utils.py` & `plone.mls.core-0.7.1/src/plone/mls/core/utils.py`

 * *Files identical despite different names*

### Comparing `plone.mls.core-0.7/src/plone.mls.core.egg-info/PKG-INFO` & `plone.mls.core-0.7.1/src/plone.mls.core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: plone.mls.core
-Version: 0.7
+Version: 0.7.1
 Summary: Plone support for the Propertyshelf MLS.
 Home-page: https://github.com/propertyshelf/plone.mls.core
 Author: Propertyshelf, Inc.
 Author-email: development@propertyshelf.com
 License: GPL
 Download-URL: http://pypi.python.org/pypi/plone.mls.core
-Description-Content-Type: UNKNOWN
 Description: Introduction
         ============
         
         .. image:: https://travis-ci.org/propertyshelf/plone.mls.core.png?branch=master
            :target: http://travis-ci.org/propertyshelf/plone.mls.core
         
         Plone support for the Propertyshelf MLS.
         
         Changelog
         =========
         
+        0.7.1 (2023-08-04)
+        ------------------
+        
+        - Add a new optional setting for an override email address which would be used as the sender for all inquiries.
+        
+        
         0.7 (2017-12-12)
         ----------------
         
         - Add dependency to ps.plone.mls.
         - Remove controlpanel settings from GS profiles (now handled by ps.plone.mls).
         
         
@@ -144,7 +149,8 @@
 Classifier: Framework :: Plone :: 5.0
 Classifier: Framework :: Plone :: 5.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
+Provides-Extra: test
```

### Comparing `plone.mls.core-0.7/src/plone.mls.core.egg-info/SOURCES.txt` & `plone.mls.core-0.7.1/src/plone.mls.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

