# Comparing `tmp/odoo14-addon-odoo_instance-14.0.1.2.0.tar.gz` & `tmp/odoo14-addon-odoo_instance-14.0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.2.0.tar", last modified: Fri Aug  4 14:36:33 2023, max compression
+gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.2.1.tar", last modified: Fri Aug  4 17:14:21 2023, max compression
```

## Comparing `odoo14-addon-odoo_instance-14.0.1.2.0.tar` & `odoo14-addon-odoo_instance-14.0.1.2.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4453 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/PKG-INFO
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4041 2023-08-04 14:36:05.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/README.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1325 2023-08-04 14:22:49.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/__manifest__.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/calendar_tags.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1389 2023-04-25 16:24:52.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/ir_cron.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo_version_data.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      136 2023-04-27 20:46:52.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/behave.ini
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      556 2023-04-26 20:12:01.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/environment.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      352 2023-04-26 18:32:47.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/instance_management.feature
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/steps/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2166 2023-04-27 23:49:22.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/steps/instance_management_steps.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      310 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-27 21:08:44.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/calendar_event.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      484 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/import_requirements_wizard.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    22207 2023-08-04 14:20:36.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      370 2023-04-25 23:19:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_database.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3078 2023-08-04 12:24:45.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_module.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1345 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_process.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1791 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_window.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      452 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_release.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      283 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_version.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      475 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/process_module_rel.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      183 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/project_project.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/res_partner.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      909 2023-08-04 14:33:04.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/HISTORY.rst
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/newsfragments/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1960 2023-08-04 14:20:36.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/ir.model.access.csv
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/security_groups.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/description/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    14521 2023-08-04 14:33:42.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/description/index.html
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.298871 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/css/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/css/project_instance.css
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/img/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/img/icon.png
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/js/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/js/project_instance.js
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/tests/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/tests/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/tests/test_project_instance.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3617 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2679 2023-04-25 20:06:20.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-25 19:54:54.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4622 2023-04-25 20:37:02.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    21548 2023-08-04 14:20:36.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3311 2023-04-25 20:56:12.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_module_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1688 2023-04-25 20:43:09.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_process_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2254 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_release_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1113 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_version_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/project_project_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/res_partner_view.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/wizards/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/wizards/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2291 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4453 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3128 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/not-zip-safe
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       50 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/requires.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-08-04 14:36:33.000000 odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/top_level.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-08-04 14:36:33.302204 odoo14-addon-odoo_instance-14.0.1.2.0/setup.cfg
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-25 22:51:42.000000 odoo14-addon-odoo_instance-14.0.1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.595339 odoo14-addon-odoo_instance-14.0.1.2.1/
+-rw-r--r--   0 root         (0) root         (0)     4611 2023-08-04 17:14:21.591339 odoo14-addon-odoo_instance-14.0.1.2.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.583339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.583339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.583339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/
+-rw-rw-rw-   0 root         (0) root         (0)     4179 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/calendar_tags.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1932 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/ir_cron.xml
+-rw-rw-rw-   0 root         (0) root         (0)    95199 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     9484 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/odoo_version_data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/features/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/features/behave.ini
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/features/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/features/instance_management.feature
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/features/steps/
+-rw-rw-rw-   0 root         (0) root         (0)     2166 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/features/steps/instance_management_steps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/calendar_event.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/import_requirements_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    22558 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance_window.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_release.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/process_module_rel.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/project_project.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/res_partner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/readme/
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/readme/HISTORY.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/readme/newsfragments/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/security/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/security/ir.model.access.csv
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/security/security_groups.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.583339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/description/
+-rw-rw-rw-   0 root         (0) root         (0)    14872 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/description/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.583339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.587339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/src/css/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/src/css/project_instance.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.591339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/src/img/
+-rw-rw-rw-   0 root         (0) root         (0)    33659 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/src/img/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.591339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/src/js/project_instance.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.591339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/tests/test_project_instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.591339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2679 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4622 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
+-rw-rw-rw-   0 root         (0) root         (0)    21548 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      971 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_module_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_process_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_release_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_version_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/project_project_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/res_partner_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.591339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/wizards/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/wizards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:14:21.591339 odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4611 2023-08-04 17:14:21.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-08-04 17:14:21.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 17:14:21.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 17:14:21.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-04 17:14:21.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 17:14:21.000000 odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 17:14:21.595339 odoo14-addon-odoo_instance-14.0.1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-08-04 17:14:08.000000 odoo14-addon-odoo_instance-14.0.1.2.1/setup.py
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo_instance
-Version: 14.0.1.2.0
+Version: 14.0.1.2.1
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 
 =============
