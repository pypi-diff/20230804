# Comparing `tmp/odoo14-addon-odoo_instance-14.0.1.1.2.dev2.tar.gz` & `tmp/odoo14-addon-odoo_instance-14.0.1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.1.2.dev2.tar", last modified: Wed Apr 26 15:57:34 2023, max compression
+gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.2.0.tar", last modified: Fri Aug  4 14:36:33 2023, max compression
```

## Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2.tar` & `odoo14-addon-odoo_instance-14.0.1.2.0.tar`

### file list

```diff
@@ -1,76 +1,82 @@
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4100 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/PKG-INFO
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3683 2023-04-25 23:36:38.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/README.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1325 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/__manifest__.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/calendar_tags.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1389 2023-04-25 16:24:52.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/ir_cron.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo_version_data.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      310 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/calendar_event.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      484 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/import_requirements_wizard.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19822 2023-04-26 15:57:11.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      370 2023-04-25 23:19:33.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_database.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3078 2023-04-25 22:38:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_module.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1345 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_process.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1791 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_window.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      452 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_release.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      283 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_version.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      475 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/process_module_rel.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      183 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/project_project.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/res_partner.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      703 2023-04-25 23:36:22.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/HISTORY.rst
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/newsfragments/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1783 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/ir.model.access.csv
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/security_groups.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/description/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    13912 2023-04-25 23:36:38.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/description/index.html
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/css/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/css/project_instance.css
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/img/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/img/icon.png
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/js/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/js/project_instance.js
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/tests/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/tests/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/tests/test_project_instance.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3617 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2679 2023-04-25 20:06:20.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-25 19:54:54.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4622 2023-04-25 20:37:02.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    20295 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3311 2023-04-25 20:56:12.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_module_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1688 2023-04-25 20:43:09.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_process_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2254 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_release_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1113 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_version_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/project_project_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/res_partner_view.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/wizards/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/wizards/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2291 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4100 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/PKG-INFO
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2899 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/not-zip-safe
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       50 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/requires.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/top_level.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/setup.cfg
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-25 22:51:42.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/setup.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4453 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/PKG-INFO
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4041 2023-08-04 14:36:05.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/README.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1325 2023-08-04 14:22:49.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/__manifest__.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/calendar_tags.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1389 2023-04-25 16:24:52.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/ir_cron.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo_version_data.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      136 2023-04-27 20:46:52.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/behave.ini
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      556 2023-04-26 20:12:01.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/environment.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      352 2023-04-26 18:32:47.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/instance_management.feature
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/steps/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2166 2023-04-27 23:49:22.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/steps/instance_management_steps.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      310 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-27 21:08:44.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/calendar_event.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      484 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/import_requirements_wizard.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    22207 2023-08-04 14:20:36.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      370 2023-04-25 23:19:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_database.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3078 2023-08-04 12:24:45.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_module.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1345 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_process.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1791 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_window.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      452 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_release.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      283 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_version.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      475 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/process_module_rel.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      183 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/project_project.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/res_partner.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      909 2023-08-04 14:33:04.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/HISTORY.rst
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/newsfragments/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1960 2023-08-04 14:20:36.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/ir.model.access.csv
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/security_groups.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/description/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    14521 2023-08-04 14:33:42.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/description/index.html
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/css/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/css/project_instance.css
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/img/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/img/icon.png
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/js/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/js/project_instance.js
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/tests/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/tests/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/tests/test_project_instance.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3617 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2679 2023-04-25 20:06:20.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-25 19:54:54.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4622 2023-04-25 20:37:02.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    21548 2023-08-04 14:20:36.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3311 2023-04-25 20:56:12.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_module_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1688 2023-04-25 20:43:09.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_process_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2254 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_release_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1113 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_version_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/project_project_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/res_partner_view.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/wizards/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/wizards/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2291 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4453 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3128 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/not-zip-safe
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       50 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/requires.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/top_level.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/setup.cfg
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-25 22:51:42.000000 odoo14-addon-odoo_instance-14.0.1.2.0/setup.py
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo_instance
-Version: 14.0.1.1.2.dev2
+Version: 14.0.1.2.0
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 
 =============
 Odoo Instance
 =============
 
-.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+.. 
+   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+   !! source digest: sha256:7c0ac8707125bdc1a9968bbd602c1bf329692ce692a4fb148a900abcbf70839b
+   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
     :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
     :alt: coopdevs/odoo14-addons
 
-|badge1| |badge2| |badge3| 
+|badge1| |badge2| |badge3|
 
 This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
 
 **Features**
 
  - Create and manage project instances, classified by Odoo version, and organize them by stages.
  - Schedule and manage deployment events for project instances, including the start time, duration, and description, with automatic calculation of the next available deployment window and a wizard to create calendar events.
@@ -50,14 +53,27 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.0 (2023-08-04)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add functional configurations section to store UI-managed configurations ()
+
+
+**Misc**
+
+- Move 'Deploy window' configuration to 'Misc' tab
+
+
 14.0.1.2.0 (2023-04-26)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Manage databases
 
@@ -105,28 +121,28 @@
 **Features**
 
 - Add instance relations to project and res.partner
 
 Bug Tracker
 ===========
 
-Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo14-addons/issues>`_.
+Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo_instance/issues>`_.
 In case of trouble, please check there if your issue has already been reported.
-If you spotted it first, help us smashing it by providing a detailed and welcomed
-`feedback <https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+If you spotted it first, help us to smash it by providing a detailed and welcomed
+`feedback <https://github.com/coopdevs/odoo_instance/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
 
 Do not contact contributors directly about support or help with technical issues.
 
 Credits
 =======
 
 Authors
 ~~~~~~~
 
 * Coopdevs
 
 Maintainers
 ~~~~~~~~~~~
 
-This module is part of the `coopdevs/odoo14-addons <https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance>`_ project on GitHub.
+This module is part of the `coopdevs/odoo_instance <https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance>`_ project on GitHub.
 
 You are welcome to contribute.
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/README.rst` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 =============
 Odoo Instance
 =============
 
