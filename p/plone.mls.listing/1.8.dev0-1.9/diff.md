# Comparing `tmp/plone.mls.listing-1.8.dev0.tar.gz` & `tmp/plone.mls.listing-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.mls.listing-1.8.dev0.tar", last modified: Mon Oct 17 12:20:39 2016, max compression
+gzip compressed data, was "dist/plone.mls.listing-1.9.tar", last modified: Tue Apr  4 15:07:48 2017, max compression
```

## Comparing `plone.mls.listing-1.8.dev0.tar` & `plone.mls.listing-1.9.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/
--rw-r--r--   0 thomas     (501) staff       (20)     9666 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/CHANGES.rst
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/docs/
--rw-r--r--   0 thomas     (501) staff       (20)     1306 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/docs/INSTALL.txt
--rw-r--r--   0 thomas     (501) staff       (20)     2115 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/docs/LICENSE.txt
--rw-r--r--   0 thomas     (501) staff       (20)      107 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/MANIFEST.in
--rw-r--r--   0 thomas     (501) staff       (20)    14979 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      754 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/README.rst
--rw-r--r--   0 thomas     (501) staff       (20)       95 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)     2345 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/
--rw-r--r--   0 thomas     (501) staff       (20)      244 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/
--rw-r--r--   0 thomas     (501) staff       (20)      244 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/
--rw-r--r--   0 thomas     (501) staff       (20)      208 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     9928 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/api.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/
--rw-r--r--   0 thomas     (501) staff       (20)       60 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      946 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/adapters.py
--rw-r--r--   0 thomas     (501) staff       (20)      967 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)      297 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/interfaces.py
--rw-r--r--   0 thomas     (501) staff       (20)     4574 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/listing.pt
--rw-r--r--   0 thomas     (501) staff       (20)     3256 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/listing.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/backports/
--rw-r--r--   0 thomas     (501) staff       (20)      145 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/backports/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      717 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/backports/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)     1389 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/backports/utils.py
--rw-r--r--   0 thomas     (501) staff       (20)     3070 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/backports/viewlets.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/
--rw-r--r--   0 thomas     (501) staff       (20)       72 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      926 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/adapter.py
--rw-r--r--   0 thomas     (501) staff       (20)     8600 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)     2231 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/controlpanel.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/
--rwxr-xr-x   0 thomas     (501) staff       (20)      944 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/apartment.png
--rwxr-xr-x   0 thomas     (501) staff       (20)     1129 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/condominium.png
--rwxr-xr-x   0 thomas     (501) staff       (20)     1164 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/house.png
--rw-r--r--   0 thomas     (501) staff       (20)     1638 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/icon_talk.png
--rw-r--r--   0 thomas     (501) staff       (20)     1222 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/no-image.png
--rwxr-xr-x   0 thomas     (501) staff       (20)      833 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/office-building.png
--rw-r--r--   0 thomas     (501) staff       (20)     1755 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/quotation_left.png
--rw-r--r--   0 thomas     (501) staff       (20)     1752 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/quotation_right.png
--rwxr-xr-x   0 thomas     (501) staff       (20)      806 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/townhouse.png
--rw-r--r--   0 thomas     (501) staff       (20)      459 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/interfaces.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/
--rw-r--r--   0 thomas     (501) staff       (20)     1456 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/classic-loader.gif
--rw-r--r--   0 thomas     (501) staff       (20)     1012 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/classic-map.png
--rw-r--r--   0 thomas     (501) staff       (20)     4250 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/galleria.classic.css
--rw-r--r--   0 thomas     (501) staff       (20)     2531 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/galleria.classic.js
--rwxr-xr-x   0 thomas     (501) staff       (20)     1387 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/galleria.classic.min.js
--rw-r--r--   0 thomas     (501) staff       (20)   119582 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/galleria-1.2.2.js
--rwxr-xr-x   0 thomas     (501) staff       (20)     4220 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/jquery.ias.min.js
--rw-r--r--   0 thomas     (501) staff       (20)     4515 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/listing.js
--rw-r--r--   0 thomas     (501) staff       (20)      855 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/listing_ias.js
--rw-r--r--   0 thomas     (501) staff       (20)    11688 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/listing_collection.py
--rw-r--r--   0 thomas     (501) staff       (20)    17787 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/listing_search.py
--rw-r--r--   0 thomas     (501) staff       (20)     3682 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/localconfig.py
--rw-r--r--   0 thomas     (501) staff       (20)      829 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/navigation.py
--rw-r--r--   0 thomas     (501) staff       (20)     7617 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/recent_listings.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/stylesheets/
--rw-r--r--   0 thomas     (501) staff       (20)     5691 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/stylesheets/main.css
--rw-r--r--   0 thomas     (501) staff       (20)     1064 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/stylesheets/print.css
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/
--rw-r--r--   0 thomas     (501) staff       (20)       64 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     1101 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)      223 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/interfaces.py
--rw-r--r--   0 thomas     (501) staff       (20)      973 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/tc_display.pt
--rw-r--r--   0 thomas     (501) staff       (20)      492 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/tc_hidden.pt
--rw-r--r--   0 thomas     (501) staff       (20)     3803 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/tc_input.pt
--rw-r--r--   0 thomas     (501) staff       (20)     1628 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/tcwidgetwrapper.pt
--rw-r--r--   0 thomas     (501) staff       (20)     1660 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/widget.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/
--rw-r--r--   0 thomas     (501) staff       (20)     6360 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/listing_collection_viewlet.pt
--rw-r--r--   0 thomas     (501) staff       (20)    12621 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/listing_details.pt
--rw-r--r--   0 thomas     (501) staff       (20)     7241 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/listing_search_viewlet.pt
--rw-r--r--   0 thomas     (501) staff       (20)     9666 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/print_listing_details.pt
--rw-r--r--   0 thomas     (501) staff       (20)     6274 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/recent_listings_viewlet.pt
--rw-r--r--   0 thomas     (501) staff       (20)     3436 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/search_form.pt
--rw-r--r--   0 thomas     (501) staff       (20)     2403 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/traversal.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/
--rw-r--r--   0 thomas     (501) staff       (20)       68 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      921 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)      201 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/interfaces.py
--rw-r--r--   0 thomas     (501) staff       (20)     1248 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/valuerange_display.pt
--rw-r--r--   0 thomas     (501) staff       (20)      809 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/valuerange_hidden.pt
--rw-r--r--   0 thomas     (501) staff       (20)     3358 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/valuerange_input.pt
--rw-r--r--   0 thomas     (501) staff       (20)     4410 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/widget.py
--rw-r--r--   0 thomas     (501) staff       (20)    14883 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/views.py
--rw-r--r--   0 thomas     (501) staff       (20)     3566 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/configure.zcml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/content/
--rw-r--r--   0 thomas     (501) staff       (20)       79 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/content/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      233 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/content/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)      399 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/content/listing.py
--rw-r--r--   0 thomas     (501) staff       (20)      165 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/i18n.py
--rw-r--r--   0 thomas     (501) staff       (20)     8340 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/interfaces.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ar/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ar/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    24614 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ar/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/cmn/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/cmn/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    24538 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/cmn/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/de/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/de/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    33795 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/de/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/en/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/en/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    24183 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/en/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/es/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/es/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    34066 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/es/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/et/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/et/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    24533 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/et/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/fr/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/fr/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    30343 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/fr/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/it/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/it/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    30908 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/it/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ja/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ja/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    29385 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ja/LC_MESSAGES/plone.mls.listing.po
--rw-r--r--   0 thomas     (501) staff       (20)      497 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/manual.pot
--rw-r--r--   0 thomas     (501) staff       (20)    24291 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/plone.mls.listing.pot
--rw-r--r--   0 thomas     (501) staff       (20)      597 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/plone.pot
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/pt/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/pt/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    30976 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/pt/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ru/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ru/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    36058 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ru/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/vi/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/vi/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    24528 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/vi/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/vi_VN/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/vi_VN/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    24545 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/vi_VN/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/zh/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/zh/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    26180 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/zh/LC_MESSAGES/plone.mls.listing.po
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/zh_TW/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 thomas     (501) staff       (20)    24540 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/zh_TW/LC_MESSAGES/plone.mls.listing.po
--rw-r--r--   0 thomas     (501) staff       (20)    12973 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/migration.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/
--rw-r--r--   0 thomas     (501) staff       (20)       62 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)    19742 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/agent_contact.py
--rw-r--r--   0 thomas     (501) staff       (20)     3159 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/agent_information.py
--rw-r--r--   0 thomas     (501) staff       (20)     1368 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/configure.zcml
--rw-r--r--   0 thomas     (501) staff       (20)    11314 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/quick_search.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/
--rw-r--r--   0 thomas     (501) staff       (20)     1459 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/agent_contact.pt
--rw-r--r--   0 thomas     (501) staff       (20)     4637 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/agent_information.pt
--rw-r--r--   0 thomas     (501) staff       (20)      699 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/quick_search.pt
--rw-r--r--   0 thomas     (501) staff       (20)     4912 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/search_form.pt
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/
--rw-r--r--   0 thomas     (501) staff       (20)     9975 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/actions.xml
--rw-r--r--   0 thomas     (501) staff       (20)      161 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/browserlayer.xml
--rw-r--r--   0 thomas     (501) staff       (20)     1146 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/controlpanel.xml
--rw-r--r--   0 thomas     (501) staff       (20)      337 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/cssregistry.xml
--rw-r--r--   0 thomas     (501) staff       (20)      694 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/jsregistry.xml
--rw-r--r--   0 thomas     (501) staff       (20)      299 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/metadata.xml
--rw-r--r--   0 thomas     (501) staff       (20)       36 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/plone.mls.listing_various.txt
--rw-r--r--   0 thomas     (501) staff       (20)      525 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/portlets.xml
--rw-r--r--   0 thomas     (501) staff       (20)      277 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/registry.xml
--rw-r--r--   0 thomas     (501) staff       (20)      226 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/repositorytool.xml
--rw-r--r--   0 thomas     (501) staff       (20)      175 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/tinymce.xml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/types/
--rw-r--r--   0 thomas     (501) staff       (20)     2507 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/types/plone.mls.listing.listing.xml
--rw-r--r--   0 thomas     (501) staff       (20)      133 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/types.xml
--rw-r--r--   0 thomas     (501) staff       (20)      258 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/viewlets.xml
--rw-r--r--   0 thomas     (501) staff       (20)     5448 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles.zcml
--rw-r--r--   0 thomas     (501) staff       (20)     1603 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/setuphandlers.py
--rw-r--r--   0 thomas     (501) staff       (20)      943 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/testing.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/
--rw-r--r--   0 thomas     (501) staff       (20)       74 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      764 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_content.py
--rw-r--r--   0 thomas     (501) staff       (20)     6191 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_portlet_agent_contact.py
--rw-r--r--   0 thomas     (501) staff       (20)     4025 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_portlet_agent_information.py
--rw-r--r--   0 thomas     (501) staff       (20)     3970 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_portlet_quick_search.py
--rw-r--r--   0 thomas     (501) staff       (20)     1846 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_setup.py
--rw-r--r--   0 thomas     (501) staff       (20)    10221 2016-10-17 12:20:38.000000 plone.mls.listing-1.8.dev0/src/plone/mls/listing/vocabularies.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)        1 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       82 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/entry_points.txt
--rw-r--r--   0 thomas     (501) staff       (20)       16 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/namespace_packages.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/not-zip-safe
--rw-r--r--   0 thomas     (501) staff       (20)    14979 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      306 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)     6984 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        6 2016-10-17 12:20:39.000000 plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/
+-rw-r--r--   0 thomas     (501) staff       (20)     9889 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/CHANGES.rst
+-rw-r--r--   0 thomas     (501) staff       (20)       83 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/CONTRIBUTORS.rst
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/docs/
+-rw-r--r--   0 thomas     (501) staff       (20)     1306 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/docs/INSTALL.txt
+-rw-r--r--   0 thomas     (501) staff       (20)     2115 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/docs/LICENSE.txt
+-rw-r--r--   0 thomas     (501) staff       (20)      132 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/MANIFEST.in
+-rw-r--r--   0 thomas     (501) staff       (20)    15341 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      754 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/README.rst
+-rw-r--r--   0 thomas     (501) staff       (20)      290 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)     2340 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/
+-rw-r--r--   0 thomas     (501) staff       (20)      244 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/
+-rw-r--r--   0 thomas     (501) staff       (20)      244 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/
+-rw-r--r--   0 thomas     (501) staff       (20)      208 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9928 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/api.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/article/
+-rw-r--r--   0 thomas     (501) staff       (20)       60 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/article/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      946 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/article/adapters.py
+-rw-r--r--   0 thomas     (501) staff       (20)      967 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/article/configure.zcml
+-rw-r--r--   0 thomas     (501) staff       (20)      297 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/article/interfaces.py
+-rw-r--r--   0 thomas     (501) staff       (20)     4574 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/article/listing.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     3256 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/article/listing.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/backports/
+-rw-r--r--   0 thomas     (501) staff       (20)      145 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/backports/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      717 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/backports/configure.zcml
+-rw-r--r--   0 thomas     (501) staff       (20)     1389 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/backports/utils.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3070 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/backports/viewlets.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/
+-rw-r--r--   0 thomas     (501) staff       (20)       72 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      926 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/adapter.py
+-rw-r--r--   0 thomas     (501) staff       (20)     8600 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/configure.zcml
+-rw-r--r--   0 thomas     (501) staff       (20)     2231 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/controlpanel.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/
+-rwxr-xr-x   0 thomas     (501) staff       (20)      944 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/apartment.png
+-rwxr-xr-x   0 thomas     (501) staff       (20)     1129 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/condominium.png
+-rwxr-xr-x   0 thomas     (501) staff       (20)     1164 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/house.png
+-rw-r--r--   0 thomas     (501) staff       (20)     1638 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/icon_talk.png
+-rw-r--r--   0 thomas     (501) staff       (20)     1222 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/no-image.png
+-rwxr-xr-x   0 thomas     (501) staff       (20)      833 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/office-building.png
+-rw-r--r--   0 thomas     (501) staff       (20)     1755 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/quotation_left.png
+-rw-r--r--   0 thomas     (501) staff       (20)     1752 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/quotation_right.png
+-rwxr-xr-x   0 thomas     (501) staff       (20)      806 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/images/townhouse.png
+-rw-r--r--   0 thomas     (501) staff       (20)      459 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/interfaces.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/
+-rw-r--r--   0 thomas     (501) staff       (20)     1456 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/classic-loader.gif
+-rw-r--r--   0 thomas     (501) staff       (20)     1012 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/classic-map.png
+-rw-r--r--   0 thomas     (501) staff       (20)     4250 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/galleria.classic.css
+-rw-r--r--   0 thomas     (501) staff       (20)     2531 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/galleria.classic.js
+-rwxr-xr-x   0 thomas     (501) staff       (20)     1387 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/galleria.classic.min.js
+-rw-r--r--   0 thomas     (501) staff       (20)   119582 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/galleria-1.2.2.js
+-rwxr-xr-x   0 thomas     (501) staff       (20)     4220 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/jquery.ias.min.js
+-rw-r--r--   0 thomas     (501) staff       (20)     4515 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/listing.js
+-rw-r--r--   0 thomas     (501) staff       (20)      855 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/listing_ias.js
+-rw-r--r--   0 thomas     (501) staff       (20)    11688 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/listing_collection.py
+-rw-r--r--   0 thomas     (501) staff       (20)    17787 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/listing_search.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3682 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/localconfig.py
+-rw-r--r--   0 thomas     (501) staff       (20)      829 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/navigation.py
+-rw-r--r--   0 thomas     (501) staff       (20)     7617 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/recent_listings.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/stylesheets/
+-rw-r--r--   0 thomas     (501) staff       (20)     5710 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/stylesheets/main.css
+-rw-r--r--   0 thomas     (501) staff       (20)     1084 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/stylesheets/print.css
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/
+-rw-r--r--   0 thomas     (501) staff       (20)       64 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1101 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/configure.zcml
+-rw-r--r--   0 thomas     (501) staff       (20)      223 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/interfaces.py
+-rw-r--r--   0 thomas     (501) staff       (20)      973 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/tc_display.pt
+-rw-r--r--   0 thomas     (501) staff       (20)      492 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/tc_hidden.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     3803 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/tc_input.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     1628 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/tcwidgetwrapper.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     1660 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/widget.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/
+-rw-r--r--   0 thomas     (501) staff       (20)     6360 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/listing_collection_viewlet.pt
+-rw-r--r--   0 thomas     (501) staff       (20)    12621 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/listing_details.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     7241 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/listing_search_viewlet.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     9666 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/print_listing_details.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     6274 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/recent_listings_viewlet.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     3436 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/search_form.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     2403 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/traversal.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/
+-rw-r--r--   0 thomas     (501) staff       (20)       68 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      921 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/configure.zcml
+-rw-r--r--   0 thomas     (501) staff       (20)      201 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/interfaces.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1248 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/valuerange_display.pt
+-rw-r--r--   0 thomas     (501) staff       (20)      809 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/valuerange_hidden.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     3358 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/valuerange_input.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     4410 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/widget.py
+-rw-r--r--   0 thomas     (501) staff       (20)    14883 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/browser/views.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3566 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/configure.zcml
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/content/
+-rw-r--r--   0 thomas     (501) staff       (20)       79 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/content/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      233 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/content/configure.zcml
+-rw-r--r--   0 thomas     (501) staff       (20)      399 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/content/listing.py
+-rw-r--r--   0 thomas     (501) staff       (20)      165 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/i18n.py
+-rw-r--r--   0 thomas     (501) staff       (20)     8340 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/interfaces.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ar/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    24614 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ar/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/cmn/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/cmn/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    24538 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/cmn/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/de/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/de/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    33795 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/de/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/en/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/en/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    24183 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/en/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/es/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/es/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    34066 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/es/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/et/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/et/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    24533 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/et/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/fr/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    30343 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/fr/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/it/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/it/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    30908 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/it/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ja/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    29385 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ja/LC_MESSAGES/plone.mls.listing.po
+-rw-r--r--   0 thomas     (501) staff       (20)      497 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/manual.pot
+-rw-r--r--   0 thomas     (501) staff       (20)    24291 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/plone.mls.listing.pot
+-rw-r--r--   0 thomas     (501) staff       (20)      597 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/plone.pot
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/pt/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    30976 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/pt/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ru/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    36058 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/ru/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/vi/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    24528 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/vi/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/vi_VN/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    24545 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/vi_VN/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/zh/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/zh/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    26180 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/zh/LC_MESSAGES/plone.mls.listing.po
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/zh_TW/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 thomas     (501) staff       (20)    24540 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/locales/zh_TW/LC_MESSAGES/plone.mls.listing.po
+-rw-r--r--   0 thomas     (501) staff       (20)    12973 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/migration.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/
+-rw-r--r--   0 thomas     (501) staff       (20)       62 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)    19699 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/agent_contact.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3159 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/agent_information.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1368 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/configure.zcml
+-rw-r--r--   0 thomas     (501) staff       (20)    11314 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/quick_search.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/
+-rw-r--r--   0 thomas     (501) staff       (20)     1459 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/agent_contact.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     4637 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/agent_information.pt
+-rw-r--r--   0 thomas     (501) staff       (20)      699 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/quick_search.pt
+-rw-r--r--   0 thomas     (501) staff       (20)     4912 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/search_form.pt
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/
+-rw-r--r--   0 thomas     (501) staff       (20)     9975 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/actions.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      161 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/browserlayer.xml
+-rw-r--r--   0 thomas     (501) staff       (20)     1146 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/controlpanel.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      337 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/cssregistry.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      694 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/jsregistry.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      299 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/metadata.xml
+-rw-r--r--   0 thomas     (501) staff       (20)       36 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/plone.mls.listing_various.txt
+-rw-r--r--   0 thomas     (501) staff       (20)      525 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/portlets.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      277 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/registry.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      226 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/repositorytool.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      175 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/tinymce.xml
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/types/
+-rw-r--r--   0 thomas     (501) staff       (20)     2507 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/types/plone.mls.listing.listing.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      133 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/types.xml
+-rw-r--r--   0 thomas     (501) staff       (20)      258 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/viewlets.xml
+-rw-r--r--   0 thomas     (501) staff       (20)     5448 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/profiles.zcml
+-rw-r--r--   0 thomas     (501) staff       (20)     1603 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/setuphandlers.py
+-rw-r--r--   0 thomas     (501) staff       (20)      943 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/testing.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone/mls/listing/tests/
+-rw-r--r--   0 thomas     (501) staff       (20)       74 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/tests/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      764 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/tests/test_content.py
+-rw-r--r--   0 thomas     (501) staff       (20)     6191 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/tests/test_portlet_agent_contact.py
+-rw-r--r--   0 thomas     (501) staff       (20)     4025 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/tests/test_portlet_agent_information.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3970 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/tests/test_portlet_quick_search.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1846 2017-04-04 15:07:46.000000 plone.mls.listing-1.9/src/plone/mls/listing/tests/test_setup.py
+-rw-r--r--   0 thomas     (501) staff       (20)    10221 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone/mls/listing/vocabularies.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2017-04-04 15:07:48.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       82 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/entry_points.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       16 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/namespace_packages.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/not-zip-safe
+-rw-r--r--   0 thomas     (501) staff       (20)    15341 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      306 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)     7001 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        6 2017-04-04 15:07:47.000000 plone.mls.listing-1.9/src/plone.mls.listing.egg-info/top_level.txt
```

### Comparing `plone.mls.listing-1.8.dev0/CHANGES.rst` & `plone.mls.listing-1.9/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 Changelog
 =========
 