@@ -16,25 +17,25 @@
 =============
 
 .. 
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-   !! source digest: sha256:7c0ac8707125bdc1a9968bbd602c1bf329692ce692a4fb148a900abcbf70839b
+   !! source digest: sha256:18157e50fb2fc08b090dd3565b448d97228713b78045c938e37785d0b7ef0e4b
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
-    :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
+    :target: https://git.coopdevs.org/coopdevs/odoo/odoo-addons/odoo14-addons/-/tree/14.0/odoo_instance
     :alt: coopdevs/odoo14-addons
 
 |badge1| |badge2| |badge3|
 
 This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
 
 **Features**
@@ -53,20 +54,28 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.1 (2023-08-04)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add cron to update instances info
+
+
 14.0.1.2.0 (2023-08-04)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
-- Add functional configurations section to store UI-managed configurations ()
+- Add functional configurations section to store UI-managed configurations
 
 
 **Misc**
 
 - Move 'Deploy window' configuration to 'Misc' tab
 
 
@@ -139,10 +148,12 @@
 ~~~~~~~
 
 * Coopdevs
 
 Maintainers
 ~~~~~~~~~~~
 
-This module is part of the `coopdevs/odoo_instance <https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance>`_ project on GitHub.
+This module is part of the `coopdevs/odoo_instance <https://git.coopdevs.org/coopdevs/odoo/odoo-addons/odoo14-addons/-/tree/14.0/odoo_instance>`_ project.
 
 You are welcome to contribute.
+
+
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/README.rst` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 =============
 
 .. 
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-   !! source digest: sha256:7c0ac8707125bdc1a9968bbd602c1bf329692ce692a4fb148a900abcbf70839b
+   !! source digest: sha256:18157e50fb2fc08b090dd3565b448d97228713b78045c938e37785d0b7ef0e4b
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
-    :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
+    :target: https://git.coopdevs.org/coopdevs/odoo/odoo-addons/odoo14-addons/-/tree/14.0/odoo_instance
     :alt: coopdevs/odoo14-addons
 
 |badge1| |badge2| |badge3|
 
 This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
 
 **Features**
@@ -40,20 +40,28 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.1 (2023-08-04)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add cron to update instances info
+
+
 14.0.1.2.0 (2023-08-04)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
-- Add functional configurations section to store UI-managed configurations ()
+- Add functional configurations section to store UI-managed configurations
 
 
 **Misc**
 
 - Move 'Deploy window' configuration to 'Misc' tab
 
 
@@ -126,10 +134,10 @@
 ~~~~~~~
 
 * Coopdevs
 
 Maintainers
 ~~~~~~~~~~~
 
-This module is part of the `coopdevs/odoo_instance <https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance>`_ project on GitHub.
+This module is part of the `coopdevs/odoo_instance <https://git.coopdevs.org/coopdevs/odoo/odoo-addons/odoo14-addons/-/tree/14.0/odoo_instance>`_ project.
 
 You are welcome to contribute.
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/__manifest__.py` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/__manifest__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {
     'name': 'Odoo Instance',
-    'version': '14.0.1.2.0',
+    'version': '14.0.1.2.1',
     'category': 'Project',
     'summary': 'Manage Odoo instances with relevant information',
     'author': 'Coopdevs',
     'website': 'https://www.coopdevs.org',
-    'depends': ['base', 'contract', 'project', 'calendar'],
+    'depends': ['base', 'contract', 'project', 'calendar', 'queue_job'],
     'data': [
         'security/security_groups.xml',
         'security/ir.model.access.csv',
         'views/odoo_instance_view.xml',
         'views/odoo_module_view.xml',
         'views/odoo_instance_window_wizard_view.xml',
         'views/odoo_version_view.xml',
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/ir_cron.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/ir_cron.xml`

 * *Files 19% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/ir_cron.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/ir_cron.xml`

```diff
@@ -20,8 +20,19 @@
     <field name="user_id" ref="base.user_root"/>
     <field name="interval_number">1</field>
     <field name="interval_type">days</field>
     <field name="numbercall">-1</field>
     <field name="doall" eval="False"/>
     <field name="active" eval="True"/>
   </record>
