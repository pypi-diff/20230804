# Comparing `tmp/zhmccli-1.7.1.tar.gz` & `tmp/zhmccli-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmccli-1.7.1.tar", last modified: Mon Jul  3 10:02:29 2023, max compression
+gzip compressed data, was "zhmccli-1.8.0.tar", last modified: Fri Aug  4 08:34:59 2023, max compression
```

## Comparing `zhmccli-1.7.1.tar` & `zhmccli-1.8.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:29.559146 zhmccli-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-03 10:01:41.000000 zhmccli-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-03 10:02:18.000000 zhmccli-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-03 10:02:29.559146 zhmccli-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-03 10:01:41.000000 zhmccli-1.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-03 10:01:41.000000 zhmccli-1.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:02:29.559146 zhmccli-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-03 10:01:41.000000 zhmccli-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:29.559146 zhmccli-1.7.1/zhmccli/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_capacitygroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_character_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_hba.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_ldap_server_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    34886 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_lpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    76333 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_storagegroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_storagevolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_unmanaged_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_vfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_vstorageresource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_cmd_vswitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    56569 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-07-03 10:01:41.000000 zhmccli-1.7.1/zhmccli/zhmccli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:29.559146 zhmccli-1.7.1/zhmccli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-03 10:02:29.000000 zhmccli-1.7.1/zhmccli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-03 10:02:29.000000 zhmccli-1.7.1/zhmccli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:02:29.000000 zhmccli-1.7.1/zhmccli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 10:02:29.000000 zhmccli-1.7.1/zhmccli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 10:02:29.000000 zhmccli-1.7.1/zhmccli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 10:02:29.000000 zhmccli-1.7.1/zhmccli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:02:29.000000 zhmccli-1.7.1/zhmccli.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:34:59.912913 zhmccli-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-08-04 08:33:59.000000 zhmccli-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-04 08:34:46.000000 zhmccli-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-04 08:34:59.912913 zhmccli-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-04 08:33:59.000000 zhmccli-1.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-08-04 08:33:59.000000 zhmccli-1.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:34:59.912913 zhmccli-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-08-04 08:33:59.000000 zhmccli-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:34:59.912913 zhmccli-1.8.0/zhmccli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_capacitygroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_character_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43019 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_hba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_ldap_server_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34886 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76333 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_storagegroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_storagevolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_unmanaged_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_vfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_vstorageresource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_cmd_vswitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56569 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-08-04 08:33:59.000000 zhmccli-1.8.0/zhmccli/zhmccli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:34:59.912913 zhmccli-1.8.0/zhmccli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-04 08:34:59.000000 zhmccli-1.8.0/zhmccli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 08:34:59.000000 zhmccli-1.8.0/zhmccli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:34:59.000000 zhmccli-1.8.0/zhmccli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 08:34:59.000000 zhmccli-1.8.0/zhmccli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-04 08:34:59.000000 zhmccli-1.8.0/zhmccli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 08:34:59.000000 zhmccli-1.8.0/zhmccli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:34:59.000000 zhmccli-1.8.0/zhmccli.egg-info/zip-safe
```

### Comparing `zhmccli-1.7.1/LICENSE` & `zhmccli-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/MANIFEST.in` & `zhmccli-1.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/PKG-INFO` & `zhmccli-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmccli
-Version: 1.7.1
+Version: 1.8.0
 Summary: A CLI for the IBM Z HMC, written in pure Python
 Home-page: https://github.com/zhmcclient/zhmccli
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmccli-1.7.1/README.rst` & `zhmccli-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/requirements.txt` & `zhmccli-1.8.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # process, which may cause wedges in the gate later.
 
 # Make sure that the package versions in minimum-constraints.txt are also
 # the minimum versions required in requirements.txt and dev-requirements.txt.
 
 # Direct dependencies (except pip, setuptools, wheel):
 
-# zhmcclient @ git+https://github.com/zhmcclient/python-zhmcclient.git@1.8/andy/fix-session-logoff
-zhmcclient>=1.8.1  # Apache
+# zhmcclient @ git+https://github.com/zhmcclient/python-zhmcclient.git@master
+zhmcclient>=1.10.0  # Apache
 
 # click <7.0 did not properly declare supported Python versions
 # click 8.0 has dropped support for Python 2.7,3.5
 # safety 2.2.0 depends on click>=8.0.2 and is run only on Python>=3.6
 click>=7.0,<8.0; python_version <= '3.5'
 click>=8.0.2; python_version >= '3.6'
 
@@ -37,26 +37,37 @@
 prompt-toolkit>=2.0.1; python_version >= '3.5'
 
 # PyYAML 5.3 has removed support for Python 3.4
 # PyYAML 5.3 fixed narrow build error on Python 2.7
 # PyYAML 5.3.1 addressed issue 38100 reported by safety
 # PyYAML 5.2 addressed issue 38639 reported by safety
 # PyYAML 5.4 fixes safety issue 39611