-1.8 (unreleased)
+1.9 (2017-04-04)
+----------------
+
+- In agent contact form, use sender for email 'from', instead of 'reply-to'.
+
+
+1.8.2 (2016-11-07)
+------------------
+
+- Fix CSS.
+
+
+1.8.1 (2016-10-17)
+------------------
+
+- Fix manifest.
+
+
+1.8 (2016-10-17)
 ----------------
 
 - Add single beds and baths for listings (hidden with CSS by default).
 - Use high resolution lead image for listing collections, if available.
 - Add listing description for listing collections (hidden with CSS by default).
 - Add calculated price for listings (hidden with CSS by default).
 - Remove colons after labels from listing templates (now added via CSS).
```

### Comparing `plone.mls.listing-1.8.dev0/docs/INSTALL.txt` & `plone.mls.listing-1.9/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/docs/LICENSE.txt` & `plone.mls.listing-1.9/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/PKG-INFO` & `plone.mls.listing-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: plone.mls.listing
-Version: 1.8.dev0
+Version: 1.9
 Summary: Plone support for MLS Listings.
 Home-page: https://github.com/propertyshelf/plone.mls.listing
 Author: Propertyshelf, Inc.
 Author-email: development@propertyshelf.com
 License: GPL
 Download-URL: http://pypi.python.org/pypi/plone.mls.listing
 Description: Introduction