-.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+.. 
+   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+   !! source digest: sha256:7c0ac8707125bdc1a9968bbd602c1bf329692ce692a4fb148a900abcbf70839b
+   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
     :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
     :alt: coopdevs/odoo14-addons
 
-|badge1| |badge2| |badge3| 
+|badge1| |badge2| |badge3|
 
 This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
 
 **Features**
 
  - Create and manage project instances, classified by Odoo version, and organize them by stages.
  - Schedule and manage deployment events for project instances, including the start time, duration, and description, with automatic calculation of the next available deployment window and a wizard to create calendar events.
@@ -37,14 +40,27 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.0 (2023-08-04)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add functional configurations section to store UI-managed configurations ()
+
+
+**Misc**
+
+- Move 'Deploy window' configuration to 'Misc' tab
+
+
 14.0.1.2.0 (2023-04-26)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Manage databases
 
@@ -92,28 +108,28 @@
 **Features**
 
 - Add instance relations to project and res.partner
 
 Bug Tracker
 ===========
 
-Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo14-addons/issues>`_.
+Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo_instance/issues>`_.
 In case of trouble, please check there if your issue has already been reported.
-If you spotted it first, help us smashing it by providing a detailed and welcomed
-`feedback <https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+If you spotted it first, help us to smash it by providing a detailed and welcomed
+`feedback <https://github.com/coopdevs/odoo_instance/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
 
 Do not contact contributors directly about support or help with technical issues.
 
 Credits
 =======
 
 Authors
 ~~~~~~~
 
 * Coopdevs
 
 Maintainers
 ~~~~~~~~~~~
 
