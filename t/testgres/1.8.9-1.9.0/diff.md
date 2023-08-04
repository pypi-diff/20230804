# Comparing `tmp/testgres-1.8.9.tar.gz` & `tmp/testgres-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgres-1.8.9.tar", last modified: Mon Jul 24 11:39:41 2023, max compression
+gzip compressed data, was "testgres-1.9.0.tar", last modified: Fri Aug  4 16:11:14 2023, max compression
```

## Comparing `testgres-1.8.9.tar` & `testgres-1.9.0.tar`

### file list

```diff
@@ -1,32 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:39:41.548547 testgres-1.8.9/
--rw-rw-r--   0 root         (0) root         (0)     1106 2023-05-10 11:22:06.000000 testgres-1.8.9/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      136 2022-02-22 09:57:57.000000 testgres-1.8.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5753 2023-07-24 11:39:41.548547 testgres-1.8.9/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5399 2023-05-05 04:23:08.000000 testgres-1.8.9/README.md
--rw-rw-r--   0 root         (0) root         (0)      160 2023-07-24 11:39:41.552547 testgres-1.8.9/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1011 2023-07-24 11:28:45.000000 testgres-1.8.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:39:41.544546 testgres-1.8.9/testgres/
--rw-rw-r--   0 root         (0) root         (0)     1519 2023-05-05 04:23:08.000000 testgres-1.8.9/testgres/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1524 2022-02-22 09:57:57.000000 testgres-1.8.9/testgres/api.py
--rw-rw-r--   0 root         (0) root         (0)     5187 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/backup.py
--rw-rw-r--   0 root         (0) root         (0)     2195 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/cache.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/config.py
--rw-rw-r--   0 root         (0) root         (0)     3080 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/connection.py
--rw-rw-r--   0 root         (0) root         (0)      819 2022-02-22 09:57:57.000000 testgres-1.8.9/testgres/consts.py
--rw-rw-r--   0 root         (0) root         (0)     1749 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/decorators.py
--rw-rw-r--   0 root         (0) root         (0)      932 2022-02-22 09:57:57.000000 testgres-1.8.9/testgres/defaults.py
--rw-rw-r--   0 root         (0) root         (0)     2451 2023-05-05 04:23:08.000000 testgres-1.8.9/testgres/enums.py
--rw-rw-r--   0 root         (0) root         (0)     1988 2022-02-22 09:57:57.000000 testgres-1.8.9/testgres/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     1428 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/logger.py
--rw-rw-r--   0 root         (0) root         (0)    51775 2023-06-07 02:28:30.000000 testgres-1.8.9/testgres/node.py
--rw-rw-r--   0 root         (0) root         (0)     8225 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/pubsub.py
--rw-rw-r--   0 root         (0) root         (0)     1547 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/standby.py
--rw-rw-r--   0 root         (0) root         (0)     6616 2023-07-24 09:08:31.000000 testgres-1.8.9/testgres/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:39:41.548547 testgres-1.8.9/testgres.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     5753 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      541 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       49 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:39:41.548547 testgres-1.8.9/tests/
--rwxrwxr-x   0 root         (0) root         (0)    34865 2023-07-24 09:08:31.000000 testgres-1.8.9/tests/test_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 16:11:14.070690 testgres-1.9.0/
+-rw-rw-r--   0 root         (0) root         (0)     1106 2023-05-10 11:22:06.000000 testgres-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-02-22 09:57:57.000000 testgres-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6740 2023-08-04 16:11:14.074690 testgres-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6386 2023-08-04 15:59:32.000000 testgres-1.9.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)      160 2023-08-04 16:11:14.074690 testgres-1.9.0/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1080 2023-08-04 15:59:32.000000 testgres-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 16:11:14.066689 testgres-1.9.0/testgres/
+-rw-rw-r--   0 root         (0) root         (0)     1802 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2008 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/api.py
+-rw-rw-r--   0 root         (0) root         (0)     5218 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/backup.py
+-rw-rw-r--   0 root         (0) root         (0)     2347 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/cache.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/config.py
+-rw-rw-r--   0 root         (0) root         (0)     3183 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/connection.py
+-rw-rw-r--   0 root         (0) root         (0)      819 2022-02-22 09:57:57.000000 testgres-1.9.0/testgres/consts.py
+-rw-rw-r--   0 root         (0) root         (0)     1749 2022-05-06 11:01:56.000000 testgres-1.9.0/testgres/decorators.py
+-rw-rw-r--   0 root         (0) root         (0)      969 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/defaults.py
+-rw-rw-r--   0 root         (0) root         (0)     2451 2023-05-05 04:23:08.000000 testgres-1.9.0/testgres/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     1988 2022-02-22 09:57:57.000000 testgres-1.9.0/testgres/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1428 2022-05-06 11:01:56.000000 testgres-1.9.0/testgres/logger.py
+-rw-rw-r--   0 root         (0) root         (0)    53271 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 16:11:14.070690 testgres-1.9.0/testgres/operations/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9433 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/operations/local_ops.py
+-rw-rw-r--   0 root         (0) root         (0)     2624 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/operations/os_ops.py
+-rw-rw-r--   0 root         (0) root         (0)    16748 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/operations/remote_ops.py
+-rw-rw-r--   0 root         (0) root         (0)     8218 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/pubsub.py
+-rw-rw-r--   0 root         (0) root         (0)     1547 2022-05-06 11:01:56.000000 testgres-1.9.0/testgres/standby.py
+-rw-rw-r--   0 root         (0) root         (0)     6136 2023-08-04 15:59:32.000000 testgres-1.9.0/testgres/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 16:11:14.066689 testgres-1.9.0/testgres.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     6740 2023-08-04 16:11:13.000000 testgres-1.9.0/testgres.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      719 2023-08-04 16:11:14.000000 testgres-1.9.0/testgres.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-08-04 16:11:13.000000 testgres-1.9.0/testgres.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       75 2023-08-04 16:11:13.000000 testgres-1.9.0/testgres.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-08-04 16:11:13.000000 testgres-1.9.0/testgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 16:11:14.070690 testgres-1.9.0/tests/
+-rwxrwxr-x   0 root         (0) root         (0)     5719 2023-08-04 15:59:32.000000 testgres-1.9.0/tests/test_remote.py
+-rwxrwxr-x   0 root         (0) root         (0)    34865 2023-07-24 09:08:31.000000 testgres-1.9.0/tests/test_simple.py
+-rwxrwxr-x   0 root         (0) root         (0)    36371 2023-08-04 15:59:32.000000 testgres-1.9.0/tests/test_simple_remote.py
```

### Comparing `testgres-1.8.9/LICENSE` & `testgres-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testgres-1.8.9/PKG-INFO` & `testgres-1.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testgres
-Version: 1.8.9
+Version: 1.9.0
 Summary: Testing utility for PostgreSQL and its extensions
 Home-page: https://github.com/postgrespro/testgres
 Author: Ildar Musin
 Author-email: zildermann@gmail.com
 License: PostgreSQL
 Keywords: test,testing,postgresql
 Platform: UNKNOWN
