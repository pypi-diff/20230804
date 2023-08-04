# Comparing `tmp/encapsule-0.1.0.tar.gz` & `tmp/encapsule-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.1.0.tar", last modified: Wed Aug  2 13:51:55 2023, max compression
+gzip compressed data, was "encapsule-0.1.1.tar", last modified: Fri Aug  4 03:18:52 2023, max compression
```

## Comparing `encapsule-0.1.0.tar` & `encapsule-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:51:55.630334 encapsule-0.1.0/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 13:51:55.630334 encapsule-0.1.0/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.1.0/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:51:55.599224 encapsule-0.1.0/encapsule/
--rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.1.0/encapsule/__init__.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     6232 2023-08-02 13:50:54.000000 encapsule-0.1.0/encapsule/isolate_bin.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     1386 2023-08-02 13:26:50.000000 encapsule-0.1.0/encapsule/isolate_mgr.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     7603 2023-08-02 13:13:45.000000 encapsule-0.1.0/encapsule/isolate_sys.py
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:51:55.630334 encapsule-0.1.0/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 13:51:54.000000 encapsule-0.1.0/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      254 2023-08-02 13:51:54.000000 encapsule-0.1.0/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-02 13:51:54.000000 encapsule-0.1.0/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-02 13:51:54.000000 encapsule-0.1.0/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-02 13:51:55.630334 encapsule-0.1.0/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-02 13:51:12.000000 encapsule-0.1.0/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-04 03:18:52.857484 encapsule-0.1.1/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-04 03:18:52.857484 encapsule-0.1.1/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.1.1/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-04 03:18:52.810623 encapsule-0.1.1/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.1.1/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     5813 2023-08-03 02:53:37.000000 encapsule-0.1.1/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     1870 2023-08-04 00:02:21.000000 encapsule-0.1.1/encapsule/isolate_mgr.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     8099 2023-08-03 02:57:27.000000 encapsule-0.1.1/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-04 03:18:52.841861 encapsule-0.1.1/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-04 03:18:51.000000 encapsule-0.1.1/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      254 2023-08-04 03:18:51.000000 encapsule-0.1.1/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-04 03:18:51.000000 encapsule-0.1.1/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-04 03:18:51.000000 encapsule-0.1.1/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-04 03:18:52.857484 encapsule-0.1.1/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-04 03:18:21.000000 encapsule-0.1.1/setup.py
```

### Comparing `encapsule-0.1.0/PKG-INFO` & `encapsule-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.1.0
+Version: 0.1.1
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.1.0/encapsule/isolate_bin.py` & `encapsule-0.1.1/encapsule/isolate_bin.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 			# todo: Is this always true?
 			self.taskId_new	= isolate_sys.taskId()
 
 		# _posixsubprocess-setuid: is this available on cygwin?
 		# Todo: cygwin multi-user testing setup.
 		# Todo: specification of UID?
 		kwd['user'] = isolate_sys.componentOwnerUser \