+  <record id="ir_cron_update_instance_info" model="ir.cron">
+    <field name="name">Update Instance Info</field>
+    <field name="model_id" ref="model_odoo_instance"/>
+    <field name="state">code</field>
+    <field name="code">model.enqueue_update_instance_info()</field>
+    <field name="user_id" ref="base.user_root"/>
+    <field name="interval_number">7</field>
+    <field name="interval_type">days</field>
+    <field name="numbercall">-1</field>
+    <field name="active" eval="True"/>
+  </record>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/data/odoo_version_data.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/data/odoo_version_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/environment.py` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/features/environment.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/features/steps/instance_management_steps.py` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/features/steps/instance_management_steps.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance.py` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,23 @@
         for instance in self:
             # Update Odoo Release
             instance.update_odoo_release()
 
             # Update Instance DBs
             instance._update_instance_dbs()
 
+    @api.model
+    def enqueue_update_instance_info(self):
+        instances = self.search([])
+        for instance in instances:
+            if instance.inventory_url:
+                instance.with_delay().update_instance_info()
+            if instance.requirements_url:
+                instance.with_delay().download_and_process_requirements_txt()
+
     def toggle_state(self):
         state_order = ['in_progress', 'running', 'paused', 'cancelled']
         next_state_index = (state_order.index(
             self.state) + 1) % len(state_order)
         self.state = state_order[next_state_index]
 
     def download_and_process_requirements_txt(self):
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_module.py` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance_module.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_process.py` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance_process.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/models/odoo_instance_window.py` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/models/odoo_instance_window.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/readme/HISTORY.rst` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/readme/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,21 @@
+14.0.1.2.1 (2023-08-04)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add cron to update instances info
+
+
 14.0.1.2.0 (2023-08-04)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
-- Add functional configurations section to store UI-managed configurations ()
+- Add functional configurations section to store UI-managed configurations
 
 
 **Misc**
 
 - Move 'Deploy window' configuration to 'Misc' tab
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/security/ir.model.access.csv` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/description/index.html`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/description/index.html`