@@ -182,14 +182,41 @@
     # add a new config line
     master.append_conf('postgresql.conf', ext_conf)
 ```
 
 Note that `default_conf()` is called by `init()` function; both of them overwrite
 the configuration file, which means that they should be called before `append_conf()`.
 
+### Remote mode
+Testgres supports the creation of PostgreSQL nodes on a remote host. This is useful when you want to run distributed tests involving multiple nodes spread across different machines.
+
+To use this feature, you need to use the RemoteOperations class.
+Here is an example of how you might set this up:
+
+```python
+from testgres import ConnectionParams, RemoteOperations, TestgresConfig, get_remote_node
+
+# Set up connection params
+conn_params = ConnectionParams(
+    host='your_host',  # replace with your host
+    username='user_name',  # replace with your username
+    ssh_key='path_to_ssh_key'  # replace with your SSH key path
+)
+os_ops = RemoteOperations(conn_params)
+
+# Add remote testgres config before test
+TestgresConfig.set_os_ops(os_ops=os_ops)
+
+# Proceed with your test
+def test_basic_query(self):
+    with get_remote_node(conn_params=conn_params) as node:
+        node.init().start()
+        res = node.execute('SELECT 1')
+        self.assertEqual(res, [(1,)])
+```
 
 ## Authors
 
 [Ildar Musin](https://github.com/zilder)  
 [Dmitry Ivanov](https://github.com/funbringer)  
 [Ildus Kurbangaliev](https://github.com/ildus)  
 [Yury Zhuravlev](https://github.com/stalkerg)
```

### Comparing `testgres-1.8.9/README.md` & `testgres-1.9.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -169,14 +169,41 @@
     # add a new config line
     master.append_conf('postgresql.conf', ext_conf)
 ```
 
 Note that `default_conf()` is called by `init()` function; both of them overwrite
 the configuration file, which means that they should be called before `append_conf()`.
 
+### Remote mode
+Testgres supports the creation of PostgreSQL nodes on a remote host. This is useful when you want to run distributed tests involving multiple nodes spread across different machines.
+
+To use this feature, you need to use the RemoteOperations class.
+Here is an example of how you might set this up:
+
+```python
+from testgres import ConnectionParams, RemoteOperations, TestgresConfig, get_remote_node
+
+# Set up connection params
+conn_params = ConnectionParams(
+    host='your_host',  # replace with your host
+    username='user_name',  # replace with your username
+    ssh_key='path_to_ssh_key'  # replace with your SSH key path
+)
+os_ops = RemoteOperations(conn_params)
+
+# Add remote testgres config before test
+TestgresConfig.set_os_ops(os_ops=os_ops)
+
+# Proceed with your test
+def test_basic_query(self):
+    with get_remote_node(conn_params=conn_params) as node:
+        node.init().start()
+        res = node.execute('SELECT 1')
+        self.assertEqual(res, [(1,)])
+```
 
 ## Authors
 
 [Ildar Musin](https://github.com/zilder)  
 [Dmitry Ivanov](https://github.com/funbringer)  
 [Ildus Kurbangaliev](https://github.com/ildus)  
 [Yury Zhuravlev](https://github.com/stalkerg)
```

### Comparing `testgres-1.8.9/setup.py` & `testgres-1.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 # Basic dependencies
 install_requires = [
     "pg8000",
     "port-for>=0.4",
     "six>=1.9.0",
     "psutil",
     "packaging",
+    "paramiko",
+    "fabric",
+    "sshtunnel"
 ]
 
 # Add compatibility enum class
 if sys.version_info < (3, 4):
     install_requires.append("enum34")
 
 # Add compatibility ipaddress module
@@ -23,17 +26,17 @@
     install_requires.append("ipaddress")
 
 # Get contents of README file
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
-    version='1.8.9',
+    version='1.9.0',
     name='testgres',
-    packages=['testgres'],
+    packages=['testgres', 'testgres.operations'],
     description='Testing utility for PostgreSQL and its extensions',
     url='https://github.com/postgrespro/testgres',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='PostgreSQL',
     author='Ildar Musin',
     author_email='zildermann@gmail.com',
```

### Comparing `testgres-1.8.9/testgres/__init__.py` & `testgres-1.9.0/testgres/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .api import get_new_node
+from .api import get_new_node, get_remote_node
 from .backup import NodeBackup
 
 from .config import \
     TestgresConfig, \
     configure_testgres, \
     scoped_config, \
     push_config, \
@@ -42,18 +42,24 @@
     get_pg_config, \
     get_pg_version
 
 from .standby import \
     First, \
     Any
 
+from .operations.os_ops import OsOperations, ConnectionParams
+from .operations.local_ops import LocalOperations
+from .operations.remote_ops import RemoteOperations
+
 __all__ = [
     "get_new_node",
+    "get_remote_node",
     "NodeBackup",
     "TestgresConfig", "configure_testgres", "scoped_config", "push_config", "pop_config",
     "NodeConnection", "DatabaseError", "InternalError", "ProgrammingError", "OperationalError",
     "TestgresException", "ExecUtilException", "QueryException", "TimeoutException", "CatchUpException", "StartNodeException", "InitNodeException", "BackupException",
     "XLogMethod", "IsolationLevel", "NodeStatus", "ProcessType", "DumpFormat",
     "PostgresNode", "NodeApp",
     "reserve_port", "release_port", "bound_ports", "get_bin_path", "get_pg_config", "get_pg_version",
     "First", "Any",
+    "OsOperations", "LocalOperations", "RemoteOperations", "ConnectionParams"
 ]
```

### Comparing `testgres-1.8.9/testgres/api.py` & `testgres-1.9.0/testgres/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,7 +36,19 @@
 def get_new_node(name=None, base_dir=None, **kwargs):
     """
     Simply a wrapper around :class:`.PostgresNode` constructor.
     See :meth:`.PostgresNode.__init__` for details.
     """
     # NOTE: leave explicit 'name' and 'base_dir' for compatibility
     return PostgresNode(name=name, base_dir=base_dir, **kwargs)
+
+
+def get_remote_node(name=None, conn_params=None):
+    """
+    Simply a wrapper around :class:`.PostgresNode` constructor for remote node.
+    See :meth:`.PostgresNode.__init__` for details.
+    For remote connection you can add the next parameter:
+    conn_params = ConnectionParams(host='127.0.0.1',
+                                   ssh_key=None,
+                                   username=default_username())
+    """
+    return get_new_node(name=name, conn_params=conn_params)
```

### Comparing `testgres-1.8.9/testgres/backup.py` & `testgres-1.9.0/testgres/backup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # coding: utf-8
 
 import os
 
-from shutil import rmtree, copytree
 from six import raise_from
-from tempfile import mkdtemp
 
 from .enums import XLogMethod
 
 from .consts import \
     DATA_DIR, \
     TMP_NODE, \
     TMP_BACKUP, \
     PG_CONF_FILE, \
     BACKUP_LOG_FILE
 
-from .defaults import default_username
-
 from .exceptions import BackupException
 
 from .utils import \
     get_bin_path, \
     execute_utility, \
     clean_on_error
 