-This module is part of the `coopdevs/odoo14-addons <https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance>`_ project on GitHub.
+This module is part of the `coopdevs/odoo_instance <https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance>`_ project on GitHub.
 
 You are welcome to contribute.
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/__manifest__.py` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Odoo Instance',
-    'version': '14.0.1.1.1',
+    'version': '14.0.1.2.0',
     'category': 'Project',
     'summary': 'Manage Odoo instances with relevant information',
     'author': 'Coopdevs',
     'website': 'https://www.coopdevs.org',
     'depends': ['base', 'contract', 'project', 'calendar'],
     'data': [
         'security/security_groups.xml',
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/ir_cron.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/ir_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo_version_data.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo_version_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance.py` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,14 +101,24 @@
     )
     available_windows = fields.One2many(
         'odoo.instance.window', 'instance_id', string='Available Windows')
 
     functional_requirement_ids = fields.One2many(
         'odoo.instance.functional_requirement', 'odoo_instance_id', string='Functional Requirements')
 
+    functional_configuration_ids = fields.Many2many(
+        'odoo.instance.functional_configuration',
+        string='Functional Configurations',
+        relation='odoo_instance_functional_configuration_rel',
+        column1='odoo_instance_id',
+        column2='functional_configuration_id',
+        track_visibility='onchange',
+        help='List of functional configurations related to the current instance.'
+    )
+
     # Commercial Information
     contact_role_id = fields.Many2one('res.partner', string='Rol de Contacto')
     maintenance_contract_ids = fields.Char(string='Contratos de Mantenimiento')
     support_contract_ids = fields.Char(string='Contratos de Soporte')
     implementation_contract_id = fields.Char(
         string='Contrato de Implementación')
 
@@ -413,14 +423,39 @@
     def action_delete_past_or_orphan_windows(self):
         self.env["odoo.instance.window"].delete_past_or_orphan_windows()
 
     def action_clear_windows(self):
         self.env['odoo.instance.window'].search(
             [('instance_id', '=', self.id)]).unlink()
 
+    def write(self, vals):
+        # Si hay cambios en 'functional_configuration_ids'
+        if 'functional_configuration_ids' in vals:
+            # Consigue las nuevas configuraciones
+            new_config_ids = set(vals['functional_configuration_ids'][0][2])
+            
+            for record in self:
+                # Consigue las configuraciones antiguas
+                old_config_ids = set(record.functional_configuration_ids.ids)
+                
+                # Encuentra las configuraciones que se añadieron y se eliminaron
+                added_config_ids = new_config_ids - old_config_ids
+                removed_config_ids = old_config_ids - new_config_ids
+
+                # Obtiene los nombres de las configuraciones añadidas y eliminadas
+                added_config_names = self.env['odoo.instance.functional_configuration'].browse(added_config_ids).mapped('name')
+                removed_config_names = self.env['odoo.instance.functional_configuration'].browse(removed_config_ids).mapped('name')
+
+                # Publica mensajes en el chatter
+                for config_name in added_config_names:
+                    record.message_post(body="Añadida configuración funcional: %s" % config_name)
+                for config_name in removed_config_names:
+                    record.message_post(body="Eliminada configuración funcional: %s" % config_name)
+                
+        return super().write(vals)
 
 class OdooInstanceSchedule(models.Model):
     _name = 'odoo.instance.schedule'
     _description = 'Deploy Schedule'
 
     instance_id = fields.Many2one('odoo.instance', string="Instance")
     day_of_week = fields.Selection([
@@ -448,15 +483,25 @@
         ('in_progress', 'In Progress'),
         ('completed', 'Completed'),
         ('waiting_validation', 'Waiting for Validation')
     ], string='Status', default='not_started', required=True)
     odoo_instance_id = fields.Many2one(
         'odoo.instance', string='Odoo Instance')
 
