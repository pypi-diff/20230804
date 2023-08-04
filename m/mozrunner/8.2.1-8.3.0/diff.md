# Comparing `tmp/mozrunner-8.2.1.tar.gz` & `tmp/mozrunner-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozrunner-8.2.1.tar", last modified: Fri Jun  4 20:00:02 2021, max compression
+gzip compressed data, was "mozrunner-8.3.0.tar", last modified: Fri Aug  4 07:23:54 2023, max compression
```

## Comparing `mozrunner-8.2.1.tar` & `mozrunner-8.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2021-06-04 20:00:02.000000 mozrunner-8.2.1/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1698 2021-06-04 09:37:46.000000 mozrunner-8.2.1/setup.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      859 2021-06-04 20:00:02.000000 mozrunner-8.2.1/PKG-INFO
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner.egg-info/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       93 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner.egg-info/entry_points.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2021-05-28 18:53:51.000000 mozrunner-8.2.1/mozrunner.egg-info/not-zip-safe
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner.egg-info/dependency_links.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      136 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner.egg-info/requires.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       10 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner.egg-info/top_level.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      859 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner.egg-info/PKG-INFO
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      708 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner.egg-info/SOURCES.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       67 2021-06-04 20:00:02.000000 mozrunner-8.2.1/setup.cfg
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5700 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/cli.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner/devices/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    38302 2021-04-22 11:44:00.000000 mozrunner-8.2.1/mozrunner/devices/android_device.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3518 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/devices/emulator_screen.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      595 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/devices/emulator_geo.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     7413 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/devices/emulator.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1643 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/devices/emulator_battery.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     9123 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/devices/base.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      585 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/devices/__init__.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4652 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/application.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5231 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/runners.py
--rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)    10204 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/utils.py
--rw-r--r--   0 jgraham   (1000) jgraham   (1000)      390 2018-10-20 23:26:05.000000 mozrunner-8.2.1/mozrunner/__init__.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2021-06-04 20:00:02.000000 mozrunner-8.2.1/mozrunner/base/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     9028 2021-05-21 18:54:50.000000 mozrunner-8.2.1/mozrunner/base/runner.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     6612 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/base/device.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      393 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/base/__init__.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4428 2021-01-11 15:46:26.000000 mozrunner-8.2.1/mozrunner/base/browser.py
--rw-r--r--   0 jgraham   (1000) jgraham   (1000)      575 2018-10-20 23:26:05.000000 mozrunner-8.2.1/mozrunner/errors.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      829 2023-08-04 07:23:54.403684 mozrunner-8.3.0/PKG-INFO
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/mozrunner/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      350 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4610 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/application.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/mozrunner/base/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      353 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/base/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4389 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/base/browser.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     6556 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/base/device.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     8839 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/base/runner.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5644 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/cli.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/mozrunner/devices/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      487 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    36892 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/android_device.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     9067 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/base.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     7373 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/emulator.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1593 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/emulator_battery.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      555 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/emulator_geo.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3478 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/devices/emulator_screen.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      535 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/errors.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5191 2023-02-28 20:00:23.000000 mozrunner-8.3.0/mozrunner/runners.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)    10403 2023-07-06 08:37:51.000000 mozrunner-8.3.0/mozrunner/utils.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-08-04 07:23:54.403684 mozrunner-8.3.0/mozrunner.egg-info/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      829 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/PKG-INFO
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      708 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       44 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/entry_points.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2023-08-01 11:17:05.000000 mozrunner-8.3.0/mozrunner.egg-info/not-zip-safe
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      136 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/requires.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       10 2023-08-04 07:23:54.000000 mozrunner-8.3.0/mozrunner.egg-info/top_level.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       67 2023-08-04 07:23:54.407684 mozrunner-8.3.0/setup.cfg
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1658 2023-08-03 14:51:45.000000 mozrunner-8.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mozrunner-8.2.1/setup.py` & `mozrunner-8.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 PACKAGE_NAME = "mozrunner"
-PACKAGE_VERSION = "8.2.1"
+PACKAGE_VERSION = "8.3.0"
 
 desc = """Reliable start/stop/configuration of Mozilla Applications (Firefox, Thunderbird, etc.)"""
 
 deps = [
     "mozdevice>=4.0.0,<5",
     "mozfile>=1.2",
     "mozinfo>=0.7,<2",
```

### Comparing `mozrunner-8.2.1/PKG-INFO` & `mozrunner-8.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mozrunner
-Version: 8.2.1
+Version: 8.3.0
 Summary: Reliable start/stop/configuration of Mozilla Applications (Firefox, Thunderbird, etc.)
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
-Description: see https://firefox-source-docs.mozilla.org/mozbase/index.html
 Keywords: mozilla
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: crash
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
```

### Comparing `mozrunner-8.2.1/mozrunner.egg-info/PKG-INFO` & `mozrunner-8.3.0/mozrunner.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mozrunner
-Version: 8.2.1
+Version: 8.3.0
 Summary: Reliable start/stop/configuration of Mozilla Applications (Firefox, Thunderbird, etc.)
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
-Description: see https://firefox-source-docs.mozilla.org/mozbase/index.html
 Keywords: mozilla
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: crash
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
```

### Comparing `mozrunner-8.2.1/mozrunner.egg-info/SOURCES.txt` & `mozrunner-8.3.0/mozrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozrunner-8.2.1/mozrunner/cli.py` & `mozrunner-8.3.0/mozrunner/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function
-
 import os
 import sys
 
 from mozprofile import MozProfileCLI
 
 from .application import get_app_context
 from .runners import runners
```

### Comparing `mozrunner-8.2.1/mozrunner/devices/android_device.py` & `mozrunner-8.3.0/mozrunner/devices/android_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function
-
 import glob
 import os
 import platform
 import posixpath
 import re
 import shutil
 import signal
-import six
 import subprocess
 import sys
 import telnetlib
 import time
 from distutils.spawn import find_executable
 from enum import Enum
 
-from mozbuild.base import MozbuildObject
-from mozdevice import ADBHost, ADBDeviceFactory
+import six
+from mozdevice import ADBDeviceFactory, ADBHost
 from six.moves import input, urllib
 
-EMULATOR_HOME_DIR = os.path.join(os.path.expanduser("~"), ".mozbuild", "android-device")
+MOZBUILD_PATH = os.environ.get(
+    "MOZBUILD_STATE_PATH", os.path.expanduser(os.path.join("~", ".mozbuild"))
+)
+
+EMULATOR_HOME_DIR = os.path.join(MOZBUILD_PATH, "android-device")
 
 EMULATOR_AUTH_FILE = os.path.join(
     os.path.expanduser("~"), ".emulator_console_auth_token"
 )
 
-TOOLTOOL_PATH = "testing/mozharness/external_tools/tooltool.py"
+TOOLTOOL_PATH = "python/mozbuild/mozbuild/action/tooltool.py"
 
 TRY_URL = "https://hg.mozilla.org/try/raw-file/default"
 
 MANIFEST_PATH = "testing/config/tooltool-manifests"
 
 SHORT_TIMEOUT = 10
 
@@ -80,59 +81,98 @@
 
 
 class AvdInfo(object):
     """
     Simple class to contain an AVD description.
     """
 
-    def __init__(
-        self, description, name, tooltool_manifest, toolchain_job, extra_args, x86
-    ):
-        assert not (tooltool_manifest and toolchain_job), (
-            "%s: specify manifest or toolchain job, not both" % description
-        )
+    def __init__(self, description, name, extra_args, x86):
         self.description = description
         self.name = name
-        self.tooltool_manifest = tooltool_manifest
-        self.toolchain_job = toolchain_job
         self.extra_args = extra_args
         self.x86 = x86
 
 
 """
    A dictionary to map an AVD type to a description of that type of AVD.
 
    There is one entry for each type of AVD used in Mozilla automated tests
    and the parameters for each reflect those used in mozharness.
 """
 AVD_DICT = {
-    "arm-4.3": AvdInfo(
-        "Android 4.3",
-        "mozemulator-4.3",
-        "testing/config/tooltool-manifests/androidarm_4_3/mach-emulator.manifest",
-        None,
-        ["-skip-adb-auth", "-verbose", "-show-kernel"],
+    "arm": AvdInfo(
+        "Android arm",
+        "mozemulator-armeabi-v7a",
+        [
+            "-skip-adb-auth",
+            "-verbose",
+            "-show-kernel",
+            "-ranchu",
+            "-selinux",
+            "permissive",
+            "-memory",
+            "3072",
+            "-cores",
+            "4",
+            "-skin",
+            "800x1280",
+            "-gpu",
+            "on",
+            "-no-snapstorage",
+            "-no-snapshot",
+            "-prop",
+            "ro.test_harness=true",
+        ],
         False,
     ),
-    "x86-7.0": AvdInfo(
-        "Android 7.0 x86/x86_64",
-        "mozemulator-x86-7.0",
-        "testing/config/tooltool-manifests/androidx86_7_0/mach-emulator.manifest",
-        None,
+    "arm64": AvdInfo(
+        "Android arm64",
+        "mozemulator-arm64",
         [
             "-skip-adb-auth",
             "-verbose",
             "-show-kernel",
             "-ranchu",
             "-selinux",
             "permissive",
             "-memory",
             "3072",
             "-cores",
             "4",
+            "-skin",
+            "800x1280",
+            "-gpu",
+            "on",
+            "-no-snapstorage",
+            "-no-snapshot",
+            "-prop",
+            "ro.test_harness=true",
+        ],
+        False,
+    ),
+    "x86_64": AvdInfo(
+        "Android x86_64",
+        "mozemulator-x86_64",
+        [
+            "-skip-adb-auth",
+            "-verbose",
+            "-show-kernel",
+            "-ranchu",
+            "-selinux",
+            "permissive",
+            "-memory",
+            "3072",
+            "-cores",
+            "4",
+            "-skin",
+            "800x1280",
+            "-prop",
+            "ro.test_harness=true",
+            "-no-snapstorage",
+            "-no-snapshot",
         ],
         True,
     ),
 }
 
 
 def _get_device(substs, device_serial=None):
@@ -160,15 +200,16 @@
         xre_path = glob.glob(os.path.join(EMULATOR_HOME_DIR, "host-utils*"))
         for path in xre_path:
             if os.path.isdir(path) and os.path.isfile(
                 os.path.join(path, _get_xpcshell_name())
             ):
                 os.environ["MOZ_HOST_BIN"] = path
                 installed = True
-                break
+            elif os.path.isfile(path):
+                os.remove(path)
         if not installed:
             _log_warning("Unable to install host utilities.")
     else:
         _log_warning(
             "Unable to install host utilities -- your platform is not supported!"
         )
 
@@ -216,15 +257,17 @@
                 m = re.search('.*"(host-utils-.*)"', line)
                 if m:
                     manifest_version = m.group(1)
                     break
 
     # Compare, prompt, update
     if existing_version and manifest_version:
-        manifest_version = manifest_version[: len(existing_version)]
+        hu_version_regex = "host-utils-([\d\.]*)"
+        manifest_version = float(re.search(hu_version_regex, manifest_version).group(1))
+        existing_version = float(re.search(hu_version_regex, existing_version).group(1))
         if existing_version < manifest_version:
             _log_info("Your host utilities are out of date!")
             _log_info(
                 "You have %s installed, but %s is available"
                 % (existing_version, manifest_version)
             )
             response = input("Update host utilities? (Y/n) ").strip()
@@ -241,14 +284,15 @@
     install=InstallIntent.NO,
     xre=False,
     debugger=False,
     network=False,
     verbose=False,
     app=None,
     device_serial=None,
+    aab=False,
 ):
     """
     Determine if any Android device is connected via adb.
     If no device is found, prompt to start an emulator.
     If a device is found or an emulator started and 'install' is
     specified, also check whether Firefox is installed on the
     device; if not, prompt to install Firefox.
@@ -279,16 +323,16 @@
         device_verified = True
     elif emulator.is_available():
         response = input(
             "No Android devices connected. Start an emulator? (Y/n) "
         ).strip()
         if response.lower().startswith("y") or response == "":
             if not emulator.check_avd():
-                _log_info("Fetching AVD...")
-                emulator.update_avd()
+                _log_info("Android AVD not found, please run |mach bootstrap|")
+                return
             _log_info(
                 "Starting emulator running %s..." % emulator.get_avd_description()
             )
             emulator.start()
             emulator.wait_for_start()
             device_verified = True
 
@@ -309,15 +353,15 @@
         # If a test app is installed, there is no way to determine whether
         # the current build is installed, and certainly no way to
         # determine if the installed build is the desired build.
         # Installing every time (without prompting) is problematic because:
         #  - it prevents testing against other builds (downloaded apk)
         #  - installation may take a couple of minutes.
         if not app:
-            app = "org.mozilla.geckoview.test"
+            app = "org.mozilla.geckoview.test_runner"
         device = _get_device(build_obj.substs, device_serial)
         response = ""
         installed = device.is_app_installed(app)
 
         if not installed:
             _log_info("It looks like %s is not installed on this device." % app)
         if "fennec" in app or "firefox" in app:
@@ -325,23 +369,39 @@
                 device.uninstall_app(app)
             _log_info("Installing Firefox...")
             build_obj._run_make(directory=".", target="install", ensure_exit_code=False)
         elif app == "org.mozilla.geckoview.test":
             if installed:
                 device.uninstall_app(app)
             _log_info("Installing geckoview AndroidTest...")
-            sub = "geckoview:installWithGeckoBinariesDebugAndroidTest"
             build_obj._mach_context.commands.dispatch(
-                "gradle", build_obj._mach_context, args=[sub]
+                "android",
+                build_obj._mach_context,
+                subcommand="install-geckoview-test",
+                args=[],
+            )
+        elif app == "org.mozilla.geckoview.test_runner":
+            if installed:
+                device.uninstall_app(app)
+            _log_info("Installing geckoview test_runner...")
+            sub = (
+                "install-geckoview-test_runner-aab"
+                if aab
+                else "install-geckoview-test_runner"
+            )
+            build_obj._mach_context.commands.dispatch(
+                "android", build_obj._mach_context, subcommand=sub, args=[]
             )
         elif app == "org.mozilla.geckoview_example":
             if installed:
                 device.uninstall_app(app)
             _log_info("Installing geckoview_example...")
-            sub = "install-geckoview_example"
+            sub = (
+                "install-geckoview_example-aab" if aab else "install-geckoview_example"
+            )
             build_obj._mach_context.commands.dispatch(
                 "android", build_obj._mach_context, subcommand=sub, args=[]
             )
         elif not installed:
             response = input(
                 "It looks like %s is not installed on this device,\n"
                 "but I don't know how to install it.\n"
@@ -511,15 +571,15 @@
 def get_adb_path(build_obj):
     return _find_sdk_exe(build_obj.substs, "adb", False)
 
 
 def grant_runtime_permissions(build_obj, app, device_serial=None):
     """
     Grant required runtime permissions to the specified app
-    (eg. org.mozilla.geckoview.test).
+    (eg. org.mozilla.geckoview.test_runner).
     """
     device = _get_device(build_obj.substs, device_serial)
     device.run_as_package = app
     device.grant_runtime_permissions(app)
 
 
 class AndroidEmulator(object):
@@ -527,15 +587,15 @@
     Support running the Android emulator with an AVD from Mozilla
     test automation.
 
     Example usage:
         emulator = AndroidEmulator()
         if not emulator.is_running() and emulator.is_available():
             if not emulator.check_avd():
-                emulator.update_avd()
+                print("Android Emulator AVD not found, please run |mach bootstrap|")
             emulator.start()
             emulator.wait_for_start()
             emulator.wait()
     """
 
     def __init__(self, avd_type=None, verbose=False, substs=None, device_serial=None):
         global verbose_logging
@@ -544,14 +604,17 @@
         verbose_logging = verbose
         self.substs = substs
         self.avd_type = self._get_avd_type(avd_type)
         self.avd_info = AVD_DICT[self.avd_type]
         self.gpu = True
         self.restarted = False
         self.device_serial = device_serial
+        self.avd_path = os.path.join(
+            EMULATOR_HOME_DIR, "avd", "%s.avd" % self.avd_info.name
+        )
         _log_debug("Running on %s" % platform.platform())
         _log_debug("Emulator created with type %s" % self.avd_type)
 
     def __del__(self):
         if self.emulator_log:
             self.emulator_log.close()
 
@@ -577,78 +640,42 @@
         found = False
         emulator_path = _find_sdk_exe(self.substs, "emulator", True)
         if emulator_path:
             self.emulator_path = emulator_path
             found = True
         return found
 
-    def check_avd(self, force=False):
+    def check_avd(self):
         """
         Determine if the AVD is already installed locally.
-        (This is usually used to determine if update_avd() is likely
-        to require a download.)
 
         Returns True if the AVD is installed.
         """
-        avd = os.path.join(EMULATOR_HOME_DIR, "avd", self.avd_info.name + ".avd")
-        if force and os.path.exists(avd):
-            shutil.rmtree(avd)
-        if os.path.exists(avd):
-            _log_debug("AVD found at %s" % avd)
+        if os.path.exists(self.avd_path):
+            _log_debug("AVD found at %s" % self.avd_path)
             return True
+        _log_warning("Could not find AVD at %s" % self.avd_path)
         return False
 
-    def update_avd(self, force=False):
-        """
-        If required, update the AVD via tooltool.
-
-        If the AVD directory is not found, or "force" is requested,
-        download the tooltool manifest associated with the AVD and then
-        invoke tooltool.py on the manifest. tooltool.py will download the
-        required archive (unless already present in the local tooltool
-        cache) and install the AVD.
-        """
-        avd = os.path.join(EMULATOR_HOME_DIR, "avd", self.avd_info.name + ".avd")
-        ini_file = os.path.join(EMULATOR_HOME_DIR, "avd", self.avd_info.name + ".ini")
-        if force and os.path.exists(avd):
-            shutil.rmtree(avd)
-        if force:
-            for f in glob.glob(os.path.join(EMULATOR_HOME_DIR, "AVD*.checksum")):
-                os.remove(f)
-        if not os.path.exists(avd):
-            if os.path.exists(ini_file):
-                os.remove(ini_file)
-            if self.avd_info.tooltool_manifest:
-                path = self.avd_info.tooltool_manifest
-                _get_tooltool_manifest(
-                    self.substs, path, EMULATOR_HOME_DIR, "releng.manifest"
-                )
-                _tooltool_fetch(self.substs)
-            elif self.avd_info.toolchain_job:
-                _install_toolchain_artifact(self.avd_info.toolchain_job)
-            else:
-                raise Exception(
-                    "either a tooltool manifest or a toolchain job is required"
-                )
-            self._update_avd_paths()
-
     def start(self, gpu_arg=None):
         """
         Launch the emulator.
         """
         if self.avd_info.x86 and "linux" in _get_host_platform():
             _verify_kvm(self.substs)
         if os.path.exists(EMULATOR_AUTH_FILE):
             os.remove(EMULATOR_AUTH_FILE)
             _log_debug("deleted %s" % EMULATOR_AUTH_FILE)
+        self._update_avd_paths()
         # create an empty auth file to disable emulator authentication
         auth_file = open(EMULATOR_AUTH_FILE, "w")
         auth_file.close()
 
         env = os.environ
+        env["ANDROID_EMULATOR_HOME"] = EMULATOR_HOME_DIR
         env["ANDROID_AVD_HOME"] = os.path.join(EMULATOR_HOME_DIR, "avd")
         command = [self.emulator_path, "-avd", self.avd_info.name]
         override = os.environ.get("MOZ_EMULATOR_COMMAND_ARGS")
         if override:
             command += override.split()
             _log_debug("Found MOZ_EMULATOR_COMMAND_ARGS in env: %s" % override)
         else:
@@ -783,31 +810,21 @@
     def get_avd_description(self):
         """
         Return the human-friendly description of this AVD.
         """
         return self.avd_info.description
 
     def _update_avd_paths(self):
-        avd_path = os.path.join(EMULATOR_HOME_DIR, "avd")
-        ini_file = os.path.join(avd_path, "test-1.ini")
-        ini_file_new = os.path.join(avd_path, self.avd_info.name + ".ini")
-        os.rename(ini_file, ini_file_new)
-        avd_dir = os.path.join(avd_path, "test-1.avd")
-        avd_dir_new = os.path.join(avd_path, self.avd_info.name + ".avd")
-        os.rename(avd_dir, avd_dir_new)
-        self._replace_ini_contents(ini_file_new)
-
-    def _replace_ini_contents(self, path):
-        with open(path, "r") as f:
+        ini_path = os.path.join(EMULATOR_HOME_DIR, "avd", "%s.ini" % self.avd_info.name)
+        with open(ini_path, "r") as f:
             lines = f.readlines()
-        with open(path, "w") as f:
+        with open(ini_path, "w") as f:
             for line in lines:
                 if line.startswith("path="):
-                    avd_path = os.path.join(EMULATOR_HOME_DIR, "avd")
-                    f.write("path=%s/%s.avd\n" % (avd_path, self.avd_info.name))
+                    f.write("path=%s\n" % self.avd_path)
                 elif line.startswith("path.rel="):
                     f.write("path.rel=avd/%s.avd\n" % self.avd_info.name)
                 else:
                     f.write(line)
 
     def _telnet_read_until(self, telnet, expected, timeout):
         if six.PY3 and isinstance(expected, six.text_type):
@@ -854,19 +871,20 @@
                     return False
         return telnet_ok
 
     def _get_avd_type(self, requested):
         if requested in AVD_DICT.keys():
             return requested
         if self.substs:
-            if not self.substs["TARGET_CPU"].startswith("arm"):
-                return "x86-7.0"
-            else:
-                return "arm-4.3"
-        return "x86-7.0"
+            target_cpu = self.substs["TARGET_CPU"]
+            if target_cpu == "aarch64":
+                return "arm64"
+            elif target_cpu.startswith("arm"):
+                return "arm"
+        return "x86_64"
 
 
 def _find_sdk_exe(substs, exe, tools):
     if tools:
         subdirs = ["emulator", "tools"]
     else:
         subdirs = ["platform-tools"]
@@ -901,19 +919,16 @@
                 else:
                     _log_debug("Unable to find executable at %s" % exe_path)
         except KeyError:
             _log_debug("ANDROID_SDK_ROOT not set")
 
     if not found:
         # Can exe be found in the default bootstrap location?
-        mozbuild_path = os.environ.get(
-            "MOZBUILD_STATE_PATH", os.path.expanduser(os.path.join("~", ".mozbuild"))
-        )
         for subdir in subdirs:
-            exe_path = os.path.join(mozbuild_path, "android-sdk-linux", subdir, exe)
+            exe_path = os.path.join(MOZBUILD_PATH, "android-sdk-linux", subdir, exe)
             if os.path.exists(exe_path):
                 found = True
                 break
             else:
                 _log_debug("Unable to find executable at %s" % exe_path)
 
     if not found:
@@ -1008,42 +1023,14 @@
     try:
         response = subprocess.check_output(command, cwd=EMULATOR_HOME_DIR)
         _log_debug(response)
     except Exception as e:
         _log_warning(str(e))
 
 
-def _install_toolchain_artifact(toolchain_job, no_unpack=False):
-    build_obj = MozbuildObject.from_environment()
-    mach_binary = os.path.join(build_obj.topsrcdir, "mach")
-    mach_binary = os.path.abspath(mach_binary)
-    if not os.path.exists(mach_binary):
-        raise ValueError("mach not found at %s" % mach_binary)
-
-    # If Python can't figure out what its own executable is, there's little
-    # chance we're going to be able to execute mach on its own, particularly
-    # on Windows.
-    if not sys.executable:
-        raise ValueError("cannot determine path to Python executable")
-
-    cmd = [
-        sys.executable,
-        mach_binary,
-        "artifact",
-        "toolchain",
-        "--from-build",
-        toolchain_job,
-    ]
-
-    if no_unpack:
-        cmd += ["--no-unpack"]
-
-    subprocess.check_call(cmd, cwd=EMULATOR_HOME_DIR)
-
-
 def _get_host_platform():
     plat = None
     if "darwin" in str(sys.platform).lower():
         plat = "macosx64"
     elif "win32" in str(sys.platform).lower():
         plat = "win32"
     elif "linux" in str(sys.platform).lower():
```

### Comparing `mozrunner-8.2.1/mozrunner/devices/emulator_screen.py` & `mozrunner-8.3.0/mozrunner/devices/emulator_screen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 
 class EmulatorScreen(object):
     """Class for screen related emulator commands."""
 
     SO_PORTRAIT_PRIMARY = "portrait-primary"
     SO_PORTRAIT_SECONDARY = "portrait-secondary"
     SO_LANDSCAPE_PRIMARY = "landscape-primary"
```

### Comparing `mozrunner-8.2.1/mozrunner/devices/emulator_geo.py` & `mozrunner-8.3.0/mozrunner/devices/emulator_geo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 
 class EmulatorGeo(object):
     def __init__(self, emulator):
         self.emulator = emulator
 
     def set_default_location(self):
         self.lon = -122.08769
```

### Comparing `mozrunner-8.2.1/mozrunner/devices/emulator.py` & `mozrunner-8.3.0/mozrunner/devices/emulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-from telnetlib import Telnet
 import datetime
 import os
 import shutil
 import subprocess
 import tempfile
 import time
+from telnetlib import Telnet
 
 from mozdevice import ADBHost
 from mozprocess import ProcessHandler
 
+from ..errors import TimeoutException
 from .base import Device
 from .emulator_battery import EmulatorBattery
 from .emulator_geo import EmulatorGeo
 from .emulator_screen import EmulatorScreen
-from ..errors import TimeoutException
 
 
 class ArchContext(object):
     def __init__(self, arch, context, binary=None, avd=None, extra_args=None):
         homedir = getattr(context, "homedir", "")
         kernel = os.path.join(homedir, "prebuilts", "qemu-kernel", "%s", "%s")
         sysdir = os.path.join(homedir, "out", "target", "product", "%s")
```

### Comparing `mozrunner-8.2.1/mozrunner/devices/emulator_battery.py` & `mozrunner-8.3.0/mozrunner/devices/emulator_battery.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, division
-
 
 class EmulatorBattery(object):
     def __init__(self, emulator):
         self.emulator = emulator
 
     def get_state(self):
         status = {}
```

### Comparing `mozrunner-8.2.1/mozrunner/devices/base.py` & `mozrunner-8.3.0/mozrunner/devices/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function
-
 import datetime
 import os
 import posixpath
 import shutil
 import tempfile
 import time
 
-from mozdevice import ADBHost, ADBError
+from mozdevice import ADBError, ADBHost
 from six.moves.configparser import ConfigParser, RawConfigParser
 
 
 class Device(object):
     connected = False
 
     def __init__(self, app_ctx, logdir=None, serial=None, restore=True):
```

### Comparing `mozrunner-8.2.1/mozrunner/application.py` & `mozrunner-8.3.0/mozrunner/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-import six
-from abc import ABCMeta, abstractmethod
-from distutils.spawn import find_executable
 import os
 import posixpath
+from abc import ABCMeta, abstractmethod
+from distutils.spawn import find_executable
 
+import six
 from mozdevice import ADBDeviceFactory
 from mozprofile import (
-    Profile,
     ChromeProfile,
     ChromiumProfile,
     FirefoxProfile,
+    Profile,
     ThunderbirdProfile,
 )
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 def get_app_context(appname):
@@ -90,15 +88,15 @@
             paths.insert(0, os.path.abspath(self.bindir))
             os.environ["PATH"] = os.pathsep.join(paths)
 
         return find_executable(binary)
 
     @abstractmethod
     def stop_application(self):
-        """ Run (device manager) command to stop application. """
+        """Run (device manager) command to stop application."""
         pass
 
 
 devices = {}
 
 
 class FennecContext(RemoteContext):
```

### Comparing `mozrunner-8.2.1/mozrunner/runners.py` & `mozrunner-8.3.0/mozrunner/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 
 
 """
 This module contains a set of shortcut methods that create runners for commonly
 used Mozilla applications, such as Firefox, Firefox for Android or Thunderbird.
 """
 
-from __future__ import absolute_import
-
 from .application import get_app_context
-from .base import GeckoRuntimeRunner, FennecRunner, BlinkRuntimeRunner
+from .base import BlinkRuntimeRunner, FennecRunner, GeckoRuntimeRunner
 from .devices import EmulatorAVD
 
 
 def Runner(*args, **kwargs):
     """
     Create a generic GeckoRuntime runner.
 
@@ -93,15 +91,15 @@
     :param cmdargs: Arguments to pass into the binary.
     """
     kwargs["app_ctx"] = get_app_context("chromium")()
     return BlinkRuntimeRunner(*args, **kwargs)
 
 
 def FennecEmulatorRunner(
-    avd="mozemulator-4.3",
+    avd="mozemulator-arm",
     adb_path=None,
     avd_home=None,
     logdir=None,
     serial=None,
     binary=None,
     app="org.mozilla.fennec",
     **kwargs
```

### Comparing `mozrunner-8.2.1/mozrunner/utils.py` & `mozrunner-8.3.0/mozrunner/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """Utility functions for mozrunner"""
 
-from __future__ import absolute_import, division, print_function
-
 import os
 import sys
 
 import mozinfo
 
 __all__ = ["findInPath", "get_metadata_from_egg"]
 
@@ -117,14 +115,18 @@
         envValue = (
             (env.get(envVar), str(ldLibraryPath))
             if mozinfo.isWin
             else (ldLibraryPath, env.get(envVar))
         )
         env[envVar] = os.path.pathsep.join([path for path in envValue if path])
 
+    # Allow non-packaged builds to access symlinked modules in the source dir
+    env["MOZ_DEVELOPER_REPO_DIR"] = mozinfo.info.get("topsrcdir")
+    env["MOZ_DEVELOPER_OBJ_DIR"] = mozinfo.info.get("topobjdir")
+
     # crashreporter
     env["GNOME_DISABLE_CRASH_DIALOG"] = "1"
     env["XRE_NO_WINDOWS_CRASH_DIALOG"] = "1"
 
     if crashreporter and not debugger:
         env["MOZ_CRASHREPORTER_NO_REPORT"] = "1"
         env["MOZ_CRASHREPORTER"] = "1"
@@ -144,25 +146,28 @@
     env.setdefault("R_LOG_DESTINATION", "stderr")
     env.setdefault("R_LOG_VERBOSE", "1")
 
     # Ask NSS to use lower-security password encryption. See Bug 1594559
     env.setdefault("NSS_MAX_MP_PBE_ITERATION_COUNT", "10")
 
     # ASan specific environment stuff
+    if "ASAN_SYMBOLIZER_PATH" in env and os.path.isfile(env["ASAN_SYMBOLIZER_PATH"]):
+        llvmsym = env["ASAN_SYMBOLIZER_PATH"]
+    else:
+        if mozinfo.isMac:
+            llvmSymbolizerDir = ldLibraryPath
+        else:
+            llvmSymbolizerDir = xrePath
+        llvmsym = os.path.join(
+            llvmSymbolizerDir, "llvm-symbolizer" + mozinfo.info["bin_suffix"]
+        )
     asan = bool(mozinfo.info.get("asan"))
     if asan:
         try:
             # Symbolizer support
-            if mozinfo.isMac:
-                llvmSymbolizerDir = ldLibraryPath
-            else:
-                llvmSymbolizerDir = xrePath
-            llvmsym = os.path.join(
-                llvmSymbolizerDir, "llvm-symbolizer" + mozinfo.info["bin_suffix"]
-            )
             if os.path.isfile(llvmsym):
                 env["ASAN_SYMBOLIZER_PATH"] = llvmsym
                 log.info("INFO | runtests.py | ASan using symbolizer at %s" % llvmsym)
             else:
                 log.error(
                     "TEST-UNEXPECTED-FAIL | runtests.py | Failed to find"
                     " ASan symbolizer at %s" % llvmsym
@@ -221,15 +226,14 @@
             )
         else:
             log.info(message)
 
     tsan = bool(mozinfo.info.get("tsan"))
     if tsan and mozinfo.isLinux:
         # Symbolizer support.
-        llvmsym = os.path.join(xrePath, "llvm-symbolizer")
         if os.path.isfile(llvmsym):
             env["TSAN_OPTIONS"] = "external_symbolizer_path=%s" % llvmsym
             log.info("INFO | runtests.py | TSan using symbolizer at %s" % llvmsym)
         else:
             log.error(
                 "TEST-UNEXPECTED-FAIL | runtests.py | Failed to find TSan"
                 " symbolizer at %s" % llvmsym
```

### Comparing `mozrunner-8.2.1/mozrunner/base/runner.py` & `mozrunner-8.3.0/mozrunner/base/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-import six
 import os
 import subprocess
 import sys
 import traceback
 from abc import ABCMeta, abstractproperty
 
+import six
 from mozlog import get_default_logger
 from mozprocess import ProcessHandler
-from six import string_types, text_type
+from six import ensure_str, string_types
 
 try:
     import mozcrash
 except ImportError:
     mozcrash = None
 from six import reraise
 
@@ -125,30 +123,26 @@
         # attach a debugger, if specified
         if debug_args:
             cmd = list(debug_args) + cmd
 
         if self.logger:
             self.logger.info("Application command: %s" % " ".join(cmd))
 
-        encoded_env = {}
+        str_env = {}
         for k in self.env:
             v = self.env[k]
-            if isinstance(v, text_type):
-                v = v.encode("utf-8")
-            if isinstance(k, text_type):
-                k = k.encode("utf-8")
-            encoded_env[k] = v
+            str_env[ensure_str(k)] = ensure_str(v)
 
         if interactive:
-            self.process_handler = subprocess.Popen(cmd, env=encoded_env)
+            self.process_handler = subprocess.Popen(cmd, env=str_env)
             # TODO: other arguments
         else:
             # this run uses the managed processhandler
             try:
-                process = self.process_class(cmd, env=encoded_env, **self.process_args)
+                process = self.process_class(cmd, env=str_env, **self.process_args)
                 process.run(self.timeout, self.output_timeout)
 
                 self.process_handler = process
             except Exception as e:
                 reraise(
                     RunnerNotStartedError,
                     RunnerNotStartedError("Failed to start the process: {}".format(e)),
```

### Comparing `mozrunner-8.2.1/mozrunner/base/device.py` & `mozrunner-8.3.0/mozrunner/base/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function
-
 import codecs
 import datetime
 import re
 import signal
-import six
 import sys
 import tempfile
 import time
 
 import mozfile
+import six
 
-from .runner import BaseRunner
 from ..devices import BaseEmulator
+from .runner import BaseRunner
 
 
 class DeviceRunner(BaseRunner):
     """
     The base runner class used for running gecko on
     remote devices (or emulators).
     """
```

### Comparing `mozrunner-8.2.1/mozrunner/base/browser.py` & `mozrunner-8.3.0/mozrunner/base/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import copy
-import mozinfo
 import os
 import sys
 
+import mozinfo
+
 from ..application import DefaultContext, FirefoxContext
 from .runner import BaseRunner
 
 
 class GeckoRuntimeRunner(BaseRunner):
     """
     The base runner class used for local gecko runtime binaries,
```

### Comparing `mozrunner-8.2.1/mozrunner/errors.py` & `mozrunner-8.3.0/mozrunner/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 
 class RunnerException(Exception):
     """Base exception handler for mozrunner related errors"""
 
 
 class RunnerNotStartedError(RunnerException):
     """Exception handler in case the runner hasn't been started"""
```