@@ -43,29 +39,29 @@
 
         Args:
             node: :class:`.PostgresNode` we're going to backup.
             base_dir: where should we store it?
             username: database user name.
             xlog_method: none | fetch | stream (see docs)
         """
-
+        self.os_ops = node.os_ops
         if not node.status():
             raise BackupException('Node must be running')
 
         # Check arguments
         if not isinstance(xlog_method, XLogMethod):
             try:
                 xlog_method = XLogMethod(xlog_method)
             except ValueError:
                 msg = 'Invalid xlog_method "{}"'.format(xlog_method)
                 raise BackupException(msg)
 
         # Set default arguments
-        username = username or default_username()
-        base_dir = base_dir or mkdtemp(prefix=TMP_BACKUP)
+        username = username or self.os_ops.get_user()
+        base_dir = base_dir or self.os_ops.mkdtemp(prefix=TMP_BACKUP)
 
         # public
         self.original_node = node
         self.base_dir = base_dir
         self.username = username
 
         # private
@@ -103,22 +99,22 @@
         if not self._available:
             raise BackupException('Backup is exhausted')
 
         # Do we want to use this backup several times?
         available = not destroy
 
         if available:
-            dest_base_dir = mkdtemp(prefix=TMP_NODE)
+            dest_base_dir = self.os_ops.mkdtemp(prefix=TMP_NODE)
 
             data1 = os.path.join(self.base_dir, DATA_DIR)
             data2 = os.path.join(dest_base_dir, DATA_DIR)
 
             try:
                 # Copy backup to new data dir
-                copytree(data1, data2)
+                self.os_ops.copytree(data1, data2)
             except Exception as e:
                 raise_from(BackupException('Failed to copy files'), e)
         else:
             dest_base_dir = self.base_dir
 
         # Is this backup exhausted?
         self._available = available
@@ -139,15 +135,15 @@
         """
 
         # Prepare a data directory for this node
         base_dir = self._prepare_dir(destroy)
 
         # Build a new PostgresNode
         NodeClass = self.original_node.__class__
-        with clean_on_error(NodeClass(name=name, base_dir=base_dir)) as node:
+        with clean_on_error(NodeClass(name=name, base_dir=base_dir, conn_params=self.original_node.os_ops.conn_params)) as node:
 
             # New nodes should always remove dir tree
             node._should_rm_dirs = True
 
             # Set a new port
             node.append_conf(filename=PG_CONF_FILE, line='\n')
             node.append_conf(filename=PG_CONF_FILE, port=node.port)
@@ -181,8 +177,8 @@
         """
         Remove all files that belong to this backup.
         No-op if it's been converted to a PostgresNode (destroy=True).
         """
 
         if self._available:
             self._available = False
-            rmtree(self.base_dir, ignore_errors=True)
+            self.os_ops.rmdirs(self.base_dir, ignore_errors=True)
```

### Comparing `testgres-1.8.9/testgres/cache.py` & `testgres-1.9.0/testgres/cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # coding: utf-8
 
-import io
 import os
 
-from shutil import copytree
 from six import raise_from
 
 from .config import testgres_config
 
 from .consts import XLOG_CONTROL_FILE
 
 from .defaults import generate_system_id
@@ -16,49 +14,54 @@
     InitNodeException, \
     ExecUtilException
 
 from .utils import \
     get_bin_path, \
     execute_utility
 
+from .operations.local_ops import LocalOperations
+from .operations.os_ops import OsOperations
 
-def cached_initdb(data_dir, logfile=None, params=None):
+
+def cached_initdb(data_dir, logfile=None, params=None, os_ops: OsOperations = LocalOperations()):
     """
     Perform initdb or use cached node files.
     """
-    def call_initdb(initdb_dir, log=None):
+
+    def call_initdb(initdb_dir, log=logfile):
         try:
             _params = [get_bin_path("initdb"), "-D", initdb_dir, "-N"]
             execute_utility(_params + (params or []), log)
         except ExecUtilException as e:
             raise_from(InitNodeException("Failed to run initdb"), e)
 
     if params or not testgres_config.cache_initdb:
         call_initdb(data_dir, logfile)
     else:
         # Fetch cached initdb dir
         cached_data_dir = testgres_config.cached_initdb_dir
 
         # Initialize cached initdb
-        if not os.path.exists(cached_data_dir) or \
-           not os.listdir(cached_data_dir):
+
+        if not os_ops.path_exists(cached_data_dir) or \
+                not os_ops.listdir(cached_data_dir):
             call_initdb(cached_data_dir)
 
         try:
             # Copy cached initdb to current data dir
-            copytree(cached_data_dir, data_dir)
+            os_ops.copytree(cached_data_dir, data_dir)
 
             # Assign this node a unique system id if asked to
             if testgres_config.cached_initdb_unique:
                 # XXX: write new unique system id to control file
                 # Some users might rely upon unique system ids, but
                 # our initdb caching mechanism breaks this contract.
                 pg_control = os.path.join(data_dir, XLOG_CONTROL_FILE)
-                with io.open(pg_control, "r+b") as f:
-                    f.write(generate_system_id())    # overwrite id
+                system_id = generate_system_id()
+                os_ops.write(pg_control, system_id, truncate=True, binary=True, read_and_write=True)
 
                 # XXX: build new WAL segment with our system id
                 _params = [get_bin_path("pg_resetwal"), "-D", data_dir, "-f"]
                 execute_utility(_params, logfile)
 
         except ExecUtilException as e:
             msg = "Failed to reset WAL for system id"
```

### Comparing `testgres-1.8.9/testgres/config.py` & `testgres-1.9.0/testgres/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # coding: utf-8
 
 import atexit
 import copy
 import tempfile
 
 from contextlib import contextmanager
-from shutil import rmtree
-from tempfile import mkdtemp
 
 from .consts import TMP_CACHE
+from .operations.os_ops import OsOperations
+from .operations.local_ops import LocalOperations
 
 
 class GlobalConfig(object):
     """
     Global configuration object which allows user to override default settings.
     """
     # NOTE: attributes must not be callable or begin with __.
@@ -39,25 +39,29 @@
     """ remove base_dir on nominal __exit__(). """
 
     node_cleanup_on_bad_exit = False
     """ remove base_dir on __exit__() via exception. """
 
     _cached_initdb_dir = None
     """ underlying class attribute for cached_initdb_dir property """
+
+    os_ops = LocalOperations()
+    """ OsOperation object that allows work on remote host """
     @property
     def cached_initdb_dir(self):
         """ path to a temp directory for cached initdb. """
         return self._cached_initdb_dir
 
     @cached_initdb_dir.setter
     def cached_initdb_dir(self, value):
         self._cached_initdb_dir = value
 
         if value:
             cached_initdb_dirs.add(value)
+        return testgres_config.cached_initdb_dir
 
     @property
     def temp_dir(self):
         """ path to temp dir containing nodes with default 'base_dir'. """
         return tempfile.tempdir
 
     @temp_dir.setter
@@ -114,14 +118,19 @@
     def copy(self):
         """
         Return a copy of this object.
         """
 
         return copy.copy(self)
 
+    @staticmethod
+    def set_os_ops(os_ops: OsOperations):
+        testgres_config.os_ops = os_ops
+        testgres_config.cached_initdb_dir = os_ops.mkdtemp(prefix=TMP_CACHE)
+
 
 # cached dirs to be removed
 cached_initdb_dirs = set()
 
 # default config object
 testgres_config = GlobalConfig()
 
@@ -131,15 +140,15 @@
 # stack of GlobalConfigs
 config_stack = []
 
 
 @atexit.register
 def _rm_cached_initdb_dirs():
     for d in cached_initdb_dirs:
-        rmtree(d, ignore_errors=True)
+        testgres_config.os_ops.rmdirs(d, ignore_errors=True)
 
 
 def push_config(**options):
     """
     Permanently set custom GlobalConfig options and
     put previous settings on top of the config stack.
     """