-
+class OdooInstanceFunctionalConfiguration(models.Model):
+    _name = 'odoo.instance.functional_configuration'
+    _description = 'Odoo Instance Functional Configuration'
+    name = fields.Char('Configuration', required=True)
+    odoo_version_id = fields.Many2one(
+        'odoo.version', string="Odoo Version", required=True)
+    description = fields.Text('Description')
+    required_modules= fields.Many2many(
+        'odoo.instance.module', string='Required Modules')
+    handbook_url = fields.Text(string='Handbook URL')
+    
 class OdooInstanceTroubleshooting(models.Model):
     _name = 'odoo.instance.troubleshooting'
     _description = 'Odoo Instance Troubleshooting'
 
     date = fields.Date(string='Date', default=fields.Date.context_today)
     title = fields.Char(string='Title', required=True)
     url = fields.Char(string='URL')
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_module.py` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_module.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_process.py` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_process.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_window.py` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_window.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/DESCRIPTION.rst` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/HISTORY.rst` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/HISTORY.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+14.0.1.2.0 (2023-08-04)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add functional configurations section to store UI-managed configurations ()
+
+
+**Misc**
+
+- Move 'Deploy window' configuration to 'Misc' tab
+
+
 14.0.1.2.0 (2023-04-26)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Manage databases
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/ir.model.access.csv` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/ir.model.access.csv`

 * *Files 6% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 access_odoo_instance_functional_requirement,odoo.instance.functional.requirement,model_odoo_instance_functional_requirement,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_window,odoo.instance.window,model_odoo_instance_window,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_window_wizard,odoo.instance.window.wizard,model_odoo_instance_window_wizard,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_troubleshooting,odoo.instance.troubleshooting,model_odoo_instance_troubleshooting,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_version,odoo.version,model_odoo_version,odoo_instance.group_odoo_instance_user,1,1,0,0
 access_odoo_release,odoo.release,model_odoo_release,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_database,odoo.instance.database,model_odoo_instance_database,odoo_instance.group_odoo_instance_user,1,1,1,1
+access_odoo_instance_functional_configuration,odoo.instance.functional.configuration,model_odoo_instance_functional_configuration,odoo_instance.group_odoo_instance_user,1,1,1,1
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/description/index.html`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/description/index.html`

```diff
@@ -359,24 +359,26 @@
   </head>
   <body>
     <div class="document" id="odoo-instance">
       <h1 class="title">Odoo Instance</h1>
       <!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !! This file is generated by oca-gen-addon-readme !!
 !! changes will be overwritten.                   !!
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+!! source digest: sha256:7c0ac8707125bdc1a9968bbd602c1bf329692ce692a4fb148a900abcbf70839b
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->
       <p>
         <a class="reference external" href="https://odoo-community.org/page/development-status">
           <img alt="Beta" src="https://img.shields.io/badge/maturity-Beta-yellow.png"/>
         </a>
         <a class="reference external" href="http://www.gnu.org/licenses/agpl-3.0-standalone.html">
           <img alt="License: AGPL-3" src="https://img.shields.io/badge/licence-AGPL--3-blue.png"/>
         </a>
-        <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance">
-          <img alt="coopdevs/odoo14-addons" src="https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github"/>
+        <a class="reference external" href="https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance">
+          <img alt="coopdevs/odoo_instance" src="https://img.shields.io/badge/github-coopdevs%2Fodoo_instance-lightgray.png?logo=github"/>
         </a>
       </p>
       <p>This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.</p>
       <p>
         <strong>Features</strong>
       </p>
       <blockquote>
@@ -394,164 +396,184 @@
       </blockquote>
       <p>
         <strong>Table of contents</strong>
       </p>
       <div class="contents local topic" id="contents">
         <ul class="simple">
           <li>
-            <a class="reference internal" href="#changelog" id="id7">Changelog</a>
+            <a class="reference internal" href="#changelog" id="id8">Changelog</a>
             <ul>
               <li>