+# PyYAML 5.3 has wheel archives for Python 2.7, 3.5 - 3.9
+# PyYAML 5.4 has wheel archives for Python 2.7, 3.6 - 3.9
+# PyYAML 6.0 has wheel archives for Python 3.6 - 3.11
+# PyYAML 5.4 and 6.0.0 fails install since Cython 3 was released, see issue
+#   https://github.com/yaml/pyyaml/issues/724.
 PyYAML>=5.3.1; python_version <= '3.5'
-PyYAML>=5.4; python_version >= '3.6'
+PyYAML>=5.3.1,!=5.4.0,!=5.4.1; python_version >= '3.6' and python_version <= '3.11'
+PyYAML>=5.3.1,!=5.4.0,!=5.4.1,!=6.0.0; python_version >= '3.12'
 
 jsonschema>=3.0.1
 yamlloader>=0.5.5
 
 # urllib3 is used to disable warnings
 urllib3>=1.26.5  # MIT
 
 
 # Indirect dependencies (commented out, only listed to document their license):
 
+# MIT, from jsonschema>=3.0
+# pyrsistent 0.15.0 started using the FileNotFoundError built-in exception that
+# was added only in Python 3. pyrsistent 0.15.1 fixed that by defining it locally for py27.
+pyrsistent>=0.15.1
+
 # certifi # MPL 2.0, from requests
 # chardet # LGPL, from requests
 # decorator # BSD, from zhmcclient
 # docopt # MIT, from stomp.py
 # idna # BSD, from requests
 # python-utils # BSD, from progressbar2
 # pytz # MIT, from zhmcclient