@@ -194,8 +203,8 @@
     Look at the GlobalConfig to learn about existing settings.
     """
 
     testgres_config.update(options)
 
 
 # NOTE: assign initial cached dir for initdb
-testgres_config.cached_initdb_dir = mkdtemp(prefix=TMP_CACHE)
+testgres_config.cached_initdb_dir = testgres_config.os_ops.mkdtemp(prefix=TMP_CACHE)
```

### Comparing `testgres-1.8.9/testgres/connection.py` & `testgres-1.9.0/testgres/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 
         # Set default arguments
         dbname = dbname or default_dbname()
         username = username or default_username()
 
         self._node = node
 
-        self._connection = pglib.connect(database=dbname,
-                                         user=username,
-                                         password=password,
-                                         host=node.host,
-                                         port=node.port)
+        self._connection = node.os_ops.db_connect(dbname=dbname,
+                                                  user=username,
+                                                  password=password,
+                                                  host=node.host,
+                                                  port=node.port)
 
         self._connection.autocommit = autocommit
         self._cursor = self.connection.cursor()
 
     @property
     def node(self):
         return self._node
@@ -99,22 +99,21 @@
     def rollback(self):
         self.connection.rollback()
 
         return self
 
     def execute(self, query, *args):
         self.cursor.execute(query, args)
-
         try:
             res = self.cursor.fetchall()
-
             # pg8000 might return tuples
             if isinstance(res, tuple):
                 res = [tuple(t) for t in res]
 
             return res
-        except Exception:
+        except Exception as e:
+            print("Error executing query: {}".format(e))
             return None
 
     def close(self):
         self.cursor.close()
         self.connection.close()
```

### Comparing `testgres-1.8.9/testgres/consts.py` & `testgres-1.9.0/testgres/consts.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.9/testgres/decorators.py` & `testgres-1.9.0/testgres/decorators.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.9/testgres/defaults.py` & `testgres-1.9.0/testgres/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import datetime
-import getpass
-import os
 import struct
 import uuid
 
+from .config import testgres_config as tconf
+
 
 def default_dbname():
     """
     Return default DB name.
     """
 
     return 'postgres'
 
 
 def default_username():
     """
     Return default username (current user).
     """
-
-    return getpass.getuser()
+    return tconf.os_ops.get_user()
 
 
 def generate_app_name():
     """
     Generate a new application name for node.
     """
 
@@ -40,11 +39,11 @@
     secs = int((date2 - date1).total_seconds())
     usecs = date2.microsecond
 
     # see pg_resetwal.c : GuessControlValues()
     system_id = 0
     system_id |= (secs << 32)
     system_id |= (usecs << 12)
-    system_id |= (os.getpid() & 0xFFF)
+    system_id |= (tconf.os_ops.get_pid() & 0xFFF)
 
     # pack ULL in native byte order
     return struct.pack('=Q', system_id)
```

### Comparing `testgres-1.8.9/testgres/enums.py` & `testgres-1.9.0/testgres/enums.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.9/testgres/exceptions.py` & `testgres-1.9.0/testgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.9/testgres/logger.py` & `testgres-1.9.0/testgres/logger.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.9/testgres/node.py` & `testgres-1.9.0/testgres/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 # coding: utf-8
 
-import io
 import os
 import random
-import shutil
 import signal
+import subprocess
 import threading
 from queue import Queue
 
-import psutil
-import subprocess
 import time
 
-
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
 # we support both pg8000 and psycopg2
 try:
     import psycopg2 as pglib
 except ImportError:
     try:
         import pg8000 as pglib
     except ImportError:
         raise ImportError("You must have psycopg2 or pg8000 modules installed")
 
-from shutil import rmtree
 from six import raise_from, iteritems, text_type
-from tempfile import mkstemp, mkdtemp
 
 from .enums import \
     NodeStatus, \
     ProcessType, \
     DumpFormat
 
 from .cache import cached_initdb
@@ -89,23 +83,26 @@
 from .standby import First
 
 from .utils import \
     PgVer, \
     eprint, \
     get_bin_path, \
     get_pg_version, \
-    file_tail, \
     reserve_port, \
     release_port, \
     execute_utility, \
     options_string, \
     clean_on_error
 
 from .backup import NodeBackup
 
+from .operations.os_ops import ConnectionParams
+from .operations.local_ops import LocalOperations
+from .operations.remote_ops import RemoteOperations
+
 InternalError = pglib.InternalError
 ProgrammingError = pglib.ProgrammingError
 OperationalError = pglib.OperationalError
 
 
 class ProcessProxy(object):
     """
@@ -126,15 +123,15 @@
     def __repr__(self):
         return '{}(ptype={}, process={})'.format(self.__class__.__name__,
                                                  str(self.ptype),
                                                  repr(self.process))
 
 
 class PostgresNode(object):
-    def __init__(self, name=None, port=None, base_dir=None):
+    def __init__(self, name=None, port=None, base_dir=None, conn_params: ConnectionParams = ConnectionParams()):
         """
         PostgresNode constructor.
 
         Args:
             name: node's application name.
             port: port to accept connections.
             base_dir: path to node's data directory.
@@ -144,18 +141,27 @@
         self._pg_version = PgVer(get_pg_version())
         self._should_free_port = port is None
         self._base_dir = base_dir
         self._logger = None
         self._master = None
 
         # basic
-        self.host = '127.0.0.1'
         self.name = name or generate_app_name()
+        if testgres_config.os_ops:
+            self.os_ops = testgres_config.os_ops
+        elif conn_params.ssh_key:
+            self.os_ops = RemoteOperations(conn_params)
+        else:
+            self.os_ops = LocalOperations(conn_params)
+
         self.port = port or reserve_port()
 
+        self.host = self.os_ops.host
+        self.ssh_key = self.os_ops.ssh_key
+
         # defaults for __exit__()
         self.cleanup_on_good_exit = testgres_config.node_cleanup_on_good_exit
         self.cleanup_on_bad_exit = testgres_config.node_cleanup_on_bad_exit
         self.shutdown_max_attempts = 3
 
         # NOTE: for compatibility
         self.utils_log_name = self.utils_log_file
@@ -191,16 +197,17 @@
     def pid(self):
         """
         Return postmaster's PID if node is running, else 0.
         """
 
         if self.status():
             pid_file = os.path.join(self.data_dir, PG_PID_FILE)
-            with io.open(pid_file) as f:
-                return int(f.readline())
+            lines = self.os_ops.readlines(pid_file)
+            pid = int(lines[0]) if lines else None
+            return pid
 
         # for clarity
         return 0
 
     @property
     def auxiliary_pids(self):
         """
@@ -232,15 +239,15 @@
     def child_processes(self):
         """
         Returns a list of all child processes.
         Each process is represented by :class:`.ProcessProxy` object.
         """
 
         # get a list of postmaster's children
