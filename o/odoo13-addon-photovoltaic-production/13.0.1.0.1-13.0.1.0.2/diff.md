# Comparing `tmp/odoo13-addon-photovoltaic_production-13.0.1.0.1.tar.gz` & `tmp/odoo13-addon-photovoltaic_production-13.0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_production-13.0.1.0.1.tar", last modified: Thu Aug  3 18:45:59 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_production-13.0.1.0.2.tar", last modified: Fri Aug  4 10:52:12 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1.tar` & `odoo13-addon-photovoltaic_production-13.0.1.0.2.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.302116 odoo13-addon-photovoltaic_production-13.0.1.0.1/
--rw-r--r--   0 root         (0) root         (0)      372 2023-08-03 18:45:59.302116 odoo13-addon-photovoltaic_production-13.0.1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.296116 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.296116 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.297116 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.298116 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    14372 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)    13599 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/i18n/photovoltaic_production.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.299116 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/photovoltaic_power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/photovoltaic_production.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/photovoltaic_production_bill.py
--rw-rw-rw-   0 root         (0) root         (0)     5746 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/photovoltaic_production_regularization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.299116 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/security/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.300116 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/
--rw-rw-rw-   0 root         (0) root         (0)      668 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_power_station.xml
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_production.xml
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_production_bill.xml
--rw-rw-rw-   0 root         (0) root         (0)     4531 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_production_regularization.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:45:59.301116 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo13_addon_photovoltaic_production.egg-info/
--rw-r--r--   0 root         (0) root         (0)      372 2023-08-03 18:45:59.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo13_addon_photovoltaic_production.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1308 2023-08-03 18:45:59.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo13_addon_photovoltaic_production.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 18:45:59.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo13_addon_photovoltaic_production.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 18:45:59.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo13_addon_photovoltaic_production.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2023-08-03 18:45:59.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo13_addon_photovoltaic_production.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 18:45:59.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo13_addon_photovoltaic_production.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 18:45:59.302116 odoo13-addon-photovoltaic_production-13.0.1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-08-03 18:45:41.000000 odoo13-addon-photovoltaic_production-13.0.1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.312769 odoo13-addon-photovoltaic_production-13.0.1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      372 2023-08-04 10:52:12.311772 odoo13-addon-photovoltaic_production-13.0.1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.305786 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.305786 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.307782 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.307782 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    14372 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)    13599 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/i18n/photovoltaic_production.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.308779 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/photovoltaic_power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/photovoltaic_production.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/photovoltaic_production_bill.py
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/photovoltaic_production_regularization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.309777 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/security/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.306784 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.309777 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/static/description/
+-rw-rw-rw-   0 root         (0) root         (0)    35296 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/static/description/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.310774 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/
+-rw-rw-rw-   0 root         (0) root         (0)      668 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_power_station.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2483 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_production.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_production_bill.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4531 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_production_regularization.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:52:12.311772 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo13_addon_photovoltaic_production.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      372 2023-08-04 10:52:12.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo13_addon_photovoltaic_production.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-08-04 10:52:12.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo13_addon_photovoltaic_production.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 10:52:12.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo13_addon_photovoltaic_production.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 10:52:12.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo13_addon_photovoltaic_production.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       81 2023-08-04 10:52:12.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo13_addon_photovoltaic_production.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 10:52:12.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo13_addon_photovoltaic_production.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 10:52:12.312769 odoo13-addon-photovoltaic_production-13.0.1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-08-04 10:51:56.000000 odoo13-addon-photovoltaic_production-13.0.1.0.2/setup.py
```

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/__manifest__.py` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Photovoltaic Production',
-    'version': '13.0.1.0.1',
+    'version': '13.0.1.0.2',
     'depends': ['photovoltaic_mgmt_extended', 'web_tree_dynamic_colored_field'],
     'external_dependencies': {
         'python': [
             'python-dateutil'
         ]
     },
     'author': 'Librecoop',
```

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/i18n/es.po` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/i18n/photovoltaic_production.pot` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/i18n/photovoltaic_production.pot`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/photovoltaic_production.py` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/photovoltaic_production.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/photovoltaic_production_bill.py` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/photovoltaic_production_bill.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/models/photovoltaic_production_regularization.py` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/models/photovoltaic_production_regularization.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/security/ir.model.access.csv` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_power_station.xml` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_power_station.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_production.xml` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_production.xml`

 * *Files 10% similar despite different names*

#### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_production.xml` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_production.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
-  <menuitem id="photovoltaic_production_menu" name="Photovoltaic Production" sequence="10"/>
+  <menuitem id="photovoltaic_production_menu" name="Photovoltaic Production" sequence="10" web_icon="photovoltaic_production,static/description/icon.png"/>
   <record id="photovoltaic_production_view_tree" model="ir.ui.view">
     <field name="name">photovoltaic_production.tree</field>
     <field name="model">photovoltaic.production</field>
     <field name="arch" type="xml">
       <tree>
         <field name="date"/>
         <field name="plant"/>
```

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_production_bill.xml` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_production_bill.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo/addons/photovoltaic_production/views/photovoltaic_production_regularization.xml` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo/addons/photovoltaic_production/views/photovoltaic_production_regularization.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_production-13.0.1.0.1/odoo13_addon_photovoltaic_production.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_production-13.0.1.0.2/odoo13_addon_photovoltaic_production.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 odoo/addons/photovoltaic_production/i18n/photovoltaic_production.pot
 odoo/addons/photovoltaic_production/models/__init__.py
 odoo/addons/photovoltaic_production/models/photovoltaic_power_station.py
 odoo/addons/photovoltaic_production/models/photovoltaic_production.py
 odoo/addons/photovoltaic_production/models/photovoltaic_production_bill.py
 odoo/addons/photovoltaic_production/models/photovoltaic_production_regularization.py
 odoo/addons/photovoltaic_production/security/ir.model.access.csv
+odoo/addons/photovoltaic_production/static/description/icon.png
 odoo/addons/photovoltaic_production/views/photovoltaic_power_station.xml
 odoo/addons/photovoltaic_production/views/photovoltaic_production.xml
 odoo/addons/photovoltaic_production/views/photovoltaic_production_bill.xml
 odoo/addons/photovoltaic_production/views/photovoltaic_production_regularization.xml
 odoo13_addon_photovoltaic_production.egg-info/PKG-INFO
 odoo13_addon_photovoltaic_production.egg-info/SOURCES.txt
 odoo13_addon_photovoltaic_production.egg-info/dependency_links.txt
```

