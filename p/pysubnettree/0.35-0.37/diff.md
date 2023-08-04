# Comparing `tmp/pysubnettree-0.35.tar.gz` & `tmp/pysubnettree-0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysubnettree-0.35.tar", last modified: Tue Dec 15 07:01:09 2020, max compression
+gzip compressed data, was "pysubnettree-0.37.tar", last modified: Fri Aug  4 11:23:07 2023, max compression
```

## Comparing `pysubnettree-0.35.tar` & `pysubnettree-0.37.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jsiwek     (501) staff       (20)        0 2020-12-15 07:01:09.248808 pysubnettree-0.35/
--rw-r--r--   0 jsiwek     (501) staff       (20)     8163 2020-12-15 06:47:24.000000 pysubnettree-0.35/CHANGES
--rw-r--r--   0 jsiwek     (501) staff       (20)     1839 2020-06-08 19:15:26.000000 pysubnettree-0.35/COPYING
--rw-r--r--   0 jsiwek     (501) staff       (20)      142 2020-06-08 19:15:26.000000 pysubnettree-0.35/MANIFEST.in
--rw-r--r--   0 jsiwek     (501) staff       (20)     1123 2020-12-07 18:12:27.000000 pysubnettree-0.35/Makefile
--rw-r--r--   0 jsiwek     (501) staff       (20)      442 2020-12-15 07:01:09.248559 pysubnettree-0.35/PKG-INFO
--rw-r--r--   0 jsiwek     (501) staff       (20)     2923 2020-12-15 06:47:24.000000 pysubnettree-0.35/README
--rw-r--r--   0 jsiwek     (501) staff       (20)     9530 2020-06-08 19:15:26.000000 pysubnettree-0.35/SubnetTree.cc
--rw-r--r--   0 jsiwek     (501) staff       (20)       85 2020-06-08 19:15:26.000000 pysubnettree-0.35/SubnetTree.i
--rw-r--r--   0 jsiwek     (501) staff       (20)     5347 2020-06-08 19:15:26.000000 pysubnettree-0.35/SubnetTree.py
--rw-r--r--   0 jsiwek     (501) staff       (20)   165484 2020-06-08 19:15:26.000000 pysubnettree-0.35/SubnetTree_wrap.cc
--rw-r--r--   0 jsiwek     (501) staff       (20)        5 2020-12-15 06:47:24.000000 pysubnettree-0.35/VERSION
-drwxr-xr-x   0 jsiwek     (501) staff       (20)        0 2020-12-15 07:01:09.246771 pysubnettree-0.35/include/
--rw-r--r--   0 jsiwek     (501) staff       (20)     4506 2020-06-08 19:15:26.000000 pysubnettree-0.35/include/SubnetTree.h
--rw-r--r--   0 jsiwek     (501) staff       (20)     6091 2020-06-08 19:15:26.000000 pysubnettree-0.35/include/patricia.h
--rw-r--r--   0 jsiwek     (501) staff       (20)    26913 2020-09-22 18:03:34.000000 pysubnettree-0.35/patricia.c
-drwxr-xr-x   0 jsiwek     (501) staff       (20)        0 2020-12-15 07:01:09.248208 pysubnettree-0.35/pysubnettree.egg-info/
--rw-r--r--   0 jsiwek     (501) staff       (20)      442 2020-12-15 07:01:09.000000 pysubnettree-0.35/pysubnettree.egg-info/PKG-INFO
--rw-r--r--   0 jsiwek     (501) staff       (20)      315 2020-12-15 07:01:09.000000 pysubnettree-0.35/pysubnettree.egg-info/SOURCES.txt
--rw-r--r--   0 jsiwek     (501) staff       (20)        1 2020-12-15 07:01:09.000000 pysubnettree-0.35/pysubnettree.egg-info/dependency_links.txt
--rw-r--r--   0 jsiwek     (501) staff       (20)       23 2020-12-15 07:01:09.000000 pysubnettree-0.35/pysubnettree.egg-info/top_level.txt
--rw-r--r--   0 jsiwek     (501) staff       (20)       38 2020-12-15 07:01:09.248890 pysubnettree-0.35/setup.cfg
--rw-r--r--   0 jsiwek     (501) staff       (20)     1034 2020-12-15 06:47:24.000000 pysubnettree-0.35/setup.py
+drwxr-xr-x   0 awelzel   (1000) awelzel   (1000)        0 2023-08-04 11:23:07.577966 pysubnettree-0.37/
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     9755 2023-08-04 11:06:20.000000 pysubnettree-0.37/CHANGES
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     1839 2022-11-02 16:26:59.000000 pysubnettree-0.37/COPYING
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)      142 2022-11-02 16:26:59.000000 pysubnettree-0.37/MANIFEST.in
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     1121 2023-08-03 09:11:37.000000 pysubnettree-0.37/Makefile
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)      692 2023-08-04 11:23:07.577966 pysubnettree-0.37/PKG-INFO
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     3054 2023-08-04 11:06:20.000000 pysubnettree-0.37/README
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     9561 2023-08-03 10:13:42.000000 pysubnettree-0.37/SubnetTree.cc
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)       85 2022-11-02 16:26:59.000000 pysubnettree-0.37/SubnetTree.i
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     5811 2023-08-04 10:52:40.000000 pysubnettree-0.37/SubnetTree.py
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)   168810 2023-08-04 10:52:43.000000 pysubnettree-0.37/SubnetTree_wrap.cc
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)        5 2023-08-04 11:06:20.000000 pysubnettree-0.37/VERSION
+drwxr-xr-x   0 awelzel   (1000) awelzel   (1000)        0 2023-08-04 11:23:07.573966 pysubnettree-0.37/include/
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     4559 2023-08-03 09:11:37.000000 pysubnettree-0.37/include/SubnetTree.h
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     9064 2023-08-03 09:11:37.000000 pysubnettree-0.37/include/patricia.h
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)    29432 2023-08-03 09:11:37.000000 pysubnettree-0.37/patricia.c
+drwxr-xr-x   0 awelzel   (1000) awelzel   (1000)        0 2023-08-04 11:23:07.577966 pysubnettree-0.37/pysubnettree.egg-info/
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)      692 2023-08-04 11:23:07.000000 pysubnettree-0.37/pysubnettree.egg-info/PKG-INFO
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)      315 2023-08-04 11:23:07.000000 pysubnettree-0.37/pysubnettree.egg-info/SOURCES.txt
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)        1 2023-08-04 11:23:07.000000 pysubnettree-0.37/pysubnettree.egg-info/dependency_links.txt
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)       23 2023-08-04 11:23:07.000000 pysubnettree-0.37/pysubnettree.egg-info/top_level.txt
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)       38 2023-08-04 11:23:07.577966 pysubnettree-0.37/setup.cfg
+-rw-r--r--   0 awelzel   (1000) awelzel   (1000)     1465 2023-08-04 11:06:20.000000 pysubnettree-0.37/setup.py
```

### Comparing `pysubnettree-0.35/CHANGES` & `pysubnettree-0.37/CHANGES`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,56 @@
+0.37 | 2023-08-04 13:05:19 +0200
+
+  * Release 0.37.
+
+0.36-24 | 2023-08-04 13:01:39 +0200
+
+  * Use devN style format in setup.py (Arne Welzel, Corelight)
+
+    Commit aa205cfa996d166ae54ce5fdcebaf4b310301a34 switched this to .postN
+    format, but update-changes only recognizes .devN, so switch to that in
+    order to make automatic updating of setup.py versions work again.
+
+0.36-23 | 2023-08-04 12:42:03 +0200
+
+  * GH-15: GH-32: GH-33: SubnetTree: Update swig generated files (Arne Welzel, Corelight)
+
+0.36-21 | 2023-08-02 11:25:16 -0700
+
+  * Update cmake submodule to deprecate FindRequiredPackage (Tim Wojtulewicz, Corelight)
+
+  * Require CMake 3.15 for consistency with other Zeek projects (Tim Wojtulewicz, Corelight)
+
+  * Fix python variable usage in configure (Tim Wojtulewicz, Corelight)
+
+  * Use find_package instead of FindRequiredPackage (Tim Wojtulewicz, Corelight)
+
+0.36-15 | 2023-06-01 10:49:13 +0200
+
+  * Use new-style version numbers for setup.py (Tim Wojtulewicz, Corelight)
+
+  * Remove old travis CI configuration, add new Github workflow instead (Tim Wojtulewicz, Corelight)
+
+  * Update patricia files to match Zeek's newer version (Tim Wojtulewicz, Corelight)
+
+0.36-5 | 2022-12-15 10:57:11 -0700
+
+  * Makefile: Fix .cc and .cpp confusion (Arne Welzel, Corelight)
+
+0.36 | 2022-06-01 09:30:15 -0700
+
+  * Release 0.36
+
+  * Update cmake submodule to latest master (Tim Wojtulewicz, Corelight)
+
+0.35-4 | 2021-03-12 13:09:15 -0800
+
+  * GH-25: Add description of supported platforms to README (Jon Siwek, Corelight)
+
+  * Add trove classifiers to setup.py (Jon Siwek, Corelight)
 
 0.35 | 2020-12-07 15:05:57 -0800
 
   * Release 0.35.
 
 0.34-16 | 2020-12-07 15:05:32 -0800
```

### Comparing `pysubnettree-0.35/COPYING` & `pysubnettree-0.37/COPYING`

 * *Files identical despite different names*

### Comparing `pysubnettree-0.35/Makefile` & `pysubnettree-0.37/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 CLEAN=build SubnetTree_wrap.cc SubnetTree.py README.html *.pyc
 
 VERSION=`test -e VERSION && cat VERSION || cat ../VERSION`
 BUILD=build
 TGZ=pysubnettree-$(VERSION)
 
-all: SubnetTree_wrap.cpp
+all: SubnetTree_wrap.cc
 
-SubnetTree_wrap.cpp SubnetTree.py: SubnetTree.i include/SubnetTree.h
+SubnetTree_wrap.cc SubnetTree.py: SubnetTree.i include/SubnetTree.h
 	swig -c++ -python -Iinclude -o SubnetTree_wrap.cc SubnetTree.i
 
 clean:
 	rm -rf $(CLEAN)
 
 .PHONY: dist
 dist:
```

### Comparing `pysubnettree-0.35/README` & `pysubnettree-0.37/README`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 ..	-*- mode: rst-mode -*-
 ..
 .. Version number is filled in automatically.
-.. |version| replace:: 0.35
+.. |version| replace:: 0.37
 
 ===============================================
 PySubnetTree - A Python Module for CIDR Lookups
 ===============================================
 
 .. rst-class:: opening
 
     The PySubnetTree package provides a Python data structure
     ``SubnetTree`` which maps subnets given in `CIDR
     <http://tools.ietf.org/html/rfc4632>`_ notation (incl.
     corresponding IPv6 versions) to Python objects. Lookups are
     performed by longest-prefix matching.
 
+    PySubnetTree should generally work on Unix-like platforms such as Linux,
+    macOS, and FreeBSD, but does not support Windows.
 
 Download
 --------
 
 You can find the latest PySubnetTree release for download at
 https://www.zeek.org/download.
```

### Comparing `pysubnettree-0.35/SubnetTree.cc` & `pysubnettree-0.37/SubnetTree.cc`

 * *Files 1% similar despite different names*

```diff
@@ -97,28 +97,28 @@
         else
             *mask = 128;
     }
 
     return true;
 }
 
-static void free_data(void *data)
+void SubnetTree::PatriciaDeleteFunction(void* data)
 {
     Py_DECREF(static_cast<PyObject*>(data));
 }
 
 SubnetTree::SubnetTree(bool arg_binary_lookup_mode)
 {
     tree = New_Patricia(128);
     binary_lookup_mode = arg_binary_lookup_mode;
 }
 
 SubnetTree::~SubnetTree()
 {
-    Destroy_Patricia(tree, (void (*)())free_data);
+    Destroy_Patricia(tree, SubnetTree::PatriciaDeleteFunction);
 }
 
 PyObject* SubnetTree::insert(const char *cidr, PyObject* data)
 {
     int family;
     inx_addr subnet;
     unsigned short mask;
```

### Comparing `pysubnettree-0.35/SubnetTree.py` & `pysubnettree-0.37/SubnetTree.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 # This file was automatically generated by SWIG (http://www.swig.org).
-# Version 3.0.7
+# Version 3.0.12
 #
 # Do not make changes to this file unless you know what you are doing--modify
 # the SWIG interface file instead.
 
-
-
-
-
-from sys import version_info
-if version_info >= (2, 6, 0):
+from sys import version_info as _swig_python_version_info
+if _swig_python_version_info >= (2, 7, 0):
+    def swig_import_helper():
+        import importlib
+        pkg = __name__.rpartition('.')[0]
+        mname = '.'.join((pkg, '_SubnetTree')).lstrip('.')
+        try:
+            return importlib.import_module(mname)
+        except ImportError:
+            return importlib.import_module('_SubnetTree')
+    _SubnetTree = swig_import_helper()
+    del swig_import_helper
+elif _swig_python_version_info >= (2, 6, 0):
     def swig_import_helper():
         from os.path import dirname
         import imp
         fp = None
         try:
             fp, pathname, description = imp.find_module('_SubnetTree', [dirname(__file__)])
         except ImportError:
             import _SubnetTree
             return _SubnetTree
-        if fp is not None:
-            try:
-                _mod = imp.load_module('_SubnetTree', fp, pathname, description)
-            finally:
+        try:
+            _mod = imp.load_module('_SubnetTree', fp, pathname, description)
+        finally:
+            if fp is not None:
                 fp.close()
-            return _mod
+        return _mod
     _SubnetTree = swig_import_helper()
     del swig_import_helper
 else:
     import _SubnetTree
-del version_info
+del _swig_python_version_info
+
 try:
     _swig_property = property
 except NameError:
     pass  # Python < 2.2 doesn't have 'property'.
 
+try:
+    import builtins as __builtin__
+except ImportError:
+    import __builtin__
 
 def _swig_setattr_nondynamic(self, class_type, name, value, static=1):
     if (name == "thisown"):
         return self.this.own(value)
     if (name == "this"):
         if type(value).__name__ == 'SwigPyObject':
             self.__dict__[name] = value
@@ -55,45 +67,38 @@
         raise AttributeError("You cannot add attributes to %s" % self)
 
 
 def _swig_setattr(self, class_type, name, value):
     return _swig_setattr_nondynamic(self, class_type, name, value, 0)
 
 
-def _swig_getattr_nondynamic(self, class_type, name, static=1):
+def _swig_getattr(self, class_type, name):
     if (name == "thisown"):
         return self.this.own()
     method = class_type.__swig_getmethods__.get(name, None)
     if method:
         return method(self)
-    if (not static):
-        return object.__getattr__(self, name)
-    else:
-        raise AttributeError(name)
-
-def _swig_getattr(self, class_type, name):
-    return _swig_getattr_nondynamic(self, class_type, name, 0)
+    raise AttributeError("'%s' object has no attribute '%s'" % (class_type.__name__, name))
 
 
 def _swig_repr(self):
     try:
         strthis = "proxy of " + self.this.__repr__()
-    except:
+    except __builtin__.Exception:
         strthis = ""
     return "<%s.%s; %s >" % (self.__class__.__module__, self.__class__.__name__, strthis,)
 
 try:
     _object = object
     _newclass = 1
-except AttributeError:
+except __builtin__.Exception:
     class _object:
         pass
     _newclass = 0
 
-
 class inx_addr(_object):
     __swig_setmethods__ = {}
     __setattr__ = lambda self, name, value: _swig_setattr(self, inx_addr, name, value)
     __swig_getmethods__ = {}
     __getattr__ = lambda self, name: _swig_getattr(self, inx_addr, name)
     __repr__ = _swig_repr
     __swig_setmethods__["sin"] = _SubnetTree.inx_addr_sin_set
@@ -105,15 +110,15 @@
     if _newclass:
         sin6 = _swig_property(_SubnetTree.inx_addr_sin6_get, _SubnetTree.inx_addr_sin6_set)
 
     def __init__(self):
         this = _SubnetTree.new_inx_addr()
         try:
             self.this.append(this)
-        except:
+        except __builtin__.Exception:
             self.this = this
     __swig_destroy__ = _SubnetTree.delete_inx_addr
     __del__ = lambda self: None
 inx_addr_swigregister = _SubnetTree.inx_addr_swigregister
 inx_addr_swigregister(inx_addr)
 
 class SubnetTree(_object):
@@ -123,15 +128,15 @@
     __getattr__ = lambda self, name: _swig_getattr(self, SubnetTree, name)
     __repr__ = _swig_repr
 
     def __init__(self, binary_lookup_mode=False):
         this = _SubnetTree.new_SubnetTree(binary_lookup_mode)
         try:
             self.this.append(this)
-        except:
+        except __builtin__.Exception:
             self.this = this
     __swig_destroy__ = _SubnetTree.delete_SubnetTree
     __del__ = lambda self: None
 
     def insert(self, *args):
         return _SubnetTree.SubnetTree_insert(self, *args)
```

### Comparing `pysubnettree-0.35/SubnetTree_wrap.cc` & `pysubnettree-0.37/SubnetTree_wrap.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 /* ----------------------------------------------------------------------------
  * This file was automatically generated by SWIG (http://www.swig.org).
- * Version 3.0.7
+ * Version 3.0.12
  *
  * This file is not intended to be easily readable and contains a number of
  * coding conventions designed to improve portability and efficiency. Do not make
  * changes to this file unless you know what you are doing--modify the SWIG
  * interface file instead.
  * ----------------------------------------------------------------------------- */
 
+
+#ifndef SWIGPYTHON
 #define SWIGPYTHON
+#endif
+
 #define SWIG_PYTHON_DIRECTOR_NO_VTABLE
 
 
 #ifdef __cplusplus
 /* SwigValueWrapper is described in swig.swg */
 template<typename T> class SwigValueWrapper {
   struct SwigMovePointer {
@@ -98,17 +102,19 @@
 
 /* internal inline SWIG method */
 #ifndef SWIGINTERNINLINE
 # define SWIGINTERNINLINE SWIGINTERN SWIGINLINE
 #endif
 
 /* exporting methods */
-#if (__GNUC__ >= 4) || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4)
-#  ifndef GCC_HASCLASSVISIBILITY
-#    define GCC_HASCLASSVISIBILITY
+#if defined(__GNUC__)
+#  if (__GNUC__ >= 4) || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4)
+#    ifndef GCC_HASCLASSVISIBILITY
+#      define GCC_HASCLASSVISIBILITY
+#    endif
 #  endif
 #endif
 
 #ifndef SWIGEXPORT
 # if defined(_WIN32) || defined(__WIN32__) || defined(__CYGWIN__)
 #   if defined(STATIC_LINKED)
 #     define SWIGEXPORT
@@ -660,24 +666,24 @@
 SWIG_UnpackData(const char *c, void *ptr, size_t sz) {
   unsigned char *u = (unsigned char *) ptr;
   const unsigned char *eu = u + sz;
   for (; u != eu; ++u) {
     char d = *(c++);
     unsigned char uu;
     if ((d >= '0') && (d <= '9'))
-      uu = ((d - '0') << 4);
+      uu = (unsigned char)((d - '0') << 4);
     else if ((d >= 'a') && (d <= 'f'))
-      uu = ((d - ('a'-10)) << 4);
+      uu = (unsigned char)((d - ('a'-10)) << 4);
     else
       return (char *) 0;
     d = *(c++);
     if ((d >= '0') && (d <= '9'))
-      uu |= (d - '0');
+      uu |= (unsigned char)(d - '0');
     else if ((d >= 'a') && (d <= 'f'))
-      uu |= (d - ('a'-10));
+      uu |= (unsigned char)(d - ('a'-10));
     else
       return (char *) 0;
     *u = uu;
   }
   return c;
 }
 
@@ -852,18 +858,14 @@
   va_start(ap, fmt);
   res = vsnprintf(buf, sizeof(buf), fmt, ap);
   va_end(ap);
   return (res < 0 || res >= (int)sizeof(buf)) ? 0 : PyString_FromString(buf);
 }
 #endif
 
-/* Add PyObject_Del for old Pythons */
-#if PY_VERSION_HEX < 0x01060000
-# define PyObject_Del(op) PyMem_DEL((op))
-#endif
 #ifndef PyObject_DEL
 # define PyObject_DEL PyObject_Del
 #endif
 
 /* A crude PyExc_StopIteration exception for old Pythons */
 #if PY_VERSION_HEX < 0x02020000
 # ifndef PyExc_StopIteration
@@ -970,14 +972,15 @@
 # define SWIGPY_USE_CAPSULE
 # define SWIGPY_CAPSULE_NAME ((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION ".type_pointer_capsule" SWIG_TYPE_TABLE_NAME)
 #endif
 
 #if PY_VERSION_HEX < 0x03020000
 #define PyDescr_TYPE(x) (((PyDescrObject *)(x))->d_type)
 #define PyDescr_NAME(x) (((PyDescrObject *)(x))->d_name)
+#define Py_hash_t long
 #endif
 
 /* -----------------------------------------------------------------------------
  * error manipulation
  * ----------------------------------------------------------------------------- */
 
 SWIGRUNTIME PyObject*
@@ -1321,29 +1324,29 @@
   }
   return result;
 #endif
 }
 
 /* Unpack the argument tuple */
 