-        children = psutil.Process(self.pid).children()
+        children = self.os_ops.get_process_children(self.pid)
 
         return [ProcessProxy(p) for p in children]
 
     @property
     def source_walsender(self):
         """
         Returns master's walsender feeding this replica.
@@ -270,29 +277,29 @@
     @property
     def master(self):
         return self._master
 
     @property
     def base_dir(self):
         if not self._base_dir:
-            self._base_dir = mkdtemp(prefix=TMP_NODE)
+            self._base_dir = self.os_ops.mkdtemp(prefix=TMP_NODE)
 
         # NOTE: it's safe to create a new dir
-        if not os.path.exists(self._base_dir):
-            os.makedirs(self._base_dir)
+        if not self.os_ops.path_exists(self._base_dir):
+            self.os_ops.makedirs(self._base_dir)
 
         return self._base_dir
 
     @property
     def logs_dir(self):
         path = os.path.join(self.base_dir, LOGS_DIR)
 
         # NOTE: it's safe to create a new dir
-        if not os.path.exists(path):
-            os.makedirs(path)
+        if not self.os_ops.path_exists(path):
+            self.os_ops.makedirs(path)
 
         return path
 
     @property
     def data_dir(self):
         # NOTE: we can't run initdb without user's args
         return os.path.join(self.base_dir, DATA_DIR)
@@ -361,17 +368,15 @@
 
         line = (
             "primary_conninfo='{}'\n"
         ).format(options_string(**conninfo))  # yapf: disable
         # Since 12 recovery.conf had disappeared
         if self.version >= PgVer('12'):
             signal_name = os.path.join(self.data_dir, "standby.signal")
-            # cross-python touch(). It is vulnerable to races, but who cares?
-            with open(signal_name, 'a'):
-                os.utime(signal_name, None)
+            self.os_ops.touch(signal_name)
         else:
             line += "standby_mode=on\n"
 
         if slot:
             # Connect to master for some additional actions
             with master.connect(username=username) as con:
                 # check if slot already exists
@@ -421,27 +426,22 @@
             (os.path.join(self.data_dir, RECOVERY_CONF_FILE), 0),
             (os.path.join(self.data_dir, HBA_CONF_FILE), 0),
             (self.pg_log_file, testgres_config.error_log_lines)
         ]  # yapf: disable
 
         for f, num_lines in files:
             # skip missing files
-            if not os.path.exists(f):
+            if not self.os_ops.path_exists(f):
                 continue
 
-            with io.open(f, "rb") as _f:
-                if num_lines > 0:
-                    # take last N lines of file
-                    lines = b''.join(file_tail(_f, num_lines)).decode('utf-8')
-                else:
-                    # read whole file
-                    lines = _f.read().decode('utf-8')
+            file_lines = self.os_ops.readlines(f, num_lines, binary=True, encoding=None)
+            lines = b''.join(file_lines)
 
-                # fill list
-                result.append((f, lines))
+            # fill list
+            result.append((f, lines))
 
         return result
 
     def init(self, initdb_params=None, **kwargs):
         """
         Perform initdb for this node.
 
@@ -452,17 +452,19 @@
             allow_streaming: should this node add a hba entry for replication?
 
         Returns:
             This instance of :class:`.PostgresNode`
         """
 
         # initialize this PostgreSQL node
-        cached_initdb(data_dir=self.data_dir,
-                      logfile=self.utils_log_file,
-                      params=initdb_params)
+        cached_initdb(
+            data_dir=self.data_dir,
+            logfile=self.utils_log_file,
+            os_ops=self.os_ops,
+            params=initdb_params)
 
         # initialize default config files
         self.default_conf(**kwargs)
 
         return self
 
     def default_conf(self,
@@ -485,51 +487,49 @@
             This instance of :class:`.PostgresNode`.
         """
 
         postgres_conf = os.path.join(self.data_dir, PG_CONF_FILE)
         hba_conf = os.path.join(self.data_dir, HBA_CONF_FILE)
 
         # filter lines in hba file
-        with io.open(hba_conf, "r+") as conf:
-            # get rid of comments and blank lines
-            lines = [
-                s for s in conf.readlines()
-                if len(s.strip()) > 0 and not s.startswith('#')
-            ]
-
-            # write filtered lines
-            conf.seek(0)
-            conf.truncate()
-            conf.writelines(lines)
-
-            # replication-related settings
-            if allow_streaming:
-                # get auth method for host or local users
-                def get_auth_method(t):
-                    return next((s.split()[-1]
-                                 for s in lines if s.startswith(t)), 'trust')
-
-                # get auth methods
-                auth_local = get_auth_method('local')
-                auth_host = get_auth_method('host')
-
-                new_lines = [
-                    u"local\treplication\tall\t\t\t{}\n".format(auth_local),
-                    u"host\treplication\tall\t127.0.0.1/32\t{}\n".format(auth_host),
-                    u"host\treplication\tall\t::1/128\t\t{}\n".format(auth_host)
-                ]  # yapf: disable
-
-                # write missing lines
-                for line in new_lines:
-                    if line not in lines:
-                        conf.write(line)
+        # get rid of comments and blank lines
+        hba_conf_file = self.os_ops.readlines(hba_conf)
+        lines = [
+            s for s in hba_conf_file
+            if len(s.strip()) > 0 and not s.startswith('#')
+        ]
+
+        # write filtered lines
+        self.os_ops.write(hba_conf, lines, truncate=True)
+
+        # replication-related settings
+        if allow_streaming:
+            # get auth method for host or local users
+            def get_auth_method(t):
+                return next((s.split()[-1]
+                             for s in lines if s.startswith(t)), 'trust')
+
+            # get auth methods
+            auth_local = get_auth_method('local')
+            auth_host = get_auth_method('host')
+            subnet_base = ".".join(self.os_ops.host.split('.')[:-1] + ['0'])
+
+            new_lines = [
+                u"local\treplication\tall\t\t\t{}\n".format(auth_local),
+                u"host\treplication\tall\t127.0.0.1/32\t{}\n".format(auth_host),
+                u"host\treplication\tall\t::1/128\t\t{}\n".format(auth_host),
+                u"host\treplication\tall\t{}/24\t\t{}\n".format(subnet_base, auth_host),
+                u"host\tall\tall\t{}/24\t\t{}\n".format(subnet_base, auth_host)
+            ]  # yapf: disable
+
+            # write missing lines
+            self.os_ops.write(hba_conf, new_lines)
 
         # overwrite config file
-        with io.open(postgres_conf, "w") as conf:
-            conf.truncate()
+        self.os_ops.write(postgres_conf, '', truncate=True)
 
         self.append_conf(fsync=fsync,
                          max_worker_processes=MAX_WORKER_PROCESSES,
                          log_statement=log_statement,
                          listen_addresses=self.host,
                          port=self.port)  # yapf:disable
 
@@ -591,23 +591,25 @@
         lines = [line]
 
         for option, value in iteritems(kwargs):
             if isinstance(value, bool):
                 value = 'on' if value else 'off'
             elif not str(value).replace('.', '', 1).isdigit():
                 value = "'{}'".format(value)
-
-            # format a new config line
-            lines.append('{} = {}'.format(option, value))
+            if value == '*':
+                lines.append("{} = '*'".format(option))
+            else:
+                # format a new config line
+                lines.append('{} = {}'.format(option, value))
 
         config_name = os.path.join(self.data_dir, filename)
