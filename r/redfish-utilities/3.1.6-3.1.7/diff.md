# Comparing `tmp/redfish_utilities-3.1.6.tar.gz` & `tmp/redfish_utilities-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_utilities-3.1.6.tar", last modified: Thu Jul 27 18:12:12 2023, max compression
+gzip compressed data, was "redfish_utilities-3.1.7.tar", last modified: Fri Aug  4 19:50:54 2023, max compression
```

## Comparing `redfish_utilities-3.1.6.tar` & `redfish_utilities-3.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42354 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:12:12.236746 redfish_utilities-3.1.6/redfish_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23508 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/resets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25527 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/redfish_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_bios_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_boot_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_diagnostic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_power_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_sensor_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_sys_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_virtual_media.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:54.028617 redfish_utilities-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-08-04 19:50:54.028617 redfish_utilities-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42354 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:54.024617 redfish_utilities-3.1.7/redfish_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23508 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/resets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25527 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/redfish_utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:54.024617 redfish_utilities-3.1.7/redfish_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-08-04 19:50:53.000000 redfish_utilities-3.1.7/redfish_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 19:50:53.000000 redfish_utilities-3.1.7/redfish_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:50:53.000000 redfish_utilities-3.1.7/redfish_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 19:50:53.000000 redfish_utilities-3.1.7/redfish_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 19:50:53.000000 redfish_utilities-3.1.7/redfish_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:54.024617 redfish_utilities-3.1.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_bios_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_boot_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_diagnostic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_power_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_sensor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_sys_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/scripts/rf_virtual_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:50:54.028617 redfish_utilities-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-04 19:50:39.000000 redfish_utilities-3.1.7/setup.py
```

### Comparing `redfish_utilities-3.1.6/LICENSE.md` & `redfish_utilities-3.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/PKG-INFO` & `redfish_utilities-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_utilities
-Version: 3.1.6
+Version: 3.1.7
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_utilities-3.1.6/README.md` & `redfish_utilities-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/__init__.py` & `redfish_utilities-3.1.7/redfish_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/accounts.py` & `redfish_utilities-3.1.7/redfish_utilities/accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/collections.py` & `redfish_utilities-3.1.7/redfish_utilities/collections.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/config.py` & `redfish_utilities-3.1.7/redfish_utilities/config.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/event_service.py` & `redfish_utilities-3.1.7/redfish_utilities/event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/inventory.py` & `redfish_utilities-3.1.7/redfish_utilities/inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/licenses.py` & `redfish_utilities-3.1.7/redfish_utilities/licenses.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/logs.py` & `redfish_utilities-3.1.7/redfish_utilities/logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/managers.py` & `redfish_utilities-3.1.7/redfish_utilities/managers.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/messages.py` & `redfish_utilities-3.1.7/redfish_utilities/messages.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/resets.py` & `redfish_utilities-3.1.7/redfish_utilities/resets.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/sensors.py` & `redfish_utilities-3.1.7/redfish_utilities/sensors.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/systems.py` & `redfish_utilities-3.1.7/redfish_utilities/systems.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/tasks.py` & `redfish_utilities-3.1.7/redfish_utilities/tasks.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities/update.py` & `redfish_utilities-3.1.7/redfish_utilities/update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/redfish_utilities.egg-info/PKG-INFO` & `redfish_utilities-3.1.7/redfish_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish-utilities
-Version: 3.1.6
+Version: 3.1.7
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_utilities-3.1.6/redfish_utilities.egg-info/SOURCES.txt` & `redfish_utilities-3.1.7/redfish_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/scripts/rf_accounts.py` & `redfish_utilities-3.1.7/scripts/rf_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to manage user accounts on a Redfish service" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--add", "-add", type = str, nargs = 3, metavar = ( "name", "password", "role" ), help = "Adds a new user account" )
@@ -86,8 +87,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_bios_settings.py` & `redfish_utilities-3.1.7/scripts/rf_bios_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to manager BIOS settings for a system" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--system", "-s", type = str, help = "The ID of the system to manage" )
@@ -77,8 +78,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_boot_override.py` & `redfish_utilities-3.1.7/scripts/rf_boot_override.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to perform a one time boot override of a system" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--system", "-s", type = str, help = "The ID of the system to set" )
@@ -80,8 +81,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_diagnostic_data.py` & `redfish_utilities-3.1.7/scripts/rf_diagnostic_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import argparse
 import datetime
 import logging
 import os
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to collect diagnostic data from a log service on a Redfish service" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--manager", "-m", type = str, nargs = "?", default = False, help = "The ID of the manager containing the log service" )
@@ -85,8 +86,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_discover.py` & `redfish_utilities-3.1.7/scripts/rf_discover.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.6/scripts/rf_event_service.py` & `redfish_utilities-3.1.7/scripts/rf_event_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to manage the event service on a Redfish service" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
@@ -67,8 +68,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_licenses.py` & `redfish_utilities-3.1.7/scripts/rf_licenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to manage licenses on a Redfish service" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
@@ -65,8 +66,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_logs.py` & `redfish_utilities-3.1.7/scripts/rf_logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to manage logs on a Redfish service" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--manager", "-m", type = str, nargs = "?", default = False, help = "The ID of the manager containing the log service" )
@@ -73,8 +74,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_manager_config.py` & `redfish_utilities-3.1.7/scripts/rf_manager_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to manage managers in a service" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--manager", "-m", type = str, help = "The ID of the manager to target" )
@@ -156,8 +157,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_power_reset.py` & `redfish_utilities-3.1.7/scripts/rf_power_reset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to perform a power/reset operation of a system" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--system", "-s", type = str, help = "The ID of the system to reset" )
@@ -64,8 +65,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_raw_request.py` & `redfish_utilities-3.1.7/scripts/rf_raw_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,26 +11,38 @@
 Brief : This script performs a raw request specified by the user
 """
 
 import argparse
 import json
 import os
 import redfish
+import re
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool perform a raw request to a Redfish service" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--method", "-m", type = str, required = False, help = "The HTTP method to perform; performs GET if not specified", default = "GET", choices = [ "GET", "HEAD", "POST", "PATCH", "PUT", "DELETE" ] )
 argget.add_argument( "--request", "-req", type = str, required = True, help = "The URI for the request" )
 argget.add_argument( "--body", "-b", type = str, required = False, help = "The body to provide with the request; can be a JSON string for a JSON request, a filename to send binary data, or an unstructured string" )
 argget.add_argument( "--verbose", "-v", action = "store_true", help = "Indicates if HTTP response codes and headers are displayed", default = False )
 args = argget.parse_args()
 
+def ifmatch_header(redfish_obj, path, headers=None):
+    if headers is None:
+        headers = {}
+    try:
+        response = redfish_obj.get(path)
+        etag = response.getheader( "ETag" )
+        if etag is not None:
+            headers[ "If-Match"] = etag
+    except Exception:
+        pass
+    return headers
 # Connect to the service
 with redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password ) as redfish_obj:
     # Encode the body
     # If the body argument points to a file, load the file
     if args.body is not None and os.path.isfile( args.body ):
         with open( args.body, mode="rb" ) as file:
             body = file.read()
@@ -46,17 +58,19 @@
 
     # Perform the requested operation
     if args.method == "HEAD":
         resp = redfish_obj.head( args.request )
     elif args.method == "POST":
         resp = redfish_obj.post( args.request, body = body )
     elif args.method == "PATCH":
-        resp = redfish_obj.patch( args.request, body = body )
+	headers = ifmatch_header(redfish_obj, args.request, headers = headers)
+        resp = redfish_obj.patch( args.request, body = body, headers = headers)
     elif args.method == "PUT":
-        resp = redfish_obj.put( args.request, body = body )
+	headers = ifmatch_header(redfish_obj, args.request, headers = headers)
+        resp = redfish_obj.put( args.request, body = body, headers = headers)
     elif args.method == "DELETE":
         resp = redfish_obj.delete( args.request )
     else:
         resp = redfish_obj.get( args.request )
 
     # Print HTTP status and headers
     if args.verbose:
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_sensor_list.py` & `redfish_utilities-3.1.7/scripts/rf_sensor_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to walk a Redfish service and list sensor info" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
@@ -45,8 +46,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_sys_inventory.py` & `redfish_utilities-3.1.7/scripts/rf_sys_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to walk a Redfish service and list component information" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--details", "-details", action = "store_true", help = "Indicates if the full details of each component should be shown" )
@@ -56,8 +57,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_update.py` & `redfish_utilities-3.1.7/scripts/rf_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,8 @@
     # Log out and cleanup
     os.chdir( start_path )
     try:
         shutil.rmtree( WEB_SERVER_FOLDER )
     except:
         pass
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

### Comparing `redfish_utilities-3.1.6/scripts/rf_virtual_media.py` & `redfish_utilities-3.1.7/scripts/rf_virtual_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
+import sys
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool to manage virtual media of a system" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--system", "-s", type = str, help = "The ID of the system containing the virtual media" )
@@ -62,8 +63,8 @@
     if args.debug:
         logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
     exit_code = 1
     print( e )
 finally:
     # Log out
     redfish_obj.logout()
-exit( exit_code )
+sys.exit( exit_code )
```