-                <a class="reference internal" href="#id1" id="id8">14.0.1.2.0 (2023-04-26)</a>
+                <a class="reference internal" href="#id1" id="id9">14.0.1.2.0 (2023-08-04)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id2" id="id9">14.0.1.1.1 (2023-04-25)</a>
+                <a class="reference internal" href="#id2" id="id10">14.0.1.2.0 (2023-04-26)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id3" id="id10">14.0.1.1.0 (2023-04-25)</a>
+                <a class="reference internal" href="#id3" id="id11">14.0.1.1.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id4" id="id11">14.0.1.0.1 (2023-04-25)</a>
+                <a class="reference internal" href="#id4" id="id12">14.0.1.1.0 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id5" id="id12">14.0.1.0.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id5" id="id13">14.0.1.0.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id6" id="id13">14.0.0.2.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id6" id="id14">14.0.1.0.0 (2023-04-24)</a>
+              </li>
+              <li>
+                <a class="reference internal" href="#id7" id="id15">14.0.0.2.0 (2023-04-24)</a>
               </li>
             </ul>
           </li>
           <li>
-            <a class="reference internal" href="#bug-tracker" id="id14">Bug Tracker</a>
+            <a class="reference internal" href="#bug-tracker" id="id16">Bug Tracker</a>
           </li>
           <li>
-            <a class="reference internal" href="#credits" id="id15">Credits</a>
+            <a class="reference internal" href="#credits" id="id17">Credits</a>
             <ul>
               <li>
-                <a class="reference internal" href="#authors" id="id16">Authors</a>
+                <a class="reference internal" href="#authors" id="id18">Authors</a>
               </li>
               <li>
-                <a class="reference internal" href="#maintainers" id="id17">Maintainers</a>
+                <a class="reference internal" href="#maintainers" id="id19">Maintainers</a>
               </li>
             </ul>
           </li>
         </ul>
       </div>
       <div class="section" id="changelog">
         <h1>
-          <a class="toc-backref" href="#id7">Changelog</a>
+          <a class="toc-backref" href="#id8">Changelog</a>
         </h1>
         <div class="section" id="id1">
           <h2>
-            <a class="toc-backref" href="#id8">14.0.1.2.0 (2023-04-26)</a>
+            <a class="toc-backref" href="#id9">14.0.1.2.0 (2023-08-04)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
-            <li>Manage databases</li>
+            <li>Add functional configurations section to store UI-managed configurations ()</li>
+          </ul>
+          <p>
+            <strong>Misc</strong>
+          </p>
+          <ul class="simple">
+            <li>Move ‘Deploy window’ configuration to ‘Misc’ tab</li>
           </ul>
         </div>
         <div class="section" id="id2">
           <h2>
-            <a class="toc-backref" href="#id9">14.0.1.1.1 (2023-04-25)</a>
+            <a class="toc-backref" href="#id10">14.0.1.2.0 (2023-04-26)</a>
+          </h2>
+          <p>
+            <strong>Features</strong>
+          </p>
+          <ul class="simple">
+            <li>Manage databases</li>
+          </ul>
+        </div>
+        <div class="section" id="id3">
+          <h2>
+            <a class="toc-backref" href="#id11">14.0.1.1.1 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Bugfixes</strong>
           </p>
           <ul class="simple">
             <li>Upcrate module versions</li>
             <li>Show installed module versions only in instance view</li>
           </ul>
         </div>
-        <div class="section" id="id3">
+        <div class="section" id="id4">
           <h2>
-            <a class="toc-backref" href="#id10">14.0.1.1.0 (2023-04-25)</a>
+            <a class="toc-backref" href="#id12">14.0.1.1.0 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Handle odoo releases</li>
           </ul>
         </div>
-        <div class="section" id="id4">
+        <div class="section" id="id5">
           <h2>
-            <a class="toc-backref" href="#id11">14.0.1.0.1 (2023-04-25)</a>
+            <a class="toc-backref" href="#id13">14.0.1.0.1 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Improved UX: Searches, filters, grouping…</li>
           </ul>
           <p>
             <strong>Bugfixes</strong>
           </p>
           <ul class="simple">
             <li>Removed forgotten debug statementes</li>
           </ul>
         </div>
-        <div class="section" id="id5">
+        <div class="section" id="id6">
           <h2>