-        with io.open(config_name, 'a') as conf:
-            for line in lines:
-                conf.write(text_type(line))
-                conf.write(text_type('\n'))
+        conf_text = ''
+        for line in lines:
+            conf_text += text_type(line) + '\n'
+        self.os_ops.write(config_name, conf_text)
 
         return self
 
     def status(self):
         """
         Check this node's status.
 
@@ -617,15 +619,19 @@
 
         try:
             _params = [
                 get_bin_path("pg_ctl"),
                 "-D", self.data_dir,
                 "status"
             ]  # yapf: disable
-            execute_utility(_params, self.utils_log_file)
+            status_code, out, err = execute_utility(_params, self.utils_log_file, verbose=True)
+            if 'does not exist' in err:
+                return NodeStatus.Uninitialized
+            elif 'no server running' in out:
+                return NodeStatus.Stopped
             return NodeStatus.Running
 
         except ExecUtilException as e:
             # Node is not running
             if e.exit_code == 3:
                 return NodeStatus.Stopped
 
@@ -649,40 +655,42 @@
 
         for line in data.splitlines():
             key, _, value = line.partition(':')
             out_dict[key.strip()] = value.strip()
 
         return out_dict
 
-    def slow_start(self, replica=False, dbname='template1', username=default_username()):
+    def slow_start(self, replica=False, dbname='template1', username=default_username(), max_attempts=0):
         """
         Starts the PostgreSQL instance and then polls the instance
         until it reaches the expected state (primary or replica). The state is checked
         using the pg_is_in_recovery() function.
 
         Args:
                dbname:
                username:
                replica: If True, waits for the instance to be in recovery (i.e., replica mode).
                         If False, waits for the instance to be in primary mode. Default is False.
+               max_attempts:
         """
         self.start()
 
         if replica:
             query = 'SELECT pg_is_in_recovery()'
         else:
             query = 'SELECT not pg_is_in_recovery()'
         # Call poll_query_until until the expected value is returned
         self.poll_query_until(query=query,
                               dbname=dbname,
                               username=username,
                               suppress={InternalError,
                                         QueryException,
                                         ProgrammingError,
-                                        OperationalError})
+                                        OperationalError},
+                              max_attempts=max_attempts)
 
     def start(self, params=[], wait=True):
         """
         Starts the PostgreSQL node using pg_ctl if node has not been started.
         By default, it waits for the operation to complete before returning.
         Optionally, it can return immediately without waiting for the start operation
         to complete by setting the `wait` parameter to False.
@@ -702,20 +710,21 @@
             "-D", self.data_dir,
             "-l", self.pg_log_file,
             "-w" if wait else '-W',  # --wait or --no-wait
             "start"
         ] + params  # yapf: disable
 
         try:
-            execute_utility(_params, self.utils_log_file)
-        except ExecUtilException as e:
+            exit_status, out, error = execute_utility(_params, self.utils_log_file, verbose=True)
+            if 'does not exist' in error:
+                raise Exception
+        except Exception as e:
             msg = 'Cannot start node'
             files = self._collect_special_files()
             raise_from(StartNodeException(msg, files), e)
-
         self._maybe_start_logger()
         self.is_started = True
         return self
 
     def stop(self, params=[], wait=True):
         """
         Stops the PostgreSQL node using pg_ctl if the node has been started.
@@ -775,15 +784,17 @@
             "-D", self.data_dir,
             "-l", self.pg_log_file,
             "-w",  # wait
             "restart"
         ] + params  # yapf: disable
 
         try:
-            execute_utility(_params, self.utils_log_file)
+            error_code, out, error = execute_utility(_params, self.utils_log_file, verbose=True)
+            if 'could not start server' in error:
+                raise ExecUtilException
         except ExecUtilException as e:
             msg = 'Cannot restart node'
             files = self._collect_special_files()
             raise_from(StartNodeException(msg, files), e)
 
         self._maybe_start_logger()
 
@@ -891,15 +902,15 @@
 
         # choose directory to be removed
         if testgres_config.node_cleanup_full:
             rm_dir = self.base_dir    # everything
         else:
             rm_dir = self.data_dir    # just data, save logs
 
-        rmtree(rm_dir, ignore_errors=True)
+        self.os_ops.rmdirs(rm_dir, ignore_errors=True)
 
         return self
 
     @method_decorator(positional_args_hack(['dbname', 'query']))
     def psql(self,
              query=None,
              filename=None,
@@ -944,32 +955,39 @@
 
         # set variables before execution
         for key, value in iteritems(variables):
             psql_params.extend(["--set", '{}={}'.format(key, value)])
 
         # select query source
         if query:
-            psql_params.extend(("-c", query))
+            if self.os_ops.remote:
+                psql_params.extend(("-c", '"{}"'.format(query)))
+            else:
+                psql_params.extend(("-c", query))
         elif filename:
             psql_params.extend(("-f", filename))
         else:
             raise QueryException('Query or filename must be provided')
 
         # should be the last one
         psql_params.append(dbname)
+        if not self.os_ops.remote:
+            # start psql process
+            process = subprocess.Popen(psql_params,
+                                       stdin=subprocess.PIPE,
+                                       stdout=subprocess.PIPE,
+                                       stderr=subprocess.PIPE)
+
+            # wait until it finishes and get stdout and stderr
+            out, err = process.communicate(input=input)
+            return process.returncode, out, err
+        else:
+            status_code, out, err = self.os_ops.exec_command(psql_params, verbose=True, input=input)
 
-        # start psql process
-        process = subprocess.Popen(psql_params,
-                                   stdin=subprocess.PIPE,
-                                   stdout=subprocess.PIPE,
-                                   stderr=subprocess.PIPE)
-
-        # wait until it finishes and get stdout and stderr
-        out, err = process.communicate(input=input)
-        return process.returncode, out, err
+            return status_code, out, err
 
     @method_decorator(positional_args_hack(['dbname', 'query']))
     def safe_psql(self, query=None, expect_error=False, **kwargs):
         """
         Execute a query using psql.
 
         Args:
@@ -985,23 +1003,27 @@
 
         Returns:
             psql's output as str.
         """
 
         # force this setting
         kwargs['ON_ERROR_STOP'] = 1
-
-        ret, out, err = self.psql(query=query, **kwargs)
+        try:
+            ret, out, err = self.psql(query=query, **kwargs)
+        except ExecUtilException as e:
+            ret = e.exit_code
+            out = e.out
+            err = e.message
         if ret:
             if expect_error:
                 out = (err or b'').decode('utf-8')
             else:
                 raise QueryException((err or b'').decode('utf-8'), query)
         elif expect_error:
-            assert False, f"Exception was expected, but query finished successfully: `{query}` "
+            assert False, "Exception was expected, but query finished successfully: `{}` ".format(query)
 
         return out
 
     def dump(self,
              filename=None,
              dbname=None,
              username=None,
@@ -1027,18 +1049,17 @@
             except ValueError:
                 msg = 'Invalid format "{}"'.format(format)
                 raise BackupException(msg)
 
         # Generate tmpfile or tmpdir
         def tmpfile():
             if format == DumpFormat.Directory:
-                fname = mkdtemp(prefix=TMP_DUMP)
+                fname = self.os_ops.mkdtemp(prefix=TMP_DUMP)
             else:
-                fd, fname = mkstemp(prefix=TMP_DUMP)
-                os.close(fd)
+                fname = self.os_ops.mkstemp(prefix=TMP_DUMP)
             return fname
 
         # Set default arguments
         dbname = dbname or default_dbname()
         username = username or default_username()
         filename = filename or tmpfile()
 
@@ -1115,17 +1136,17 @@
             >>> poll_query_until('select false', expected=True, max_attempts=4)
             >>> poll_query_until('select 1', suppress={testgres.OperationalError})
         """
 
         # sanity checks
         assert max_attempts >= 0
         assert sleep_time > 0
-
         attempts = 0
         while max_attempts == 0 or attempts < max_attempts:
+            print(f"Pooling {attempts}")
             try:
                 res = self.execute(dbname=dbname,
                                    query=query,
                                    username=username,
                                    commit=commit)
 
                 if expected is None and res is None:
