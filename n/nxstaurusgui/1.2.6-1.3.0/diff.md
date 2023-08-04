# Comparing `tmp/nxstaurusgui-1.2.6.tar.gz` & `tmp/nxstaurusgui-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nxstaurusgui-1.2.6.tar", last modified: Mon Oct 14 17:36:10 2019, max compression
+gzip compressed data, was "nxstaurusgui-1.3.0.tar", last modified: Fri Aug  4 05:47:31 2023, max compression
```

## Comparing `nxstaurusgui-1.2.6.tar` & `nxstaurusgui-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      725 2017-05-08 08:12:16.000000 nxstaurusgui-1.2.6/man/nxsmacrogui.1
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/nxstaurusgui/
--rw-r--r--   0 jkotan   (15949) irc         (39)     1361 2017-01-31 10:51:28.000000 nxstaurusgui-1.2.6/nxstaurusgui/heartbeat.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/nxstaurusgui/data/
--rw-r--r--   0 jkotan   (15949) irc         (39)      955 2016-06-01 07:40:37.000000 nxstaurusgui-1.2.6/nxstaurusgui/data/config.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)        0 2017-01-31 10:51:33.000000 nxstaurusgui-1.2.6/nxstaurusgui/data/__init__.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)    72727 2015-05-06 11:01:51.000000 nxstaurusgui-1.2.6/nxstaurusgui/data/desylogo.png
--rw-r--r--   0 jkotan   (15949) irc         (39)     4990 2019-10-14 17:35:34.000000 nxstaurusgui-1.2.6/nxstaurusgui/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      214 2019-01-30 15:50:32.000000 nxstaurusgui-1.2.6/nxstaurusgui/config.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      300 2017-01-31 10:51:28.000000 nxstaurusgui-1.2.6/nxstaurusgui/serverinfo.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2015-05-06 11:54:49.000000 nxstaurusgui-1.2.6/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)      209 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     3807 2019-10-14 17:35:34.000000 nxstaurusgui-1.2.6/setup.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3406 2019-10-14 17:35:34.000000 nxstaurusgui-1.2.6/README.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)      139 2016-06-01 07:40:37.000000 nxstaurusgui-1.2.6/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     2989 2019-10-01 08:46:24.000000 nxstaurusgui-1.2.6/nxsmacrogui
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/nxstaurusgui.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/nxstaurusgui.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       31 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/nxstaurusgui.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       18 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/nxstaurusgui.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      486 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/nxstaurusgui.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-14 17:35:46.000000 nxstaurusgui-1.2.6/nxstaurusgui.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)     5890 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/nxstaurusgui.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     5890 2019-10-14 17:36:10.000000 nxstaurusgui-1.2.6/PKG-INFO
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-04 05:47:31.029697 nxstaurusgui-1.3.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2015-05-06 11:54:49.000000 nxstaurusgui-1.3.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)      139 2016-06-01 07:40:37.000000 nxstaurusgui-1.3.0/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7105 2023-08-04 05:47:31.029697 nxstaurusgui-1.3.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4227 2023-06-23 08:17:35.000000 nxstaurusgui-1.3.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-04 05:47:31.029697 nxstaurusgui-1.3.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      725 2017-05-08 08:12:16.000000 nxstaurusgui-1.3.0/man/nxsmacrogui.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      993 2023-08-04 05:47:07.000000 nxstaurusgui-1.3.0/nxsmacrogui
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-04 05:47:31.029697 nxstaurusgui-1.3.0/nxstaurusgui/
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     3792 2023-08-04 05:47:07.000000 nxstaurusgui-1.3.0/nxstaurusgui/NXSMacroGUI.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5034 2023-08-04 05:47:07.000000 nxstaurusgui-1.3.0/nxstaurusgui/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      214 2019-01-30 15:50:32.000000 nxstaurusgui-1.3.0/nxstaurusgui/config.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-04 05:47:31.029697 nxstaurusgui-1.3.0/nxstaurusgui/data/
+-rw-r--r--   0 jkotan   (15949) irc         (39)        0 2017-01-31 10:51:33.000000 nxstaurusgui-1.3.0/nxstaurusgui/data/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      955 2016-06-01 07:40:37.000000 nxstaurusgui-1.3.0/nxstaurusgui/data/config.xml
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    72727 2015-05-06 11:01:51.000000 nxstaurusgui-1.3.0/nxstaurusgui/data/desylogo.png
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1361 2017-01-31 10:51:28.000000 nxstaurusgui-1.3.0/nxstaurusgui/heartbeat.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      300 2017-01-31 10:51:28.000000 nxstaurusgui-1.3.0/nxstaurusgui/serverinfo.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-08-04 05:47:31.029697 nxstaurusgui-1.3.0/nxstaurusgui.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7105 2023-08-04 05:47:30.000000 nxstaurusgui-1.3.0/nxstaurusgui.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      514 2023-08-04 05:47:30.000000 nxstaurusgui-1.3.0/nxstaurusgui.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-08-04 05:47:30.000000 nxstaurusgui-1.3.0/nxstaurusgui.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-14 17:35:46.000000 nxstaurusgui-1.3.0/nxstaurusgui.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       18 2023-08-04 05:47:30.000000 nxstaurusgui-1.3.0/nxstaurusgui.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       31 2023-08-04 05:47:30.000000 nxstaurusgui-1.3.0/nxstaurusgui.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      209 2023-08-04 05:47:31.029697 nxstaurusgui-1.3.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4005 2023-07-04 12:57:09.000000 nxstaurusgui-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nxstaurusgui-1.2.6/man/nxsmacrogui.1` & `nxstaurusgui-1.3.0/man/nxsmacrogui.1`

 * *Files identical despite different names*

### Comparing `nxstaurusgui-1.2.6/nxstaurusgui/heartbeat.py` & `nxstaurusgui-1.3.0/nxstaurusgui/heartbeat.py`

 * *Files identical despite different names*

### Comparing `nxstaurusgui-1.2.6/nxstaurusgui/data/config.xml` & `nxstaurusgui-1.3.0/nxstaurusgui/data/config.xml`

 * *Files identical despite different names*

### Comparing `nxstaurusgui-1.2.6/nxstaurusgui/data/desylogo.png` & `nxstaurusgui-1.3.0/nxstaurusgui/data/desylogo.png`

 * *Files identical despite different names*

### Comparing `nxstaurusgui-1.2.6/nxstaurusgui/__init__.py` & `nxstaurusgui-1.3.0/nxstaurusgui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,22 @@
 GUI for taurusgui
 """
 
 from . import serverinfo
 from . import config
 from xml.dom import minidom
 import tempfile
-import PyTango
+
+try:
+    import tango
+except Exception:
+    import PyTango as tango
 
 #: version of the application
-__version__ = "1.2.6"
+__version__ = "1.3.0"
 
 
 def replaceText(node, text):
     """
     replace text in the minidom node
 
     :param node: minidom node