```diff
@@ -360,24 +360,24 @@
   <body>
     <div class="document" id="odoo-instance">
       <h1 class="title">Odoo Instance</h1>
       <!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !! This file is generated by oca-gen-addon-readme !!
 !! changes will be overwritten.                   !!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-!! source digest: sha256:7c0ac8707125bdc1a9968bbd602c1bf329692ce692a4fb148a900abcbf70839b
+!! source digest: sha256:18157e50fb2fc08b090dd3565b448d97228713b78045c938e37785d0b7ef0e4b
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->
       <p>
         <a class="reference external" href="https://odoo-community.org/page/development-status">
           <img alt="Beta" src="https://img.shields.io/badge/maturity-Beta-yellow.png"/>
         </a>
         <a class="reference external" href="http://www.gnu.org/licenses/agpl-3.0-standalone.html">
           <img alt="License: AGPL-3" src="https://img.shields.io/badge/licence-AGPL--3-blue.png"/>
         </a>
-        <a class="reference external" href="https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance">
+        <a class="reference external" href="https://git.coopdevs.org/coopdevs/odoo/odoo-addons/odoo14-addons/-/tree/14.0/odoo_instance">
           <img alt="coopdevs/odoo_instance" src="https://img.shields.io/badge/github-coopdevs%2Fodoo_instance-lightgray.png?logo=github"/>
         </a>
       </p>
       <p>This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.</p>
       <p>
         <strong>Features</strong>
       </p>
@@ -396,184 +396,198 @@
       </blockquote>
       <p>
         <strong>Table of contents</strong>
       </p>
       <div class="contents local topic" id="contents">
         <ul class="simple">
           <li>
-            <a class="reference internal" href="#changelog" id="id8">Changelog</a>
+            <a class="reference internal" href="#changelog" id="id9">Changelog</a>
             <ul>
               <li>
-                <a class="reference internal" href="#id1" id="id9">14.0.1.2.0 (2023-08-04)</a>
+                <a class="reference internal" href="#id1" id="id10">14.0.1.2.1 (2023-08-04)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id2" id="id10">14.0.1.2.0 (2023-04-26)</a>
+                <a class="reference internal" href="#id2" id="id11">14.0.1.2.0 (2023-08-04)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id3" id="id11">14.0.1.1.1 (2023-04-25)</a>
+                <a class="reference internal" href="#id3" id="id12">14.0.1.2.0 (2023-04-26)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id4" id="id12">14.0.1.1.0 (2023-04-25)</a>
+                <a class="reference internal" href="#id4" id="id13">14.0.1.1.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id5" id="id13">14.0.1.0.1 (2023-04-25)</a>
+                <a class="reference internal" href="#id5" id="id14">14.0.1.1.0 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id6" id="id14">14.0.1.0.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id6" id="id15">14.0.1.0.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id7" id="id15">14.0.0.2.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id7" id="id16">14.0.1.0.0 (2023-04-24)</a>
+              </li>
+              <li>
+                <a class="reference internal" href="#id8" id="id17">14.0.0.2.0 (2023-04-24)</a>
               </li>
             </ul>
           </li>
           <li>
-            <a class="reference internal" href="#bug-tracker" id="id16">Bug Tracker</a>
+            <a class="reference internal" href="#bug-tracker" id="id18">Bug Tracker</a>
           </li>
           <li>
-            <a class="reference internal" href="#credits" id="id17">Credits</a>
+            <a class="reference internal" href="#credits" id="id19">Credits</a>
             <ul>
               <li>
-                <a class="reference internal" href="#authors" id="id18">Authors</a>
+                <a class="reference internal" href="#authors" id="id20">Authors</a>
               </li>
               <li>
-                <a class="reference internal" href="#maintainers" id="id19">Maintainers</a>
+                <a class="reference internal" href="#maintainers" id="id21">Maintainers</a>
               </li>
             </ul>
           </li>
         </ul>
       </div>
       <div class="section" id="changelog">
         <h1>
-          <a class="toc-backref" href="#id8">Changelog</a>
+          <a class="toc-backref" href="#id9">Changelog</a>
         </h1>
         <div class="section" id="id1">
           <h2>
-            <a class="toc-backref" href="#id9">14.0.1.2.0 (2023-08-04)</a>
+            <a class="toc-backref" href="#id10">14.0.1.2.1 (2023-08-04)</a>
+          </h2>
+          <p>
+            <strong>Features</strong>
+          </p>
+          <ul class="simple">
+            <li>Add cron to update instances info</li>
+          </ul>
+        </div>
+        <div class="section" id="id2">
+          <h2>
+            <a class="toc-backref" href="#id11">14.0.1.2.0 (2023-08-04)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
-            <li>Add functional configurations section to store UI-managed configurations ()</li>
+            <li>Add functional configurations section to store UI-managed configurations</li>
           </ul>
           <p>
             <strong>Misc</strong>
           </p>
           <ul class="simple">
             <li>Move ‘Deploy window’ configuration to ‘Misc’ tab</li>
           </ul>
         </div>
-        <div class="section" id="id2">
+        <div class="section" id="id3">
           <h2>
-            <a class="toc-backref" href="#id10">14.0.1.2.0 (2023-04-26)</a>
+            <a class="toc-backref" href="#id12">14.0.1.2.0 (2023-04-26)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Manage databases</li>
           </ul>
         </div>
-        <div class="section" id="id3">
+        <div class="section" id="id4">
           <h2>
-            <a class="toc-backref" href="#id11">14.0.1.1.1 (2023-04-25)</a>
+            <a class="toc-backref" href="#id13">14.0.1.1.1 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Bugfixes</strong>
           </p>
           <ul class="simple">
             <li>Upcrate module versions</li>
             <li>Show installed module versions only in instance view</li>
           </ul>
         </div>
-        <div class="section" id="id4">
+        <div class="section" id="id5">
           <h2>
-            <a class="toc-backref" href="#id12">14.0.1.1.0 (2023-04-25)</a>
+            <a class="toc-backref" href="#id14">14.0.1.1.0 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Handle odoo releases</li>
           </ul>
         </div>
-        <div class="section" id="id5">
+        <div class="section" id="id6">
           <h2>
-            <a class="toc-backref" href="#id13">14.0.1.0.1 (2023-04-25)</a>
+            <a class="toc-backref" href="#id15">14.0.1.0.1 (2023-04-25)</a>
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
-        <div class="section" id="id6">
+        <div class="section" id="id7">
           <h2>
-            <a class="toc-backref" href="#id14">14.0.1.0.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id16">14.0.1.0.0 (2023-04-24)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Rename models and split logic in files</li>
           </ul>
         </div>
-        <div class="section" id="id7">
+        <div class="section" id="id8">
           <h2>
-            <a class="toc-backref" href="#id15">14.0.0.2.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id17">14.0.0.2.0 (2023-04-24)</a>
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
-          <a class="toc-backref" href="#id16">Bug Tracker</a>
+          <a class="toc-backref" href="#id18">Bug Tracker</a>
         </h1>
         <p>
           Bugs are tracked on
           <a class="reference external" href="https://github.com/coopdevs/odoo_instance/issues">GitHub Issues</a>
           .
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us to smash it by providing a detailed and welcomed
           <a class="reference external" href="https://github.com/coopdevs/odoo_instance/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>
           .
         </p>
         <p>Do not contact contributors directly about support or help with technical issues.</p>
       </div>
       <div class="section" id="credits">
         <h1>
-          <a class="toc-backref" href="#id17">Credits</a>
+          <a class="toc-backref" href="#id19">Credits</a>
         </h1>
         <div class="section" id="authors">
           <h2>
-            <a class="toc-backref" href="#id18">Authors</a>
+            <a class="toc-backref" href="#id20">Authors</a>
           </h2>
           <ul class="simple">
             <li>Coopdevs</li>
           </ul>
         </div>
         <div class="section" id="maintainers">
           <h2>
-            <a class="toc-backref" href="#id19">Maintainers</a>
+            <a class="toc-backref" href="#id21">Maintainers</a>
           </h2>
           <p>
             This module is part of the
-            <a class="reference external" href="https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance">coopdevs/odoo_instance</a>
+            <a class="reference external" href="https://git.coopdevs.org/coopdevs/odoo/odoo-addons/odoo14-addons/-/tree/14.0/odoo_instance">coopdevs/odoo_instance</a>
             project on GitHub.
           </p>
           <p>You are welcome to contribute.</p>
         </div>
       </div>
     </div>
   </body>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/static/src/img/icon.png` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/static/src/img/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_module_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_module_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_process_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_process_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_release_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_release_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/odoo_version_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/odoo_version_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/project_project_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/project_project_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/views/res_partner_view.xml` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo-instance
-Version: 14.0.1.2.0
+Version: 14.0.1.2.1
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 
 =============
@@ -16,25 +17,25 @@
 =============
 
 .. 
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-   !! source digest: sha256:7c0ac8707125bdc1a9968bbd602c1bf329692ce692a4fb148a900abcbf70839b
+   !! source digest: sha256:18157e50fb2fc08b090dd3565b448d97228713b78045c938e37785d0b7ef0e4b
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
-    :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
+    :target: https://git.coopdevs.org/coopdevs/odoo/odoo-addons/odoo14-addons/-/tree/14.0/odoo_instance
     :alt: coopdevs/odoo14-addons
 
 |badge1| |badge2| |badge3|
 
 This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
 
 **Features**
@@ -53,20 +54,28 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.1 (2023-08-04)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add cron to update instances info
+
+
 14.0.1.2.0 (2023-08-04)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
-- Add functional configurations section to store UI-managed configurations ()
+- Add functional configurations section to store UI-managed configurations
 
 
 **Misc**
 
 - Move 'Deploy window' configuration to 'Misc' tab
 
 
@@ -139,10 +148,12 @@
 ~~~~~~~
 
 * Coopdevs
 
 Maintainers
 ~~~~~~~~~~~
 
-This module is part of the `coopdevs/odoo_instance <https://github.com/coopdevs/odoo_instance/tree/14.0/odoo_instance>`_ project on GitHub.
+This module is part of the `coopdevs/odoo_instance <https://git.coopdevs.org/coopdevs/odoo/odoo-addons/odoo14-addons/-/tree/14.0/odoo_instance>`_ project.
 
 You are welcome to contribute.
+
+
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.2.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt` & `odoo14-addon-odoo_instance-14.0.1.2.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