-            <a class="toc-backref" href="#id12">14.0.1.0.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id14">14.0.1.0.0 (2023-04-24)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Rename models and split logic in files</li>
           </ul>
         </div>
-        <div class="section" id="id6">
+        <div class="section" id="id7">
           <h2>
-            <a class="toc-backref" href="#id13">14.0.0.2.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id15">14.0.0.2.0 (2023-04-24)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Add instance relations to project and res.partner</li>
           </ul>
         </div>
       </div>
       <div class="section" id="bug-tracker">
         <h1>
-          <a class="toc-backref" href="#id14">Bug Tracker</a>
+          <a class="toc-backref" href="#id16">Bug Tracker</a>
         </h1>
         <p>
           Bugs are tracked on
-          <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/issues">GitHub Issues</a>
+          <a class="reference external" href="https://github.com/coopdevs/odoo_instance/issues">GitHub Issues</a>
           .
 In case of trouble, please check there if your issue has already been reported.
-If you spotted it first, help us smashing it by providing a detailed and welcomed
-          <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>
+If you spotted it first, help us to smash it by providing a detailed and welcomed
+          <a class="reference external" href="https://github.com/coopdevs/odoo_instance/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>
           .
         </p>
         <p>Do not contact contributors directly about support or help with technical issues.</p>
       </div>
       <div class="section" id="credits">
         <h1>
-          <a class="toc-backref" href="#id15">Credits</a>
+          <a class="toc-backref" href="#id17">Credits</a>
         </h1>
         <div class="section" id="authors">
           <h2>
-            <a class="toc-backref" href="#id16">Authors</a>
+            <a class="toc-backref" href="#id18">Authors</a>
           </h2>
           <ul class="simple">
             <li>Coopdevs</li>
           </ul>
         </div>
         <div class="section" id="maintainers">
           <h2>
-            <a class="toc-backref" href="#id17">Maintainers</a>
+            <a class="toc-backref" href="#id19">Maintainers</a>
           </h2>
           <p>
             This module is part of the
-            <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance">coopdevs/odoo14-addons</a>
+            <a class="reference external" href="https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance">coopdevs/odoo_instance</a>
             project on GitHub.
           </p>
           <p>You are welcome to contribute.</p>
         </div>
       </div>
     </div>
   </body>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/img/icon.png` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/img/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_actions.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_searches.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

 * *Files 1% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

```diff
@@ -68,24 +68,24 @@
                       <field name="name"/>
                       <field name="description"/>
                       <field name="module_ids" widget="many2many_tags"/>
                       <field name="handbook_url" widget="url"/>
                     </tree>
                   </field>
                 </group>
-                <group name="Deploy Windows" string="Non-deploy windows">
+                <group name="Functional Configurations" string="Functional Configurations">
                   <group>
-                    <div>Schedule of working hours in those we can't make
-                                            deployments</div>
+                    <div>Configurations made through UI.</div>
                   </group>
-                  <field name="unavailable_windows" widget="one2many_list" nolabel="1">
+                  <field name="functional_configuration_ids" domain="[('odoo_version_id', '=', odoo_version_id)]" widget="one2many_list" nolabel="1" options="{'open': True}">
                     <tree editable="bottom">
-                      <field name="day_of_week"/>
-                      <field name="start_time" widget="float_time"/>
-                      <field name="end_time" widget="float_time"/>
+                      <field name="name"/>
+                      <field name="description" widget="text"/>
+                      <field name="required_modules" widget="many2many_tags"/>
+                      <field name="handbook_url" widget="url"/>
                     </tree>
                   </field>
                 </group>
                 <group string="Functional Requirements">
                   <field name="functional_requirement_ids" nolabel="1" context="{'default_odoo_instance_id': active_id}">
                     <tree editable="bottom">
                       <field name="name"/>
@@ -172,14 +172,27 @@
                 </group>
               </page>
               <page string="Misc">
                 <group>
                   <field name="description"/>
                   <field name="start_date"/>
                 </group>