@@ -45,55 +49,55 @@
 
 
 def findDevices():
     """
     find NXS and Sardana devices and store them in
     :class:`nxstaurusgui.serverinfo`
     """
-    db = PyTango.Database()
+    db = tango.Database()
     if not serverinfo.SELECTORSERVER_NAME:
         dvs = db.get_device_exported_for_class("NXSRecSelector")
 
         for dv in dvs:
             try:
-                dp = PyTango.DeviceProxy(dv)
+                dp = tango.DeviceProxy(dv)
                 dp.ping()
                 if not serverinfo.DOOR_NAME:
                     serverinfo.DOOR_NAME = dp.Door
                 serverinfo.SELECTORSERVER_NAME = dv
                 break
             except Exception:
                 pass
     elif not serverinfo.DOOR_NAME:
         try:
-            dp = PyTango.DeviceProxy(serverinfo.SELECTORSERVER_NAME)
+            dp = tango.DeviceProxy(serverinfo.SELECTORSERVER_NAME)
             dp.ping()
             serverinfo.DOOR_NAME = dp.Door
         except Exception:
             pass
 
     if not serverinfo.SELECTORSERVER_NAME:
         serverinfo.SELECTORSERVER_NAME = 'module'
     if not serverinfo.DOOR_NAME:
         dvs = db.get_device_exported_for_class("Door")
 
         for dv in dvs:
             try:
-                dp = PyTango.DeviceProxy(dv)
+                dp = tango.DeviceProxy(dv)
                 dp.ping()
                 serverinfo.DOOR_NAME = dv
                 break
             except Exception:
                 pass
 
     if not serverinfo.MACROSERVER_NAME:
         dvs = db.get_device_exported_for_class("MacroServer")
         for dv in dvs:
             try:
-                dp = PyTango.DeviceProxy(dv)
+                dp = tango.DeviceProxy(dv)
                 dp.ping()
                 dl = dp.DoorList
                 if serverinfo.DOOR_NAME in dl:
                     serverinfo.MACROSERVER_NAME = dv
                     break
             except Exception:
                 pass
```

### Comparing `nxstaurusgui-1.2.6/COPYRIGHT` & `nxstaurusgui-1.3.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxstaurusgui-1.2.6/setup.py` & `nxstaurusgui-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,14 +110,18 @@
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     command_options={
         'build_sphinx': {
             'project': ('setup.py', name),
             'version': ('setup.py', version),
             'release': ('setup.py', release)}},
     long_description=read('README.rst')
```

### Comparing `nxstaurusgui-1.2.6/nxsmacrogui` & `nxstaurusgui-1.3.0/nxstaurusgui/NXSMacroGUI.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,22 +18,40 @@
 #
 
 """ NXS Scan - GUI for setting sardana scans with NeXus Recorder"""
 
 import logging
 import sys
 import os
-# from optparse import OptionParser
-import nxstaurusgui
-from nxstaurusgui import serverinfo
+from . import serverinfo
 
 
 logger = logging.getLogger(__name__)
 
 
+def setLoggerLevel(logger, level):
+    global _logginglevel
+    """ sets logging level from string
+    :param logger: logger
+    :type logger: :obj:`logging.logger`
+    :param level: logging level
+    :type level: :obj:`str`
+    """
+    levels = {'debug': logging.DEBUG,
+              'info': logging.INFO,
+              'warning': logging.WARNING,
+              'error': logging.ERROR,
+              'critical': logging.CRITICAL}
+    _logginglevel = level if level in levels else "warning"
+    dlevel = levels.get(level, logging.WARNING)
+    logger.setLevel(dlevel)
+    from taurus.core.util.log import Logger
+    Logger.log_level = dlevel
+
+
 # the main function
 def remove_option(sopt, lopt):
     pos = None
     single = True
     for i, ar in enumerate(sys.argv):
         if ar.startswith(sopt):
             pos = i
@@ -53,39 +71,45 @@
 
     if "GNOME_DESKTOP_SESSION_ID" not in os.environ:
         os.environ["GNOME_DESKTOP_SESSION_ID"] = "qtconfig"
     if os.path.isdir("/usr/lib/kde4/plugins/") and \
        "QT_PLUGIN_PATH" not in os.environ:
         os.environ["QT_PLUGIN_PATH"] = "/usr/lib/kde4/plugins/"
 
-    import taurus.core.util.argparse
-    parser = taurus.core.util.argparse.get_taurus_parser()
+    import argparse
+    parser = argparse.ArgumentParser(
+        description="NeXus Macro GUI")
 