```

### Comparing `zhmccli-1.7.1/setup.py` & `zhmccli-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/__init__.py` & `zhmccli-1.8.0/zhmccli/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_adapter.py` & `zhmccli-1.8.0/zhmccli/_cmd_adapter.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_capacitygroup.py` & `zhmccli-1.8.0/zhmccli/_cmd_capacitygroup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_certificates.py` & `zhmccli-1.8.0/zhmccli/_cmd_certificates.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_character_rule.py` & `zhmccli-1.8.0/zhmccli/_cmd_character_rule.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_cpc.py` & `zhmccli-1.8.0/zhmccli/_cmd_cpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,14 +518,64 @@
     general options (see 'zhmc --help') can also be specified right after the
     'zhmc' command name.
     """
     cmd_ctx.execute_cmd(
         lambda: cmd_cpc_list_api_features(cmd_ctx, cpc, options))
 
 
+@cpc_group.command('upgrade', options_metavar=COMMAND_OPTIONS_METAVAR)
+@click.option('--bundle-level', '-b', type=str, required=True,
+              help="Name of the bundle to be installed on the SE "
+              "(e.g. 'S71').")
+@click.option('--accept-firmware', '-a', type=bool, required=False,
+              default=True,
+              help="Boolean indicating to accept the previous bundle level "
+              "before installing the new level.")
+@click.option('--timeout', '-T', type=int, required=False, default=600,
+              help='Timeout (in seconds) when waiting for the SE upgrade '
+              'to be complete. Default: 600.')
+@click.pass_obj
+def cpc_upgrade(cmd_ctx, cpc, **options):
+    """
+    Upgrade the firmware on the Support Element (SE) of a CPC to a new bundle
+    level.
+
+    This is done by performing the "CPC Single Step Install" operation
+    which performs the following steps:
+
+    \b
+    * A backup of the target CPC is performed to its SE hard drive.
+    * If `accept_firmware` is True, the firmware currently installed on the SE
+      of this CPC is accepted. Note that once firmware is accepted, it cannot be
+      removed.
+    * The new firmware identified by the bundle-level field is retrieved from
+      the IBM support site and installed.
+    * The newly installed firmware is activated, which includes rebooting the SE
+      of this CPC.
+
+    If an error occurrs when installing the upgrades for the components of
+    the new bundle, any components that were successfully installed are
+    rolled back.
+
+    If an error occurs after the firmware is accepted, the firmware remains
+    accepted.
+
+    Note that it is not possible to downgrade the SE firmware with this
+    operation.
+
+    If the SE firmware is already at the requested bundle level, nothing is
+    changed and the command succeeds.
+
+    In addition to the command-specific options shown in this help text, the
+    general options (see 'zhmc --help') can also be specified right after the
+    'zhmc' command name.
+    """
+    cmd_ctx.execute_cmd(lambda: cmd_cpc_upgrade(cmd_ctx, cpc, options))
+
+
 def cmd_cpc_list(cmd_ctx, options):
     # pylint: disable=missing-function-docstring
 
     client = zhmcclient.Client(cmd_ctx.session)
 
     try:
         cpcs = client.cpcs.list()
@@ -1015,7 +1065,54 @@
     name = options['name']
     try:
         features = cpc.list_api_features(name)
     except zhmcclient.Error as exc:
         raise click_exception(exc, cmd_ctx.error_format)
 
     print_list(cmd_ctx, features, cmd_ctx.output_format)
+
+
+def cmd_cpc_upgrade(cmd_ctx, cpc_name, options):
+    # pylint: disable=missing-function-docstring
+
+    client = zhmcclient.Client(cmd_ctx.session)
+    cpc = find_cpc(cmd_ctx, client, cpc_name)
+    console = client.consoles.console
+
+    bundle_level = options['bundle_level']
+    accept_firmware = options['accept_firmware']
+    timeout = options['timeout']
+
+    ec_mcl = console.prop('ec-mcl-description')
+    hmc_bundle_level = ec_mcl.get('bundle-level', None)
+    if hmc_bundle_level is None:
+        hmc_version = console.prop('version')
+        raise click_exception(
+            "HMC version {v} does not support firmware upgrade through "
+            "the Web Services API".format(v=hmc_version),
+            cmd_ctx.error_format)
+
+    click.echo("Upgrading the SE of CPC {c} to bundle level {bl} and waiting "
+               "for completion (timeout: {t} s)".
+               format(c=cpc_name, bl=bundle_level, t=timeout))
+
+    try:
+        cpc.single_step_install(
+            bundle_level=bundle_level,
+            accept_firmware=accept_firmware,
+            wait_for_completion=True,
+            operation_timeout=timeout)
+    except zhmcclient.HTTPError as exc:
+        if exc.http_status == 400 and exc.reason == 356:
+            # HMC was already at that bundle level
+            cmd_ctx.spinner.stop()
+            click.echo("The SE of CPC {c} was already at bundle level {bl} "
+                       "and did not need to be changed".
+                       format(c=cpc_name, bl=bundle_level))
+            return
+        raise click_exception(exc, cmd_ctx.error_format)
+    except zhmcclient.Error as exc:
+        raise click_exception(exc, cmd_ctx.error_format)
+
+    cmd_ctx.spinner.stop()
+    click.echo("The SE of CPC {c} has been upgraded to bundle level {bl}".
+               format(c=cpc_name, bl=bundle_level))
```

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_hba.py` & `zhmccli-1.8.0/zhmccli/_cmd_hba.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_info.py` & `zhmccli-1.8.0/zhmccli/_cmd_info.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_ldap_server_definition.py` & `zhmccli-1.8.0/zhmccli/_cmd_ldap_server_definition.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_lpar.py` & `zhmccli-1.8.0/zhmccli/_cmd_lpar.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_metrics.py` & `zhmccli-1.8.0/zhmccli/_cmd_metrics.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_nic.py` & `zhmccli-1.8.0/zhmccli/_cmd_nic.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_partition.py` & `zhmccli-1.8.0/zhmccli/_cmd_partition.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_password_rule.py` & `zhmccli-1.8.0/zhmccli/_cmd_password_rule.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_port.py` & `zhmccli-1.8.0/zhmccli/_cmd_port.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_session.py` & `zhmccli-1.8.0/zhmccli/_cmd_session.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_storagegroup.py` & `zhmccli-1.8.0/zhmccli/_cmd_storagegroup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_storagevolume.py` & `zhmccli-1.8.0/zhmccli/_cmd_storagevolume.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_unmanaged_cpc.py` & `zhmccli-1.8.0/zhmccli/_cmd_unmanaged_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_user.py` & `zhmccli-1.8.0/zhmccli/_cmd_user.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_user_role.py` & `zhmccli-1.8.0/zhmccli/_cmd_user_role.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_vfunction.py` & `zhmccli-1.8.0/zhmccli/_cmd_vfunction.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_vstorageresource.py` & `zhmccli-1.8.0/zhmccli/_cmd_vstorageresource.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_cmd_vswitch.py` & `zhmccli-1.8.0/zhmccli/_cmd_vswitch.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_helper.py` & `zhmccli-1.8.0/zhmccli/_helper.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli/_version.py` & `zhmccli-1.8.0/zhmccli/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.U.dev1": A not yet released version M.N.U
 #: * "M.N.U": A released version M.N.U
-__version__ = '1.7.1'
+__version__ = '1.8.0'
```

### Comparing `zhmccli-1.7.1/zhmccli/zhmccli.py` & `zhmccli-1.8.0/zhmccli/zhmccli.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.7.1/zhmccli.egg-info/PKG-INFO` & `zhmccli-1.8.0/zhmccli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmccli
-Version: 1.7.1
+Version: 1.8.0
 Summary: A CLI for the IBM Z HMC, written in pure Python
 Home-page: https://github.com/zhmcclient/zhmccli
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmccli-1.7.1/zhmccli.egg-info/SOURCES.txt` & `zhmccli-1.8.0/zhmccli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