@@ -1346,15 +1367,15 @@
             "-h", self.host,
             "-U", username,
         ] + options  # yapf: disable
 
         # should be the last one
         _params.append(dbname)
 
-        proc = subprocess.Popen(_params, stdout=stdout, stderr=stderr)
+        proc = self.os_ops.exec_command(_params, stdout=stdout, stderr=stderr, wait_exit=True, proc=True)
 
         return proc
 
     def pgbench_init(self, **kwargs):
         """
         Small wrapper for pgbench_run().
         Sets initialize=True.
@@ -1519,26 +1540,24 @@
                                      Defaults to 'postgresql.auto.conf'.
             rm_options (set, optional): A set containing the names of the options to remove.
                                          Defaults to an empty set.
         """
         # parse postgresql.auto.conf
         path = os.path.join(self.data_dir, config)
 
-        with open(path, 'r') as f:
-            raw_content = f.read()
-
+        lines = self.os_ops.readlines(path)
         current_options = {}
         current_directives = []
-        for line in raw_content.splitlines():
+        for line in lines:
 
             # ignore comments
             if line.startswith('#'):
                 continue
 
-            if line == '':
+            if line.strip() == '':
                 continue
 
             if line.startswith('include'):
                 current_directives.append(line)
                 continue
 
             name, var = line.partition('=')[::2]
@@ -1560,30 +1579,30 @@
         for option in current_options:
             auto_conf += "{0} = '{1}'\n".format(
                 option, current_options[option])
 
         for directive in current_directives:
             auto_conf += directive + "\n"
 
-        with open(path, 'wt') as f:
-            f.write(auto_conf)
+        self.os_ops.write(path, auto_conf, truncate=True)
 
 
 class NodeApp:
 
-    def __init__(self, test_path, nodes_to_cleanup):
+    def __init__(self, test_path, nodes_to_cleanup, os_ops=LocalOperations()):
         self.test_path = test_path
         self.nodes_to_cleanup = nodes_to_cleanup
+        self.os_ops = os_ops
 
     def make_empty(
             self,
             base_dir=None):
         real_base_dir = os.path.join(self.test_path, base_dir)
-        shutil.rmtree(real_base_dir, ignore_errors=True)
-        os.makedirs(real_base_dir)
+        self.os_ops.rmdirs(real_base_dir, ignore_errors=True)
+        self.os_ops.makedirs(real_base_dir)
 
         node = PostgresNode(base_dir=real_base_dir)
         node.should_rm_dirs = True
         self.nodes_to_cleanup.append(node)
 
         return node
 
@@ -1598,35 +1617,32 @@
         if checksum and '--data-checksums' not in initdb_params:
             initdb_params.append('--data-checksums')
         node = self.make_empty(base_dir)
         node.init(
             initdb_params=initdb_params, allow_streaming=set_replication)
 
         # set major version
-        with open(os.path.join(node.data_dir, 'PG_VERSION')) as f:
-            node.major_version_str = str(f.read().rstrip())
-            node.major_version = float(node.major_version_str)
-
-        # Sane default parameters
-        options = {}
-        options['max_connections'] = 100
-        options['shared_buffers'] = '10MB'
-        options['fsync'] = 'off'
-
-        options['wal_level'] = 'logical'
-        options['hot_standby'] = 'off'
-
-        options['log_line_prefix'] = '%t [%p]: [%l-1] '
-        options['log_statement'] = 'none'
-        options['log_duration'] = 'on'
-        options['log_min_duration_statement'] = 0
-        options['log_connections'] = 'on'
-        options['log_disconnections'] = 'on'
-        options['restart_after_crash'] = 'off'
-        options['autovacuum'] = 'off'
+        pg_version_file = self.os_ops.read(os.path.join(node.data_dir, 'PG_VERSION'))
+        node.major_version_str = str(pg_version_file.rstrip())
+        node.major_version = float(node.major_version_str)
+
+        # Set default parameters
+        options = {'max_connections': 100,
+                   'shared_buffers': '10MB',
+                   'fsync': 'off',
+                   'wal_level': 'logical',
+                   'hot_standby': 'off',
+                   'log_line_prefix': '%t [%p]: [%l-1] ',
+                   'log_statement': 'none',
+                   'log_duration': 'on',
+                   'log_min_duration_statement': 0,
+                   'log_connections': 'on',
+                   'log_disconnections': 'on',
+                   'restart_after_crash': 'off',
+                   'autovacuum': 'off'}
 
         # Allow replication in pg_hba.conf
         if set_replication:
             options['max_wal_senders'] = 10
 
         if ptrack_enable:
             options['ptrack.map_size'] = '1'
```

### Comparing `testgres-1.8.9/testgres/pubsub.py` & `testgres-1.9.0/testgres/pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,8 +210,8 @@
             """
             self.node.poll_query_until(
                 query=query,
                 dbname=self.pub.dbname,
                 username=username or self.pub.username,
                 max_attempts=LOGICAL_REPL_MAX_CATCHUP_ATTEMPTS)
         except Exception as e:
-            raise_from(CatchUpException("Failed to catch up", query), e)
+            raise_from(CatchUpException("Failed to catch up"), e)
```

### Comparing `testgres-1.8.9/testgres/standby.py` & `testgres-1.9.0/testgres/standby.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.9/testgres/utils.py` & `testgres-1.9.0/testgres/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 from __future__ import division
 from __future__ import print_function
 
-import io
 import os
 import port_for
-import subprocess
 import sys
-import tempfile
 
 from contextlib import contextmanager
 from packaging.version import Version, InvalidVersion
 import re
-try:
-    from shutil import which as find_executable
-except ImportError:
-    from distutils.spawn import find_executable
+
 from six import iteritems
 
-from .config import testgres_config
 from .exceptions import ExecUtilException
+from .config import testgres_config as tconf
 
 # rows returned by PG_CONFIG
 _pg_config_data = {}
 
 # ports used by nodes
 bound_ports = set()
 
@@ -54,145 +48,117 @@
     """
     Free port provided by reserve_port().
     """
 
     bound_ports.discard(port)
 
 
-def execute_utility(args, logfile=None):
+def execute_utility(args, logfile=None, verbose=False):
     """
     Execute utility (pg_ctl, pg_dump etc).
 
     Args:
         args: utility + arguments (list).
         logfile: path to file to store stdout and stderr.
 
     Returns:
         stdout of executed utility.
     """
-
-    # run utility
-    if os.name == 'nt':
-        # using output to a temporary file in Windows
-        buf = tempfile.NamedTemporaryFile()
-
-        process = subprocess.Popen(
-            args,    # util + params
-            stdout=buf,
-            stderr=subprocess.STDOUT)
-        process.communicate()
-
-        # get result
-        buf.file.flush()
-        buf.file.seek(0)
-        out = buf.file.read()
-        buf.close()
-    else:
-        process = subprocess.Popen(
-            args,    # util + params
-            stdout=subprocess.PIPE,
-            stderr=subprocess.STDOUT)
-
-        # get result
-        out, _ = process.communicate()
-
+    exit_status, out, error = tconf.os_ops.exec_command(args, verbose=True)
     # decode result
-    out = '' if not out else out.decode('utf-8')
-
-    # format command
-    command = u' '.join(args)
+    out = '' if not out else out
+    if isinstance(out, bytes):
+        out = out.decode('utf-8')
+    if isinstance(error, bytes):
+        error = error.decode('utf-8')
 
     # write new log entry if possible
     if logfile:
         try:
-            with io.open(logfile, 'a') as file_out:
-                file_out.write(command)
-
-                if out:
-                    # comment-out lines
-                    lines = ('# ' + line for line in out.splitlines(True))
-                    file_out.write(u'\n')
-                    file_out.writelines(lines)
-
-                file_out.write(u'\n')
+            tconf.os_ops.write(filename=logfile, data=args, truncate=True)
+            if out:
+                # comment-out lines
+                lines = [u'\n'] + ['# ' + line for line in out.splitlines()] + [u'\n']
+                tconf.os_ops.write(filename=logfile, data=lines)
         except IOError:
-            pass
-
-    exit_code = process.returncode
-    if exit_code:
-        message = 'Utility exited with non-zero code'
-        raise ExecUtilException(message=message,
-                                command=command,
-                                exit_code=exit_code,
-                                out=out)
-
-    return out
+            raise ExecUtilException("Problem with writing to logfile `{}` during run command `{}`".format(logfile, args))
+    if verbose:
+        return exit_status, out, error
+    else:
+        return out
 
 
 def get_bin_path(filename):
     """
     Return absolute path to an executable using PG_BIN or PG_CONFIG.
     This function does nothing if 'filename' is already absolute.
     """
-
     # check if it's already absolute
     if os.path.isabs(filename):
         return filename
+    if tconf.os_ops.remote:
+        pg_config = os.environ.get("PG_CONFIG_REMOTE") or os.environ.get("PG_CONFIG")
+    else:
+        # try PG_CONFIG - get from local machine
+        pg_config = os.environ.get("PG_CONFIG")
 
-    # try PG_CONFIG
-    pg_config = os.environ.get("PG_CONFIG")
     if pg_config:
         bindir = get_pg_config()["BINDIR"]
         return os.path.join(bindir, filename)
 
     # try PG_BIN
-    pg_bin = os.environ.get("PG_BIN")
+    pg_bin = tconf.os_ops.environ("PG_BIN")
     if pg_bin:
         return os.path.join(pg_bin, filename)
 
-    pg_config_path = find_executable('pg_config')
+    pg_config_path = tconf.os_ops.find_executable('pg_config')
     if pg_config_path:
         bindir = get_pg_config(pg_config_path)["BINDIR"]
         return os.path.join(bindir, filename)
 
     return filename
 
 
 def get_pg_config(pg_config_path=None):
     """
     Return output of pg_config (provided that it is installed).