-    parser.add_option(
+    parser.add_argument(
         "-s", "--server", dest="server",
         help="selector server")
-    parser.add_option(
+    parser.add_argument(
         "-d", "--door", dest="door",
         help="door device name")
-
-    (options, _) = parser.parse_args()
-
+    parser.add_argument(
+        "--log", dest="log",
+        help="logging level, i.e. debug, info, warning, error, critical")
+
+    options = parser.parse_args()
+    if options.log:
+        setLoggerLevel(logger, options.log)
+        remove_option("", "--log")
     if options.door:
         serverinfo.DOOR_NAME = options.door
         remove_option("-d", "--door")
     if options.server:
         serverinfo.SELECTORSERVER_NAME = options.server
         remove_option("-s", "--server")
     try:
         from taurus.external.qt import Qt
     except Exception:
         from taurus.qt import Qt
     Qt.QCoreApplication.setAttribute(Qt.Qt.AA_X11InitThreads)
     import sys
-    sys.argv.insert(1, str(nxstaurusgui.__path__[0]))
+    sys.argv.insert(1, str(os.path.dirname(__file__)))
     try:
         from taurus.qt.qtgui.taurusgui.taurusgui import main as tmain
     except Exception:
         from taurus.qt.qtgui.taurusgui.taurusgui import gui_cmd as tmain
     try:
         serverinfo.FIND = True
         tmain()
```

### Comparing `nxstaurusgui-1.2.6/nxstaurusgui.egg-info/PKG-INFO` & `nxstaurusgui-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,54 @@
 Metadata-Version: 1.2
 Name: nxstaurusgui
-Version: 1.2.6
+Version: 1.3.0
 Summary: NXSelector MacroGUI for taurusgui
 Home-page: https://github.com/jkotan/nexdatas
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 Maintainer: Jan Kotanski
 Maintainer-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE, version 3
 Description: Welcome to nxstaurusgui's documentation!
         ========================================
         
+        
+        |github workflow|
+        |docs|
+        |Pypi Version|
+        |Python Versions|
+        
+        .. |github workflow| image:: https://github.com/nexdatas/nxsmacrogui/actions/workflows/tests.yml/badge.svg
+           :target: https://github.com/nexdatas/nxsmacrogui/actions
+           :alt:
+        
+        .. |docs| image:: https://img.shields.io/badge/Documentation-webpages-ADD8E6.svg
+           :target: https://nexdatas.github.io/nxsmacrogui/index.html
+           :alt:
+        
+        .. |Pypi Version| image:: https://img.shields.io/pypi/v/nxstaurusgui.svg
+                          :target: https://pypi.python.org/pypi/nxstaurusgui
+                          :alt:
+        
+        .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/nxstaurusgui.svg
+                             :target: https://pypi.python.org/pypi/nxstaurusgui/
+                             :alt:
+        
+        
+        
         Authors: Jan Kotanski
         
-        NXS TaurusGUI is taurusgui Configuration for Component Selector
+        NXS MacroGUI is taurus gui Configuration for Component Selector
         
         .. figure:: png/nxstaurusgui.png
            :alt: NeXus Taurus GUI
         
         
-        | Source code: https://github.com/nexdatas/taurusgui/
-        | Web page: https://nexdatas.github.io/taurusgui/
+        | Source code: https://github.com/nexdatas/nxsmacrogui/
+        | Web page: https://nexdatas.github.io/nxsmacrogui/
         | NexDaTaS Web page: https://nexdatas.github.io
         
         
         
         ------------
         Installation
         ------------
@@ -34,59 +58,59 @@
         |    Sardana, PyTango, sphinx, Taurus, NXSRecSelector, Selector
         
         From sources
         ^^^^^^^^^^^^
         
         Download the latest version of NeXuS Configuration Server from
         
-        |    https://github.com/nexdatas/taurusgui/
+        |    https://github.com/nexdatas/nxsmacrogui/
         
         Extract the sources and run
         
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian Jessie (and Wheezy) packages can be found in the HDRI repository.
+        Debian Bookworm, Bullseye, Buster and  Ubuntu Lunar, Jammy, Focal  packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/jessie-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         Finally,
         
         .. code-block:: console
         
         	  $ apt-get update
-        	  $ apt-get install python-nxsrecselector nxselector nxstaurusgui
+        	  $ apt-get install python3-nxsrecselector nxselector nxstaurusgui
         
         To instal other NexDaTaS packages
         
         .. code-block:: console
         
         	  $ apt-get install python-nxswriter nxsconfigtool nxstools python-nxsconfigserver nxsconfigserver-db
         
         and
         
         .. code-block:: console
         
-        	  $ apt-get install python-sardana-nxsrecorder
+        	  $ apt-get install python3-sardana-nxsrecorder
         
         for NeXus recorder.
         
         From pip
         ^^^^^^^^
         
         To install it from pip you need also to install pyqt5, e.g.
@@ -143,21 +167,21 @@
         Next, run Astor and change start-up levels: for Pool to 2,
         for MacroServer to 3 and restart servers.
         
         Alternatively, terminate Pool and MacroServer in the terminals and run
         
         .. code-block:: console
         
-                  $ nxsetup -s Pool -l2
+                  $ nxsetup start Pool -l2
         
         wait until Pool is started and run
         
         .. code-block:: console
         
-                  $ nxsetup -s MacroServer -l3
+                  $ nxsetup start MacroServer -l3
         
         
         Additionally, one can create dummy devices by running `sar_demo` in
         
         .. code-block:: console
         
         	  $ spock
@@ -167,31 +191,31 @@
         Setting NeXus Servers
         ^^^^^^^^^^^^^^^^^^^^^
         
         To set up  NeXus Servers run
         
         .. code-block:: console
         
-        	  $ nxsetup -x
+        	  $ nxsetup set
         
         or
         
         .. code-block:: console
         
-                  $ nxsetup -x NXSDataWriter
-                  $ nxsetup -x NXSConfigServer
-        	  $ nxsetup -x NXSRecSelector
+                  $ nxsetup set NXSDataWriter
+                  $ nxsetup set NXSConfigServer
+        	  $ nxsetup set NXSRecSelector
         
         for specific servers.
         
         If the `RecoderPath` property of MacroServer is not set one can do it by
         
         .. code-block:: console
         
-        	  $ nxsetup -a /usr/lib/python2.7/dist-packages/sardananxsrecorder
+        	  $ nxsetup add-recorder-path  /usr/lib/python2.7/dist-packages/sardananxsrecorder
         
         where the path should point the `sardananxsrecorder` package.
         
         
 Keywords: configuration scan nexus sardana recorder tango component data
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
@@ -201,7 +225,11 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `nxstaurusgui-1.2.6/PKG-INFO` & `nxstaurusgui-1.3.0/nxstaurusgui.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,54 @@
 Metadata-Version: 1.2
 Name: nxstaurusgui
-Version: 1.2.6
+Version: 1.3.0
 Summary: NXSelector MacroGUI for taurusgui
 Home-page: https://github.com/jkotan/nexdatas
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 Maintainer: Jan Kotanski
 Maintainer-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE, version 3
 Description: Welcome to nxstaurusgui's documentation!
         ========================================
         
+        
+        |github workflow|
+        |docs|
+        |Pypi Version|
+        |Python Versions|
+        
+        .. |github workflow| image:: https://github.com/nexdatas/nxsmacrogui/actions/workflows/tests.yml/badge.svg
+           :target: https://github.com/nexdatas/nxsmacrogui/actions
+           :alt:
+        
+        .. |docs| image:: https://img.shields.io/badge/Documentation-webpages-ADD8E6.svg
+           :target: https://nexdatas.github.io/nxsmacrogui/index.html
+           :alt:
+        
+        .. |Pypi Version| image:: https://img.shields.io/pypi/v/nxstaurusgui.svg
+                          :target: https://pypi.python.org/pypi/nxstaurusgui
+                          :alt:
+        
+        .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/nxstaurusgui.svg
+                             :target: https://pypi.python.org/pypi/nxstaurusgui/
+                             :alt:
+        
+        
+        
         Authors: Jan Kotanski
         
-        NXS TaurusGUI is taurusgui Configuration for Component Selector
+        NXS MacroGUI is taurus gui Configuration for Component Selector
         
         .. figure:: png/nxstaurusgui.png
            :alt: NeXus Taurus GUI
         
         
-        | Source code: https://github.com/nexdatas/taurusgui/
-        | Web page: https://nexdatas.github.io/taurusgui/
+        | Source code: https://github.com/nexdatas/nxsmacrogui/
+        | Web page: https://nexdatas.github.io/nxsmacrogui/
         | NexDaTaS Web page: https://nexdatas.github.io
         
         
         
         ------------
         Installation
         ------------
@@ -34,59 +58,59 @@
         |    Sardana, PyTango, sphinx, Taurus, NXSRecSelector, Selector
         
         From sources
         ^^^^^^^^^^^^
         
         Download the latest version of NeXuS Configuration Server from
         
-        |    https://github.com/nexdatas/taurusgui/
+        |    https://github.com/nexdatas/nxsmacrogui/
         
         Extract the sources and run
         
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian Jessie (and Wheezy) packages can be found in the HDRI repository.
+        Debian Bookworm, Bullseye, Buster and  Ubuntu Lunar, Jammy, Focal  packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/jessie-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         Finally,
         
         .. code-block:: console
         
         	  $ apt-get update
-        	  $ apt-get install python-nxsrecselector nxselector nxstaurusgui
+        	  $ apt-get install python3-nxsrecselector nxselector nxstaurusgui
         
         To instal other NexDaTaS packages
         
         .. code-block:: console
         
         	  $ apt-get install python-nxswriter nxsconfigtool nxstools python-nxsconfigserver nxsconfigserver-db
         
         and
         
         .. code-block:: console
         
-        	  $ apt-get install python-sardana-nxsrecorder
+        	  $ apt-get install python3-sardana-nxsrecorder
         
         for NeXus recorder.
         
         From pip
         ^^^^^^^^
         
         To install it from pip you need also to install pyqt5, e.g.
@@ -143,21 +167,21 @@
         Next, run Astor and change start-up levels: for Pool to 2,
         for MacroServer to 3 and restart servers.
         
         Alternatively, terminate Pool and MacroServer in the terminals and run
         
         .. code-block:: console
         
-                  $ nxsetup -s Pool -l2
+                  $ nxsetup start Pool -l2
         
         wait until Pool is started and run
         
         .. code-block:: console
         
-                  $ nxsetup -s MacroServer -l3
+                  $ nxsetup start MacroServer -l3
         
         
         Additionally, one can create dummy devices by running `sar_demo` in
         
         .. code-block:: console
         
         	  $ spock
@@ -167,31 +191,31 @@
         Setting NeXus Servers
         ^^^^^^^^^^^^^^^^^^^^^
         
         To set up  NeXus Servers run
         
         .. code-block:: console
         
-        	  $ nxsetup -x
+        	  $ nxsetup set
         
         or
         
         .. code-block:: console
         
-                  $ nxsetup -x NXSDataWriter
-                  $ nxsetup -x NXSConfigServer
-        	  $ nxsetup -x NXSRecSelector
+                  $ nxsetup set NXSDataWriter
+                  $ nxsetup set NXSConfigServer
+        	  $ nxsetup set NXSRecSelector
         
         for specific servers.
         
         If the `RecoderPath` property of MacroServer is not set one can do it by
         
         .. code-block:: console
         
-        	  $ nxsetup -a /usr/lib/python2.7/dist-packages/sardananxsrecorder
+        	  $ nxsetup add-recorder-path  /usr/lib/python2.7/dist-packages/sardananxsrecorder
         
         where the path should point the `sardananxsrecorder` package.
         
         
 Keywords: configuration scan nexus sardana recorder tango component data
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
@@ -201,7 +225,11 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