@@ -39,15 +39,33 @@
         
         - Thomas Massmann, thomas@propertyshelf.com
         - Zach Cashero, zach@propertyshelf.com
         
         Changelog
         =========
         
-        1.8 (unreleased)
+        1.9 (2017-04-04)
+        ----------------
+        
+        - In agent contact form, use sender for email 'from', instead of 'reply-to'.
+        
+        
+        1.8.2 (2016-11-07)
+        ------------------
+        
+        - Fix CSS.
+        
+        
+        1.8.1 (2016-10-17)
+        ------------------
+        
+        - Fix manifest.
+        
+        
+        1.8 (2016-10-17)
         ----------------
         
         - Add single beds and baths for listings (hidden with CSS by default).
         - Use high resolution lead image for listing collections, if available.
         - Add listing description for listing collections (hidden with CSS by default).
         - Add calculated price for listings (hidden with CSS by default).
         - Remove colons after labels from listing templates (now added via CSS).
```

### Comparing `plone.mls.listing-1.8.dev0/README.rst` & `plone.mls.listing-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/setup.py` & `plone.mls.listing-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Setup for plone.mls.listing package."""
 
 from setuptools import (
     find_packages,
     setup,
 )
 
-version = '1.8.dev0'
+version = '1.9'
 description = 'Plone support for MLS Listings.'
 long_description = ('\n'.join([
     open('README.rst').read(),
     'Contributors',
     '------------\n',
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
```

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/api.py` & `plone.mls.listing-1.9/src/plone/mls/listing/api.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/adapters.py` & `plone.mls.listing-1.9/src/plone/mls/listing/article/adapters.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/configure.zcml` & `plone.mls.listing-1.9/src/plone/mls/listing/article/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/listing.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/article/listing.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/article/listing.py` & `plone.mls.listing-1.9/src/plone/mls/listing/article/listing.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/backports/configure.zcml` & `plone.mls.listing-1.9/src/plone/mls/listing/backports/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/backports/utils.py` & `plone.mls.listing-1.9/src/plone/mls/listing/backports/utils.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/backports/viewlets.py` & `plone.mls.listing-1.9/src/plone/mls/listing/backports/viewlets.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/adapter.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/adapter.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/configure.zcml` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/controlpanel.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/apartment.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/apartment.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/condominium.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/condominium.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/house.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/house.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/icon_talk.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/icon_talk.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/no-image.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/no-image.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/office-building.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/office-building.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/quotation_left.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/quotation_left.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/quotation_right.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/quotation_right.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/images/townhouse.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/images/townhouse.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/classic-loader.gif` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/classic-loader.gif`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/classic-map.png` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/classic-map.png`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/galleria.classic.css` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/galleria.classic.css`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/galleria.classic.js` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/galleria.classic.js`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/classic/galleria.classic.min.js` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/classic/galleria.classic.min.js`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/galleria-1.2.2.js` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/galleria-1.2.2.js`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/jquery.ias.min.js` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/jquery.ias.min.js`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/listing.js` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/listing.js`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/javascript/listing_ias.js` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/javascript/listing_ias.js`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/listing_collection.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/listing_collection.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/listing_search.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/listing_search.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/localconfig.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/localconfig.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/navigation.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/recent_listings.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/recent_listings.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/stylesheets/main.css` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/stylesheets/main.css`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   display: none;
 }
 
 
 .listing-summary dl dt:after,
 .listing__summary dl dt:after {
   content: ":";
+  display: inline;
 }
 
 
 /* HTML5 Elements
    ==============
 */
```

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/stylesheets/print.css` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/stylesheets/print.css`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
   max-width: 275px;
 }
 
 .contact-information dl dt:after,
 .listing__details dl dt:after,
 .listing__summary dl dt:after {
   content: ":";
+  display: inline;
 }
 
 #listing-info img {
   float: right;
   max-width: 25%;
 }
 
@@ -85,8 +86,8 @@
 blockquote {
   margin: 1em 0;
   text-align: justify;
 }
 
 .visualClear {
   clear: both;
-}
+}
```

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/configure.zcml` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/tc_display.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/tc_display.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/tc_input.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/tc_input.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/tcwidgetwrapper.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/tcwidgetwrapper.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/tcwidget/widget.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/tcwidget/widget.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/listing_collection_viewlet.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/listing_collection_viewlet.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/listing_details.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/listing_details.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/listing_search_viewlet.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/listing_search_viewlet.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/print_listing_details.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/print_listing_details.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/recent_listings_viewlet.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/recent_listings_viewlet.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/templates/search_form.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/templates/search_form.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/traversal.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/configure.zcml` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/valuerange_display.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/valuerange_display.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/valuerange_hidden.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/valuerange_hidden.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/valuerange_input.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/valuerange_input.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/valuerange/widget.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/valuerange/widget.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/browser/views.py` & `plone.mls.listing-1.9/src/plone/mls/listing/browser/views.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/configure.zcml` & `plone.mls.listing-1.9/src/plone/mls/listing/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/interfaces.py` & `plone.mls.listing-1.9/src/plone/mls/listing/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ar/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/ar/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/cmn/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/cmn/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/de/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/de/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/en/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/en/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/es/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/es/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/et/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/et/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/fr/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/fr/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/it/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/it/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ja/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/ja/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/plone.mls.listing.pot` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/plone.mls.listing.pot`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/plone.pot` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/pt/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/pt/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/ru/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/ru/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/vi/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/vi/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/vi_VN/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/vi_VN/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/zh/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/zh/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/locales/zh_TW/LC_MESSAGES/plone.mls.listing.po` & `plone.mls.listing-1.9/src/plone/mls/listing/locales/zh_TW/LC_MESSAGES/plone.mls.listing.po`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/migration.py` & `plone.mls.listing-1.9/src/plone/mls/listing/migration.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/agent_contact.py` & `plone.mls.listing-1.9/src/plone/mls/listing/portlets/agent_contact.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,18 +415,17 @@
         message = translate(
             EMAIL_TEMPLATE,
             context=self.request,
         ).format(**data)
 
         message = message_from_string(message.encode(email_charset))
         message['To'] = rcp
-        message['From'] = from_address
+        message['From'] = sender
         if getattr(self.data, 'bcc', None) is not None:
             message['Bcc'] = self.data.bcc
-        message['Reply-to'] = sender
         message['Subject'] = subject
 
         mailhost.send(message, immediate=True, charset=email_charset)
         return
 
 # Register Captcha validator for the captcha field in the ICaptchaForm
 validator.WidgetValidatorDiscriminators(
```

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/agent_information.py` & `plone.mls.listing-1.9/src/plone/mls/listing/portlets/agent_information.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/configure.zcml` & `plone.mls.listing-1.9/src/plone/mls/listing/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/quick_search.py` & `plone.mls.listing-1.9/src/plone/mls/listing/portlets/quick_search.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/agent_contact.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/agent_contact.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/agent_information.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/agent_information.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/quick_search.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/quick_search.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/portlets/templates/search_form.pt` & `plone.mls.listing-1.9/src/plone/mls/listing/portlets/templates/search_form.pt`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/actions.xml` & `plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/controlpanel.xml` & `plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/jsregistry.xml` & `plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/portlets.xml` & `plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/portlets.xml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles/default/types/plone.mls.listing.listing.xml` & `plone.mls.listing-1.9/src/plone/mls/listing/profiles/default/types/plone.mls.listing.listing.xml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/profiles.zcml` & `plone.mls.listing-1.9/src/plone/mls/listing/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/setuphandlers.py` & `plone.mls.listing-1.9/src/plone/mls/listing/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/testing.py` & `plone.mls.listing-1.9/src/plone/mls/listing/testing.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_content.py` & `plone.mls.listing-1.9/src/plone/mls/listing/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_portlet_agent_contact.py` & `plone.mls.listing-1.9/src/plone/mls/listing/tests/test_portlet_agent_contact.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_portlet_agent_information.py` & `plone.mls.listing-1.9/src/plone/mls/listing/tests/test_portlet_agent_information.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_portlet_quick_search.py` & `plone.mls.listing-1.9/src/plone/mls/listing/tests/test_portlet_quick_search.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/tests/test_setup.py` & `plone.mls.listing-1.9/src/plone/mls/listing/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone/mls/listing/vocabularies.py` & `plone.mls.listing-1.9/src/plone/mls/listing/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/PKG-INFO` & `plone.mls.listing-1.9/src/plone.mls.listing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: plone.mls.listing
-Version: 1.8.dev0
+Version: 1.9
 Summary: Plone support for MLS Listings.
 Home-page: https://github.com/propertyshelf/plone.mls.listing
 Author: Propertyshelf, Inc.
 Author-email: development@propertyshelf.com
 License: GPL
 Download-URL: http://pypi.python.org/pypi/plone.mls.listing
 Description: Introduction
@@ -39,15 +39,33 @@
         
         - Thomas Massmann, thomas@propertyshelf.com
         - Zach Cashero, zach@propertyshelf.com
         
         Changelog
         =========
         
-        1.8 (unreleased)
+        1.9 (2017-04-04)
+        ----------------
+        
+        - In agent contact form, use sender for email 'from', instead of 'reply-to'.
+        
+        
+        1.8.2 (2016-11-07)
+        ------------------
+        
+        - Fix CSS.
+        
+        
+        1.8.1 (2016-10-17)
+        ------------------
+        
+        - Fix manifest.
+        
+        
+        1.8 (2016-10-17)
         ----------------
         
         - Add single beds and baths for listings (hidden with CSS by default).
         - Use high resolution lead image for listing collections, if available.
         - Add listing description for listing collections (hidden with CSS by default).
         - Add calculated price for listings (hidden with CSS by default).
         - Remove colons after labels from listing templates (now added via CSS).
```

### Comparing `plone.mls.listing-1.8.dev0/src/plone.mls.listing.egg-info/SOURCES.txt` & `plone.mls.listing-1.9/src/plone.mls.listing.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.rst
+CONTRIBUTORS.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/INSTALL.txt
 docs/LICENSE.txt
 src/plone/__init__.py
```