-    NOTE: this fuction caches the result by default (see GlobalConfig).
+    NOTE: this function caches the result by default (see GlobalConfig).
     """
+
     def cache_pg_config_data(cmd):
         # execute pg_config and get the output
-        out = subprocess.check_output([cmd]).decode('utf-8')
+        out = tconf.os_ops.exec_command(cmd, encoding='utf-8')
 
         data = {}
         for line in out.splitlines():
             if line and '=' in line:
                 key, _, value = line.partition('=')
                 data[key.strip()] = value.strip()
 
         # cache data
         global _pg_config_data
         _pg_config_data = data
 
         return data
 
     # drop cache if asked to
-    if not testgres_config.cache_pg_config:
+    if not tconf.cache_pg_config:
         global _pg_config_data
         _pg_config_data = {}
 
     # return cached data
     if _pg_config_data:
         return _pg_config_data
 
     # try specified pg_config path or PG_CONFIG
-    pg_config = pg_config_path or os.environ.get("PG_CONFIG")
+    if tconf.os_ops.remote:
+        pg_config = pg_config_path or os.environ.get("PG_CONFIG_REMOTE") or os.environ.get("PG_CONFIG")
+    else:
+        # try PG_CONFIG - get from local machine
+        pg_config = pg_config_path or os.environ.get("PG_CONFIG")
     if pg_config:
         return cache_pg_config_data(pg_config)
 
     # try PG_BIN
     pg_bin = os.environ.get("PG_BIN")
     if pg_bin:
         cmd = os.path.join(pg_bin, "pg_config")
@@ -205,15 +171,15 @@
 def get_pg_version():
     """
     Return PostgreSQL version provided by postmaster.
     """
 
     # get raw version (e.g. postgres (PostgreSQL) 9.5.7)
     _params = [get_bin_path('postgres'), '--version']
-    raw_ver = subprocess.check_output(_params).decode('utf-8')
+    raw_ver = tconf.os_ops.exec_command(_params, encoding='utf-8')
 
     # cook version of PostgreSQL
     version = raw_ver.strip().split(' ')[-1] \
                      .partition('devel')[0] \
                      .partition('beta')[0] \
                      .partition('rc')[0]
```

### Comparing `testgres-1.8.9/testgres.egg-info/PKG-INFO` & `testgres-1.9.0/testgres.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testgres
-Version: 1.8.9
+Version: 1.9.0
 Summary: Testing utility for PostgreSQL and its extensions
 Home-page: https://github.com/postgrespro/testgres
 Author: Ildar Musin
 Author-email: zildermann@gmail.com
 License: PostgreSQL
 Keywords: test,testing,postgresql
 Platform: UNKNOWN
@@ -182,14 +182,41 @@
     # add a new config line
     master.append_conf('postgresql.conf', ext_conf)
 ```
 
 Note that `default_conf()` is called by `init()` function; both of them overwrite
 the configuration file, which means that they should be called before `append_conf()`.
 
+### Remote mode
+Testgres supports the creation of PostgreSQL nodes on a remote host. This is useful when you want to run distributed tests involving multiple nodes spread across different machines.
+
+To use this feature, you need to use the RemoteOperations class.
+Here is an example of how you might set this up:
+
+```python
+from testgres import ConnectionParams, RemoteOperations, TestgresConfig, get_remote_node
+
+# Set up connection params
+conn_params = ConnectionParams(
+    host='your_host',  # replace with your host
+    username='user_name',  # replace with your username
+    ssh_key='path_to_ssh_key'  # replace with your SSH key path
+)
+os_ops = RemoteOperations(conn_params)
+
+# Add remote testgres config before test
+TestgresConfig.set_os_ops(os_ops=os_ops)
+
+# Proceed with your test
+def test_basic_query(self):
+    with get_remote_node(conn_params=conn_params) as node:
+        node.init().start()
+        res = node.execute('SELECT 1')
+        self.assertEqual(res, [(1,)])
+```
 
 ## Authors
 
 [Ildar Musin](https://github.com/zilder)  
 [Dmitry Ivanov](https://github.com/funbringer)  
 [Ildus Kurbangaliev](https://github.com/ildus)  
 [Yury Zhuravlev](https://github.com/stalkerg)
```

### Comparing `testgres-1.8.9/testgres.egg-info/SOURCES.txt` & `testgres-1.9.0/testgres.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -20,8 +20,14 @@
 testgres/standby.py
 testgres/utils.py
 testgres.egg-info/PKG-INFO
 testgres.egg-info/SOURCES.txt
 testgres.egg-info/dependency_links.txt
 testgres.egg-info/requires.txt
 testgres.egg-info/top_level.txt
-tests/test_simple.py
+testgres/operations/__init__.py
+testgres/operations/local_ops.py
+testgres/operations/os_ops.py
+testgres/operations/remote_ops.py
+tests/test_remote.py
+tests/test_simple.py
+tests/test_simple_remote.py
```

### Comparing `testgres-1.8.9/tests/test_simple.py` & `testgres-1.9.0/tests/test_simple.py`

 * *Files identical despite different names*