-			(self.name, enforce = kwd.get('userId') \
+			(self.name, enforce = kwd.pop('userId') \
 				or isolate_sys.effectiveContextId())
 
 		return kwd
 
 	@contextmanager
 	def runContext(self, process):
 		# grr
@@ -161,24 +161,14 @@
 		# XXX DISABLED FOR TESTING XXX
 		# isolate_sys.checkAccessCurrentUser(self.name)
 
 		settings = self.newTaskId_env \
 			(runContext = self.runContext,
 			 userId = kwd.get('userId'))
 
-		# XXX Todo: inside, set system-level 'current frame process id'
-		# for whatever this task is.  Do this in a python context, when
-		# exiting, reset to 'this frame process id.'
-		# return self.executable.pipeStringContext \
-		# 	(isolate_sys.effectiveContextId(), args,
-		# 	 # segments = self.parentOptions.segments,
-		# 	 # setTaskFrame_pid = isolate_sys.setTaskFrame_pid,
-		# 	 **settings)
-
-		# To work:
 		# import pdb; pdb.set_trace()
 		return self.executable.pipe \
 			(*args, **settings) \
 			.decode() # Why subprocess returns bytes stream,
 					  # but sys.stdout is default opened str.
 
 def main(argv):
```

### Comparing `encapsule-0.1.0/encapsule/isolate_mgr.py` & `encapsule-0.1.1/encapsule/isolate_mgr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 from . import isolate_sys
 
+
+def gdbAttach(processId, name = 'gdb'):
+    for bin in io.which(name):
+        return bin(name).spawn('-p', str(processId))
+
+
 def main(argv = None):
     from optparse import OptionParser
     parser = OptionParser()
 
     (options, args) = parser.parse_args(argv)
     (command, *args) = args
 
@@ -23,14 +29,24 @@
             isolate_sys.resumeTask(name)
 
         elif subcmd in ['kill']:
             (name,) = args
             (frame,) = isolate_sys.orchObject_i.taskOf(name)
             frame.process.terminate()
 
+        elif subcmd in ['pidof', 'pid', 'pidOf']:
+            (name,) = args
+            (frame,) = isolate_sys.orchObject_i.taskOf(name)
+            print(frame.process.pid)
+
+        elif subcmd in ['attach']:
+            (name,) = args
+            (frame,) = isolate_sys.orchObject_i.taskOf(name)
+            gdbAttach(frame.process.pid)
+
     elif command == 'access':
         (subcmd, *args) = args
 
         if subcmd in ['grant']:
             # encapsule.isolate_mgr access grant op read services/x/bin
             (userId, access, name) = args
             isolate_sys.grantAccess(userId, name, access = access)
```

### Comparing `encapsule-0.1.0/encapsule/isolate_sys.py` & `encapsule-0.1.1/encapsule/isolate_sys.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,30 +64,54 @@
 		try: return self.pathOf(i, name).read()
 		except Exception as e:
 			try: return kwd['default']
 			except:
 				raise e
 
 	def erase(self, i, name):
-		return self.pathOf(i, name).delete()
+		# Todo: audit this destructive method.
+		# return self.pathOf(i, name).delete()
 
-		# path = self.pathOf(i, name)
+		path = self.pathOf(i, name)
 
-		# if path.isdir:
-		#   # XXX removedirs doesn't remove non-empty dirs
-		#	from os import removedirs
-		# 	return removedirs(path)
+		if path.isdir:
+			return destroydirs(path, force = True)
 
-		# return path.delete()
+			# XXX removedirs might not be right algo at all
+		    # XXX removedirs doesn't remove non-empty dirs
+			# from os import removedirs
+			# return removedirs(path)
+
+		return path.delete()
 
 	def touch(self, i, name):
 		return self.store(i, name, '')
 
 
 # Filesystem
+from os import rmdir, listdir, unlink
+from os.path import join as joindir, isdir
+
+def destroydirs(name, force = False):
+	if isdir(name):
+		for c in listdir(name):
+			# recurse
+			destroydirs(joindir(name, c), force = force)
+
+		if force:
+			rmdir(name)
+		else:
+			print(f'removing {name}')
+
+	elif force:
+		unlink(name)
+
+	else:
+		print(f'removing {name}')
+
 def restrict_path(root, path):
 	r = root = io.path(root)
 
 	for p in path:
 		if p != '..' or r != root:
 			# Note: empty components are ignored.
 			r = r(p)
@@ -105,21 +129,22 @@
 def setTaskFrame_pid(i, pid, compartment):
 	# "addTaskFrame"
 
 	# i = taskId()
 
 	# import pdb; pdb.set_trace()
 
-	u = int(retrieve(storageClass.TASKS, f'{i}:frameCurrent', default = -1))
+	fu = f'{i}:frameCurrent'
+
+	u = int(retrieve(storageClass.TASKS, fu, default = -1))
 	ui = u + 1
 
 	newU = f'{i}:processId:{ui}'
 	store(storageClass.TASKS, newU, pid)
 
-	fu = f'{i}:frameCurrent'
 	store(storageClass.TASKS, fu, ui)
 
 	try: yield
 	finally:
 		erase(storageClass.TASKS, newU)
 
 		if compartment:
```

### Comparing `encapsule-0.1.0/encapsule.egg-info/PKG-INFO` & `encapsule-0.1.1/encapsule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.1.0
+Version: 0.1.1
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.1.0/setup.py` & `encapsule-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 try: from setuptools import setup, find_packages
 except ImportError: from distutils.core import setup, find_packages
 
 SETUP_CONF = \
 dict (name = "encapsule",
       description = "POSIX application security.",
```