-SWIGINTERN int
+SWIGINTERN Py_ssize_t
 SWIG_Python_UnpackTuple(PyObject *args, const char *name, Py_ssize_t min, Py_ssize_t max, PyObject **objs)
 {
   if (!args) {
     if (!min && !max) {
       return 1;
     } else {
       PyErr_Format(PyExc_TypeError, "%s expected %s%d arguments, got none", 
 		   name, (min == max ? "" : "at least "), (int)min);
       return 0;
     }
   }  
   if (!PyTuple_Check(args)) {
     if (min <= 1 && max >= 1) {
-      int i;
+      Py_ssize_t i;
       objs[0] = args;
       for (i = 1; i < max; ++i) {
 	objs[i] = 0;
       }
       return 2;
     }
     PyErr_SetString(PyExc_SystemError, "UnpackTuple() argument list is not a tuple");
@@ -1355,15 +1358,15 @@
 		   name, (min == max ? "" : "at least "), (int)min, (int)l);
       return 0;
     } else if (l > max) {
       PyErr_Format(PyExc_TypeError, "%s expected %s%d arguments, got %d", 
 		   name, (min == max ? "" : "at most "), (int)max, (int)l);
       return 0;
     } else {
-      int i;
+      Py_ssize_t i;
       for (i = 0; i < l; ++i) {
 	objs[i] = PyTuple_GET_ITEM(args, i);
       }
       for (; l < max; ++l) {
 	objs[l] = 0;
       }
       return i + 1;
@@ -1625,14 +1628,22 @@
 # else
     PyString_ConcatAndDel(&repr,nrep);
 # endif
   }
   return repr;  
 }
 
+/* We need a version taking two PyObject* parameters so it's a valid
+ * PyCFunction to use in swigobject_methods[]. */
+SWIGRUNTIME PyObject *
+SwigPyObject_repr2(PyObject *v, PyObject *SWIGUNUSEDPARM(args))
+{
+  return SwigPyObject_repr((SwigPyObject*)v);
+}
+
 SWIGRUNTIME int
 SwigPyObject_compare(SwigPyObject *v, SwigPyObject *w)
 {
   void *i = v->ptr;
   void *j = w->ptr;
   return (i < j) ? -1 : ((i > j) ? 1 : 0);
 }
@@ -1696,24 +1707,40 @@
   if (sobj->own == SWIG_POINTER_OWN) {
     swig_type_info *ty = sobj->ty;
     SwigPyClientData *data = ty ? (SwigPyClientData *) ty->clientdata : 0;
     PyObject *destroy = data ? data->destroy : 0;
     if (destroy) {
       /* destroy is always a VARARGS method */
       PyObject *res;
+
+      /* PyObject_CallFunction() has the potential to silently drop
+         the active active exception.  In cases of unnamed temporary
+         variable or where we just finished iterating over a generator
+         StopIteration will be active right now, and this needs to
+         remain true upon return from SwigPyObject_dealloc.  So save
+         and restore. */
+      
+      PyObject *val = NULL, *type = NULL, *tb = NULL;
+      PyErr_Fetch(&val, &type, &tb);
+
       if (data->delargs) {
-	/* we need to create a temporary object to carry the destroy operation */
-	PyObject *tmp = SwigPyObject_New(sobj->ptr, ty, 0);
-	res = SWIG_Python_CallFunctor(destroy, tmp);
-	Py_DECREF(tmp);
+        /* we need to create a temporary object to carry the destroy operation */
+        PyObject *tmp = SwigPyObject_New(sobj->ptr, ty, 0);
+        res = SWIG_Python_CallFunctor(destroy, tmp);
+        Py_DECREF(tmp);
       } else {
-	PyCFunction meth = PyCFunction_GET_FUNCTION(destroy);
-	PyObject *mself = PyCFunction_GET_SELF(destroy);
-	res = ((*meth)(mself, v));
+        PyCFunction meth = PyCFunction_GET_FUNCTION(destroy);
+        PyObject *mself = PyCFunction_GET_SELF(destroy);
+        res = ((*meth)(mself, v));
       }
+      if (!res)
+        PyErr_WriteUnraisable(destroy);
+
+      PyErr_Restore(val, type, tb);
+
       Py_XDECREF(res);
     } 
 #if !defined(SWIG_PYTHON_SILENT_MEMLEAK)
     else {
       const char *name = SWIG_TypePrettyName(ty);
       printf("swig/python detected a memory leak of type '%s', no destructor found.\n", (name ? name : "unknown"));
     }
@@ -1729,27 +1756,24 @@
   SwigPyObject *sobj = (SwigPyObject *) v;
 #ifndef METH_O
   PyObject *tmp = 0;
   if (!PyArg_ParseTuple(next,(char *)"O:append", &tmp)) return NULL;
   next = tmp;
 #endif
   if (!SwigPyObject_Check(next)) {
+    PyErr_SetString(PyExc_TypeError, "Attempt to append a non SwigPyObject");
     return NULL;
   }
   sobj->next = next;
   Py_INCREF(next);
   return SWIG_Py_Void();
 }
 
 SWIGRUNTIME PyObject* 