+                <group name="Deploy Windows" string="Non-deploy windows">
+                  <group>
+                    <div>Schedule of working hours in those we can't make
+                                            deployments</div>
+                  </group>
+                  <field name="unavailable_windows" widget="one2many_list" nolabel="1">
+                    <tree editable="bottom">
+                      <field name="day_of_week"/>
+                      <field name="start_time" widget="float_time"/>
+                      <field name="end_time" widget="float_time"/>
+                    </tree>
+                  </field>
+                </group>
               </page>
             </notebook>
           </sheet>
           <div class="oe_chatter">
             <field name="message_follower_ids" widget="mail_followers" groups="base.group_user"/>
             <field name="message_ids" widget="mail_thread" groups="base.group_user"/>
           </div>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_module_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_module_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_process_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_process_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_release_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_release_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_version_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_version_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/project_project_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/project_project_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/res_partner_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo-instance
-Version: 14.0.1.1.2.dev2
+Version: 14.0.1.2.0
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 
 =============
 Odoo Instance
 =============
 
-.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+.. 
+   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+   !! source digest: sha256:7c0ac8707125bdc1a9968bbd602c1bf329692ce692a4fb148a900abcbf70839b
+   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
     :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
     :alt: coopdevs/odoo14-addons
 
-|badge1| |badge2| |badge3| 
+|badge1| |badge2| |badge3|
 
 This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
 
 **Features**
 
  - Create and manage project instances, classified by Odoo version, and organize them by stages.
  - Schedule and manage deployment events for project instances, including the start time, duration, and description, with automatic calculation of the next available deployment window and a wizard to create calendar events.
@@ -50,14 +53,27 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.0 (2023-08-04)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add functional configurations section to store UI-managed configurations ()
+
+
+**Misc**
+
+- Move 'Deploy window' configuration to 'Misc' tab
+
+
 14.0.1.2.0 (2023-04-26)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Manage databases
 
@@ -105,28 +121,28 @@
 **Features**
 
 - Add instance relations to project and res.partner
 
 Bug Tracker
 ===========
 
-Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo14-addons/issues>`_.
+Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo_instance/issues>`_.
 In case of trouble, please check there if your issue has already been reported.
-If you spotted it first, help us smashing it by providing a detailed and welcomed
-`feedback <https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+If you spotted it first, help us to smash it by providing a detailed and welcomed
+`feedback <https://github.com/coopdevs/odoo_instance/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
 
 Do not contact contributors directly about support or help with technical issues.
 
 Credits
 =======
 
 Authors
 ~~~~~~~
 
 * Coopdevs
 
 Maintainers
 ~~~~~~~~~~~
 
-This module is part of the `coopdevs/odoo14-addons <https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance>`_ project on GitHub.
+This module is part of the `coopdevs/odoo_instance <https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance>`_ project on GitHub.
 
 You are welcome to contribute.
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/SOURCES.txt` & `odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 odoo/addons/odoo_instance/__init__.py
 odoo/addons/odoo_instance/__manifest__.py
 odoo/addons/odoo_instance/data/calendar_tags.xml
 odoo/addons/odoo_instance/data/ir_cron.xml
 odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
 odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
 odoo/addons/odoo_instance/data/odoo_version_data.xml
+odoo/addons/odoo_instance/features/behave.ini
+odoo/addons/odoo_instance/features/environment.py
+odoo/addons/odoo_instance/features/instance_management.feature
+odoo/addons/odoo_instance/features/steps/instance_management_steps.py
 odoo/addons/odoo_instance/models/__init__.py
 odoo/addons/odoo_instance/models/calendar_event.py
 odoo/addons/odoo_instance/models/import_requirements_wizard.py
 odoo/addons/odoo_instance/models/odoo_instance.py
 odoo/addons/odoo_instance/models/odoo_instance_database.py
 odoo/addons/odoo_instance/models/odoo_instance_module.py
 odoo/addons/odoo_instance/models/odoo_instance_process.py
```