-#ifdef METH_NOARGS
-SwigPyObject_next(PyObject* v)
-#else
 SwigPyObject_next(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
-#endif
 {
   SwigPyObject *sobj = (SwigPyObject *) v;
   if (sobj->next) {    
     Py_INCREF(sobj->next);
     return sobj->next;
   } else {
     return SWIG_Py_Void();
@@ -1776,14 +1800,28 @@
 #endif
 {
   SwigPyObject *sobj = (SwigPyObject *)v;
   sobj->own = SWIG_POINTER_OWN;
   return SWIG_Py_Void();
 }
 
+#ifdef METH_NOARGS
+static PyObject*
+SwigPyObject_disown2(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
+{
+  return SwigPyObject_disown(v);
+}
+
+static PyObject*
+SwigPyObject_acquire2(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
+{
+  return SwigPyObject_acquire(v);
+}
+#endif
+
 SWIGINTERN PyObject*
 SwigPyObject_own(PyObject *v, PyObject *args)
 {
   PyObject *val = 0;
 #if (PY_VERSION_HEX < 0x02020000)
   if (!PyArg_ParseTuple(args,(char *)"|O:own",&val))
 #elif (PY_VERSION_HEX < 0x02050000)
@@ -1816,31 +1854,31 @@
       return obj;
     }
 }
 
 #ifdef METH_O
 static PyMethodDef
 swigobject_methods[] = {
-  {(char *)"disown",  (PyCFunction)SwigPyObject_disown,  METH_NOARGS,  (char *)"releases ownership of the pointer"},
-  {(char *)"acquire", (PyCFunction)SwigPyObject_acquire, METH_NOARGS,  (char *)"acquires ownership of the pointer"},
+  {(char *)"disown",  (PyCFunction)SwigPyObject_disown2, METH_NOARGS,  (char *)"releases ownership of the pointer"},
+  {(char *)"acquire", (PyCFunction)SwigPyObject_acquire2,METH_NOARGS,  (char *)"acquires ownership of the pointer"},
   {(char *)"own",     (PyCFunction)SwigPyObject_own,     METH_VARARGS, (char *)"returns/sets ownership of the pointer"},
   {(char *)"append",  (PyCFunction)SwigPyObject_append,  METH_O,       (char *)"appends another 'this' object"},
   {(char *)"next",    (PyCFunction)SwigPyObject_next,    METH_NOARGS,  (char *)"returns the next 'this' object"},
-  {(char *)"__repr__",(PyCFunction)SwigPyObject_repr,    METH_NOARGS,  (char *)"returns object representation"},
+  {(char *)"__repr__",(PyCFunction)SwigPyObject_repr2,   METH_NOARGS,  (char *)"returns object representation"},
   {0, 0, 0, 0}  
 };
 #else
 static PyMethodDef
 swigobject_methods[] = {
   {(char *)"disown",  (PyCFunction)SwigPyObject_disown,  METH_VARARGS,  (char *)"releases ownership of the pointer"},
   {(char *)"acquire", (PyCFunction)SwigPyObject_acquire, METH_VARARGS,  (char *)"acquires ownership of the pointer"},
   {(char *)"own",     (PyCFunction)SwigPyObject_own,     METH_VARARGS,  (char *)"returns/sets ownership of the pointer"},
   {(char *)"append",  (PyCFunction)SwigPyObject_append,  METH_VARARGS,  (char *)"appends another 'this' object"},
   {(char *)"next",    (PyCFunction)SwigPyObject_next,    METH_VARARGS,  (char *)"returns the next 'this' object"},
-  {(char *)"__repr__",(PyCFunction)SwigPyObject_repr,   METH_VARARGS,  (char *)"returns object representation"},
+  {(char *)"__repr__",(PyCFunction)SwigPyObject_repr,    METH_VARARGS,  (char *)"returns object representation"},
   {0, 0, 0, 0}  
 };
 #endif
 
 #if PY_VERSION_HEX < 0x02020000
 SWIGINTERN PyObject *
 SwigPyObject_getattr(SwigPyObject *sobj,char *name)
@@ -1884,59 +1922,60 @@
     0, /*nb_reserved*/
 #endif
     (unaryfunc)0,                 /*nb_float*/
 #if PY_VERSION_HEX < 0x03000000
     (unaryfunc)SwigPyObject_oct,  /*nb_oct*/
     (unaryfunc)SwigPyObject_hex,  /*nb_hex*/
 #endif
-#if PY_VERSION_HEX >= 0x03000000 /* 3.0 */
+#if PY_VERSION_HEX >= 0x03050000 /* 3.5 */
+    0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_matrix_multiply */
+#elif PY_VERSION_HEX >= 0x03000000 /* 3.0 */
     0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_index, nb_inplace_divide removed */
 #elif PY_VERSION_HEX >= 0x02050000 /* 2.5.0 */
     0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_index */
 #elif PY_VERSION_HEX >= 0x02020000 /* 2.2.0 */
     0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_true_divide */
 #elif PY_VERSION_HEX >= 0x02000000 /* 2.0.0 */
     0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_or */
 #endif
   };
 
   static PyTypeObject swigpyobject_type;
   static int type_init = 0;
   if (!type_init) {
     const PyTypeObject tmp = {
-      /* PyObject header changed in Python 3 */
 #if PY_VERSION_HEX >= 0x03000000
       PyVarObject_HEAD_INIT(NULL, 0)
 #else
       PyObject_HEAD_INIT(NULL)
       0,                                    /* ob_size */
 #endif
       (char *)"SwigPyObject",               /* tp_name */
       sizeof(SwigPyObject),                 /* tp_basicsize */
       0,                                    /* tp_itemsize */
       (destructor)SwigPyObject_dealloc,     /* tp_dealloc */
-      0,				    /* tp_print */
+      0,                                    /* tp_print */
 #if PY_VERSION_HEX < 0x02020000
       (getattrfunc)SwigPyObject_getattr,    /* tp_getattr */
 #else
       (getattrfunc)0,                       /* tp_getattr */
 #endif
       (setattrfunc)0,                       /* tp_setattr */
 #if PY_VERSION_HEX >= 0x03000000
-    0, /* tp_reserved in 3.0.1, tp_compare in 3.0.0 but not used */
+      0, /* tp_reserved in 3.0.1, tp_compare in 3.0.0 but not used */
 #else
       (cmpfunc)SwigPyObject_compare,        /* tp_compare */
 #endif
       (reprfunc)SwigPyObject_repr,          /* tp_repr */
       &SwigPyObject_as_number,              /* tp_as_number */
       0,                                    /* tp_as_sequence */
       0,                                    /* tp_as_mapping */
       (hashfunc)0,                          /* tp_hash */
       (ternaryfunc)0,                       /* tp_call */
-      0,				    /* tp_str */
+      0,                                    /* tp_str */
       PyObject_GenericGetAttr,              /* tp_getattro */
       0,                                    /* tp_setattro */
       0,                                    /* tp_as_buffer */
       Py_TPFLAGS_DEFAULT,                   /* tp_flags */
       swigobject_doc,                       /* tp_doc */
       0,                                    /* tp_traverse */
       0,                                    /* tp_clear */
@@ -1964,18 +2003,27 @@
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
 #endif
 #if PY_VERSION_HEX >= 0x02030000
       0,                                    /* tp_del */
 #endif
 #if PY_VERSION_HEX >= 0x02060000
-      0,                                    /* tp_version */
+      0,                                    /* tp_version_tag */
+#endif
+#if PY_VERSION_HEX >= 0x03040000
+      0,                                    /* tp_finalize */
 #endif
 #ifdef COUNT_ALLOCS
-      0,0,0,0                               /* tp_alloc -> tp_next */
+      0,                                    /* tp_allocs */
+      0,                                    /* tp_frees */
+      0,                                    /* tp_maxalloc */
+#if PY_VERSION_HEX >= 0x02050000
+      0,                                    /* tp_prev */
+#endif
+      0                                     /* tp_next */
 #endif
     };
     swigpyobject_type = tmp;
     type_init = 1;
 #if PY_VERSION_HEX < 0x02020000
     swigpyobject_type.ob_type = &PyType_Type;
 #else
@@ -2082,15 +2130,14 @@
 SWIGRUNTIME PyTypeObject*
 SwigPyPacked_TypeOnce(void) {
   static char swigpacked_doc[] = "Swig object carries a C/C++ instance pointer";
   static PyTypeObject swigpypacked_type;
   static int type_init = 0;
   if (!type_init) {
     const PyTypeObject tmp = {
-      /* PyObject header changed in Python 3 */
 #if PY_VERSION_HEX>=0x03000000
       PyVarObject_HEAD_INIT(NULL, 0)
 #else
       PyObject_HEAD_INIT(NULL)
       0,                                    /* ob_size */
 #endif
       (char *)"SwigPyPacked",               /* tp_name */
@@ -2143,18 +2190,27 @@
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
 #endif
 #if PY_VERSION_HEX >= 0x02030000
       0,                                    /* tp_del */
 #endif
 #if PY_VERSION_HEX >= 0x02060000
-      0,                                    /* tp_version */
+      0,                                    /* tp_version_tag */
+#endif
+#if PY_VERSION_HEX >= 0x03040000
+      0,                                    /* tp_finalize */
 #endif
 #ifdef COUNT_ALLOCS
-      0,0,0,0                               /* tp_alloc -> tp_next */
+      0,                                    /* tp_allocs */
+      0,                                    /* tp_frees */
+      0,                                    /* tp_maxalloc */
+#if PY_VERSION_HEX >= 0x02050000
+      0,                                    /* tp_prev */
+#endif
+      0                                     /* tp_next */
 #endif
     };
     swigpypacked_type = tmp;
     type_init = 1;
 #if PY_VERSION_HEX < 0x02020000
     swigpypacked_type.ob_type = &PyType_Type;
 #else
@@ -2674,21 +2730,19 @@
 /* PyModule_AddObject function was introduced in Python 2.0.  The following function
    is copied out of Python/modsupport.c in python version 2.3.4 */
 SWIGINTERN int
 PyModule_AddObject(PyObject *m, char *name, PyObject *o)
 {
   PyObject *dict;
   if (!PyModule_Check(m)) {
-    PyErr_SetString(PyExc_TypeError,
-		    "PyModule_AddObject() needs module as first arg");
+    PyErr_SetString(PyExc_TypeError, "PyModule_AddObject() needs module as first arg");
     return SWIG_ERROR;
   }
   if (!o) {
-    PyErr_SetString(PyExc_TypeError,
-		    "PyModule_AddObject() needs non-NULL value");
+    PyErr_SetString(PyExc_TypeError, "PyModule_AddObject() needs non-NULL value");
     return SWIG_ERROR;
   }
   
   dict = PyModule_GetDict(m);
   if (dict == NULL) {
     /* Internal error -- modules must have a dict! */
     PyErr_Format(PyExc_SystemError, "module '%s' has no __dict__",
@@ -2993,15 +3047,15 @@
 
 #else
 #  define SWIG_init    init_SubnetTree
 
 #endif
 #define SWIG_name    "_SubnetTree"
 
-#define SWIGVERSION 0x030007 
+#define SWIGVERSION 0x030012 
 #define SWIG_VERSION SWIGVERSION
 
 
 #define SWIG_as_voidptr(a) const_cast< void * >(static_cast< const void * >(a)) 
 #define SWIG_as_voidptrptr(a) ((void)SWIG_as_voidptr(*a),reinterpret_cast< void** >(a)) 
 
 
@@ -3084,17 +3138,19 @@
 SWIGINTERN int
 SWIG_AsVal_double (PyObject *obj, double *val)
 {
   int res = SWIG_TypeError;
   if (PyFloat_Check(obj)) {
     if (val) *val = PyFloat_AsDouble(obj);
     return SWIG_OK;
+#if PY_VERSION_HEX < 0x03000000
   } else if (PyInt_Check(obj)) {
-    if (val) *val = PyInt_AsLong(obj);
+    if (val) *val = (double) PyInt_AsLong(obj);
     return SWIG_OK;
+#endif
   } else if (PyLong_Check(obj)) {
     double v = PyLong_AsDouble(obj);
     if (!PyErr_Occurred()) {
       if (val) *val = v;
       return SWIG_OK;
     } else {
       PyErr_Clear();
@@ -3160,24 +3216,28 @@
   return 0;
 }
 
 
 SWIGINTERN int
 SWIG_AsVal_long (PyObject *obj, long* val)
 {
+#if PY_VERSION_HEX < 0x03000000
   if (PyInt_Check(obj)) {
     if (val) *val = PyInt_AsLong(obj);
     return SWIG_OK;
-  } else if (PyLong_Check(obj)) {
+  } else
+#endif
+  if (PyLong_Check(obj)) {
     long v = PyLong_AsLong(obj);
     if (!PyErr_Occurred()) {
       if (val) *val = v;
       return SWIG_OK;
     } else {
       PyErr_Clear();
+      return SWIG_OverflowError;
     }
   }
 #ifdef SWIG_PYTHON_CAST_MODE
   {
     int dispatch = 0;
     long v = PyInt_AsLong(obj);
     if (!PyErr_Occurred()) {
@@ -3227,31 +3287,37 @@
 }
 
 
 SWIGINTERN int
 SWIG_AsCharPtrAndSize(PyObject *obj, char** cptr, size_t* psize, int *alloc)
 {
 #if PY_VERSION_HEX>=0x03000000
+#if defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
+  if (PyBytes_Check(obj))
+#else
   if (PyUnicode_Check(obj))
+#endif
 #else  
   if (PyString_Check(obj))
 #endif
   {
     char *cstr; Py_ssize_t len;
 #if PY_VERSION_HEX>=0x03000000
+#if !defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
     if (!alloc && cptr) {
         /* We can't allow converting without allocation, since the internal
            representation of string in Python 3 is UCS-2/UCS-4 but we require
            a UTF-8 representation.
            TODO(bhy) More detailed explanation */
         return SWIG_RuntimeError;
     }
     obj = PyUnicode_AsUTF8String(obj);
-    PyBytes_AsStringAndSize(obj, &cstr, &len);
     if(alloc) *alloc = SWIG_NEWOBJ;
+#endif
+    PyBytes_AsStringAndSize(obj, &cstr, &len);
 #else
     PyString_AsStringAndSize(obj, &cstr, &len);
 #endif
     if (cptr) {
       if (alloc) {
 	/* 
 	   In python the user should not be able to modify the inner
@@ -3263,35 +3329,66 @@
 	   so, be careful.
 	*/ 
 #if defined(SWIG_PYTHON_SAFE_CSTRINGS)
 	if (*alloc != SWIG_OLDOBJ) 
 #else
 	if (*alloc == SWIG_NEWOBJ) 
 #endif
-	  {
-	    *cptr = reinterpret_cast< char* >(memcpy((new char[len + 1]), cstr, sizeof(char)*(len + 1)));
-	    *alloc = SWIG_NEWOBJ;
-	  }
-	else {
+	{
+	  *cptr = reinterpret_cast< char* >(memcpy(new char[len + 1], cstr, sizeof(char)*(len + 1)));
+	  *alloc = SWIG_NEWOBJ;
+	} else {
 	  *cptr = cstr;
 	  *alloc = SWIG_OLDOBJ;
 	}
       } else {
-        #if PY_VERSION_HEX>=0x03000000
-        assert(0); /* Should never reach here in Python 3 */
-        #endif
+#if PY_VERSION_HEX>=0x03000000
+#if defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
+	*cptr = PyBytes_AsString(obj);
+#else
+	assert(0); /* Should never reach here with Unicode strings in Python 3 */
+#endif
+#else
 	*cptr = SWIG_Python_str_AsChar(obj);
+#endif
       }
     }
     if (psize) *psize = len + 1;
-#if PY_VERSION_HEX>=0x03000000
+#if PY_VERSION_HEX>=0x03000000 && !defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
     Py_XDECREF(obj);
 #endif
     return SWIG_OK;
   } else {
+#if defined(SWIG_PYTHON_2_UNICODE)
+#if defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
+#error "Cannot use both SWIG_PYTHON_2_UNICODE and SWIG_PYTHON_STRICT_BYTE_CHAR at once"
+#endif
+#if PY_VERSION_HEX<0x03000000
+    if (PyUnicode_Check(obj)) {
+      char *cstr; Py_ssize_t len;
+      if (!alloc && cptr) {
+        return SWIG_RuntimeError;
+      }
+      obj = PyUnicode_AsUTF8String(obj);
+      if (PyString_AsStringAndSize(obj, &cstr, &len) != -1) {
+        if (cptr) {
+          if (alloc) *alloc = SWIG_NEWOBJ;
+          *cptr = reinterpret_cast< char* >(memcpy(new char[len + 1], cstr, sizeof(char)*(len + 1)));
+        }
+        if (psize) *psize = len + 1;
+
+        Py_XDECREF(obj);
+        return SWIG_OK;
+      } else {
+        Py_XDECREF(obj);
+      }
+    }
+#endif
+#endif
+
     swig_type_info* pchar_descriptor = SWIG_pchar_descriptor();
     if (pchar_descriptor) {
       void* vptr = 0;
       if (SWIG_ConvertPtr(obj, &vptr, pchar_descriptor, 0) == SWIG_OK) {
 	if (cptr) *cptr = (char *) vptr;
 	if (psize) *psize = vptr ? (strlen((char *)vptr) + 1) : 0;
 	if (alloc) *alloc = SWIG_OLDOBJ;
@@ -3323,26 +3420,15 @@
   if (PyLong_Check(obj)) {
     unsigned long v = PyLong_AsUnsignedLong(obj);
     if (!PyErr_Occurred()) {
       if (val) *val = v;
       return SWIG_OK;
     } else {
       PyErr_Clear();
-#if PY_VERSION_HEX >= 0x03000000
-      {
-        long v = PyLong_AsLong(obj);
-        if (!PyErr_Occurred()) {
-          if (v < 0) {
-            return SWIG_OverflowError;
-          }
-        } else {
-          PyErr_Clear();
-        }
-      }
-#endif
+      return SWIG_OverflowError;
     }
   }
 #ifdef SWIG_PYTHON_CAST_MODE
   {
     int dispatch = 0;
     unsigned long v = PyLong_AsUnsignedLong(obj);
     if (!PyErr_Occurred()) {
@@ -3640,15 +3726,15 @@
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *inx_addr_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *obj;
-  if (!PyArg_ParseTuple(args,(char*)"O:swigregister", &obj)) return NULL;
+  if (!PyArg_ParseTuple(args,(char *)"O:swigregister", &obj)) return NULL;
   SWIG_TypeNewClientData(SWIGTYPE_p__inx_addr, SWIG_NewClientData(obj));
   return SWIG_Py_Void();
 }
 
 SWIGINTERN PyObject *_wrap_new_SubnetTree__SWIG_0(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   bool arg1 ;
@@ -3681,22 +3767,22 @@
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_new_SubnetTree(PyObject *self, PyObject *args) {
-  int argc;
+  Py_ssize_t argc;
   PyObject *argv[2] = {
     0
   };
-  int ii;
+  Py_ssize_t ii;
   
   if (!PyTuple_Check(args)) SWIG_fail;
-  argc = args ? (int)PyObject_Length(args) : 0;
+  argc = args ? PyObject_Length(args) : 0;
   for (ii = 0; (ii < 1) && (ii < argc); ii++) {
     argv[ii] = PyTuple_GET_ITEM(args,ii);
   }
   if (argc == 0) {
     return _wrap_new_SubnetTree__SWIG_1(self, args);
   }
   if (argc == 1) {
@@ -3891,22 +3977,22 @@
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_SubnetTree_insert(PyObject *self, PyObject *args) {
-  int argc;
+  Py_ssize_t argc;
   PyObject *argv[5] = {
     0
   };
-  int ii;
+  Py_ssize_t ii;
   
   if (!PyTuple_Check(args)) SWIG_fail;
-  argc = args ? (int)PyObject_Length(args) : 0;
+  argc = args ? PyObject_Length(args) : 0;
   for (ii = 0; (ii < 4) && (ii < argc); ii++) {
     argv[ii] = PyTuple_GET_ITEM(args,ii);
   }
   if (argc == 2) {
     int _v;
     void *vptr = 0;
     int res = SWIG_ConvertPtr(argv[0], &vptr, SWIGTYPE_p_SubnetTree, 0);
@@ -4063,22 +4149,22 @@
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_SubnetTree_remove(PyObject *self, PyObject *args) {
-  int argc;
+  Py_ssize_t argc;
   PyObject *argv[4] = {
     0
   };
-  int ii;
+  Py_ssize_t ii;
   
   if (!PyTuple_Check(args)) SWIG_fail;
-  argc = args ? (int)PyObject_Length(args) : 0;
+  argc = args ? PyObject_Length(args) : 0;
   for (ii = 0; (ii < 3) && (ii < argc); ii++) {
     argv[ii] = PyTuple_GET_ITEM(args,ii);
   }
   if (argc == 2) {
     int _v;
     void *vptr = 0;
     int res = SWIG_ConvertPtr(argv[0], &vptr, SWIGTYPE_p_SubnetTree, 0);
@@ -4193,22 +4279,22 @@
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_SubnetTree_lookup(PyObject *self, PyObject *args) {
-  int argc;
+  Py_ssize_t argc;
   PyObject *argv[4] = {
     0
   };
-  int ii;
+  Py_ssize_t ii;
   
   if (!PyTuple_Check(args)) SWIG_fail;
-  argc = args ? (int)PyObject_Length(args) : 0;
+  argc = args ? PyObject_Length(args) : 0;
   for (ii = 0; (ii < 3) && (ii < argc); ii++) {
     argv[ii] = PyTuple_GET_ITEM(args,ii);
   }
   if (argc == 2) {
     int _v;
     void *vptr = 0;
     int res = SWIG_ConvertPtr(argv[0], &vptr, SWIGTYPE_p_SubnetTree, 0);
@@ -4342,22 +4428,22 @@
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_SubnetTree_prefixes(PyObject *self, PyObject *args) {
-  int argc;
+  Py_ssize_t argc;
   PyObject *argv[4] = {
     0
   };
-  int ii;
+  Py_ssize_t ii;
   
   if (!PyTuple_Check(args)) SWIG_fail;
-  argc = args ? (int)PyObject_Length(args) : 0;
+  argc = args ? PyObject_Length(args) : 0;
   for (ii = 0; (ii < 3) && (ii < argc); ii++) {
     argv[ii] = PyTuple_GET_ITEM(args,ii);
   }
   if (argc == 1) {
     int _v;
     void *vptr = 0;
     int res = SWIG_ConvertPtr(argv[0], &vptr, SWIGTYPE_p_SubnetTree, 0);
@@ -4483,22 +4569,22 @@
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_SubnetTree_set_binary_lookup_mode(PyObject *self, PyObject *args) {
-  int argc;
+  Py_ssize_t argc;
   PyObject *argv[3] = {
     0
   };
-  int ii;
+  Py_ssize_t ii;
   
   if (!PyTuple_Check(args)) SWIG_fail;
-  argc = args ? (int)PyObject_Length(args) : 0;
+  argc = args ? PyObject_Length(args) : 0;
   for (ii = 0; (ii < 2) && (ii < argc); ii++) {
     argv[ii] = PyTuple_GET_ITEM(args,ii);
   }
   if (argc == 1) {
     int _v;
     void *vptr = 0;
     int res = SWIG_ConvertPtr(argv[0], &vptr, SWIGTYPE_p_SubnetTree, 0);
@@ -4535,33 +4621,44 @@
 SWIGINTERN PyObject *_wrap_SubnetTree___contains____SWIG_0(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   SubnetTree *arg1 = (SubnetTree *) 0 ;
   char *arg2 = (char *) 0 ;
   int arg3 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
+  PyObject *ascii2 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject *result = 0 ;
   
+  {
+    ascii2 = NULL;
+  }
   if (!PyArg_ParseTuple(args,(char *)"OO:SubnetTree___contains__",&obj0,&obj1)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_SubnetTree, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "SubnetTree___contains__" "', argument " "1"" of type '" "SubnetTree *""'"); 
   }
   arg1 = reinterpret_cast< SubnetTree * >(argp1);
   
   Py_ssize_t len;
+  
 #if PY_MAJOR_VERSION >= 3
   if ( PyUnicode_Check(obj1) )
   {
-    PyObject* ascii = PyUnicode_AsASCIIString(obj1);
-    PyBytes_AsStringAndSize(ascii, &arg2, &len);
+    ascii2 = PyUnicode_AsASCIIString(obj1);
+    
+    if ( ! ascii2 )
+    {
+      PyErr_SetString(PyExc_TypeError, "Expected a ASCII encodable string or bytes");
+      return NULL;
+    }
+    
+    PyBytes_AsStringAndSize(ascii2, &arg2, &len);
     arg3 = len;
-    Py_DECREF(ascii);
   }
   else if ( PyBytes_Check(obj1) )
   {
     PyBytes_AsStringAndSize(obj1, &arg2, &len);
     arg3 = len;
   }
   else
@@ -4580,16 +4677,22 @@
     PyString_AsStringAndSize(obj1, &arg2, &len);
     arg3 = len;
   }
 #endif
   
   result = (PyObject *)SubnetTree___contains____SWIG_0(arg1,arg2,arg3);
   resultobj = result;
+  {
+    Py_XDECREF(ascii2);
+  }
   return resultobj;
 fail:
+  {
+    Py_XDECREF(ascii2);
+  }
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_SubnetTree___contains____SWIG_1(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   SubnetTree *arg1 = (SubnetTree *) 0 ;
@@ -4618,22 +4721,22 @@
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_SubnetTree___contains__(PyObject *self, PyObject *args) {
-  int argc;
+  Py_ssize_t argc;
   PyObject *argv[3] = {
     0
   };
-  int ii;
+  Py_ssize_t ii;
   
   if (!PyTuple_Check(args)) SWIG_fail;
-  argc = args ? (int)PyObject_Length(args) : 0;
+  argc = args ? PyObject_Length(args) : 0;
   for (ii = 0; (ii < 2) && (ii < argc); ii++) {
     argv[ii] = PyTuple_GET_ITEM(args,ii);
   }
   if (argc == 2) {
     int _v;
     void *vptr = 0;
     int res = SWIG_ConvertPtr(argv[0], &vptr, SWIGTYPE_p_SubnetTree, 0);
@@ -4680,33 +4783,44 @@
 SWIGINTERN PyObject *_wrap_SubnetTree___getitem__(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   SubnetTree *arg1 = (SubnetTree *) 0 ;
   char *arg2 = (char *) 0 ;
   int arg3 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
+  PyObject *ascii2 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject *result = 0 ;
   
+  {
+    ascii2 = NULL;
+  }
   if (!PyArg_ParseTuple(args,(char *)"OO:SubnetTree___getitem__",&obj0,&obj1)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_SubnetTree, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "SubnetTree___getitem__" "', argument " "1"" of type '" "SubnetTree *""'"); 
   }
   arg1 = reinterpret_cast< SubnetTree * >(argp1);
   
   Py_ssize_t len;
+  
 #if PY_MAJOR_VERSION >= 3
   if ( PyUnicode_Check(obj1) )
   {
-    PyObject* ascii = PyUnicode_AsASCIIString(obj1);
-    PyBytes_AsStringAndSize(ascii, &arg2, &len);
+    ascii2 = PyUnicode_AsASCIIString(obj1);
+    
+    if ( ! ascii2 )
+    {
+      PyErr_SetString(PyExc_TypeError, "Expected a ASCII encodable string or bytes");
+      return NULL;
+    }
+    
+    PyBytes_AsStringAndSize(ascii2, &arg2, &len);
     arg3 = len;
-    Py_DECREF(ascii);
   }
   else if ( PyBytes_Check(obj1) )
   {
     PyBytes_AsStringAndSize(obj1, &arg2, &len);
     arg3 = len;
   }
   else
@@ -4725,16 +4839,22 @@
     PyString_AsStringAndSize(obj1, &arg2, &len);
     arg3 = len;
   }
 #endif
   
   result = (PyObject *)SubnetTree___getitem__(arg1,arg2,arg3);
   resultobj = result;
+  {
+    Py_XDECREF(ascii2);
+  }
   return resultobj;
 fail:
+  {
+    Py_XDECREF(ascii2);
+  }
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_SubnetTree___setitem__(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   SubnetTree *arg1 = (SubnetTree *) 0 ;
@@ -4804,41 +4924,41 @@
   if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
   return NULL;
 }
 
 
 SWIGINTERN PyObject *SubnetTree_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *obj;
-  if (!PyArg_ParseTuple(args,(char*)"O:swigregister", &obj)) return NULL;
+  if (!PyArg_ParseTuple(args,(char *)"O:swigregister", &obj)) return NULL;
   SWIG_TypeNewClientData(SWIGTYPE_p_SubnetTree, SWIG_NewClientData(obj));
   return SWIG_Py_Void();
 }
 
 static PyMethodDef SwigMethods[] = {
-	 { (char *)"SWIG_PyInstanceMethod_New", (PyCFunction)SWIG_PyInstanceMethod_New, METH_O, NULL},
-	 { (char *)"inx_addr_sin_set", _wrap_inx_addr_sin_set, METH_VARARGS, NULL},
-	 { (char *)"inx_addr_sin_get", _wrap_inx_addr_sin_get, METH_VARARGS, NULL},
-	 { (char *)"inx_addr_sin6_set", _wrap_inx_addr_sin6_set, METH_VARARGS, NULL},
-	 { (char *)"inx_addr_sin6_get", _wrap_inx_addr_sin6_get, METH_VARARGS, NULL},
-	 { (char *)"new_inx_addr", _wrap_new_inx_addr, METH_VARARGS, NULL},
-	 { (char *)"delete_inx_addr", _wrap_delete_inx_addr, METH_VARARGS, NULL},
-	 { (char *)"inx_addr_swigregister", inx_addr_swigregister, METH_VARARGS, NULL},
-	 { (char *)"new_SubnetTree", _wrap_new_SubnetTree, METH_VARARGS, NULL},
-	 { (char *)"delete_SubnetTree", _wrap_delete_SubnetTree, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree_insert", _wrap_SubnetTree_insert, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree_remove", _wrap_SubnetTree_remove, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree_lookup", _wrap_SubnetTree_lookup, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree_prefixes", _wrap_SubnetTree_prefixes, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree_get_binary_lookup_mode", _wrap_SubnetTree_get_binary_lookup_mode, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree_set_binary_lookup_mode", _wrap_SubnetTree_set_binary_lookup_mode, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree___contains__", _wrap_SubnetTree___contains__, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree___getitem__", _wrap_SubnetTree___getitem__, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree___setitem__", _wrap_SubnetTree___setitem__, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree___delitem__", _wrap_SubnetTree___delitem__, METH_VARARGS, NULL},
-	 { (char *)"SubnetTree_swigregister", SubnetTree_swigregister, METH_VARARGS, NULL},
+	 { "SWIG_PyInstanceMethod_New", SWIG_PyInstanceMethod_New, METH_O, NULL},
+	 { "inx_addr_sin_set", _wrap_inx_addr_sin_set, METH_VARARGS, NULL},
+	 { "inx_addr_sin_get", _wrap_inx_addr_sin_get, METH_VARARGS, NULL},
+	 { "inx_addr_sin6_set", _wrap_inx_addr_sin6_set, METH_VARARGS, NULL},
+	 { "inx_addr_sin6_get", _wrap_inx_addr_sin6_get, METH_VARARGS, NULL},
+	 { "new_inx_addr", _wrap_new_inx_addr, METH_VARARGS, NULL},
+	 { "delete_inx_addr", _wrap_delete_inx_addr, METH_VARARGS, NULL},
+	 { "inx_addr_swigregister", inx_addr_swigregister, METH_VARARGS, NULL},
+	 { "new_SubnetTree", _wrap_new_SubnetTree, METH_VARARGS, NULL},
+	 { "delete_SubnetTree", _wrap_delete_SubnetTree, METH_VARARGS, NULL},
+	 { "SubnetTree_insert", _wrap_SubnetTree_insert, METH_VARARGS, NULL},
+	 { "SubnetTree_remove", _wrap_SubnetTree_remove, METH_VARARGS, NULL},
+	 { "SubnetTree_lookup", _wrap_SubnetTree_lookup, METH_VARARGS, NULL},
+	 { "SubnetTree_prefixes", _wrap_SubnetTree_prefixes, METH_VARARGS, NULL},
+	 { "SubnetTree_get_binary_lookup_mode", _wrap_SubnetTree_get_binary_lookup_mode, METH_VARARGS, NULL},
+	 { "SubnetTree_set_binary_lookup_mode", _wrap_SubnetTree_set_binary_lookup_mode, METH_VARARGS, NULL},
+	 { "SubnetTree___contains__", _wrap_SubnetTree___contains__, METH_VARARGS, NULL},
+	 { "SubnetTree___getitem__", _wrap_SubnetTree___getitem__, METH_VARARGS, NULL},
+	 { "SubnetTree___setitem__", _wrap_SubnetTree___setitem__, METH_VARARGS, NULL},
+	 { "SubnetTree___delitem__", _wrap_SubnetTree___delitem__, METH_VARARGS, NULL},
+	 { "SubnetTree_swigregister", SubnetTree_swigregister, METH_VARARGS, NULL},
 	 { NULL, NULL, 0, NULL }
 };
 
 
 /* -------- TYPE CONVERSION AND EQUIVALENCE RULES (BEGIN) -------- */
 
 static swig_type_info _swigt__p_SubnetTree = {"_p_SubnetTree", "SubnetTree *", 0, 0, (void*)0, 0};
@@ -5242,15 +5362,14 @@
   SWIGINTERN PyTypeObject*
   swig_varlink_type(void) {
     static char varlink__doc__[] = "Swig var link object";
     static PyTypeObject varlink_type;
     static int type_init = 0;
     if (!type_init) {
       const PyTypeObject tmp = {
-        /* PyObject header changed in Python 3 */
 #if PY_VERSION_HEX >= 0x03000000
         PyVarObject_HEAD_INIT(NULL, 0)
 #else
         PyObject_HEAD_INIT(NULL)
         0,                                  /* ob_size */
 #endif
         (char *)"swigvarlink",              /* tp_name */
@@ -5280,18 +5399,27 @@
 #if PY_VERSION_HEX >= 0x02020000
         0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0, /* tp_iter -> tp_weaklist */
 #endif
 #if PY_VERSION_HEX >= 0x02030000
         0,                                  /* tp_del */
 #endif
 #if PY_VERSION_HEX >= 0x02060000
-        0,                                  /* tp_version */
+        0,                                  /* tp_version_tag */
+#endif
+#if PY_VERSION_HEX >= 0x03040000
+        0,                                  /* tp_finalize */
 #endif
 #ifdef COUNT_ALLOCS
-        0,0,0,0                             /* tp_alloc -> tp_next */
+        0,                                  /* tp_allocs */
+        0,                                  /* tp_frees */
+        0,                                  /* tp_maxalloc */
+#if PY_VERSION_HEX >= 0x02050000
+        0,                                  /* tp_prev */
+#endif
+        0                                   /* tp_next */
 #endif
       };
       varlink_type = tmp;
       type_init = 1;
 #if PY_VERSION_HEX < 0x02020000
       varlink_type.ob_type = &PyType_Type;
 #else
@@ -5395,17 +5523,17 @@
             size_t shift = (ci->ptype) - types;
             swig_type_info *ty = types_initial[shift];
             size_t ldoc = (c - methods[i].ml_doc);
             size_t lptr = strlen(ty->name)+2*sizeof(void*)+2;
             char *ndoc = (char*)malloc(ldoc + lptr + 10);
             if (ndoc) {
               char *buff = ndoc;
-              strncpy(buff, methods[i].ml_doc, ldoc);
+              memcpy(buff, methods[i].ml_doc, ldoc);
               buff += ldoc;
-              strncpy(buff, "swig_ptr: ", 10);
+              memcpy(buff, "swig_ptr: ", 10);
               buff += 10;
               SWIG_PackVoidPtr(buff, ptr, ty->name, lptr);
               methods[i].ml_doc = ndoc;
             }
           }
         }
       }
@@ -5459,49 +5587,44 @@
   static SwigPyClientData SwigPyObject_clientdata = {
     0, 0, 0, 0, 0, 0, 0
   };
   static PyGetSetDef this_getset_def = {
     (char *)"this", &SwigPyBuiltin_ThisClosure, NULL, NULL, NULL
   };
   static SwigPyGetSet thisown_getset_closure = {
-    (PyCFunction) SwigPyObject_own,
-    (PyCFunction) SwigPyObject_own
+    SwigPyObject_own,
+    SwigPyObject_own
   };
   static PyGetSetDef thisown_getset_def = {
     (char *)"thisown", SwigPyBuiltin_GetterClosure, SwigPyBuiltin_SetterClosure, NULL, &thisown_getset_closure
   };
-  PyObject *metatype_args;
   PyTypeObject *builtin_pytype;
   int builtin_base_count;
   swig_type_info *builtin_basetype;
   PyObject *tuple;
   PyGetSetDescrObject *static_getset;
   PyTypeObject *metatype;
+  PyTypeObject *swigpyobject;
   SwigPyClientData *cd;
   PyObject *public_interface, *public_symbol;
   PyObject *this_descr;
   PyObject *thisown_descr;
   PyObject *self = 0;
   int i;
   
   (void)builtin_pytype;
   (void)builtin_base_count;
   (void)builtin_basetype;
   (void)tuple;
   (void)static_getset;
   (void)self;
   
-  /* metatype is used to implement static member variables. */
-  metatype_args = Py_BuildValue("(s(O){})", "SwigPyObjectType", &PyType_Type);
-  assert(metatype_args);
-  metatype = (PyTypeObject *) PyType_Type.tp_call((PyObject *) &PyType_Type, metatype_args, NULL);
+  /* Metaclass is used to implement static member variables */
+  metatype = SwigPyObjectType();
   assert(metatype);
-  Py_DECREF(metatype_args);
-  metatype->tp_setattro = (setattrofunc) &SwigPyObjectType_setattro;
-  assert(PyType_Ready(metatype) >= 0);
 #endif
   
   /* Fix SwigMethods to carry the callback ptrs when needed */
   SWIG_Python_FixMethods(SwigMethods, swig_const_table, swig_types, swig_type_initial);
   
 #if PY_VERSION_HEX >= 0x03000000
   m = PyModule_Create(&SWIG_module);
@@ -5511,21 +5634,23 @@
   
   md = d = PyModule_GetDict(m);
   (void)md;
   
   SWIG_InitializeModule(0);
   
 #ifdef SWIGPYTHON_BUILTIN
+  swigpyobject = SwigPyObject_TypeOnce();
+  
   SwigPyObject_stype = SWIG_MangledTypeQuery("_p_SwigPyObject");
   assert(SwigPyObject_stype);
   cd = (SwigPyClientData*) SwigPyObject_stype->clientdata;
   if (!cd) {
     SwigPyObject_stype->clientdata = &SwigPyObject_clientdata;
-    SwigPyObject_clientdata.pytype = SwigPyObject_TypeOnce();
-  } else if (SwigPyObject_TypeOnce()->tp_basicsize != cd->pytype->tp_basicsize) {
+    SwigPyObject_clientdata.pytype = swigpyobject;
+  } else if (swigpyobject->tp_basicsize != cd->pytype->tp_basicsize) {
     PyErr_SetString(PyExc_RuntimeError, "Import error: attempted to load two incompatible swig-generated modules.");
 # if PY_VERSION_HEX >= 0x03000000
     return NULL;
 # else
     return;
 # endif
   }
```

### Comparing `pysubnettree-0.35/include/SubnetTree.h` & `pysubnettree-0.37/include/SubnetTree.h`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,17 @@
                return 0;
        }
 
    }
 #endif
 
 private:
+
    PyObject* insert(int family, inx_addr subnet, unsigned short mask, PyObject * data);
    PyObject* remove(int family, inx_addr subnet, unsigned short mask);
    PyObject* lookup(int family, inx_addr subnet) const;
 
+   static void PatriciaDeleteFunction(void* data);
+
    patricia_tree_t* tree;
    bool binary_lookup_mode;
 };
```

### Comparing `pysubnettree-0.35/patricia.c` & `pysubnettree-0.37/patricia.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,1056 +1,1109 @@
 /*
+ * $Id: patricia.c,v 1.7 2005/12/07 20:46:41 dplonka Exp $
  * Dave Plonka <plonka@doit.wisc.edu>
  *
  * This product includes software developed by the University of Michigan,
  * Merit Network, Inc., and their contributors.
  *
  * This file had been called "radix.c" in the MRT sources.
  *
  * I renamed it to "patricia.c" since it's not an implementation of a general
  * radix trie.  Also I pulled in various requirements from "prefix.c" and
  * "demo.c" so that it could be used as a standalone API.
  */
 
-/* From copyright.txt:
- *
- * Copyright (c) 1997, 1998, 1999
+/*
+ * This code originates from Dave Plonka's Net::Security perl module. An
+ * adaptation of it in C is kept at
+ * https://github.com/CAIDA/cc-common/tree/master/libpatricia. That repository
+ * is considered the upstream version for Zeek's fork. We make some custom
+ * changes to this upstream:
+ * - Replaces void_fn_t with data_fn_t and prefix_data_fn_t
+ * - Adds patricia_search_all method
+ * - One commented-out portion of an if statement that breaks one of our tests
  *
+ * The current version is based on commit
+ * fd262ab5ac5bae8b0d4a8b5e2e723115b1846376 from that repo.
+ */
+
+/*
+ * Johanna Amann <johanna@icir.org>
  *
- * The Regents of the University of Michigan ("The Regents") and Merit Network,
- * Inc.  All rights reserved.
- * Redistribution and use in source and binary forms, with or without
- * modification, are permitted provided that the following conditions are met:
- * 1.  Redistributions of source code must retain the above
- *     copyright notice, this list of conditions and the
- *     following disclaimer.
- * 2.  Redistributions in binary form must reproduce the above
- *     copyright notice, this list of conditions and the
- *     following disclaimer in the documentation and/or other
- *     materials provided with the distribution.
- * 3.  All advertising materials mentioning features or use of
- *     this software must display the following acknowledgement:
- * This product includes software developed by the University of Michigan, Merit
- * Network, Inc., and their contributors.
- * 4.  Neither the name of the University, Merit Network, nor the
- *     names of their contributors may be used to endorse or
- *     promote products derived from this software without
- *     specific prior written permission.
- * THIS SOFTWARE IS PROVIDED BY THE REGENTS AND CONTRIBUTORS "AS IS" AND ANY
- * EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
- * WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
- * DISCLAIMED.  IN NO EVENT SHALL THE REGENTS OR CONTRIBUTORS BE LIABLE FOR ANY
- * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
- * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
- * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
- * ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
- * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
- * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ * Added patricia_search_all function.
  */
 
-static char copyright[] =
-"This product includes software developed by the University of Michigan, Merit"
-"Network, Inc., and their contributors.";
-
-#include <assert.h> /* assert */
-#include <ctype.h> /* isdigit */
-#include <errno.h> /* errno */
-#include <math.h> /* sin */
-#include <stddef.h> /* NULL */
-#include <stdio.h> /* sprintf, fprintf, stderr */
-#include <stdlib.h> /* free, atol, calloc */
-#include <string.h> /* memcpy, strchr, strlen */
-#include <netinet/in.h> /* for struct in_addr */
-#include <arpa/inet.h> /* for inet_addr */
-#include <sys/types.h> /* for u_short, etc. */
+#ifndef UNUSED
+#if __GNUC__ >= 3
+#define UNUSED __attribute__((unused))
+#else
+#define UNUSED
+#endif
+#endif
+
+UNUSED static char copyright[] = "This product includes software developed by "
+                                 "the University of Michigan, Merit"
+                                 "Network, Inc., and their contributors.";
+
+#include <arpa/inet.h>  /* BSD, Linux, Solaris: for inet_addr */
+#include <assert.h>     /* assert */
+#include <ctype.h>      /* isdigit */
+#include <errno.h>      /* errno */
+#include <math.h>       /* sin */
+#include <netinet/in.h> /* BSD, Linux: for inet_addr */
+#include <stddef.h>     /* NULL */
+#include <stdio.h>      /* snprintf, fprintf, stderr */
+#include <stdlib.h>     /* free, atol, calloc */
+#include <string.h>     /* memcpy, strchr, strlen */
+#include <sys/socket.h> /* BSD, Linux: for inet_addr */
+#include <sys/types.h>  /* BSD: for inet_addr */
 
 #include "patricia.h"
 
 #define Delete free
 
-void out_of_memory(const char* where)
-    {
-    fprintf(stderr, "out of memory in %s.\n", where);
+static void out_of_memory(const char* where)
+	{
+	fprintf(stderr, "out of memory in %s.\n", where);
+	abort();
+	}
 
-    abort();
-    }
+// From Zeek for reporting memory exhaustion.
+extern void out_of_memory(const char *where);
 
 /* { from prefix.c */
 
 /* prefix_tochar
  * convert prefix information to bytes
  */
-u_char *
-prefix_tochar (prefix_t * prefix)
+u_char *prefix_tochar(prefix_t *prefix)
 {
-    if (prefix == NULL)
-	return (NULL);
+  if (prefix == NULL)
+    return (NULL);
 
-    return ((u_char *) & prefix->add.sin);
+  return ((u_char *)&prefix->add.sin);
 }
 
-int
-comp_with_mask (void *addr, void *dest, u_int mask)
+int comp_with_mask(void *addr, void *dest, u_int mask)
 {
 
-    if ( /* mask/8 == 0 || */ memcmp (addr, dest, mask / 8) == 0) {
-	int n = mask / 8;
-	int m = -(1 << (8 - (mask % 8)));
-
-	if (mask % 8 == 0 || (((u_char *)addr)[n] & m) == (((u_char *)dest)[n] & m))
-	    return (1);
-    }
-    return (0);
-}
-
-/* inet_pton substitute implementation
- * Uses inet_addr to convert an IP address in dotted decimal notation into
- * unsigned long and copies the result to dst.
- * Only supports AF_INET.  Follows standard error return conventions of
- * inet_pton.
- */
-int
-local_inet_pton (int af, const char *src, void *dst)
-{
-    u_long result;
+  if (/* mask/8 == 0 || */ memcmp(addr, dest, mask / 8) == 0) {
+    int n = mask / 8;
+    int m = -(1 << (8 - (mask % 8)));
 
-    if (af == AF_INET) {
-	result = inet_addr(src);
-	if (result == -1)
-	    return 0;
-	else {
-			memcpy (dst, &result, 4);
-	    return 1;
-		}
-	}
-#ifdef NT
-	else if (af == AF_INET6) {
-		struct in6_addr Address;
-		return (inet6_addr(src, &Address));
-	}
-#else
-    else {
-	errno = EAFNOSUPPORT;
-	return -1;
-    }
-#endif /* NT */
+    if (mask % 8 == 0 || (((u_char *)addr)[n] & m) == (((u_char *)dest)[n] & m))
+      return (1);
+  }
+  return (0);
 }
 
 /* this allows imcomplete prefix */
-int
-my_inet_pton (int af, const char *src, void *dst)
+int my_inet_pton(int af, const char *src, void *dst)
 {
-    if (af == AF_INET) {
-        int i, c, val;
-        u_char xp[4] = {0, 0, 0, 0};
-
-        for (i = 0; ; i++) {
-	    c = *src++;
-	    if (!isdigit (c))
-		return (-1);
-	    val = 0;
-	    do {
-		val = val * 10 + c - '0';
-		if (val > 255)
-		    return (0);
-		c = *src++;
-	    } while (c && isdigit (c));
-            xp[i] = val;
-	    if (c == '\0')
-		break;
-            if (c != '.')
-                return (0);
-	    if (i >= 3)
-		return (0);
-        }
-	memcpy (dst, xp, 4);
-        return (1);
-    } else if (af == AF_INET6) {
-        return (local_inet_pton (af, src, dst));
-    } else {
+  if (af == AF_INET) {
+    int i, c, val;
+    u_char xp[sizeof(struct in_addr)] = {0, 0, 0, 0};
+
+    for (i = 0;; i++) {
+      c = *src++;
+      if (!isdigit(c))
+        return (-1);
+      val = 0;
+      do {
+        val = val * 10 + c - '0';
+        if (val > 255)
+          return (0);
+        c = *src++;
+      } while (c && isdigit(c));
+      xp[i] = val;
+      if (c == '\0')
+        break;
+      if (c != '.')
+        return (0);
+      if (i >= 3)
+        return (0);
+    }
+    memcpy(dst, xp, sizeof(struct in_addr));
+    return (1);
+#ifdef HAVE_IPV6
+  } else if (af == AF_INET6) {
+    return (inet_pton(af, src, dst));
+#endif /* HAVE_IPV6 */
+  } else {
 #ifndef NT
-	errno = EAFNOSUPPORT;
+    errno = EAFNOSUPPORT;
 #endif /* NT */
-	return -1;
-    }
+    return -1;
+  }
 }
 
+#define PATRICIA_MAX_THREADS 16
+#define PATRICIA_PREFIX_BUF_LEN 53
+
 /*
  * convert prefix information to ascii string with length
  * thread safe and (almost) re-entrant implementation
  */
-char *
-prefix_toa2x (prefix_t *prefix, char *buff, int with_len)
+char *prefix_toa2x(prefix_t *prefix, char *buff, int with_len)
 {
-    if (prefix == NULL)
-	return ("(Null)");
-    assert (prefix->ref_count >= 0);
-    if (buff == NULL) {
-
-        struct buffer {
-            char buffs[16][48+5];
-            u_int i;
-        } *buffp;
+  if (prefix == NULL)
+    return ("(Null)");
+  assert(prefix->ref_count >= 0);
+  if (buff == NULL) {
+
+    struct buffer {
+      char buffs[PATRICIA_MAX_THREADS][PATRICIA_PREFIX_BUF_LEN];
+      u_int i;
+    } * buffp;
 
-#    if 0
+#if 0
 	THREAD_SPECIFIC_DATA (struct buffer, buffp, 1);
-#    else
-        { /* for scope only */
-	   static struct buffer local_buff;
-           buffp = &local_buff;
-	}
-#    endif
-	if (buffp == NULL) {
-	    /* XXX should we report an error? */
-	    return (NULL);
-	}
-
-	buff = buffp->buffs[buffp->i++%16];
-    }
-    if (prefix->family == AF_INET) {
-	u_char *a;
-	assert (prefix->bitlen <= 32);
-	a = prefix_touchar (prefix);
-	if (with_len) {
-	    sprintf (buff, "%d.%d.%d.%d/%d", a[0], a[1], a[2], a[3],
-		     prefix->bitlen);
-	}
-	else {
-	    sprintf (buff, "%d.%d.%d.%d", a[0], a[1], a[2], a[3]);
-	}
-	return (buff);
-    }
-    else if (prefix->family == AF_INET6) {
-	char *r;
-	r = (char *) inet_ntop (AF_INET6, &prefix->add.sin6, buff, 48 /* a guess value */ );
-	if (r && with_len) {
-	    assert (prefix->bitlen <= 128);
-	    sprintf (buff + strlen (buff), "/%d", prefix->bitlen);
-	}
-	return (buff);
+#else
+    { /* for scope only */
+      static struct buffer local_buff;
+      buffp = &local_buff;
+    }
+#endif
+    if (buffp == NULL) {
+      /* XXX should we report an error? */
+      return (NULL);
+    }
+
+    buff = buffp->buffs[buffp->i++ % PATRICIA_MAX_THREADS];
+  }
+  if (prefix->family == AF_INET) {
+    u_char *a;
+    assert(prefix->bitlen <= sizeof(struct in_addr) * 8);
+    a = prefix_touchar(prefix);
+    if (with_len) {
+      snprintf(buff, PATRICIA_PREFIX_BUF_LEN, "%d.%d.%d.%d/%d", a[0], a[1], a[2], a[3], prefix->bitlen);
+    } else {
+      snprintf(buff, PATRICIA_PREFIX_BUF_LEN, "%d.%d.%d.%d", a[0], a[1], a[2], a[3]);
     }
-    else
-	return (NULL);
+    return (buff);
+  }
+#ifdef HAVE_IPV6
+  else if (prefix->family == AF_INET6) {
+    char *r;
+    r = (char *)inet_ntop(AF_INET6, &prefix->add.sin6, buff,
+                          48 /* a guess value */);
+    if (r && with_len) {
+      assert(prefix->bitlen <= sizeof(struct in6_addr) * 8);
+      snprintf(buff + strlen(buff), PATRICIA_PREFIX_BUF_LEN-strlen(buff), "/%d", prefix->bitlen);
+    }
+    return (buff);
+  }
+#endif /* HAVE_IPV6 */
+  else
+    return (NULL);
 }
 
 /* prefix_toa2
  * convert prefix information to ascii string
  */
-char *
-prefix_toa2 (prefix_t *prefix, char *buff)
+char *prefix_toa2(prefix_t *prefix, char *buff)
 {
-    return (prefix_toa2x (prefix, buff, 0));
+  return (prefix_toa2x(prefix, buff, 0));
 }
 
 /* prefix_toa
  */
-char *
-prefix_toa (prefix_t * prefix)
+char *prefix_toa(prefix_t *prefix)
 {
-    return (prefix_toa2 (prefix, (char *) NULL));
+  return (prefix_toa2(prefix, (char *)NULL));
 }
 
-prefix_t *
-New_Prefix2 (int family, void *dest, int bitlen, prefix_t *prefix)
+prefix_t *New_Prefix2(int family, void *dest, int bitlen, prefix_t *prefix)
 {
-    int dynamic_allocated = 0;
-    int default_bitlen = 32;
+  int dynamic_allocated = 0;
+  int default_bitlen = sizeof(struct in_addr) * 8;
+  prefix4_t *p4 = NULL;
 
-    if (family == AF_INET6) {
-        default_bitlen = 128;
-	if (prefix == NULL) {
-            prefix = calloc(1, sizeof (prefix_t));
-            if (prefix == NULL)
-                out_of_memory("patricia/new_prefix2");
-
-	    dynamic_allocated++;
-	}
-	memcpy (&prefix->add.sin6, dest, 16);
+#ifdef HAVE_IPV6
+  if (family == AF_INET6) {
+    default_bitlen = sizeof(struct in6_addr) * 8;
+    if (prefix == NULL) {
+      prefix = calloc(1, sizeof(prefix_t));
+      if (prefix == NULL)
+        out_of_memory("patricia/new_prefix2: unable to allocate memory");
+      dynamic_allocated++;
     }
-    else
+    memcpy(&prefix->add.sin6, dest, sizeof(struct in6_addr));
+  } else
+#endif /* HAVE_IPV6 */
     if (family == AF_INET) {
-		if (prefix == NULL) {
+      if (prefix == NULL) {
 #ifndef NT
-            prefix = calloc(1, sizeof (prefix4_t));
+        prefix = calloc(1, sizeof(prefix4_t));
+        if (prefix == NULL)
+          out_of_memory("patricia/new_prefix2: unable to allocate memory");
 #else
-			//for some reason, compiler is getting
-			//prefix4_t size incorrect on NT
-			prefix = calloc(1, sizeof (prefix_t));
+      // for some reason, compiler is getting
+      // prefix4_t size incorrect on NT
+      prefix = calloc(1, sizeof(prefix_t));
+      if (prefix == NULL)
+        out_of_memory("patricia/new_prefix2: unable to allocate memory");
 #endif /* NT */
-			if (prefix == NULL)
-				out_of_memory("patricia/new_prefix2");
 
-			dynamic_allocated++;
-		}
-		memcpy (&prefix->add.sin, dest, 4);
-    }
-    else {
-        return (NULL);
+        dynamic_allocated++;
+      }
+      memcpy(&prefix->add.sin, dest, sizeof(struct in_addr));
+    } else {
+      return (NULL);
     }
 
-    prefix->bitlen = (bitlen >= 0)? bitlen: default_bitlen;
-    prefix->family = family;
-    prefix->ref_count = 0;
-    if (dynamic_allocated) {
-        prefix->ref_count++;
-   }
-/* fprintf(stderr, "[C %s, %d]\n", prefix_toa (prefix), prefix->ref_count); */
-    return (prefix);
+  p4 = (prefix4_t*) prefix;
+  p4->bitlen = (bitlen >= 0) ? bitlen : default_bitlen;
+  p4->family = family;
+  p4->ref_count = 0;
+  if (dynamic_allocated) {
+    p4->ref_count++;
+  }
+  /* fprintf(stderr, "[C %s, %d]\n", prefix_toa (prefix), prefix->ref_count);
+   */
+  return (prefix);
 }
 
-prefix_t *
-New_Prefix (int family, void *dest, int bitlen)
+prefix_t *New_Prefix(int family, void *dest, int bitlen)
 {
-    return (New_Prefix2 (family, dest, bitlen, NULL));
+  return (New_Prefix2(family, dest, bitlen, NULL));
 }
 
 /* ascii2prefix
  */
-prefix_t *
-ascii2prefix (int family, char *string)
+prefix_t *ascii2prefix(int family, char *string)
 {
-    u_long bitlen, maxbitlen = 0;
-    char *cp;
-    struct in_addr sin;
-    struct in6_addr sin6;
-    int result;
-    char save[MAXLINE];
-
-    if (string == NULL)
-		return (NULL);
-
-    /* easy way to handle both families */
-    if (family == 0) {
-       family = AF_INET;
-       if (strchr (string, ':')) family = AF_INET6;
-    }
+  u_long bitlen, maxbitlen = 0;
+  char *cp;
+  struct in_addr sin;
+#ifdef HAVE_IPV6
+  struct in6_addr sin6;
+#endif /* HAVE_IPV6 */
+  int result;
+  char save[MAXLINE];
 
-    if (family == AF_INET) {
-		maxbitlen = 32;
-    }
-    else if (family == AF_INET6) {
-		maxbitlen = 128;
-    }
+  if (string == NULL)
+    return (NULL);
 
-    if ((cp = strchr (string, '/')) != NULL) {
-		bitlen = atol (cp + 1);
-		/* *cp = '\0'; */
-		/* copy the string to save. Avoid destroying the string */
-		assert (cp - string < MAXLINE);
-		memcpy (save, string, cp - string);
-		save[cp - string] = '\0';
-		string = save;
-		if (bitlen > maxbitlen)
-			bitlen = maxbitlen;
-		}
-		else {
-			bitlen = maxbitlen;
-		}
-
-		if (family == AF_INET) {
-			if ((result = my_inet_pton (AF_INET, string, &sin)) <= 0)
-				return (NULL);
-			return (New_Prefix (AF_INET, &sin, bitlen));
-		}
+  /* easy way to handle both families */
+  if (family == 0) {
+    family = AF_INET;
+#ifdef HAVE_IPV6
+    if (strchr(string, ':'))
+      family = AF_INET6;
+#endif /* HAVE_IPV6 */
+  }
+
+  if (family == AF_INET) {
+    maxbitlen = sizeof(struct in_addr) * 8;
+  }
+#ifdef HAVE_IPV6
+  else if (family == AF_INET6) {
+    maxbitlen = sizeof(struct in6_addr) * 8;
+  }
+#endif /* HAVE_IPV6 */
+
+  if ((cp = strchr(string, '/')) != NULL) {
+    bitlen = atol(cp + 1);
+    /* *cp = '\0'; */
+    /* copy the string to save. Avoid destroying the string */
+    assert(cp - string < MAXLINE);
+    memcpy(save, string, cp - string);
+    save[cp - string] = '\0';
+    string = save;
+    if (/* bitlen < 0 || */ bitlen > maxbitlen)
+      bitlen = maxbitlen;
+  } else {
+    bitlen = maxbitlen;
+  }
+
+  if (family == AF_INET) {
+    if ((result = my_inet_pton(AF_INET, string, &sin)) <= 0)
+      return (NULL);
+    return (New_Prefix(AF_INET, &sin, bitlen));
+  }
 
-		else if (family == AF_INET6) {
+#ifdef HAVE_IPV6
+  else if (family == AF_INET6) {
 // Get rid of this with next IPv6 upgrade
 #if defined(NT) && !defined(HAVE_INET_NTOP)
-			inet6_addr(string, &sin6);
-			return (New_Prefix (AF_INET6, &sin6, bitlen));
+    inet6_addr(string, &sin6);
+    return (New_Prefix(AF_INET6, &sin6, bitlen));
 #else
-			if ((result = local_inet_pton (AF_INET6, string, &sin6)) <= 0)
-				return (NULL);
+    if ((result = inet_pton(AF_INET6, string, &sin6)) <= 0)
+      return (NULL);
 #endif /* NT */
-			return (New_Prefix (AF_INET6, &sin6, bitlen));
-		}
-		else
-			return (NULL);
-}
-
-prefix_t *
-Ref_Prefix (prefix_t * prefix)
-{
-    if (prefix == NULL)
-	return (NULL);
-    if (prefix->ref_count == 0) {
-	/* make a copy in case of a static prefix */
-        return (New_Prefix2 (prefix->family, &prefix->add, prefix->bitlen, NULL));
-    }
-    prefix->ref_count++;
-/* fprintf(stderr, "[A %s, %d]\n", prefix_toa (prefix), prefix->ref_count); */
-    return (prefix);
-}
-
-void
-Deref_Prefix (prefix_t * prefix)
-{
-    if (prefix == NULL)
-	return;
-    /* for secure programming, raise an assert. no static prefix can call this */
-    assert (prefix->ref_count > 0);
-
-    prefix->ref_count--;
-    assert (prefix->ref_count >= 0);
-    if (prefix->ref_count <= 0) {
-	Delete (prefix);
-	return;
-    }
+    return (New_Prefix(AF_INET6, &sin6, bitlen));
+  }
+#endif /* HAVE_IPV6 */
+  else
+    return (NULL);
+}
+
+prefix_t *Ref_Prefix(prefix_t *prefix)
+{
+  if (prefix == NULL)
+    return (NULL);
+  if (prefix->ref_count == 0) {
+    /* make a copy in case of a static prefix */
+    return (New_Prefix2(prefix->family, &prefix->add, prefix->bitlen, NULL));
+  }
+  prefix->ref_count++;
+  /* fprintf(stderr, "[A %s, %d]\n", prefix_toa (prefix), prefix->ref_count);
+   */
+  return (prefix);
+}
+
+void Deref_Prefix(prefix_t *prefix)
+{
+  if (prefix == NULL)
+    return;
+  /* for secure programming, raise an assert. no static prefix can call this
+   */
+  assert(prefix->ref_count > 0);
+
+  prefix->ref_count--;
+  assert(prefix->ref_count >= 0);
+  if (prefix->ref_count <= 0) {
+    Delete(prefix);
+    return;
+  }
 }
 
 /* } */
 
 /* #define PATRICIA_DEBUG 1 */
 
 static int num_active_patricia = 0;
 
 /* these routines support continuous mask only */
 
-patricia_tree_t *
-New_Patricia (int maxbits)
+patricia_tree_t *New_Patricia(int maxbits)
 {
-    patricia_tree_t *patricia = calloc(1, sizeof *patricia);
-    if (patricia == NULL)
-        out_of_memory("patricia/new_patricia");
-
-    patricia->maxbits = maxbits;
-    patricia->head = NULL;
-    patricia->num_active_node = 0;
-    assert (maxbits <= PATRICIA_MAXBITS); /* XXX */
-    num_active_patricia++;
-    return (patricia);
+  patricia_tree_t *patricia = calloc(1, sizeof *patricia);
+  if (patricia == NULL)
+    out_of_memory("patricia/new_patricia: unable to allocate memory");
+
+  patricia->maxbits = maxbits;
+  patricia->head = NULL;
+  patricia->num_active_node = 0;
+  assert(maxbits <= PATRICIA_MAXBITS); /* XXX */
+  num_active_patricia++;
+  return (patricia);
 }
 
-
 /*
  * if func is supplied, it will be called as func(node->data)
  * before deleting the node
  */
 
-void
-Clear_Patricia (patricia_tree_t *patricia, void_fn_t func)
+void Clear_Patricia(patricia_tree_t *patricia, data_fn_t func)
 {
-    assert (patricia);
-    if (patricia->head) {
+  assert(patricia);
+  if (patricia->head) {
 
-        patricia_node_t *Xstack[PATRICIA_MAXBITS+1];
-        patricia_node_t **Xsp = Xstack;
-        patricia_node_t *Xrn = patricia->head;
-
-        while (Xrn) {
-            patricia_node_t *l = Xrn->l;
-            patricia_node_t *r = Xrn->r;
-
-    	    if (Xrn->prefix) {
-		Deref_Prefix (Xrn->prefix);
-		if (Xrn->data && func)
-	    	    func (Xrn->data);
-    	    }
-    	    else {
-		assert (Xrn->data == NULL);
-    	    }
-    	    Delete (Xrn);
-	    patricia->num_active_node--;
-
-            if (l) {
-                if (r) {
-                    *Xsp++ = r;
-                }
-                Xrn = l;
-            } else if (r) {
-                Xrn = r;
-            } else if (Xsp != Xstack) {
-                Xrn = *(--Xsp);
-            } else {
-                Xrn = (patricia_node_t *) 0;
-            }
+    patricia_node_t *Xstack[PATRICIA_MAXBITS + 1];
+    patricia_node_t **Xsp = Xstack;
+    patricia_node_t *Xrn = patricia->head;
+
+    while (Xrn) {
+      patricia_node_t *l = Xrn->l;
+      patricia_node_t *r = Xrn->r;
+
+      if (Xrn->prefix) {
+        Deref_Prefix(Xrn->prefix);
+        if (Xrn->data && func)
+          func(Xrn->data);
+      } else {
+        assert(Xrn->data == NULL);
+      }
+      Delete(Xrn);
+      patricia->num_active_node--;
+
+      if (l) {
+        if (r) {
+          *Xsp++ = r;
         }
-    }
-    assert (patricia->num_active_node == 0);
-    /* Delete (patricia); */
-}
-
-
-void
-Destroy_Patricia (patricia_tree_t *patricia, void_fn_t func)
-{
-    Clear_Patricia (patricia, func);
-    Delete (patricia);
-    num_active_patricia--;
+        Xrn = l;
+      } else if (r) {
+        Xrn = r;
+      } else if (Xsp != Xstack) {
+        Xrn = *(--Xsp);
+      } else {
+        Xrn = NULL;
+      }
+    }
+  }
+  assert(patricia->num_active_node == 0);
+  /* Delete (patricia); */
+}
+
+void Destroy_Patricia(patricia_tree_t *patricia, data_fn_t func)
+{
+  Clear_Patricia(patricia, func);
+  Delete(patricia);
+  num_active_patricia--;
 }
 
-
 /*
  * if func is supplied, it will be called as func(node->prefix, node->data)
  */
 
-void
-patricia_process (patricia_tree_t *patricia, void_fn_t func)
+void patricia_process(patricia_tree_t *patricia, prefix_data_fn_t func)
 {
-    patricia_node_t *node;
-    assert (func);
+  patricia_node_t *node;
+  assert(func);
 
-    PATRICIA_WALK (patricia->head, node) {
-	func (node->prefix, node->data);
-    } PATRICIA_WALK_END;
+  PATRICIA_WALK(patricia->head, node)
+  {
+    func(node->prefix, node->data);
+  }
+  PATRICIA_WALK_END;
 }
 
+size_t patricia_walk_inorder(patricia_node_t *node, prefix_data_fn_t func)
+{
+  size_t n = 0;
+  assert(func);
+
+  if (node->l) {
+    n += patricia_walk_inorder(node->l, func);
+  }
+
+  if (node->prefix) {
+    func(node->prefix, node->data);
+    n++;
+  }
+
+  if (node->r) {
+    n += patricia_walk_inorder(node->r, func);
+  }
+
+  return n;
+}
 
-patricia_node_t *
-patricia_search_exact (patricia_tree_t *patricia, prefix_t *prefix)
+patricia_node_t *patricia_search_exact(patricia_tree_t *patricia,
+                                       prefix_t *prefix)
 {
-    patricia_node_t *node;
-    u_char *addr;
-    u_int bitlen;
+  patricia_node_t *node;
+  u_char *addr;
+  u_int bitlen;
 
-    assert (patricia);
-    assert (prefix);
-    assert (prefix->bitlen <= patricia->maxbits);
+  assert(patricia);
+  assert(prefix);
+  assert(prefix->bitlen <= patricia->maxbits);
 
-    if (patricia->head == NULL)
-	return (NULL);
+  if (patricia->head == NULL)
+    return (NULL);
 
-    node = patricia->head;
-    addr = prefix_touchar (prefix);
-    bitlen = prefix->bitlen;
+  node = patricia->head;
+  addr = prefix_touchar(prefix);
+  bitlen = prefix->bitlen;
 
-    while (node->bit < bitlen) {
+  while (node->bit < bitlen) {
 
-	if (BIT_TEST (addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
+    if (BIT_TEST(addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
 #ifdef PATRICIA_DEBUG
-	    if (node->prefix)
-    	        fprintf (stderr, "patricia_search_exact: take right %s/%d\n",
-	                 prefix_toa (node->prefix), node->prefix->bitlen);
-	    else
-    	        fprintf (stderr, "patricia_search_exact: take right at %d\n",
-			 node->bit);
+      if (node->prefix)
+        fprintf(stderr, "patricia_search_exact: take right %s/%d\n",
+                prefix_toa(node->prefix), node->prefix->bitlen);
+      else
+        fprintf(stderr, "patricia_search_exact: take right at %u\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-	    node = node->r;
-	}
-	else {
+      node = node->r;
+    } else {
 #ifdef PATRICIA_DEBUG
-	    if (node->prefix)
-    	        fprintf (stderr, "patricia_search_exact: take left %s/%d\n",
-	                 prefix_toa (node->prefix), node->prefix->bitlen);
-	    else
-    	        fprintf (stderr, "patricia_search_exact: take left at %d\n",
-			 node->bit);
+      if (node->prefix)
+        fprintf(stderr, "patricia_search_exact: take left %s/%d\n",
+                prefix_toa(node->prefix), node->prefix->bitlen);
+      else
+        fprintf(stderr, "patricia_search_exact: take left at %u\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-	    node = node->l;
-	}
-
-	if (node == NULL)
-	    return (NULL);
+      node = node->l;
     }
 
+    if (node == NULL)
+      return (NULL);
+  }
+
 #ifdef PATRICIA_DEBUG
-    if (node->prefix)
-        fprintf (stderr, "patricia_search_exact: stop at %s/%d\n",
-	         prefix_toa (node->prefix), node->prefix->bitlen);
-    else
-        fprintf (stderr, "patricia_search_exact: stop at %d\n", node->bit);
+  if (node->prefix)
+    fprintf(stderr, "patricia_search_exact: stop at %s/%d\n",
+            prefix_toa(node->prefix), node->prefix->bitlen);
+  else
+    fprintf(stderr, "patricia_search_exact: stop at %u\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-    if (node->bit > bitlen || node->prefix == NULL)
-	return (NULL);
-    assert (node->bit == bitlen);
-    assert (node->bit == node->prefix->bitlen);
-    if (comp_with_mask (prefix_tochar (node->prefix), prefix_tochar (prefix),
-			bitlen)) {
+  if (node->bit > bitlen || node->prefix == NULL)
+    return (NULL);
+  assert(node->bit == bitlen);
+  assert(node->bit == node->prefix->bitlen);
+  if (comp_with_mask(prefix_tochar(node->prefix), prefix_tochar(prefix),
+                     bitlen)) {
 #ifdef PATRICIA_DEBUG
-        fprintf (stderr, "patricia_search_exact: found %s/%d\n",
-	         prefix_toa (node->prefix), node->prefix->bitlen);
+    fprintf(stderr, "patricia_search_exact: found %s/%d\n",
+            prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-	return (node);
-    }
-    return (NULL);
+    return (node);
+  }
+  return (NULL);
 }
 
-
-/* if inclusive != 0, "best" may be the given prefix itself */
-patricia_node_t *
-patricia_search_best2 (patricia_tree_t *patricia, prefix_t *prefix, int inclusive)
+int patricia_search_all(patricia_tree_t *patricia, prefix_t *prefix,
+                        patricia_node_t ***list, int *n)
 {
-    patricia_node_t *node;
-    patricia_node_t *stack[PATRICIA_MAXBITS + 1];
-    u_char *addr;
-    u_int bitlen;
-    int cnt = 0;
+  patricia_node_t *node;
+  patricia_node_t *stack[PATRICIA_MAXBITS + 1];
+  u_char *addr;
+  u_int bitlen;
+  int cnt = 0;
+
+  assert(patricia);
+  assert(prefix);
+  assert(prefix->bitlen <= patricia->maxbits);
+  assert(n);
+  assert(list);
+  assert(*list == NULL);
 
-    assert (patricia);
-    assert (prefix);
-    assert (prefix->bitlen <= patricia->maxbits);
+  *n = 0;
 
-    if (patricia->head == NULL)
-	return (NULL);
+  if (patricia->head == NULL)
+    return 0;
 
-    node = patricia->head;
-    addr = prefix_touchar (prefix);
-    bitlen = prefix->bitlen;
+  node = patricia->head;
+  addr = prefix_touchar(prefix);
+  bitlen = prefix->bitlen;
 
-    while (node->bit < bitlen) {
+  while (node->bit < bitlen) {
 
-	if (node->prefix) {
+    if (node->prefix) {
 #ifdef PATRICIA_DEBUG
-            fprintf (stderr, "patricia_search_best: push %s/%d\n",
-	             prefix_toa (node->prefix), node->prefix->bitlen);
+      fprintf(stderr, "patricia_search_all: push %s/%d\n",
+              prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-	    stack[cnt++] = node;
-	}
+      stack[cnt++] = node;
+    }
 
-	if (BIT_TEST (addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
+    if (BIT_TEST(addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
 #ifdef PATRICIA_DEBUG
-	    if (node->prefix)
-    	        fprintf (stderr, "patricia_search_best: take right %s/%d\n",
-	                 prefix_toa (node->prefix), node->prefix->bitlen);
-	    else
-    	        fprintf (stderr, "patricia_search_best: take right at %d\n",
-			 node->bit);
+      if (node->prefix)
+        fprintf(stderr, "patricia_search_all: take right %s/%d\n",
+                prefix_toa(node->prefix), node->prefix->bitlen);
+      else
+        fprintf(stderr, "patricia_search_all: take right at %d\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-	    node = node->r;
-	}
-	else {
+      node = node->r;
+    } else {
 #ifdef PATRICIA_DEBUG
-	    if (node->prefix)
-    	        fprintf (stderr, "patricia_search_best: take left %s/%d\n",
-	                 prefix_toa (node->prefix), node->prefix->bitlen);
-	    else
-    	        fprintf (stderr, "patricia_search_best: take left at %d\n",
-			 node->bit);
+      if (node->prefix)
+        fprintf(stderr, "patricia_search_all: take left %s/%d\n",
+                prefix_toa(node->prefix), node->prefix->bitlen);
+      else
+        fprintf(stderr, "patricia_search_all: take left at %d\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-	    node = node->l;
-	}
-
-	if (node == NULL)
-	    break;
+      node = node->l;
     }
 
-    if (inclusive && node && node->prefix)
-	stack[cnt++] = node;
+    if (node == NULL)
+      break;
+  }
+
+  if (node && node->prefix)
+    stack[cnt++] = node;
 
 #ifdef PATRICIA_DEBUG
-    if (node == NULL)
-        fprintf (stderr, "patricia_search_best: stop at null\n");
-    else if (node->prefix)
-        fprintf (stderr, "patricia_search_best: stop at %s/%d\n",
-	         prefix_toa (node->prefix), node->prefix->bitlen);
-    else
-        fprintf (stderr, "patricia_search_best: stop at %d\n", node->bit);
+  if (node == NULL)
+    fprintf(stderr, "patricia_search_all: stop at null\n");
+  else if (node->prefix)
+    fprintf(stderr, "patricia_search_all: stop at %s/%d\n",
+            prefix_toa(node->prefix), node->prefix->bitlen);
+  else
+    fprintf(stderr, "patricia_search_all: stop at %d\n", node->bit);
 #endif /* PATRICIA_DEBUG */
 
-    if (cnt <= 0)
-	return (NULL);
+  if (cnt <= 0)
+    return 0;
+
+  // ok, now we have an upper bound of how much we can return. Let's just alloc
+  // that...
+  patricia_node_t **outlist = calloc(cnt, sizeof(patricia_node_t *));
+  if (outlist == NULL)
+    out_of_memory("patricia/patricia_search_all: unable to allocate memory");
 
-    while (--cnt >= 0) {
-	node = stack[cnt];
+  while (--cnt >= 0) {
+    node = stack[cnt];
 #ifdef PATRICIA_DEBUG
-        fprintf (stderr, "patricia_search_best: pop %s/%d\n",
-	         prefix_toa (node->prefix), node->prefix->bitlen);
+    fprintf(stderr, "patricia_search_all: pop %s/%d\n",
+            prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-	if (comp_with_mask (prefix_tochar (node->prefix),
-			    prefix_tochar (prefix),
-			    node->prefix->bitlen)) {
+    if (comp_with_mask(prefix_tochar(node->prefix), prefix_tochar(prefix),
+                       node->prefix->bitlen)) {
 #ifdef PATRICIA_DEBUG
-            fprintf (stderr, "patricia_search_best: found %s/%d\n",
-	             prefix_toa (node->prefix), node->prefix->bitlen);
+      fprintf(stderr, "patricia_search_all: found %s/%d\n",
+              prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-	    return (node);
-	}
+      outlist[*n] = node;
+      (*n)++;
     }
-    return (NULL);
+  }
+  *list = outlist;
+  return *n != 0 ? 1 : 0;
 }
 
-
-patricia_node_t *
-patricia_search_best (patricia_tree_t *patricia, prefix_t *prefix)
+/* if inclusive != 0, "best" may be the given prefix itself */
+patricia_node_t *patricia_search_best2(patricia_tree_t *patricia,
+                                       prefix_t *prefix, int inclusive)
 {
-    return (patricia_search_best2 (patricia, prefix, 1));
-}
-
+  patricia_node_t *node;
+  patricia_node_t *stack[PATRICIA_MAXBITS + 1];
+  u_char *addr;
+  u_int bitlen;
+  int cnt = 0;
+
+  assert(patricia);
+  assert(prefix);
+  assert(prefix->bitlen <= patricia->maxbits);
 
-patricia_node_t *
-patricia_lookup (patricia_tree_t *patricia, prefix_t *prefix)
-{
-    patricia_node_t *node, *new_node, *parent, *glue;
-    u_char *addr, *test_addr;
-    u_int bitlen, check_bit, differ_bit;
-    int i, j, r;
+  if (patricia->head == NULL)
+    return (NULL);
 
-    assert (patricia);
-    assert (prefix);
-    assert (prefix->bitlen <= patricia->maxbits);
+  node = patricia->head;
+  addr = prefix_touchar(prefix);
+  bitlen = prefix->bitlen;
 
-    if (patricia->head == NULL) {
-	node = calloc(1, sizeof *node);
-	if (node == NULL)
-		out_of_memory("patricia/patricia_lookup");
+  while (node->bit < bitlen) {
 
-	node->bit = prefix->bitlen;
-	node->prefix = Ref_Prefix (prefix);
-	node->parent = NULL;
-	node->l = node->r = NULL;
-	node->data = NULL;
-	patricia->head = node;
+    if (node->prefix) {
 #ifdef PATRICIA_DEBUG
-	fprintf (stderr, "patricia_lookup: new_node #0 %s/%d (head)\n",
-		 prefix_toa (prefix), prefix->bitlen);
+      fprintf(stderr, "patricia_search_best: push %s/%d\n",
+              prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-	patricia->num_active_node++;
-	return (node);
+      stack[cnt++] = node;
     }
 
-    addr = prefix_touchar (prefix);
-    bitlen = prefix->bitlen;
-    node = patricia->head;
-
-    while (node->bit < bitlen || node->prefix == NULL) {
-
-	if (node->bit < patricia->maxbits &&
-	    BIT_TEST (addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
-	    if (node->r == NULL)
-		break;
+    if (BIT_TEST(addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
 #ifdef PATRICIA_DEBUG
-	    if (node->prefix)
-    	        fprintf (stderr, "patricia_lookup: take right %s/%d\n",
-	                 prefix_toa (node->prefix), node->prefix->bitlen);
-	    else
-    	        fprintf (stderr, "patricia_lookup: take right at %d\n", node->bit);
+      if (node->prefix)
+        fprintf(stderr, "patricia_search_best: take right %s/%d\n",
+                prefix_toa(node->prefix), node->prefix->bitlen);
+      else
+        fprintf(stderr, "patricia_search_best: take right at %u\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-	    node = node->r;
-	}
-	else {
-	    if (node->l == NULL)
-		break;
-#ifdef PATRICIA_DEBUG
-	    if (node->prefix)
-    	        fprintf (stderr, "patricia_lookup: take left %s/%d\n",
-	             prefix_toa (node->prefix), node->prefix->bitlen);
-	    else
-    	        fprintf (stderr, "patricia_lookup: take left at %d\n", node->bit);
+      node = node->r;
+    } else {
+#ifdef PATRICIA_DEBUG
+      if (node->prefix)
+        fprintf(stderr, "patricia_search_best: take left %s/%d\n",
+                prefix_toa(node->prefix), node->prefix->bitlen);
+      else
+        fprintf(stderr, "patricia_search_best: take left at %u\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-	    node = node->l;
-	}
-
-	assert (node);
+      node = node->l;
     }
 
-    assert (node->prefix);
+    if (node == NULL)
+      break;
+  }
+
+  if (inclusive && node && node->prefix)
+    stack[cnt++] = node;
+
 #ifdef PATRICIA_DEBUG
-    fprintf (stderr, "patricia_lookup: stop at %s/%d\n",
-	     prefix_toa (node->prefix), node->prefix->bitlen);
+  if (node == NULL)
+    fprintf(stderr, "patricia_search_best: stop at null\n");
+  else if (node->prefix)
+    fprintf(stderr, "patricia_search_best: stop at %s/%d\n",
+            prefix_toa(node->prefix), node->prefix->bitlen);
+  else
+    fprintf(stderr, "patricia_search_best: stop at %u\n", node->bit);
 #endif /* PATRICIA_DEBUG */
 
-    test_addr = prefix_touchar (node->prefix);
-    /* find the first bit different */
-    check_bit = (node->bit < bitlen)? node->bit: bitlen;
-    differ_bit = 0;
-    for (i = 0; i*8 < check_bit; i++) {
-	if ((r = (addr[i] ^ test_addr[i])) == 0) {
-	    differ_bit = (i + 1) * 8;
-	    continue;
-	}
-	/* I know the better way, but for now */
-	for (j = 0; j < 8; j++) {
-	    if (BIT_TEST (r, (0x80 >> j)))
-		break;
-	}
-	/* must be found */
-	assert (j < 8);
-	differ_bit = i * 8 + j;
-	break;
-    }
-    if (differ_bit > check_bit)
-	differ_bit = check_bit;
+  if (cnt <= 0)
+    return (NULL);
+
+  while (--cnt >= 0) {
+    node = stack[cnt];
 #ifdef PATRICIA_DEBUG
-    fprintf (stderr, "patricia_lookup: differ_bit %d\n", differ_bit);
+    fprintf(stderr, "patricia_search_best: pop %s/%d\n",
+            prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-
-    parent = node->parent;
-    while (parent && parent->bit >= differ_bit) {
-	node = parent;
-	parent = node->parent;
+    if (comp_with_mask(prefix_tochar(node->prefix), prefix_tochar(prefix),
+                       node->prefix->bitlen) &&
+        node->prefix->bitlen <= bitlen) {
 #ifdef PATRICIA_DEBUG
-	if (node->prefix)
-            fprintf (stderr, "patricia_lookup: up to %s/%d\n",
-	             prefix_toa (node->prefix), node->prefix->bitlen);
-	else
-            fprintf (stderr, "patricia_lookup: up to %d\n", node->bit);
+      fprintf(stderr, "patricia_search_best: found %s/%d\n",
+              prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
+      return (node);
     }
+  }
+  return (NULL);
+}
 
-    if (differ_bit == bitlen && node->bit == bitlen) {
-	if (node->prefix) {
+patricia_node_t *patricia_search_best(patricia_tree_t *patricia,
+                                      prefix_t *prefix)
+{
+  return (patricia_search_best2(patricia, prefix, 1));
+}
+
+patricia_node_t *patricia_lookup(patricia_tree_t *patricia, prefix_t *prefix)
+{
+  patricia_node_t *node, *new_node, *parent, *glue;
+  u_char *addr, *test_addr;
+  u_int bitlen, check_bit, differ_bit;
+  int i, j, r;
+
+  assert(patricia);
+  assert(prefix);
+  assert(prefix->bitlen <= patricia->maxbits);
+
+  if (patricia->head == NULL) {
+    node = calloc(1, sizeof *node);
+    if (node == NULL)
+      out_of_memory("patricia/patricia_lookup: unable to allocate memory");
+    node->bit = prefix->bitlen;
+    node->prefix = Ref_Prefix(prefix);
+    node->parent = NULL;
+    node->l = node->r = NULL;
+    node->data = NULL;
+    patricia->head = node;
 #ifdef PATRICIA_DEBUG
-    	    fprintf (stderr, "patricia_lookup: found %s/%d\n",
-		     prefix_toa (node->prefix), node->prefix->bitlen);
+    fprintf(stderr, "patricia_lookup: new_node #0 %s/%d (head)\n",
+            prefix_toa(prefix), prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-	    return (node);
-	}
-	node->prefix = Ref_Prefix (prefix);
+    patricia->num_active_node++;
+    return (node);
+  }
+
+  addr = prefix_touchar(prefix);
+  bitlen = prefix->bitlen;
+  node = patricia->head;
+
+  while (node->bit < bitlen || node->prefix == NULL) {
+
+    if (node->bit < patricia->maxbits &&
+        BIT_TEST(addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
+      if (node->r == NULL)
+        break;
+#ifdef PATRICIA_DEBUG
+      if (node->prefix)
+        fprintf(stderr, "patricia_lookup: take right %s/%d\n",
+                prefix_toa(node->prefix), node->prefix->bitlen);
+      else
+        fprintf(stderr, "patricia_lookup: take right at %u\n", node->bit);
+#endif /* PATRICIA_DEBUG */
+      node = node->r;
+    } else {
+      if (node->l == NULL)
+        break;
 #ifdef PATRICIA_DEBUG
-	fprintf (stderr, "patricia_lookup: new node #1 %s/%d (glue mod)\n",
-		 prefix_toa (prefix), prefix->bitlen);
+      if (node->prefix)
+        fprintf(stderr, "patricia_lookup: take left %s/%d\n",
+                prefix_toa(node->prefix), node->prefix->bitlen);
+      else
+        fprintf(stderr, "patricia_lookup: take left at %u\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-	assert (node->data == NULL);
-	return (node);
+      node = node->l;
     }
 
-    new_node = calloc(1, sizeof *new_node);
-    if (new_node == NULL)
-        out_of_memory("patricia/patricia_lookup");
+    assert(node);
+  }
 
-    new_node->bit = prefix->bitlen;
-    new_node->prefix = Ref_Prefix (prefix);
-    new_node->parent = NULL;
-    new_node->l = new_node->r = NULL;
-    new_node->data = NULL;
-    patricia->num_active_node++;
-
-    if (node->bit == differ_bit) {
-	new_node->parent = node;
-	if (node->bit < patricia->maxbits &&
-	    BIT_TEST (addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
-	    assert (node->r == NULL);
-	    node->r = new_node;
-	}
-	else {
-	    assert (node->l == NULL);
-	    node->l = new_node;
-	}
+  assert(node->prefix);
 #ifdef PATRICIA_DEBUG
-	fprintf (stderr, "patricia_lookup: new_node #2 %s/%d (child)\n",
-		 prefix_toa (prefix), prefix->bitlen);
+  fprintf(stderr, "patricia_lookup: stop at %s/%d\n", prefix_toa(node->prefix),
+          node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-	return (new_node);
+
+  test_addr = prefix_touchar(node->prefix);
+  /* find the first bit different */
+  check_bit = (node->bit < bitlen) ? node->bit : bitlen;
+  differ_bit = 0;
+  for (i = 0; i * 8 < check_bit; i++) {
+    if ((r = (addr[i] ^ test_addr[i])) == 0) {
+      differ_bit = (i + 1) * 8;
+      continue;
+    }
+    /* I know the better way, but for now */
+    for (j = 0; j < 8; j++) {
+      if (BIT_TEST(r, (0x80 >> j)))
+        break;
     }
+    /* must be found */
+    assert(j < 8);
+    differ_bit = i * 8 + j;
+    break;
+  }
+  if (differ_bit > check_bit)
+    differ_bit = check_bit;
+#ifdef PATRICIA_DEBUG
+  fprintf(stderr, "patricia_lookup: differ_bit %d\n", differ_bit);
+#endif /* PATRICIA_DEBUG */
 
-    if (bitlen == differ_bit) {
-	if (bitlen < patricia->maxbits &&
-	    BIT_TEST (test_addr[bitlen >> 3], 0x80 >> (bitlen & 0x07))) {
-	    new_node->r = node;
-	}
-	else {
-	    new_node->l = node;
-	}
-	new_node->parent = node->parent;
-	if (node->parent == NULL) {
-	    assert (patricia->head == node);
-	    patricia->head = new_node;
-	}
-	else if (node->parent->r == node) {
-	    node->parent->r = new_node;
-	}
-	else {
-	    node->parent->l = new_node;
-	}
-	node->parent = new_node;
+  parent = node->parent;
+  while (parent && parent->bit >= differ_bit) {
+    node = parent;
+    parent = node->parent;
 #ifdef PATRICIA_DEBUG
-	fprintf (stderr, "patricia_lookup: new_node #3 %s/%d (parent)\n",
-		 prefix_toa (prefix), prefix->bitlen);
+    if (node->prefix)
+      fprintf(stderr, "patricia_lookup: up to %s/%d\n",
+              prefix_toa(node->prefix), node->prefix->bitlen);
+    else
+      fprintf(stderr, "patricia_lookup: up to %u\n", node->bit);
 #endif /* PATRICIA_DEBUG */
-    }
-    else {
-        glue = calloc(1, sizeof *glue);
-        if (glue == NULL)
-            out_of_memory("patricia/patricia_lookup");
-
-        glue->bit = differ_bit;
-        glue->prefix = NULL;
-        glue->parent = node->parent;
-        glue->data = NULL;
-        patricia->num_active_node++;
-	if (differ_bit < patricia->maxbits &&
-	    BIT_TEST (addr[differ_bit >> 3], 0x80 >> (differ_bit & 0x07))) {
-	    glue->r = new_node;
-	    glue->l = node;
-	}
-	else {
-	    glue->r = node;
-	    glue->l = new_node;
-	}
-	new_node->parent = glue;
+  }
 
-	if (node->parent == NULL) {
-	    assert (patricia->head == node);
-	    patricia->head = glue;
-	}
-	else if (node->parent->r == node) {
-	    node->parent->r = glue;
-	}
-	else {
-	    node->parent->l = glue;
-	}
-	node->parent = glue;
+  if (differ_bit == bitlen && node->bit == bitlen) {
+    if (node->prefix) {
 #ifdef PATRICIA_DEBUG
-	fprintf (stderr, "patricia_lookup: new_node #4 %s/%d (glue+node)\n",
-		 prefix_toa (prefix), prefix->bitlen);
+      fprintf(stderr, "patricia_lookup: found %s/%d\n",
+              prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
+      return (node);
     }
-    return (new_node);
-}
-
-
-void
-patricia_remove (patricia_tree_t *patricia, patricia_node_t *node)
-{
-    patricia_node_t *parent, *child;
-
-    assert (patricia);
-    assert (node);
-
-    if (node->r && node->l) {
+    node->prefix = Ref_Prefix(prefix);
 #ifdef PATRICIA_DEBUG
-	fprintf (stderr, "patricia_remove: #0 %s/%d (r & l)\n",
-		 prefix_toa (node->prefix), node->prefix->bitlen);
+    fprintf(stderr, "patricia_lookup: new node #1 %s/%d (glue mod)\n",
+            prefix_toa(prefix), prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
+    assert(node->data == NULL);
+    return (node);
+  }
 
-	/* this might be a placeholder node -- have to check and make sure
-	 * there is a prefix aossciated with it ! */
-	if (node->prefix != NULL)
-	  Deref_Prefix (node->prefix);
-	node->prefix = NULL;
-	/* Also I needed to clear data pointer -- masaki */
-	node->data = NULL;
-	return;
+  new_node = calloc(1, sizeof *new_node);
+  if (new_node == NULL)
+    out_of_memory("patricia/patricia_lookup: unable to allocate memory");
+  new_node->bit = prefix->bitlen;
+  new_node->prefix = Ref_Prefix(prefix);
+  new_node->parent = NULL;
+  new_node->l = new_node->r = NULL;
+  new_node->data = NULL;
+  patricia->num_active_node++;
+
+  if (node->bit == differ_bit) {
+    new_node->parent = node;
+    if (node->bit < patricia->maxbits &&
+        BIT_TEST(addr[node->bit >> 3], 0x80 >> (node->bit & 0x07))) {
+      assert(node->r == NULL);
+      node->r = new_node;
+    } else {
+      assert(node->l == NULL);
+      node->l = new_node;
     }
+#ifdef PATRICIA_DEBUG
+    fprintf(stderr, "patricia_lookup: new_node #2 %s/%d (child)\n",
+            prefix_toa(prefix), prefix->bitlen);
+#endif /* PATRICIA_DEBUG */
+    return (new_node);
+  }
 
-    if (node->r == NULL && node->l == NULL) {
+  if (bitlen == differ_bit) {
+    if (bitlen < patricia->maxbits &&
+        BIT_TEST(test_addr[bitlen >> 3], 0x80 >> (bitlen & 0x07))) {
+      new_node->r = node;
+    } else {
+      new_node->l = node;
+    }
+    new_node->parent = node->parent;
+    if (node->parent == NULL) {
+      assert(patricia->head == node);
+      patricia->head = new_node;
+    } else if (node->parent->r == node) {
+      node->parent->r = new_node;
+    } else {
+      node->parent->l = new_node;
+    }
+    node->parent = new_node;
 #ifdef PATRICIA_DEBUG
-	fprintf (stderr, "patricia_remove: #1 %s/%d (!r & !l)\n",
-		 prefix_toa (node->prefix), node->prefix->bitlen);
+    fprintf(stderr, "patricia_lookup: new_node #3 %s/%d (parent)\n",
+            prefix_toa(prefix), prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-	parent = node->parent;
-	Deref_Prefix (node->prefix);
-	Delete (node);
-        patricia->num_active_node--;
+  } else {
+    glue = calloc(1, sizeof *glue);
+    if (glue == NULL)
+      out_of_memory("patricia/patricia_lookup: unable to allocate memory");
+    glue->bit = differ_bit;
+    glue->prefix = NULL;
+    glue->parent = node->parent;
+    glue->data = NULL;
+    patricia->num_active_node++;
+    if (differ_bit < patricia->maxbits &&
+        BIT_TEST(addr[differ_bit >> 3], 0x80 >> (differ_bit & 0x07))) {
+      glue->r = new_node;
+      glue->l = node;
+    } else {
+      glue->r = node;
+      glue->l = new_node;
+    }
+    new_node->parent = glue;
 
-	if (parent == NULL) {
-	    assert (patricia->head == node);
-	    patricia->head = NULL;
-	    return;
-	}
+    if (node->parent == NULL) {
+      assert(patricia->head == node);
+      patricia->head = glue;
+    } else if (node->parent->r == node) {
+      node->parent->r = glue;
+    } else {
+      node->parent->l = glue;
+    }
+    node->parent = glue;
+#ifdef PATRICIA_DEBUG
+    fprintf(stderr, "patricia_lookup: new_node #4 %s/%d (glue+node)\n",
+            prefix_toa(prefix), prefix->bitlen);
+#endif /* PATRICIA_DEBUG */
+  }
+  return (new_node);
+}
 
-	if (parent->r == node) {
-	    parent->r = NULL;
-	    child = parent->l;
-	}
-	else {
-	    assert (parent->l == node);
-	    parent->l = NULL;
-	    child = parent->r;
-	}
+void patricia_remove(patricia_tree_t *patricia, patricia_node_t *node)
+{
+  patricia_node_t *parent, *child;
 
-	if (parent->prefix)
-	    return;
+  assert(patricia);
+  assert(node);
 
-	/* we need to remove parent too */
+  if (node->r && node->l) {
+#ifdef PATRICIA_DEBUG
+    fprintf(stderr, "patricia_remove: #0 %s/%d (r & l)\n",
+            prefix_toa(node->prefix), node->prefix->bitlen);
+#endif /* PATRICIA_DEBUG */
 
-	if (parent->parent == NULL) {
-	    assert (patricia->head == parent);
-	    patricia->head = child;
-	}
-	else if (parent->parent->r == parent) {
-	    parent->parent->r = child;
-	}
-	else {
-	    assert (parent->parent->l == parent);
-	    parent->parent->l = child;
-	}
-	child->parent = parent->parent;
-	Delete (parent);
-        patricia->num_active_node--;
-	return;
-    }
+    /* this might be a placeholder node -- have to check and make sure
+     * there is a prefix aossciated with it ! */
+    if (node->prefix != NULL)
+      Deref_Prefix(node->prefix);
+    node->prefix = NULL;
+    /* Also I needed to clear data pointer -- masaki */
+    node->data = NULL;
+    return;
+  }
 
+  if (node->r == NULL && node->l == NULL) {
 #ifdef PATRICIA_DEBUG
-    fprintf (stderr, "patricia_remove: #2 %s/%d (r ^ l)\n",
-	     prefix_toa (node->prefix), node->prefix->bitlen);
+    fprintf(stderr, "patricia_remove: #1 %s/%d (!r & !l)\n",
+            prefix_toa(node->prefix), node->prefix->bitlen);
 #endif /* PATRICIA_DEBUG */
-    if (node->r) {
-	child = node->r;
-    }
-    else {
-	assert (node->l);
-	child = node->l;
-    }
     parent = node->parent;
-    child->parent = parent;
-
-    Deref_Prefix (node->prefix);
-    Delete (node);
+    Deref_Prefix(node->prefix);
+    Delete(node);
     patricia->num_active_node--;
 
     if (parent == NULL) {
-	assert (patricia->head == node);
-	patricia->head = child;
-	return;
+      assert(patricia->head == node);
+      patricia->head = NULL;
+      return;
     }
 
     if (parent->r == node) {
-	parent->r = child;
+      parent->r = NULL;
+      child = parent->l;
+    } else {
+      assert(parent->l == node);
+      parent->l = NULL;
+      child = parent->r;
     }
-    else {
-        assert (parent->l == node);
-	parent->l = child;
+
+    if (parent->prefix)
+      return;
+
+    /* we need to remove parent too */
+
+    if (parent->parent == NULL) {
+      assert(patricia->head == parent);
+      patricia->head = child;
+    } else if (parent->parent->r == parent) {
+      parent->parent->r = child;
+    } else {
+      assert(parent->parent->l == parent);
+      parent->parent->l = child;
     }
+    child->parent = parent->parent;
+    Delete(parent);
+    patricia->num_active_node--;
+    return;
+  }
+
+#ifdef PATRICIA_DEBUG
+  fprintf(stderr, "patricia_remove: #2 %s/%d (r ^ l)\n",
+          prefix_toa(node->prefix), node->prefix->bitlen);
+#endif /* PATRICIA_DEBUG */
+  if (node->r) {
+    child = node->r;
+  } else {
+    assert(node->l);
+    child = node->l;
+  }
+  parent = node->parent;
+  child->parent = parent;
+
+  Deref_Prefix(node->prefix);
+  Delete(node);
+  patricia->num_active_node--;
+
+  if (parent == NULL) {
+    assert(patricia->head == node);
+    patricia->head = child;
+    return;
+  }
+
+  if (parent->r == node) {
+    parent->r = child;
+  } else {
+    assert(parent->l == node);
+    parent->l = child;
+  }
 }
 
 /* { from demo.c */
 
-patricia_node_t *
-make_and_lookup (patricia_tree_t *tree, char *string)
+patricia_node_t *make_and_lookup(patricia_tree_t *tree, char *string)
 {
-    prefix_t *prefix;
-    patricia_node_t *node;
+  prefix_t *prefix;
+  patricia_node_t *node;
 
-    prefix = ascii2prefix (AF_INET, string);
-    printf ("make_and_lookup: %s/%d\n", prefix_toa (prefix), prefix->bitlen);
-    node = patricia_lookup (tree, prefix);
-    Deref_Prefix (prefix);
-    return (node);
+  prefix = ascii2prefix(AF_INET, string);
+  printf("make_and_lookup: %s/%d\n", prefix_toa(prefix), prefix->bitlen);
+  node = patricia_lookup(tree, prefix);
+  Deref_Prefix(prefix);
+  return (node);
 }
 
-patricia_node_t *
-try_search_exact (patricia_tree_t *tree, char *string)
+patricia_node_t *try_search_exact(patricia_tree_t *tree, char *string)
 {
-    prefix_t *prefix;
-    patricia_node_t *node;
+  prefix_t *prefix;
+  patricia_node_t *node;
 
-    prefix = ascii2prefix (AF_INET, string);
-    printf ("try_search_exact: %s/%d\n", prefix_toa (prefix), prefix->bitlen);
-    if ((node = patricia_search_exact (tree, prefix)) == NULL) {
-        printf ("try_search_exact: not found\n");
-    }
-    else {
-        printf ("try_search_exact: %s/%d found\n",
-	        prefix_toa (node->prefix), node->prefix->bitlen);
-    }
-    Deref_Prefix (prefix);
-    return (node);
+  prefix = ascii2prefix(AF_INET, string);
+  printf("try_search_exact: %s/%d\n", prefix_toa(prefix), prefix->bitlen);
+  if ((node = patricia_search_exact(tree, prefix)) == NULL) {
+    printf("try_search_exact: not found\n");
+  } else {
+    printf("try_search_exact: %s/%d found\n", prefix_toa(node->prefix),
+           node->prefix->bitlen);
+  }
+  Deref_Prefix(prefix);
+  return (node);
 }
 
-void
-lookup_then_remove (patricia_tree_t *tree, char *string)
+void lookup_then_remove(patricia_tree_t *tree, char *string)
 {
-    patricia_node_t *node;
+  patricia_node_t *node;
 
-    if ( (node = try_search_exact(tree, string)) )
-        patricia_remove (tree, node);
+  if ((node = try_search_exact(tree, string)))
+    patricia_remove(tree, node);
 }
 
-patricia_node_t *
-try_search_best (patricia_tree_t *tree, char *string)
+patricia_node_t *try_search_best(patricia_tree_t *tree, char *string)
 {
-    prefix_t *prefix;
-    patricia_node_t *node;
+  prefix_t *prefix;
+  patricia_node_t *node;
 
-    prefix = ascii2prefix (AF_INET, string);
-    printf ("try_search_best: %s/%d\n", prefix_toa (prefix), prefix->bitlen);
-    if ((node = patricia_search_best (tree, prefix)) == NULL)
-        printf ("try_search_best: not found\n");
-    else
-        printf ("try_search_best: %s/%d found\n",
-	        prefix_toa (node->prefix), node->prefix->bitlen);
-    Deref_Prefix (prefix);
-    return 0; // [RS] What is supposed to be returned here?
- }
+  prefix = ascii2prefix(AF_INET, string);
+  printf("try_search_best: %s/%d\n", prefix_toa(prefix), prefix->bitlen);
+  if ((node = patricia_search_best(tree, prefix)) == NULL)
+    printf("try_search_best: not found\n");
+  else
+    printf("try_search_best: %s/%d found\n", prefix_toa(node->prefix),
+           node->prefix->bitlen);
+  Deref_Prefix(prefix);
+  return (node);
+}
 
 /* } */
```

