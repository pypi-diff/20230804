# Comparing `tmp/doki-Mowstyl-1.4.0.tar.gz` & `tmp/doki-Mowstyl-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doki-Mowstyl-1.4.0.tar", last modified: Wed May 10 18:24:39 2023, max compression
+gzip compressed data, was "doki-Mowstyl-1.5.0.tar", last modified: Fri Aug  4 16:52:18 2023, max compression
```

## Comparing `doki-Mowstyl-1.4.0.tar` & `doki-Mowstyl-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 18:24:39.994444 doki-Mowstyl-1.4.0/
--rw-rw-rw-   0        0        0     1111 2021-09-20 14:20:25.000000 doki-Mowstyl-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     1148 2023-05-10 18:24:39.993445 doki-Mowstyl-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      824 2021-09-15 23:16:12.000000 doki-Mowstyl-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 18:24:39.983444 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/
--rw-rw-rw-   0        0        0     1148 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-10 18:24:39.000000 doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2023-05-10 16:36:21.000000 doki-Mowstyl-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 18:24:39.994444 doki-Mowstyl-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2966 2023-05-10 16:36:50.000000 doki-Mowstyl-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 18:24:39.976446 doki-Mowstyl-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 18:24:39.992447 doki-Mowstyl-1.4.0/src/doki/
--rw-rw-rw-   0        0        0     1812 2021-10-19 13:02:35.000000 doki-Mowstyl-1.4.0/src/doki/arraylist.c
--rw-rw-rw-   0        0        0     1035 2021-10-19 12:10:13.000000 doki-Mowstyl-1.4.0/src/doki/arraylist.h
--rw-rw-rw-   0        0        0    50644 2023-05-10 18:15:50.000000 doki-Mowstyl-1.4.0/src/doki/doki.c
--rw-rw-rw-   0        0        0    12726 2022-02-15 21:10:06.000000 doki-Mowstyl-1.4.0/src/doki/funmatrix.c
--rw-rw-rw-   0        0        0     4006 2022-02-15 21:10:06.000000 doki-Mowstyl-1.4.0/src/doki/funmatrix.h
--rw-rw-rw-   0        0        0     4149 2021-10-19 12:10:13.000000 doki-Mowstyl-1.4.0/src/doki/platform.c
--rw-rw-rw-   0        0        0     7445 2023-05-10 14:44:41.000000 doki-Mowstyl-1.4.0/src/doki/platform.h
--rw-rw-rw-   0        0        0      313 2021-07-24 11:59:20.000000 doki-Mowstyl-1.4.0/src/doki/qgate.h
--rw-rw-rw-   0        0        0    11412 2022-02-15 19:02:13.000000 doki-Mowstyl-1.4.0/src/doki/qops.c
--rw-rw-rw-   0        0        0     2059 2021-10-19 12:10:13.000000 doki-Mowstyl-1.4.0/src/doki/qops.h
--rw-rw-rw-   0        0        0     3064 2022-02-15 14:46:56.000000 doki-Mowstyl-1.4.0/src/doki/qstate.c
--rw-rw-rw-   0        0        0     2320 2022-02-15 14:46:56.000000 doki-Mowstyl-1.4.0/src/doki/qstate.h
+drwxrwxrwx   0        0        0        0 2023-08-04 16:52:18.616209 doki-Mowstyl-1.5.0/
+-rw-rw-rw-   0        0        0     1111 2021-09-20 14:20:25.000000 doki-Mowstyl-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1148 2023-08-04 16:52:18.616209 doki-Mowstyl-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2021-09-15 23:16:12.000000 doki-Mowstyl-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 16:52:18.605209 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/
+-rw-rw-rw-   0        0        0     1148 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2023-05-10 16:36:21.000000 doki-Mowstyl-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 16:52:18.616209 doki-Mowstyl-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2966 2023-08-04 16:44:51.000000 doki-Mowstyl-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:52:18.599209 doki-Mowstyl-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 16:52:18.615209 doki-Mowstyl-1.5.0/src/doki/
+-rw-rw-rw-   0        0        0     1816 2023-07-21 13:17:38.000000 doki-Mowstyl-1.5.0/src/doki/arraylist.c
+-rw-rw-rw-   0        0        0     1059 2023-07-21 13:17:34.000000 doki-Mowstyl-1.5.0/src/doki/arraylist.h
+-rw-rw-rw-   0        0        0    73129 2023-07-27 20:22:54.000000 doki-Mowstyl-1.5.0/src/doki/doki.c
+-rw-rw-rw-   0        0        0    35772 2023-08-04 11:43:53.000000 doki-Mowstyl-1.5.0/src/doki/funmatrix.c
+-rw-rw-rw-   0        0        0     6219 2023-07-27 18:04:35.000000 doki-Mowstyl-1.5.0/src/doki/funmatrix.h
+-rw-rw-rw-   0        0        0     1424 2023-07-27 11:20:10.000000 doki-Mowstyl-1.5.0/src/doki/platform.c
+-rw-rw-rw-   0        0        0    10504 2023-07-27 19:54:26.000000 doki-Mowstyl-1.5.0/src/doki/platform.h
+-rw-rw-rw-   0        0        0      336 2023-07-21 13:16:44.000000 doki-Mowstyl-1.5.0/src/doki/qgate.h
+-rw-rw-rw-   0        0        0    19350 2023-07-27 21:22:31.000000 doki-Mowstyl-1.5.0/src/doki/qops.c
+-rw-rw-rw-   0        0        0     2213 2023-07-27 17:55:06.000000 doki-Mowstyl-1.5.0/src/doki/qops.h
+-rw-rw-rw-   0        0        0     3096 2023-07-21 13:17:25.000000 doki-Mowstyl-1.5.0/src/doki/qstate.c
+-rw-rw-rw-   0        0        0     2344 2023-07-21 13:17:20.000000 doki-Mowstyl-1.5.0/src/doki/qstate.h
```

### Comparing `doki-Mowstyl-1.4.0/LICENSE` & `doki-Mowstyl-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.4.0/PKG-INFO` & `doki-Mowstyl-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doki-Mowstyl
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python interface for Doki (QSimov core)
 Home-page: https://github.com/Mowstyl/Doki
 Author: Hernán Indíbil de la Cruz Calvo
 Author-email: HernanIndibil.LaCruz@alu.uclm.es
 License: MIT
 Keywords: qsimov simulator quantum
 Classifier: Intended Audience :: Developers
```

### Comparing `doki-Mowstyl-1.4.0/README.md` & `doki-Mowstyl-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/PKG-INFO` & `doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doki-Mowstyl
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python interface for Doki (QSimov core)
 Home-page: https://github.com/Mowstyl/Doki
 Author: Hernán Indíbil de la Cruz Calvo
 Author-email: HernanIndibil.LaCruz@alu.uclm.es
 License: MIT
 Keywords: qsimov simulator quantum
 Classifier: Intended Audience :: Developers
```

### Comparing `doki-Mowstyl-1.4.0/doki_Mowstyl.egg-info/SOURCES.txt` & `doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.4.0/setup.py` & `doki-Mowstyl-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         build_ext.build_extensions(self)
 
 
 def main():
     """Code to be executed on install."""
     setup(
         name="doki-Mowstyl",
-        version="1.4.0",
+        version="1.5.0",
         author="Hernán Indíbil de la Cruz Calvo",
         author_email="HernanIndibil.LaCruz@alu.uclm.es",
         cmdclass={'build_ext': DokiBuild},
         license="MIT",
         url="https://github.com/Mowstyl/Doki",
         description="Python interface for Doki (QSimov core)",
         long_description="Python module containing Doki, the core of QSimov" +
@@ -68,15 +68,15 @@
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: Implementation :: CPython',
             'Topic :: Software Development :: Libraries :: Python Modules',
             "Topic :: Scientific/Engineering",
         ],
         keywords="qsimov simulator quantum",
         install_requires=[
-            "numpy>=1.21"
+            "numpy>=1.19"
         ],
         ext_modules=[Extension('doki', sources=sources,
                                extra_compile_args=_comp_args,
                                extra_link_args=_comp_args,
                                include_dirs=[np.get_include()])],
         data_files=[('headers', headers)],
         python_requires=">=3.6",
```

### Comparing `doki-Mowstyl-1.4.0/src/doki/arraylist.c` & `doki-Mowstyl-1.5.0/src/doki/arraylist.c`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,86 @@
-#include "platform.h"
 #include "arraylist.h"
-
+#include "platform.h"
 
 unsigned char
-alist_init(struct array_list_e *this, NATURAL_TYPE size)
+alist_init (struct array_list_e *this, NATURAL_TYPE size)
 {
-    size_t i, offset, errored_chunk;
-    _Bool errored;
+  size_t i, offset, errored_chunk;
+  _Bool errored;
 
-    this->size = size;
-    this->num_chunks = this->size / NATURAL_ARRAY_SIZE;
-    offset = this->size % NATURAL_ARRAY_SIZE;
-    if (offset > 0) {
-        this->num_chunks++;
-    }
-    else {
-        offset = NATURAL_ARRAY_SIZE;
-    }
-    this->vector = MALLOC_TYPE(this->num_chunks, NATURAL_TYPE*);
-    if (this->vector == NULL) {
-        return 1;
-    }
-    errored = 0;
-    for (i = 0; i < this->num_chunks - 1; i++) {
-        this->vector[i] = MALLOC_TYPE(NATURAL_ARRAY_SIZE, NATURAL_TYPE);
-        if (this->vector[i] == NULL) {
-            errored = 1;
-            errored_chunk = i;
-            break;
+  this->size = size;
+  this->num_chunks = this->size / NATURAL_ARRAY_SIZE;
+  offset = this->size % NATURAL_ARRAY_SIZE;
+  if (offset > 0)
+    {
+      this->num_chunks++;
+    }
+  else
+    {
+      offset = NATURAL_ARRAY_SIZE;
+    }
+  this->vector = MALLOC_TYPE (this->num_chunks, NATURAL_TYPE *);
+  if (this->vector == NULL)
+    {
+      return 1;
+    }
+  errored = 0;
+  for (i = 0; i < this->num_chunks - 1; i++)
+    {
+      this->vector[i] = MALLOC_TYPE (NATURAL_ARRAY_SIZE, NATURAL_TYPE);
+      if (this->vector[i] == NULL)
+        {
+          errored = 1;
+          errored_chunk = i;
+          break;
         }
     }
-    if (!errored) {
-        this->vector[this->num_chunks-1] = MALLOC_TYPE(offset, NATURAL_TYPE);
-        if (this->vector[this->num_chunks-1] == NULL) {
-            errored = 1;
-            errored_chunk = this->num_chunks-1;
+  if (!errored)
+    {
+      this->vector[this->num_chunks - 1] = MALLOC_TYPE (offset, NATURAL_TYPE);
+      if (this->vector[this->num_chunks - 1] == NULL)
+        {
+          errored = 1;
+          errored_chunk = this->num_chunks - 1;
         }
     }
-    if (errored) {
-        for (i = 0; i < errored_chunk; i++) {
-            free(this->vector[i]);
+  if (errored)
+    {
+      for (i = 0; i < errored_chunk; i++)
+        {
+          free (this->vector[i]);
         }
-        free(this->vector);
-        return 2;
+      free (this->vector);
+      return 2;
     }
 
-    return 0;
+  return 0;
 }
 
-
 void
-alist_clear(struct array_list_e *this)
+alist_clear (struct array_list_e *this)
 {
-    size_t i;
-    if (this->vector != NULL) {
-        for (i = 0; i < this->num_chunks; i++) {
-            free(this->vector[i]);
+  size_t i;
+  if (this->vector != NULL)
+    {
+      for (i = 0; i < this->num_chunks; i++)
+        {
+          free (this->vector[i]);
         }
-        free(this->vector);
+      free (this->vector);
     }
-    this->vector = NULL;
-    this->num_chunks = 0;
-    this->size = 0;
+  this->vector = NULL;
+  this->num_chunks = 0;
+  this->size = 0;
 }
 
 void
-alist_set(struct array_list_e *this, NATURAL_TYPE i, NATURAL_TYPE value)
+alist_set (struct array_list_e *this, NATURAL_TYPE i, NATURAL_TYPE value)
 {
-    this->vector[i/COMPLEX_ARRAY_SIZE][i%COMPLEX_ARRAY_SIZE] = value;
+  this->vector[i / COMPLEX_ARRAY_SIZE][i % COMPLEX_ARRAY_SIZE] = value;
 }
 
 NATURAL_TYPE
-alist_get(struct array_list_e *this, NATURAL_TYPE i)
+alist_get (struct array_list_e *this, NATURAL_TYPE i)
 {
-    return this->vector[i/COMPLEX_ARRAY_SIZE][i%COMPLEX_ARRAY_SIZE];
+  return this->vector[i / COMPLEX_ARRAY_SIZE][i % COMPLEX_ARRAY_SIZE];
 }
```

### Comparing `doki-Mowstyl-1.4.0/src/doki/arraylist.h` & `doki-Mowstyl-1.5.0/src/doki/arraylist.h`

 * *Files 27% similar despite different names*

```diff
@@ -12,35 +12,33 @@
  */
 
 /** \struct array_list_e arraylist.h "arraylist.h"
  *  \brief List of int arrays.
  *  A list of int arrays (chunks).
  */
 
-#ifndef __ARRAYLIST_H
-#define __ARRAYLIST_H
+#pragma once
+#ifndef ARRAYLIST_H_
+#define ARRAYLIST_H_
 
 #include "platform.h"
 
 struct array_list_e
 {
   /* total (not partial) size of the vector */
-  NATURAL_TYPE   size;
+  NATURAL_TYPE size;
   /* number of chunks */
-  size_t         num_chunks;
+  size_t num_chunks;
   /* vector */
   NATURAL_TYPE **vector;
 };
 
-unsigned char
-alist_init(struct array_list_e *this, NATURAL_TYPE size);
+unsigned char alist_init (struct array_list_e *this, NATURAL_TYPE size);
 
-void
-alist_clear(struct array_list_e *this);
+void alist_clear (struct array_list_e *this);
 
-void
-alist_set(struct array_list_e *this, NATURAL_TYPE i, NATURAL_TYPE value);
+void alist_set (struct array_list_e *this, NATURAL_TYPE i, NATURAL_TYPE value);
 
 NATURAL_TYPE
-alist_get(struct array_list_e *this, NATURAL_TYPE i);
+alist_get (struct array_list_e *this, NATURAL_TYPE i);
 
-#endif
+#endif /* ARRAYLIST_H_ */
```

### Comparing `doki-Mowstyl-1.4.0/src/doki/doki.c` & `doki-Mowstyl-1.5.0/src/doki/doki.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,1579 +1,2559 @@
 #define PY_SSIZE_T_CLEAN
-#include <Python.h>
-#include <omp.h>
-#include <numpy/arrayobject.h>
 #include "platform.h"
-#include "qstate.h"
 #include "qgate.h"
 #include "qops.h"
-
+#include "qstate.h"
+#include <Python.h>
+#include <complex.h>
+#include <errno.h>
+#include <numpy/arrayobject.h>
+#include <omp.h>
 
 static PyObject *DokiError;
 
-void
-doki_registry_destroy (PyObject *capsule);
+void doki_registry_destroy (PyObject *capsule);
 
-void
-doki_gate_destroy (PyObject *capsule);
+void doki_gate_destroy (PyObject *capsule);
 
-void
-doki_funmatrix_destroy (PyObject *capsule);
+void doki_funmatrix_destroy (PyObject *capsule);
 
-static PyObject *
-doki_registry_new (PyObject *self, PyObject *args);
+static PyObject *doki_registry_new (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_registry_clone (PyObject *self, PyObject *args);
+static PyObject *doki_registry_clone (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_registry_del (PyObject *self, PyObject *args);
+static PyObject *doki_registry_del (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_gate_new (PyObject *self, PyObject *args);
+static PyObject *doki_gate_new (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_gate_get (PyObject *self, PyObject *args);
+static PyObject *doki_gate_get (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_registry_get (PyObject *self, PyObject *args);
+static PyObject *doki_registry_get (PyObject *self, PyObject *args);
 
-void
-custom_state_init_py(PyObject *values, struct state_vector *state);
+void custom_state_init_py (PyObject *values, struct state_vector *state);
 
-void
-custom_state_init_np(PyObject *values, struct state_vector *state);
+void custom_state_init_np (PyObject *values, struct state_vector *state);
 
-static PyObject *
-doki_registry_new_data (PyObject *self, PyObject *args);
+static PyObject *doki_registry_new_data (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_registry_apply (PyObject *self, PyObject *args);
+static PyObject *doki_registry_apply (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_registry_join (PyObject *self, PyObject *args);
+static PyObject *doki_registry_join (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_registry_measure (PyObject *self, PyObject *args);
+static PyObject *doki_registry_measure (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_registry_prob (PyObject *self, PyObject *args);
+static PyObject *doki_registry_prob (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_registry_density (PyObject *self, PyObject *args);
+static PyObject *doki_registry_density (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_get (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_create (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_add (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_identity (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_sub (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_densityzero (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_scalar_mul (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_statezero (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_scalar_div (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_hadamard (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_matmul (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_addcontrol (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_ewmul (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_get (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_kron (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_add (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_transpose (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_sub (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_dagger (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_scalar_mul (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_shape (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_scalar_div (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_partialtrace (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_matmul (PyObject *self, PyObject *args);
 
-static PyObject *
-doki_funmatrix_trace (PyObject *self, PyObject *args);
+static PyObject *doki_funmatrix_ewmul (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_kron (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_eyekron (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_transpose (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_dagger (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_projection (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_shape (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_partialtrace (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_trace (PyObject *self, PyObject *args);
+
+static PyObject *doki_funmatrix_apply (PyObject *self, PyObject *args);
 
 static PyMethodDef DokiMethods[] = {
-    {"gate_new", doki_gate_new, METH_VARARGS, "Create new gate"},
-    {"gate_get", doki_gate_get, METH_VARARGS, "Get matrix associated to gate"},
-    {"registry_new", doki_registry_new, METH_VARARGS, "Create new registry"},
-    {"registry_new_data", doki_registry_new_data, METH_VARARGS, "Create new registry initialized with the specified values"},
-    {"registry_clone", doki_registry_clone, METH_VARARGS, "Clone a registry"},
-    {"registry_del", doki_registry_del, METH_VARARGS, "Destroy a registry"},
-    {"registry_get", doki_registry_get, METH_VARARGS, "Get value from registry"},
-    {"registry_apply", doki_registry_apply, METH_VARARGS, "Apply a gate"},
-    {"registry_join", doki_registry_join, METH_VARARGS, "Merges two registries"},
-    {"registry_measure", doki_registry_measure, METH_VARARGS, "Measures and collapses specified qubits"},
-    {"registry_prob", doki_registry_prob, METH_VARARGS, "Get the chances of obtaining 1 when measuring a certain qubit"},
-    {"registry_density", doki_registry_density, METH_VARARGS, "Get the density matrix"},
-    {"funmatrix_get", doki_funmatrix_get, METH_VARARGS, "Get a value from a functional matrix"},
-    {"funmatrix_add", doki_funmatrix_add, METH_VARARGS, "Get the addition of two functional matrices"},
-    {"funmatrix_sub", doki_funmatrix_sub, METH_VARARGS, "Get the substraction of two functional matrices"},
-    {"funmatrix_scalar_mul", doki_funmatrix_scalar_mul, METH_VARARGS, "Get the product of a scalar and a functional matrix"},
-    {"funmatrix_scalar_div", doki_funmatrix_scalar_div, METH_VARARGS, "Get the division of a functional matrix by a scalar"},
-    {"funmatrix_matmul", doki_funmatrix_matmul, METH_VARARGS, "Get the matrix product of two functional matrices"},
-    {"funmatrix_ewmul", doki_funmatrix_ewmul, METH_VARARGS, "Get the entity-wise multiplication of two functional matrices"},
-    {"funmatrix_kron", doki_funmatrix_kron, METH_VARARGS, "Get the Kronecker product of two functional matrices"},
-    {"funmatrix_transpose", doki_funmatrix_transpose, METH_VARARGS, "Get the transpose of a functional matrix"},
-    {"funmatrix_dagger", doki_funmatrix_dagger, METH_VARARGS, "Get the conjugate-transpose of a functional matrix"},
-    {"funmatrix_shape", doki_funmatrix_shape, METH_VARARGS, "Get a tuple with the shape of the matrix"},
-    {"funmatrix_partialtrace", doki_funmatrix_partialtrace, METH_VARARGS, "Get the partial trace of a functional matrix"},
-    {"funmatrix_trace", doki_funmatrix_trace, METH_VARARGS, "Get the trace of a functional matrix"},
-    {NULL, NULL, 0, NULL}        /* Sentinel */
+  { "gate_new", doki_gate_new, METH_VARARGS, "Create new gate" },
+  { "gate_get", doki_gate_get, METH_VARARGS, "Get matrix associated to gate" },
+  { "registry_new", doki_registry_new, METH_VARARGS, "Create new registry" },
+  { "registry_new_data", doki_registry_new_data, METH_VARARGS,
+    "Create new registry initialized with the specified values" },
+  { "registry_clone", doki_registry_clone, METH_VARARGS, "Clone a registry" },
+  { "registry_del", doki_registry_del, METH_VARARGS, "Destroy a registry" },
+  { "registry_get", doki_registry_get, METH_VARARGS,
+    "Get value from registry" },
+  { "registry_apply", doki_registry_apply, METH_VARARGS, "Apply a gate" },
+  { "registry_join", doki_registry_join, METH_VARARGS,
+    "Merges two registries" },
+  { "registry_measure", doki_registry_measure, METH_VARARGS,
+    "Measures and collapses specified qubits" },
+  { "registry_prob", doki_registry_prob, METH_VARARGS,
+    "Get the chances of obtaining 1 when measuring a certain qubit" },
+  { "registry_density", doki_registry_density, METH_VARARGS,
+    "Get the density matrix" },
+  { "funmatrix_create", doki_funmatrix_create, METH_VARARGS,
+    "Create a functional matrix from a matrix" },
+  { "funmatrix_identity", doki_funmatrix_identity, METH_VARARGS,
+    "Create an identity functional matrix of the specified number "
+    "of qubits" },
+  { "funmatrix_statezero", doki_funmatrix_statezero, METH_VARARGS,
+    "Create a functional matrix representing the state vector of "
+    "a quantum system of n qubits at state zero" },
+  { "funmatrix_densityzero", doki_funmatrix_densityzero, METH_VARARGS,
+    "Create a functional matrix representing the density matrix of "
+    "a quantum system of n qubits at state zero" },
+  { "funmatrix_hadamard", doki_funmatrix_hadamard, METH_VARARGS,
+    "Create a functional matrix from a Hadamard gate of the specified number "
+    "of qubits" },
+  { "funmatrix_addcontrol", doki_funmatrix_addcontrol, METH_VARARGS,
+    "Takes a gate as an input and returns the same gate with a control "
+    "qubit" },
+  { "funmatrix_get", doki_funmatrix_get, METH_VARARGS,
+    "Get a value from a functional matrix" },
+  { "funmatrix_add", doki_funmatrix_add, METH_VARARGS,
+    "Get the addition of two functional matrices" },
+  { "funmatrix_sub", doki_funmatrix_sub, METH_VARARGS,
+    "Get the substraction of two functional matrices" },
+  { "funmatrix_scalar_mul", doki_funmatrix_scalar_mul, METH_VARARGS,
+    "Get the product of a scalar and a functional matrix" },
+  { "funmatrix_scalar_div", doki_funmatrix_scalar_div, METH_VARARGS,
+    "Get the division of a functional matrix by a scalar" },
+  { "funmatrix_matmul", doki_funmatrix_matmul, METH_VARARGS,
+    "Get the matrix product of two functional matrices" },
+  { "funmatrix_ewmul", doki_funmatrix_ewmul, METH_VARARGS,
+    "Get the entity-wise multiplication of two functional matrices" },
+  { "funmatrix_kron", doki_funmatrix_kron, METH_VARARGS,
+    "Get the Kronecker product of two functional matrices" },
+  { "funmatrix_eyekron", doki_funmatrix_eyekron, METH_VARARGS,
+    "Get the Kronecker product of I(2^left), U and I(2^right)" },
+  { "funmatrix_transpose", doki_funmatrix_transpose, METH_VARARGS,
+    "Get the transpose of a functional matrix" },
+  { "funmatrix_dagger", doki_funmatrix_dagger, METH_VARARGS,
+    "Get the conjugate-transpose of a functional matrix" },
+  { "funmatrix_projection", doki_funmatrix_projection, METH_VARARGS,
+    "Get the result of a projection over a column vector" },
+  { "funmatrix_shape", doki_funmatrix_shape, METH_VARARGS,
+    "Get a tuple with the shape of the matrix" },
+  { "funmatrix_partialtrace", doki_funmatrix_partialtrace, METH_VARARGS,
+    "Get the partial trace of a functional matrix" },
+  { "funmatrix_trace", doki_funmatrix_trace, METH_VARARGS,
+    "Get the trace of a functional matrix" },
+  { "funmatrix_apply", doki_funmatrix_apply, METH_VARARGS,
+    "Get the resulting functional matrix after applying a gate to a state "
+    "vector" },
+  { NULL, NULL, 0, NULL } /* Sentinel */
 };
 
-static struct PyModuleDef dokimodule = {
-    PyModuleDef_HEAD_INIT,
-    "doki",   /* name of module */
-    NULL, /* module documentation, may be NULL */
-    -1,       /* size of per-interpreter state of the module,
-                 or -1 if the module keeps state in global variables. */
-    DokiMethods
-};
+static struct PyModuleDef dokimodule
+    = { PyModuleDef_HEAD_INIT, "doki", /* name of module */
+        NULL,                          /* module documentation, may be NULL */
+        -1, /* size of per-interpreter state of the module,
+               or -1 if the module keeps state in global variables. */
+        DokiMethods };
 
 PyMODINIT_FUNC
-PyInit_doki(void)
+PyInit_doki (void)
 {
-    PyObject *m;
+  PyObject *m;
 
-    assert(!PyErr_Occurred());
-    import_array(); // Initialise Numpy
-    m = PyModule_Create(&dokimodule);
-    if (m == NULL)
-        return NULL;
-
-    DokiError = PyErr_NewException("qsimov.doki.error", NULL, NULL);
-    Py_XINCREF(DokiError);
-    if (PyModule_AddObject(m, "error", DokiError) < 0) {
-        Py_XDECREF(DokiError);
-        Py_CLEAR(DokiError);
-        Py_DECREF(m);
-        return NULL;
+  assert (!PyErr_Occurred ());
+  import_array (); // Initialise Numpy
+  m = PyModule_Create (&dokimodule);
+  if (m == NULL)
+    return NULL;
+
+  DokiError = PyErr_NewException ("qsimov.doki.error", NULL, NULL);
+  Py_XINCREF (DokiError);
+  if (PyModule_AddObject (m, "error", DokiError) < 0)
+    {
+      Py_XDECREF (DokiError);
+      Py_CLEAR (DokiError);
+      Py_DECREF (m);
+      return NULL;
     }
 
-    return m;
+  return m;
 }
 
 int
-main(int argc, char *argv[])
+main (int argc, char *argv[])
 {
-    wchar_t *program = Py_DecodeLocale(argv[0], NULL);
-    if (program == NULL) {
-        fprintf(stderr, "Fatal error: cannot decode argv[0]\n");
-        exit(1);
+  wchar_t *program = Py_DecodeLocale (argv[0], NULL);
+  if (program == NULL)
+    {
+      fprintf (stderr, "Fatal error: cannot decode argv[0]\n");
+      exit (1);
     }
 
-    /* Add a built-in module, before Py_Initialize */
-    if (PyImport_AppendInittab("doki", PyInit_doki) == -1) {
-        fprintf(stderr, "Error: could not extend in-built modules table\n");
-        exit(1);
+  /* Add a built-in module, before Py_Initialize */
+  if (PyImport_AppendInittab ("doki", PyInit_doki) == -1)
+    {
+      fprintf (stderr, "Error: could not extend in-built modules table\n");
+      exit (1);
     }
 
-    /* Pass argv[0] to the Python interpreter */
-    Py_SetProgramName(program);
+  /* Pass argv[0] to the Python interpreter */
+  Py_SetProgramName (program);
 
-    /* Initialize the Python interpreter.  Required.
-       If this step fails, it will be a fatal error. */
-    Py_Initialize();
-
-    /* Optionally import the module; alternatively,
-       import can be deferred until the embedded script
-       imports it. */
-    PyObject *pmodule = PyImport_ImportModule("doki");
-    if (!pmodule) {
-        PyErr_Print();
-        fprintf(stderr, "Error: could not import module 'doki'\n");
+  /* Initialize the Python interpreter.  Required.
+     If this step fails, it will be a fatal error. */
+  Py_Initialize ();
+
+  /* Optionally import the module; alternatively,
+     import can be deferred until the embedded script
+     imports it. */
+  PyObject *pmodule = PyImport_ImportModule ("doki");
+  if (!pmodule)
+    {
+      PyErr_Print ();
+      fprintf (stderr, "Error: could not import module 'doki'\n");
     }
-    PyMem_RawFree(program);
-    return 0;
+  PyMem_RawFree (program);
+  return 0;
 }
 
 void
 doki_registry_destroy (PyObject *capsule)
 {
-    struct state_vector *state;
-    void *raw_state;
-    raw_state = PyCapsule_GetPointer(capsule, "qsimov.doki.state_vector");
-
-    if (raw_state != NULL) {
-        state = (struct state_vector*) raw_state;
-        state_clear(state);
-        free(state);
+  struct state_vector *state;
+  void *raw_state;
+  raw_state = PyCapsule_GetPointer (capsule, "qsimov.doki.state_vector");
+
+  if (raw_state != NULL)
+    {
+      state = (struct state_vector *)raw_state;
+      state_clear (state);
+      free (state);
     }
 }
 
 void
 doki_gate_destroy (PyObject *capsule)
 {
-    struct qgate *gate;
-    void *raw_gate;
-    NATURAL_TYPE i;
+  struct qgate *gate;
+  void *raw_gate;
+  NATURAL_TYPE i;
 
-    raw_gate = PyCapsule_GetPointer(capsule, "qsimov.doki.gate");
+  raw_gate = PyCapsule_GetPointer (capsule, "qsimov.doki.gate");
 
-    if (raw_gate != NULL) {
-        gate = (struct qgate*) raw_gate;
+  if (raw_gate != NULL)
+    {
+      gate = (struct qgate *)raw_gate;
 
-        for (i = 0; i < gate->size; i++) {
-            free(gate->matrix[i]);
+      for (i = 0; i < gate->size; i++)
+        {
+          free (gate->matrix[i]);
         }
-        free(gate->matrix);
-        free(gate);
+      free (gate->matrix);
+      free (gate);
     }
 }
 
 void
 doki_funmatrix_destroy (PyObject *capsule)
 {
-    FunctionalMatrix *matrix;
-    void *raw_matrix;
+  struct FMatrix *matrix;
+  void *raw_matrix;
 
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix != NULL) {
-        matrix = (FunctionalMatrix*) raw_matrix;
-        free(matrix);
+  raw_matrix = PyCapsule_GetPointer (capsule, "qsimov.doki.funmatrix");
+  if (raw_matrix != NULL)
+    {
+      matrix = (struct FMatrix *)raw_matrix;
+      FM_destroy (matrix);
     }
 }
 
 static PyObject *
 doki_registry_new (PyObject *self, PyObject *args)
 {
-    unsigned int num_qubits;
-    unsigned char result;
-    struct state_vector *state;
-    int debug_enabled;
-
-    if (!PyArg_ParseTuple(args, "Ip", &num_qubits, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_new(num_qubits, verbose)");
-        return NULL;
-    }
-    if (num_qubits == 0) {
-        PyErr_SetString(DokiError, "num_qubits can't be zero");
-        return NULL;
-    }
-
-    state = MALLOC_TYPE(1, struct state_vector);
-    if (state == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate state structure");
-        return NULL;
-    }
-    result = state_init(state, num_qubits, 1);
-    if (result == 1) {
-        PyErr_SetString(DokiError, "Failed to allocate state vector");
-        return NULL;
-    }
-    else if (result == 2) {
-        PyErr_SetString(DokiError, "Failed to allocate state chunk");
-        return NULL;
-    }
-    else if (result == 3) {
-        PyErr_SetString(DokiError, "Number of qubits exceeds maximum");
-        return NULL;
-    }
-    else if (result != 0) {
-        PyErr_SetString(DokiError, "Unknown error when creating state");
-        return NULL;
+  unsigned int num_qubits;
+  unsigned char result;
+  struct state_vector *state;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "Ip", &num_qubits, &debug_enabled))
+    {
+      PyErr_SetString (DokiError, "Syntax: registry_new(num_qubits, verbose)");
+      return NULL;
+    }
+  if (num_qubits == 0)
+    {
+      PyErr_SetString (DokiError, "num_qubits can't be zero");
+      return NULL;
+    }
+
+  state = MALLOC_TYPE (1, struct state_vector);
+  if (state == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state structure");
+      return NULL;
+    }
+  result = state_init (state, num_qubits, 1);
+  if (result == 1)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state vector");
+      return NULL;
     }
-    return PyCapsule_New((void*) state, "qsimov.doki.state_vector",
-                         &doki_registry_destroy);
+  else if (result == 2)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state chunk");
+      return NULL;
+    }
+  else if (result == 3)
+    {
+      PyErr_SetString (DokiError, "Number of qubits exceeds maximum");
+      return NULL;
+    }
+  else if (result != 0)
+    {
+      PyErr_SetString (DokiError, "Unknown error when creating state");
+      return NULL;
+    }
+  return PyCapsule_New ((void *)state, "qsimov.doki.state_vector",
+                        &doki_registry_destroy);
 }
 
 static PyObject *
 doki_registry_clone (PyObject *self, PyObject *args)
 {
-    PyObject *source_capsule;
-    unsigned char result;
-    void *raw_source;
-    struct state_vector *source, *dest;
-    int num_threads, debug_enabled;
+  PyObject *source_capsule;
+  unsigned char result;
+  void *raw_source;
+  struct state_vector *source, *dest;
+  int num_threads, debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "Oip", &source_capsule,
-                          &num_threads, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_clone(registry, num_threads, verbose)");
-        return NULL;
+  if (!PyArg_ParseTuple (args, "Oip", &source_capsule, &num_threads,
+                         &debug_enabled))
+    {
+      PyErr_SetString (
+          DokiError, "Syntax: registry_clone(registry, num_threads, verbose)");
+      return NULL;
     }
 
-    if (num_threads <= 0 && num_threads != -1) {
-        PyErr_SetString(DokiError, "num_threads must be at least 1 (or -1 to let OpenMP choose)");
-        return NULL;
+  if (num_threads <= 0 && num_threads != -1)
+    {
+      PyErr_SetString (
+          DokiError,
+          "num_threads must be at least 1 (or -1 to let OpenMP choose)");
+      return NULL;
     }
 
-    raw_source = PyCapsule_GetPointer(source_capsule, "qsimov.doki.state_vector");
-    if (raw_source == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to source registry");
-        return NULL;
+  raw_source
+      = PyCapsule_GetPointer (source_capsule, "qsimov.doki.state_vector");
+  if (raw_source == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to source registry");
+      return NULL;
     }
-    source = (struct state_vector*) raw_source;
+  source = (struct state_vector *)raw_source;
 
-    dest = MALLOC_TYPE(1, struct state_vector);
-    if (dest == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate new state structure");
-        return NULL;
+  dest = MALLOC_TYPE (1, struct state_vector);
+  if (dest == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate new state structure");
+      return NULL;
     }
 
-    if (num_threads != -1) {
-        omp_set_num_threads(num_threads);
+  if (num_threads != -1)
+    {
+      omp_set_num_threads (num_threads);
     }
 
-    result = state_clone(dest, source);
-    if (result == 1) {
-        PyErr_SetString(DokiError, "Failed to allocate state vector");
-        return NULL;
+  result = state_clone (dest, source);
+  if (result == 1)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state vector");
+      return NULL;
     }
-    else if (result == 2) {
-        PyErr_SetString(DokiError, "Failed to allocate state chunk");
-        return NULL;
+  else if (result == 2)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state chunk");
+      return NULL;
     }
-    else if (result != 0) {
-        PyErr_SetString(DokiError, "Unknown error when cloning state");
-        return NULL;
+  else if (result != 0)
+    {
+      PyErr_SetString (DokiError, "Unknown error when cloning state");
+      return NULL;
     }
-    return PyCapsule_New((void*) dest, "qsimov.doki.state_vector",
-                         &doki_registry_destroy);
+  return PyCapsule_New ((void *)dest, "qsimov.doki.state_vector",
+                        &doki_registry_destroy);
 }
 
 static PyObject *
 doki_registry_del (PyObject *self, PyObject *args)
 {
-    PyObject *capsule;
-    int debug_enabled;
+  PyObject *capsule;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "Op", &capsule, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_del(registry, verbose)");
-        return NULL;
+  if (!PyArg_ParseTuple (args, "Op", &capsule, &debug_enabled))
+    {
+      PyErr_SetString (DokiError, "Syntax: registry_del(registry, verbose)");
+      return NULL;
     }
 
-    doki_registry_destroy(capsule);
-    PyCapsule_SetDestructor(capsule, NULL);
+  doki_registry_destroy (capsule);
+  PyCapsule_SetDestructor (capsule, NULL);
 
-    Py_RETURN_NONE;
+  Py_RETURN_NONE;
 }
 
 static PyObject *
 doki_gate_new (PyObject *self, PyObject *args)
 {
-    PyObject *list, *row, *raw_val;
-    unsigned int num_qubits;
-    NATURAL_TYPE i, j, k;
-    COMPLEX_TYPE val;
-    struct qgate *gate;
-    int debug_enabled;
-
-    if (!PyArg_ParseTuple(args, "IOp", &num_qubits, &list, &debug_enabled))
-    {
-        PyErr_SetString(DokiError, "Syntax: gate_new(num_qubits, gate, verbose)");
-        return NULL;
-    }
-    if (num_qubits == 0) {
-        PyErr_SetString(DokiError, "num_qubits can't be zero");
-        return NULL;
-    }
-    if (!PyList_Check(list)) {
-        PyErr_SetString(DokiError, "gate must be a list of lists (matrix)");
-        return NULL;
-    }
-
-    gate = MALLOC_TYPE(1, struct qgate);
-    if (gate == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate qgate");
-        return NULL;
-    }
-
-    gate->num_qubits = num_qubits;
-    gate->size = NATURAL_ONE << num_qubits;
-    if ((NATURAL_TYPE) PyList_Size(list) != gate->size) {
-        PyErr_SetString(DokiError, "Wrong matrix size for specified number of qubits");
-        free(gate);
-        return NULL;
-    }
-
-    gate->matrix = MALLOC_TYPE(gate->size, COMPLEX_TYPE*);
-    if (gate->matrix == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate qgate matrix");
-        free(gate);
-        return NULL;
-    }
-
-    for (i = 0; i < gate->size; i++) {
-        row = PyList_GetItem(list, i);
-        if (!PyList_Check(row) || (NATURAL_TYPE) PyList_Size(row) != gate->size) {
-            PyErr_SetString(DokiError, "rows must be lists of size 2^num_qubits");
-            for (k = 0; k < i; k++) {
-                free(gate->matrix[k]);
-            }
-            free(gate->matrix);
-            free(gate);
-            return NULL;
-        }
-        gate->matrix[i] = MALLOC_TYPE(gate->size, COMPLEX_TYPE);
-        for (j = 0; j < gate->size; j++) {
-            raw_val = PyList_GetItem(row, j);
-            if (PyComplex_Check(raw_val)) {
-                val = complex_init(PyComplex_RealAsDouble(raw_val), PyComplex_ImagAsDouble(raw_val));
-            }
-            else if(PyFloat_Check(raw_val)) {
-                val = complex_init(PyFloat_AsDouble(raw_val), 0.0);
-            }
-            else if(PyLong_Check(raw_val)) {
-                val = complex_init((double) PyLong_AsLong(raw_val), 0.0);
-            }
-            else {
-                PyErr_SetString(DokiError, "matrix elements must be complex numbers");
-                for (k = 0; k <= i; k++) {
-                    free(gate->matrix[k]);
+  PyObject *list, *row, *raw_val;
+  unsigned int num_qubits;
+  NATURAL_TYPE i, j, k;
+  COMPLEX_TYPE val;
+  struct qgate *gate;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "IOp", &num_qubits, &list, &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: gate_new(num_qubits, gate, verbose)");
+      return NULL;
+    }
+  if (num_qubits == 0)
+    {
+      PyErr_SetString (DokiError, "num_qubits can't be zero");
+      return NULL;
+    }
+  if (!PyList_Check (list))
+    {
+      PyErr_SetString (DokiError, "gate must be a list of lists (matrix)");
+      return NULL;
+    }
+
+  gate = MALLOC_TYPE (1, struct qgate);
+  if (gate == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate qgate");
+      return NULL;
+    }
+
+  gate->num_qubits = num_qubits;
+  gate->size = NATURAL_ONE << num_qubits;
+  if ((NATURAL_TYPE)PyList_Size (list) != gate->size)
+    {
+      PyErr_SetString (DokiError,
+                       "Wrong matrix size for specified number of qubits");
+      free (gate);
+      return NULL;
+    }
+
+  gate->matrix = MALLOC_TYPE (gate->size, COMPLEX_TYPE *);
+  if (gate->matrix == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate qgate matrix");
+      free (gate);
+      return NULL;
+    }
+
+  for (i = 0; i < gate->size; i++)
+    {
+      row = PyList_GetItem (list, i);
+      if (!PyList_Check (row) || (NATURAL_TYPE)PyList_Size (row) != gate->size)
+        {
+          PyErr_SetString (DokiError,
+                           "rows must be lists of size 2^num_qubits");
+          for (k = 0; k < i; k++)
+            {
+              free (gate->matrix[k]);
+            }
+          free (gate->matrix);
+          free (gate);
+          return NULL;
+        }
+      gate->matrix[i] = MALLOC_TYPE (gate->size, COMPLEX_TYPE);
+      for (j = 0; j < gate->size; j++)
+        {
+          raw_val = PyList_GetItem (row, j);
+          if (PyComplex_Check (raw_val))
+            {
+              val = COMPLEX_INIT (PyComplex_RealAsDouble (raw_val),
+                                  PyComplex_ImagAsDouble (raw_val));
+            }
+          else if (PyFloat_Check (raw_val))
+            {
+              val = COMPLEX_INIT (PyFloat_AsDouble (raw_val), 0.0);
+            }
+          else if (PyLong_Check (raw_val))
+            {
+              val = COMPLEX_INIT ((double)PyLong_AsLong (raw_val), 0.0);
+            }
+          else
+            {
+              PyErr_SetString (DokiError,
+                               "matrix elements must be complex numbers");
+              for (k = 0; k <= i; k++)
+                {
+                  free (gate->matrix[k]);
                 }
-                free(gate->matrix);
-                free(gate);
-                return NULL;
+              free (gate->matrix);
+              free (gate);
+              return NULL;
             }
-            gate->matrix[i][j] = val;
+          gate->matrix[i][j] = val;
         }
     }
 
-    return PyCapsule_New((void*) gate, "qsimov.doki.gate", &doki_gate_destroy);
+  return PyCapsule_New ((void *)gate, "qsimov.doki.gate", &doki_gate_destroy);
 }
 
-
 static PyObject *
 doki_gate_get (PyObject *self, PyObject *args)
 {
-    PyObject *capsule, *result, *aux;
-    COMPLEX_TYPE val;
-    NATURAL_TYPE i, j;
-    void *raw_gate;
-    struct qgate *gate;
-    int debug_enabled;
+  PyObject *capsule, *result, *aux;
+  COMPLEX_TYPE val;
+  NATURAL_TYPE i, j;
+  void *raw_gate;
+  struct qgate *gate;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "Op", &capsule, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "Op", &capsule, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: gate_get(gate, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError, "Syntax: gate_get(gate, verbose)");
+      return NULL;
     }
 
-    raw_gate = PyCapsule_GetPointer(capsule, "qsimov.doki.gate");
-    if (raw_gate == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to gate");
-        return NULL;
+  raw_gate = PyCapsule_GetPointer (capsule, "qsimov.doki.gate");
+  if (raw_gate == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to gate");
+      return NULL;
     }
-    gate = (struct qgate*) raw_gate;
-    result = PyList_New(gate->size);
-    for (i = 0; i < gate->size; i++) {
-        aux = PyList_New(gate->size);
-        for (j = 0; j < gate->size; j++) {
-            val = gate->matrix[i][j];
-            PyList_SET_ITEM(aux, j, PyComplex_FromDoubles(RE(val), IM(val)));
+  gate = (struct qgate *)raw_gate;
+  result = PyList_New (gate->size);
+  for (i = 0; i < gate->size; i++)
+    {
+      aux = PyList_New (gate->size);
+      for (j = 0; j < gate->size; j++)
+        {
+          val = gate->matrix[i][j];
+          PyList_SET_ITEM (aux, j, PyComplex_FromDoubles (RE (val), IM (val)));
         }
-        PyList_SET_ITEM(result, i, aux);
+      PyList_SET_ITEM (result, i, aux);
     }
 
-    return result;
+  return result;
 }
 
 static PyObject *
 doki_registry_get (PyObject *self, PyObject *args)
 {
-    PyObject *capsule, *result;
-    void *raw_state;
-    struct state_vector *state;
-    NATURAL_TYPE id;
-    COMPLEX_TYPE val, aux;
-    REAL_TYPE phase;
-    int canonical, debug_enabled;
-
-    if (!PyArg_ParseTuple(args, "OKpp", &capsule, &id, &canonical, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_get(registry, id, canonical, verbose)");
-        return NULL;
-    }
-
-    raw_state = PyCapsule_GetPointer(capsule, "qsimov.doki.state_vector");
-    if (raw_state == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to registry");
-        return NULL;
-    }
-    state = (struct state_vector*) raw_state;
-    val = state_get(state, id);
-    if (debug_enabled) {
-        printf("[DEBUG] raw = " COMPLEX_STRING_FORMAT "\n", COMPLEX_STRING(state->vector[id/COMPLEX_ARRAY_SIZE][id%COMPLEX_ARRAY_SIZE]));
-        printf("[DEBUG] normconst = %lf\n", state->norm_const);
-        printf("[DEBUG] res = " COMPLEX_STRING_FORMAT "\n", COMPLEX_STRING(val));
-    }
-    if (canonical) {
-        phase = get_global_phase(state);
-        if (debug_enabled) {
-            printf("[DEBUG] phase = " REAL_STRING_FORMAT "\n", phase);
+  PyObject *capsule, *result;
+  void *raw_state;
+  struct state_vector *state;
+  NATURAL_TYPE id;
+  COMPLEX_TYPE val, aux;
+  REAL_TYPE phase;
+  int canonical, debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OKpp", &capsule, &id, &canonical,
+                         &debug_enabled))
+    {
+      PyErr_SetString (
+          DokiError, "Syntax: registry_get(registry, id, canonical, verbose)");
+      return NULL;
+    }
+
+  raw_state = PyCapsule_GetPointer (capsule, "qsimov.doki.state_vector");
+  if (raw_state == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry");
+      return NULL;
+    }
+  state = (struct state_vector *)raw_state;
+  val = state_get (state, id);
+  if (debug_enabled)
+    {
+      printf ("[DEBUG] raw = " COMPLEX_STRING_FORMAT "\n",
+              COMPLEX_STRING (state->vector[id / COMPLEX_ARRAY_SIZE]
+                                           [id % COMPLEX_ARRAY_SIZE]));
+      printf ("[DEBUG] normconst = %lf\n", state->norm_const);
+      printf ("[DEBUG] res = " COMPLEX_STRING_FORMAT "\n",
+              COMPLEX_STRING (val));
+    }
+  if (canonical)
+    {
+      phase = get_global_phase (state);
+      if (debug_enabled)
+        {
+          printf ("[DEBUG] phase = " REAL_STRING_FORMAT "\n", phase);
         }
-        aux = complex_init(COS(phase), -SIN(phase));
-        val = complex_mult(val, aux);
+      aux = COMPLEX_INIT (COS (phase), -SIN (phase));
+      val = COMPLEX_MULT (val, aux);
     }
-    result = PyComplex_FromDoubles(RE(val), IM(val));
+  result = PyComplex_FromDoubles (RE (val), IM (val));
 
-    return result;
+  return result;
 }
 
 void
-custom_state_init_py(PyObject *values, struct state_vector *state)
+custom_state_init_py (PyObject *values, struct state_vector *state)
 {
-    NATURAL_TYPE i;
-    COMPLEX_TYPE val;
-    PyObject *aux;
-
-    for (i = 0; i < state->size; i++) {
-        aux = PyList_GetItem(values, i);
-        val = complex_init(PyComplex_RealAsDouble(aux), PyComplex_ImagAsDouble(aux));
-        state_set(state, i, val);
+  NATURAL_TYPE i;
+  COMPLEX_TYPE val;
+  PyObject *aux;
+
+  for (i = 0; i < state->size; i++)
+    {
+      aux = PyList_GetItem (values, i);
+      val = COMPLEX_INIT (PyComplex_RealAsDouble (aux),
+                          PyComplex_ImagAsDouble (aux));
+      state_set (state, i, val);
     }
 }
 
 void
-custom_state_init_np(PyObject *values, struct state_vector *state)
+custom_state_init_np (PyObject *values, struct state_vector *state)
 {
-    NATURAL_TYPE i;
-    COMPLEX_TYPE val;
-    PyObject *aux;
-
-    for (i = 0; i < state->size; i++) {
-        aux = PyArray_GETITEM(values, PyArray_GETPTR1(values, i));
-        val = complex_init(PyComplex_RealAsDouble(aux), PyComplex_ImagAsDouble(aux));
-        state_set(state, i, val);
+  NATURAL_TYPE i;
+  COMPLEX_TYPE val;
+  PyObject *aux;
+
+  for (i = 0; i < state->size; i++)
+    {
+      aux = PyArray_GETITEM (values, PyArray_GETPTR1 (values, i));
+      val = COMPLEX_INIT (PyComplex_RealAsDouble (aux),
+                          PyComplex_ImagAsDouble (aux));
+      state_set (state, i, val);
     }
 }
 
 static PyObject *
 doki_registry_new_data (PyObject *self, PyObject *args)
 {
-    PyObject *raw_vals;
-    unsigned int num_qubits;
-    unsigned char result;
-    struct state_vector *state;
-    short debug_enabled;
+  PyObject *raw_vals;
+  unsigned int num_qubits;
+  unsigned char result;
+  struct state_vector *state;
+  short debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "IOh", &num_qubits, &raw_vals, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_new_data(num_qubits, values, verbose)");
-        return NULL;
+  if (!PyArg_ParseTuple (args, "IOh", &num_qubits, &raw_vals, &debug_enabled))
+    {
+      PyErr_SetString (
+          DokiError, "Syntax: registry_new_data(num_qubits, values, verbose)");
+      return NULL;
     }
-    if (num_qubits == 0) {
-        PyErr_SetString(DokiError, "num_qubits can't be zero");
-        return NULL;
+  if (num_qubits == 0)
+    {
+      PyErr_SetString (DokiError, "num_qubits can't be zero");
+      return NULL;
     }
-    if (debug_enabled) {
-        printf("[DEBUG] State allocation\n");
+  if (debug_enabled)
+    {
+      printf ("[DEBUG] State allocation\n");
     }
-    state = MALLOC_TYPE(1, struct state_vector);
-    if (state == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate state structure");
-        return NULL;
+  state = MALLOC_TYPE (1, struct state_vector);
+  if (state == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state structure");
+      return NULL;
     }
-    if (debug_enabled) {
-        printf("[DEBUG] State initialization\n");
+  if (debug_enabled)
+    {
+      printf ("[DEBUG] State initialization\n");
     }
-    result = state_init(state, num_qubits, 0);
-    if (result == 1) {
-        PyErr_SetString(DokiError, "Failed to allocate state vector");
-        return NULL;
+  result = state_init (state, num_qubits, 0);
+  if (result == 1)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state vector");
+      return NULL;
     }
-    else if (result == 2) {
-        PyErr_SetString(DokiError, "Failed to allocate state chunk");
-        return NULL;
+  else if (result == 2)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state chunk");
+      return NULL;
     }
-    else if (result == 3) {
-        PyErr_SetString(DokiError, "Number of qubits exceeds maximum");
-        return NULL;
+  else if (result == 3)
+    {
+      PyErr_SetString (DokiError, "Number of qubits exceeds maximum");
+      return NULL;
     }
-    else if (result != 0) {
-        PyErr_SetString(DokiError, "Unknown error when creating state");
-        return NULL;
+  else if (result != 0)
+    {
+      PyErr_SetString (DokiError, "Unknown error when creating state");
+      return NULL;
     }
-    if (debug_enabled) {
-        printf("[DEBUG] Dumping data...\n");
+  if (debug_enabled)
+    {
+      printf ("[DEBUG] Dumping data...\n");
     }
-    if (PyArray_Check(raw_vals)) {
-        if (debug_enabled) {
-            printf("[DEBUG] Checking array type\n");
-        }
-        if (!PyArray_ISNUMBER(raw_vals)) {
-            PyErr_SetString(DokiError, "values have to be numbers");
-            return NULL;
-        }
-        if (debug_enabled) {
-            printf("[DEBUG] Checking array size\n");
-        }
-        if (PyArray_SIZE(raw_vals) != state->size) {
-            PyErr_SetString(DokiError, "Wrong array size for the specified number of qubits");
-            return NULL;
-        }
-        if (debug_enabled) {
-            printf("[DEBUG] Working with numpy array\n");
+  if (PyArray_Check (raw_vals))
+    {
+      if (debug_enabled)
+        {
+          printf ("[DEBUG] Checking array type\n");
+        }
+      if (!PyArray_ISNUMBER (raw_vals))
+        {
+          PyErr_SetString (DokiError, "values have to be numbers");
+          return NULL;
+        }
+      if (debug_enabled)
+        {
+          printf ("[DEBUG] Checking array size\n");
+        }
+      if (PyArray_SIZE (raw_vals) != state->size)
+        {
+          PyErr_SetString (
+              DokiError,
+              "Wrong array size for the specified number of qubits");
+          return NULL;
+        }
+      if (debug_enabled)
+        {
+          printf ("[DEBUG] Working with numpy array\n");
         }
-        custom_state_init_np(raw_vals, state);
+      custom_state_init_np (raw_vals, state);
     }
-    else if (PyList_Check(raw_vals)) {
-        if (debug_enabled) {
-            printf("[DEBUG] Checking list size\n");
-        }
-        if (PyList_GET_SIZE(raw_vals) != state->size) {
-            PyErr_SetString(DokiError, "Wrong list size for the specified number of qubits\n");
-            return NULL;
-        }
-        if (debug_enabled) {
-            printf("[DEBUG] Working with python list\n");
+  else if (PyList_Check (raw_vals))
+    {
+      if (debug_enabled)
+        {
+          printf ("[DEBUG] Checking list size\n");
+        }
+      if (PyList_GET_SIZE (raw_vals) != state->size)
+        {
+          PyErr_SetString (
+              DokiError,
+              "Wrong list size for the specified number of qubits\n");
+          return NULL;
+        }
+      if (debug_enabled)
+        {
+          printf ("[DEBUG] Working with python list\n");
         }
-        custom_state_init_py(raw_vals, state);
+      custom_state_init_py (raw_vals, state);
     }
-    else {
-        PyErr_SetString(DokiError, "values has to be either a python list or a numpy array");
-        return NULL;
+  else
+    {
+      PyErr_SetString (
+          DokiError, "values has to be either a python list or a numpy array");
+      return NULL;
     }
-    if (debug_enabled) {
-        printf("[DEBUG] Starting creation\n");
+  if (debug_enabled)
+    {
+      printf ("[DEBUG] Starting creation\n");
     }
 
-    return PyCapsule_New((void*) state, "qsimov.doki.state_vector",
-                         &doki_registry_destroy);
+  return PyCapsule_New ((void *)state, "qsimov.doki.state_vector",
+                        &doki_registry_destroy);
 }
 
 static PyObject *
 doki_registry_apply (PyObject *self, PyObject *args)
 {
-    PyObject *raw_val, *state_capsule, *gate_capsule,
-             *target_list, *control_set, *acontrol_set, *aux;
-    void *raw_state, *raw_gate;
-    struct state_vector *state, *new_state;
-    struct qgate *gate;
-    unsigned char exit_code;
-    unsigned int num_targets, num_controls, num_anticontrols, i;
-    unsigned int *targets, *controls, *anticontrols;
-    int num_threads, debug_enabled;
-
-    if (!PyArg_ParseTuple(args, "OOOOOip", &state_capsule, &gate_capsule,
-                          &target_list, &control_set, &acontrol_set, &num_threads, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_apply(registry, gate, target_list, control_set, anticontrol_set, num_threads, verbose)");
-        return NULL;
+  PyObject *raw_val, *state_capsule, *gate_capsule, *target_list, *control_set,
+      *acontrol_set, *aux;
+  void *raw_state, *raw_gate;
+  struct state_vector *state, *new_state;
+  struct qgate *gate;
+  unsigned char exit_code;
+  unsigned int num_targets, num_controls, num_anticontrols, i;
+  unsigned int *targets, *controls, *anticontrols;
+  int num_threads, debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OOOOOip", &state_capsule, &gate_capsule,
+                         &target_list, &control_set, &acontrol_set,
+                         &num_threads, &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: registry_apply(registry, gate, target_list, "
+                       "control_set, anticontrol_set, num_threads, verbose)");
+      return NULL;
     }
 
-    if (num_threads <= 0 && num_threads != -1) {
-        PyErr_SetString(DokiError, "num_threads must be at least 1 (or -1 to let OpenMP choose)");
-        return NULL;
+  if (num_threads <= 0 && num_threads != -1)
+    {
+      PyErr_SetString (
+          DokiError,
+          "num_threads must be at least 1 (or -1 to let OpenMP choose)");
+      return NULL;
     }
 
-    raw_state = PyCapsule_GetPointer(state_capsule, "qsimov.doki.state_vector");
-    if (raw_state == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to registry");
-        return NULL;
+  raw_state = PyCapsule_GetPointer (state_capsule, "qsimov.doki.state_vector");
+  if (raw_state == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry");
+      return NULL;
     }
-    state = (struct state_vector*) raw_state;
+  state = (struct state_vector *)raw_state;
 
-    raw_gate = PyCapsule_GetPointer(gate_capsule, "qsimov.doki.gate");
-    if (raw_gate == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to gate");
-        return NULL;
+  raw_gate = PyCapsule_GetPointer (gate_capsule, "qsimov.doki.gate");
+  if (raw_gate == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to gate");
+      return NULL;
     }
-    gate = (struct qgate*) raw_gate;
+  gate = (struct qgate *)raw_gate;
 
-    if (!PyList_Check(target_list)) {
-        PyErr_SetString(DokiError, "target_list must be a list");
-        return NULL;
+  if (!PyList_Check (target_list))
+    {
+      PyErr_SetString (DokiError, "target_list must be a list");
+      return NULL;
     }
 
-    num_targets = (unsigned int) PyList_Size(target_list);
-    if (num_targets != gate->num_qubits) {
-        PyErr_SetString(DokiError, "Wrong number of targets specified for that gate");
-        return NULL;
+  num_targets = (unsigned int)PyList_Size (target_list);
+  if (num_targets != gate->num_qubits)
+    {
+      PyErr_SetString (DokiError,
+                       "Wrong number of targets specified for that gate");
+      return NULL;
     }
 
-    num_controls = 0;
-    if (PySet_Check(control_set)) {
-        num_controls = (unsigned int) PySet_Size(control_set);
+  num_controls = 0;
+  if (PySet_Check (control_set))
+    {
+      num_controls = (unsigned int)PySet_Size (control_set);
     }
-    else if (control_set != Py_None) {
-        PyErr_SetString(DokiError, "control_set must be a set or None");
-        return NULL;
+  else if (control_set != Py_None)
+    {
+      PyErr_SetString (DokiError, "control_set must be a set or None");
+      return NULL;
     }
 
-    num_anticontrols = 0;
-    if (PySet_Check(acontrol_set)) {
-        num_anticontrols = (unsigned int) PySet_Size(acontrol_set);
+  num_anticontrols = 0;
+  if (PySet_Check (acontrol_set))
+    {
+      num_anticontrols = (unsigned int)PySet_Size (acontrol_set);
     }
-    else if (acontrol_set != Py_None) {
-        PyErr_SetString(DokiError, "anticontrol_set must be a set or None");
-        return NULL;
+  else if (acontrol_set != Py_None)
+    {
+      PyErr_SetString (DokiError, "anticontrol_set must be a set or None");
+      return NULL;
     }
 
-    targets = MALLOC_TYPE(num_targets, unsigned int);
-    if (targets == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate target array");
-        return NULL;
+  targets = MALLOC_TYPE (num_targets, unsigned int);
+  if (targets == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate target array");
+      return NULL;
     }
-    controls = NULL;
-    if (num_controls > 0) {
-        controls = MALLOC_TYPE(num_controls, unsigned int);
-        if (controls == NULL) {
-            PyErr_SetString(DokiError, "Failed to allocate control array");
-            return NULL;
+  controls = NULL;
+  if (num_controls > 0)
+    {
+      controls = MALLOC_TYPE (num_controls, unsigned int);
+      if (controls == NULL)
+        {
+          PyErr_SetString (DokiError, "Failed to allocate control array");
+          return NULL;
         }
     }
-    anticontrols = NULL;
-    if (num_anticontrols > 0) {
-        anticontrols = MALLOC_TYPE(num_anticontrols, unsigned int);
-        if (anticontrols == NULL) {
-            PyErr_SetString(DokiError, "Failed to allocate anticontrol array");
-            return NULL;
+  anticontrols = NULL;
+  if (num_anticontrols > 0)
+    {
+      anticontrols = MALLOC_TYPE (num_anticontrols, unsigned int);
+      if (anticontrols == NULL)
+        {
+          PyErr_SetString (DokiError, "Failed to allocate anticontrol array");
+          return NULL;
         }
     }
 
-    if (num_controls > 0) {
-        aux = PySet_New(control_set);
-        for (i = 0; i < num_controls; i++) {
-            raw_val = PySet_Pop(aux);
-            if(!PyLong_Check(raw_val)) {
-                PyErr_SetString(DokiError, "control_set must be a set qubit ids (unsigned integers)");
-                return NULL;
+  if (num_controls > 0)
+    {
+      aux = PySet_New (control_set);
+      for (i = 0; i < num_controls; i++)
+        {
+          raw_val = PySet_Pop (aux);
+          if (!PyLong_Check (raw_val))
+            {
+              PyErr_SetString (
+                  DokiError,
+                  "control_set must be a set qubit ids (unsigned integers)");
+              return NULL;
             }
-            controls[i] = PyLong_AsLong(raw_val);
-            if (controls[i] >= state->num_qubits) {
-                PyErr_SetString(DokiError, "Control qubit out of range");
-                return NULL;
+          controls[i] = PyLong_AsLong (raw_val);
+          if (controls[i] >= state->num_qubits)
+            {
+              PyErr_SetString (DokiError, "Control qubit out of range");
+              return NULL;
             }
         }
     }
 
-    if (num_anticontrols > 0) {
-        aux = PySet_New(acontrol_set);
-        for (i = 0; i < num_anticontrols; i++) {
-            raw_val = PySet_Pop(aux);
-            if(!PyLong_Check(raw_val)) {
-                PyErr_SetString(DokiError, "anticontrol_set must be a set qubit ids (unsigned integers)");
-                return NULL;
+  if (num_anticontrols > 0)
+    {
+      aux = PySet_New (acontrol_set);
+      for (i = 0; i < num_anticontrols; i++)
+        {
+          raw_val = PySet_Pop (aux);
+          if (!PyLong_Check (raw_val))
+            {
+              PyErr_SetString (DokiError, "anticontrol_set must be a set "
+                                          "qubit ids (unsigned integers)");
+              return NULL;
             }
-            if (PySet_Contains(control_set, raw_val)) {
-                PyErr_SetString(DokiError, "A control cannot also be an anticontrol");
-                return NULL;
+          if (PySet_Contains (control_set, raw_val))
+            {
+              PyErr_SetString (DokiError,
+                               "A control cannot also be an anticontrol");
+              return NULL;
             }
-            anticontrols[i] = PyLong_AsLong(raw_val);
-            if (anticontrols[i] >= state->num_qubits) {
-                PyErr_SetString(DokiError, "Anticontrol qubit out of range");
-                return NULL;
+          anticontrols[i] = PyLong_AsLong (raw_val);
+          if (anticontrols[i] >= state->num_qubits)
+            {
+              PyErr_SetString (DokiError, "Anticontrol qubit out of range");
+              return NULL;
             }
         }
     }
 
-    for (i = 0; i < num_targets; i++) {
-        raw_val = PyList_GetItem(target_list, i);
-        if(!PyLong_Check(raw_val)) {
-            PyErr_SetString(DokiError, "target_list must be a list of qubit ids (unsigned integers)");
-            return NULL;
-        }
-        if ((num_controls > 0 && PySet_Contains(control_set, raw_val)) || (num_anticontrols > 0 && PySet_Contains(acontrol_set, raw_val))) {
-            PyErr_SetString(DokiError, "A target cannot also be a control or an anticontrol");
-            return NULL;
-        }
-        targets[i] = PyLong_AsLong(raw_val);
-        if (targets[i] >= state->num_qubits) {
-            PyErr_SetString(DokiError, "Target qubit out of range");
-            return NULL;
+  for (i = 0; i < num_targets; i++)
+    {
+      raw_val = PyList_GetItem (target_list, i);
+      if (!PyLong_Check (raw_val))
+        {
+          PyErr_SetString (
+              DokiError,
+              "target_list must be a list of qubit ids (unsigned integers)");
+          return NULL;
+        }
+      if ((num_controls > 0 && PySet_Contains (control_set, raw_val))
+          || (num_anticontrols > 0 && PySet_Contains (acontrol_set, raw_val)))
+        {
+          PyErr_SetString (
+              DokiError,
+              "A target cannot also be a control or an anticontrol");
+          return NULL;
+        }
+      targets[i] = PyLong_AsLong (raw_val);
+      if (targets[i] >= state->num_qubits)
+        {
+          PyErr_SetString (DokiError, "Target qubit out of range");
+          return NULL;
         }
     }
 
-    new_state = MALLOC_TYPE(1, struct state_vector);
-    if (new_state == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate new state structure");
-        return NULL;
+  new_state = MALLOC_TYPE (1, struct state_vector);
+  if (new_state == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate new state structure");
+      return NULL;
     }
-    if (num_threads != -1) {
-        omp_set_num_threads(num_threads);
+  if (num_threads != -1)
+    {
+      omp_set_num_threads (num_threads);
     }
-    // printf("[DEBUG] nums: %u, %u, %u\n", num_targets, num_controls, num_anticontrols);
-    exit_code = apply_gate(state, gate, targets, num_targets, controls,
-                           num_controls, anticontrols, num_anticontrols,
-                           new_state);
+  // printf("[DEBUG] nums: %u, %u, %u\n", num_targets, num_controls,
+  // num_anticontrols);
+  exit_code
+      = apply_gate (state, gate, targets, num_targets, controls, num_controls,
+                    anticontrols, num_anticontrols, new_state);
 
-    if (exit_code == 1) {
-        PyErr_SetString(DokiError, "Failed to initialize new state chunk");
+  if (exit_code == 1)
+    {
+      PyErr_SetString (DokiError, "Failed to initialize new state chunk");
     }
-    else if (exit_code == 2) {
-        PyErr_SetString(DokiError, "Failed to allocate new state chunk");
+  else if (exit_code == 2)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate new state chunk");
     }
-    else if (exit_code == 3) {
-        PyErr_SetString(DokiError, "[BUG] THIS SHOULD NOT HAPPEN. Failed to set first value to 1");
+  else if (exit_code == 3)
+    {
+      PyErr_SetString (
+          DokiError,
+          "[BUG] THIS SHOULD NOT HAPPEN. Failed to set first value to 1");
     }
-    else if (exit_code == 4) {
-        PyErr_SetString(DokiError, "Failed to allocate new state vector structure");
+  else if (exit_code == 4)
+    {
+      PyErr_SetString (DokiError,
+                       "Failed to allocate new state vector structure");
     }
-    else if (exit_code == 5) {
-        PyErr_SetString(DokiError, "Failed to apply gate");
+  else if (exit_code == 5)
+    {
+      PyErr_SetString (DokiError, "Failed to apply gate");
     }
-    else if (exit_code == 11) {
-        PyErr_SetString(DokiError, "Failed to allocate not_copy structure");
+  else if (exit_code == 11)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate not_copy structure");
     }
-    else if (exit_code != 0) {
-        PyErr_SetString(DokiError, "Unknown error when applying gate");
+  else if (exit_code != 0)
+    {
+      PyErr_SetString (DokiError, "Unknown error when applying gate");
     }
 
-    if (exit_code > 0) {
-        free(targets);
-        if (num_controls > 0) {
-            free(controls);
+  if (exit_code > 0)
+    {
+      free (targets);
+      if (num_controls > 0)
+        {
+          free (controls);
         }
-        if (num_anticontrols > 0) {
-            free(anticontrols);
+      if (num_anticontrols > 0)
+        {
+          free (anticontrols);
         }
-        return NULL;
+      return NULL;
     }
 
-    return PyCapsule_New((void*) new_state, "qsimov.doki.state_vector",
-                         &doki_registry_destroy);
+  return PyCapsule_New ((void *)new_state, "qsimov.doki.state_vector",
+                        &doki_registry_destroy);
 }
 
 static PyObject *
 doki_registry_join (PyObject *self, PyObject *args)
 {
-    PyObject *capsule1, *capsule2;
-    void *raw_state1, *raw_state2;
-    struct state_vector *state1, *state2, *result;
-    unsigned char exit_code;
-    int num_threads, debug_enabled;
-
-    if (!PyArg_ParseTuple(args, "OOip", &capsule1, &capsule2, &num_threads, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_join(most_registry, least_registry, num_threads, verbose)");
-        return NULL;
-    }
-
-    if (num_threads <= 0 && num_threads != -1) {
-        PyErr_SetString(DokiError, "num_threads must be at least 1 (or -1 to let OpenMP choose)");
-        return NULL;
-    }
-
-    raw_state1 = PyCapsule_GetPointer(capsule1, "qsimov.doki.state_vector");
-    if (raw_state1 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to registry1");
-        return NULL;
-    }
-
-    raw_state2 = PyCapsule_GetPointer(capsule2, "qsimov.doki.state_vector");
-    if (raw_state2 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to registry2");
-        return NULL;
-    }
-    state1 = (struct state_vector*) raw_state1;
-    state2 = (struct state_vector*) raw_state2;
-    result = MALLOC_TYPE(1, struct state_vector);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate new state structure");
-        return NULL;
-    }
-    if (num_threads != -1) {
-        omp_set_num_threads(num_threads);
-    }
-    exit_code = join(result, state1, state2);
-    if (exit_code != 0) {
-        switch (exit_code) {
-            case 1:
-                PyErr_SetString(DokiError, "Failed to initialize new state chunk");
-                break;
-            case 2:
-                PyErr_SetString(DokiError, "Failed to allocate new state chunk");
-                break;
-            case 3:
-                PyErr_SetString(DokiError, "[BUG] THIS SHOULD NOT HAPPEN. Failed to set first value to 1");
-                break;
-            case 4:
-                PyErr_SetString(DokiError, "Failed to allocate new state vector structure");
-                break;
-            case 5:
-                PyErr_SetString(DokiError, "Failed to get/set a value");
-                break;
-            default:
-                PyErr_SetString(DokiError, "Unknown error when joining states");
+  PyObject *capsule1, *capsule2;
+  void *raw_state1, *raw_state2;
+  struct state_vector *state1, *state2, *result;
+  unsigned char exit_code;
+  int num_threads, debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OOip", &capsule1, &capsule2, &num_threads,
+                         &debug_enabled))
+    {
+      PyErr_SetString (DokiError, "Syntax: registry_join(most_registry, "
+                                  "least_registry, num_threads, verbose)");
+      return NULL;
+    }
+
+  if (num_threads <= 0 && num_threads != -1)
+    {
+      PyErr_SetString (
+          DokiError,
+          "num_threads must be at least 1 (or -1 to let OpenMP choose)");
+      return NULL;
+    }
+
+  raw_state1 = PyCapsule_GetPointer (capsule1, "qsimov.doki.state_vector");
+  if (raw_state1 == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry1");
+      return NULL;
+    }
+
+  raw_state2 = PyCapsule_GetPointer (capsule2, "qsimov.doki.state_vector");
+  if (raw_state2 == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry2");
+      return NULL;
+    }
+  state1 = (struct state_vector *)raw_state1;
+  state2 = (struct state_vector *)raw_state2;
+  result = MALLOC_TYPE (1, struct state_vector);
+  if (result == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate new state structure");
+      return NULL;
+    }
+  if (num_threads != -1)
+    {
+      omp_set_num_threads (num_threads);
+    }
+  exit_code = join (result, state1, state2);
+  if (exit_code != 0)
+    {
+      switch (exit_code)
+        {
+        case 1:
+          PyErr_SetString (DokiError, "Failed to initialize new state chunk");
+          break;
+        case 2:
+          PyErr_SetString (DokiError, "Failed to allocate new state chunk");
+          break;
+        case 3:
+          PyErr_SetString (
+              DokiError,
+              "[BUG] THIS SHOULD NOT HAPPEN. Failed to set first value to 1");
+          break;
+        case 4:
+          PyErr_SetString (DokiError,
+                           "Failed to allocate new state vector structure");
+          break;
+        case 5:
+          PyErr_SetString (DokiError, "Failed to get/set a value");
+          break;
+        default:
+          PyErr_SetString (DokiError, "Unknown error when joining states");
         }
-        return NULL;
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.state_vector",
-                         &doki_registry_destroy);
+  return PyCapsule_New ((void *)result, "qsimov.doki.state_vector",
+                        &doki_registry_destroy);
 }
 
 static PyObject *
 doki_registry_measure (PyObject *self, PyObject *args)
 {
-    PyObject *capsule, *py_measured_val, *result, *new_capsule, *roll_list;
-    Py_ssize_t roll_id;
-    void *raw_state;
-    struct state_vector *state, *new_state, *aux;
-    NATURAL_TYPE mask;
-    REAL_TYPE roll;
-    unsigned int i, curr_id, initial_num_qubits, measured_qty;
-    _Bool measure_id, measured_val;
-    unsigned char exit_code;
-    int debug_enabled, num_threads;
-
-    if (!PyArg_ParseTuple(args, "OKOip", &capsule, &mask, &roll_list, &num_threads, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_measure(registry, mask, roll_list, num_threads, verbose)");
-        return NULL;
-    }
-
-    if (num_threads <= 0 && num_threads != -1) {
-        PyErr_SetString(DokiError, "num_threads must be at least 1 (or -1 to let OpenMP choose)");
-        return NULL;
-    }
-
-    raw_state = PyCapsule_GetPointer(capsule, "qsimov.doki.state_vector");
-    if (raw_state == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to registry");
-        return NULL;
-    }
-    if (!PyList_Check(roll_list)) {
-        PyErr_SetString(DokiError, "roll_list must be a list of real numbers in [0, 1)!");
-        return NULL;
-    }
-    state = (struct state_vector*) raw_state;
-    initial_num_qubits = state->num_qubits;
-    result = PyList_New(initial_num_qubits);
-
-    new_state = MALLOC_TYPE(1, struct state_vector);
-    if (new_state == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate new state structure");
-        return NULL;
-    }
-
-    if (num_threads != -1) {
-        omp_set_num_threads(num_threads);
-    }
-    exit_code = state_clone(new_state, state);
-    if (exit_code == 1) {
-        PyErr_SetString(DokiError, "Failed to allocate state vector");
-        return NULL;
-    }
-    else if (exit_code == 2) {
-        PyErr_SetString(DokiError, "Failed to allocate state chunk");
-        return NULL;
-    }
-    else if (exit_code == 3) {
-        if (debug_enabled) {
-            printf("[DEBUG] %u", state->num_qubits);
-        }
-        PyErr_SetString(DokiError, "Wrong number of qubits");
-        return NULL;
-    }
-    else if (exit_code != 0) {
-        PyErr_SetString(DokiError, "Unknown error when cloning state");
-        return NULL;
-    }
-
-    measured_qty = 0;
-    roll_id = 0;
-    aux = NULL;
-    for (i = 0; i < initial_num_qubits; i++) {
-        curr_id = initial_num_qubits - i - 1;
-        measure_id = mask & (NATURAL_ONE << curr_id);
-        py_measured_val = Py_None;
-        if (measure_id) {
-            if (new_state == NULL || new_state->num_qubits == 0) {
-                if (new_state != NULL) {
-                    state_clear(new_state);
-                    free(new_state);
+  PyObject *capsule, *py_measured_val, *result, *new_capsule, *roll_list;
+  Py_ssize_t roll_id;
+  void *raw_state;
+  struct state_vector *state, *new_state, *aux;
+  NATURAL_TYPE mask;
+  REAL_TYPE roll;
+  unsigned int i, curr_id, initial_num_qubits, measured_qty;
+  _Bool measure_id, measured_val;
+  unsigned char exit_code;
+  int debug_enabled, num_threads;
+
+  if (!PyArg_ParseTuple (args, "OKOip", &capsule, &mask, &roll_list,
+                         &num_threads, &debug_enabled))
+    {
+      PyErr_SetString (DokiError, "Syntax: registry_measure(registry, mask, "
+                                  "roll_list, num_threads, verbose)");
+      return NULL;
+    }
+
+  if (num_threads <= 0 && num_threads != -1)
+    {
+      PyErr_SetString (
+          DokiError,
+          "num_threads must be at least 1 (or -1 to let OpenMP choose)");
+      return NULL;
+    }
+
+  raw_state = PyCapsule_GetPointer (capsule, "qsimov.doki.state_vector");
+  if (raw_state == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry");
+      return NULL;
+    }
+  if (!PyList_Check (roll_list))
+    {
+      PyErr_SetString (DokiError,
+                       "roll_list must be a list of real numbers in [0, 1)!");
+      return NULL;
+    }
+  state = (struct state_vector *)raw_state;
+  initial_num_qubits = state->num_qubits;
+  result = PyList_New (initial_num_qubits);
+
+  new_state = MALLOC_TYPE (1, struct state_vector);
+  if (new_state == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate new state structure");
+      return NULL;
+    }
+
+  if (num_threads != -1)
+    {
+      omp_set_num_threads (num_threads);
+    }
+  exit_code = state_clone (new_state, state);
+  if (exit_code == 1)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state vector");
+      return NULL;
+    }
+  else if (exit_code == 2)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate state chunk");
+      return NULL;
+    }
+  else if (exit_code == 3)
+    {
+      if (debug_enabled)
+        {
+          printf ("[DEBUG] %u", state->num_qubits);
+        }
+      PyErr_SetString (DokiError, "Wrong number of qubits");
+      return NULL;
+    }
+  else if (exit_code != 0)
+    {
+      PyErr_SetString (DokiError, "Unknown error when cloning state");
+      return NULL;
+    }
+
+  measured_qty = 0;
+  roll_id = 0;
+  aux = NULL;
+  for (i = 0; i < initial_num_qubits; i++)
+    {
+      curr_id = initial_num_qubits - i - 1;
+      measure_id = mask & (NATURAL_ONE << curr_id);
+      py_measured_val = Py_None;
+      if (measure_id)
+        {
+          if (new_state == NULL || new_state->num_qubits == 0)
+            {
+              if (new_state != NULL)
+                {
+                  state_clear (new_state);
+                  free (new_state);
                 }
-                PyErr_SetString(DokiError, "Could not measure non_existant qubits");
-                return NULL;
+              PyErr_SetString (DokiError,
+                               "Could not measure non_existant qubits");
+              return NULL;
+            }
+          roll = PyFloat_AsDouble (PyList_GetItem (roll_list, roll_id));
+          if (roll < 0 || roll >= 1)
+            {
+              state_clear (new_state);
+              free (new_state);
+              PyErr_SetString (DokiError, "roll not in interval [0, 1)!");
+              return NULL;
+            }
+          roll_id++;
+          aux = MALLOC_TYPE (1, struct state_vector);
+          if (aux == NULL)
+            {
+              state_clear (new_state);
+              free (new_state);
+              PyErr_SetString (DokiError,
+                               "Failed to allocate aux state structure");
+              return NULL;
             }
-            roll = PyFloat_AsDouble(PyList_GetItem(roll_list, roll_id));
-            if (roll < 0 || roll >= 1) {
-                state_clear(new_state);
-                free(new_state);
-                PyErr_SetString(DokiError, "roll not in interval [0, 1)!");
-                return NULL;
-            }
-            roll_id++;
-            aux = MALLOC_TYPE(1, struct state_vector);
-            if (aux == NULL) {
-                state_clear(new_state);
-                free(new_state);
-                PyErr_SetString(DokiError, "Failed to allocate aux state structure");
-                return NULL;
-            }
-            exit_code = measure(new_state, &measured_val, curr_id, aux, roll);
-            if (exit_code != 0) {
-                state_clear(aux);
-                free(aux);
-                aux = NULL;
-                break;
-            }
-            if (aux->num_qubits > 0 && aux->norm_const == 0.0) {
-                state_clear(aux);
-                free(aux);
-                state_clear(new_state);
-                free(new_state);
-                PyErr_SetString(DokiError, "New normalization constant is 0. Please report this error with the steps to reproduce it.");
-                return NULL;
-            }
-            measured_qty++;
-            py_measured_val = measured_val ? Py_True : Py_False;
-            state_clear(new_state);
-            free(new_state);
-            new_state = aux;
-            aux = NULL;
-        }
-        PyList_SET_ITEM(result, i, py_measured_val);
-    }
-    if (exit_code != 0) {
-        if (new_state != NULL) {
-            state_clear(new_state);
-            free(new_state);
+          exit_code = measure (new_state, &measured_val, curr_id, aux, roll);
+          if (exit_code != 0)
+            {
+              state_clear (aux);
+              free (aux);
+              aux = NULL;
+              break;
+            }
+          if (aux->num_qubits > 0 && aux->norm_const == 0.0)
+            {
+              state_clear (aux);
+              free (aux);
+              state_clear (new_state);
+              free (new_state);
+              PyErr_SetString (
+                  DokiError, "New normalization constant is 0. Please report "
+                             "this error with the steps to reproduce it.");
+              return NULL;
+            }
+          measured_qty++;
+          py_measured_val = measured_val ? Py_True : Py_False;
+          state_clear (new_state);
+          free (new_state);
+          new_state = aux;
+          aux = NULL;
         }
-        switch (exit_code) {
-            case 1:
-                PyErr_SetString(DokiError, "Failed to allocate state vector");
-                break;
-            case 2:
-                PyErr_SetString(DokiError, "Failed to allocate state chunk");
-                break;
-            default:
-                PyErr_SetString(DokiError, "Unknown error while collapsing state");
+      PyList_SET_ITEM (result, i, py_measured_val);
+    }
+  if (exit_code != 0)
+    {
+      if (new_state != NULL)
+        {
+          state_clear (new_state);
+          free (new_state);
+        }
+      switch (exit_code)
+        {
+        case 1:
+          PyErr_SetString (DokiError, "Failed to allocate state vector");
+          break;
+        case 2:
+          PyErr_SetString (DokiError, "Failed to allocate state chunk");
+          break;
+        default:
+          PyErr_SetString (DokiError, "Unknown error while collapsing state");
         }
-        return NULL;
+      return NULL;
     }
 
-    if (state->num_qubits - measured_qty > 0) {
-        new_capsule = PyCapsule_New((void*) new_state, "qsimov.doki.state_vector",
-                                    &doki_registry_destroy);
+  if (state->num_qubits - measured_qty > 0)
+    {
+      new_capsule
+          = PyCapsule_New ((void *)new_state, "qsimov.doki.state_vector",
+                           &doki_registry_destroy);
     }
-    else {
-        if (new_state != NULL) {
-            state_clear(new_state);
-            free(new_state);
+  else
+    {
+      if (new_state != NULL)
+        {
+          state_clear (new_state);
+          free (new_state);
         }
-        new_capsule = Py_None;
+      new_capsule = Py_None;
     }
-    return PyTuple_Pack(2, new_capsule, result);
+  return PyTuple_Pack (2, new_capsule, result);
 }
 
 static PyObject *
 doki_registry_prob (PyObject *self, PyObject *args)
 {
-    PyObject *capsule;
-    void *raw_state;
-    struct state_vector *state;
-    unsigned int id;
-    int debug_enabled, num_threads;
+  PyObject *capsule;
+  void *raw_state;
+  struct state_vector *state;
+  unsigned int id;
+  int debug_enabled, num_threads;
 
-    if (!PyArg_ParseTuple(args, "OIip", &capsule, &id, &num_threads, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: registry_prob(registry, qubit_id, num_threads, verbose)");
-        return NULL;
+  if (!PyArg_ParseTuple (args, "OIip", &capsule, &id, &num_threads,
+                         &debug_enabled))
+    {
+      PyErr_SetString (
+          DokiError,
+          "Syntax: registry_prob(registry, qubit_id, num_threads, verbose)");
+      return NULL;
     }
 
-    if (num_threads <= 0 && num_threads != -1) {
-        PyErr_SetString(DokiError, "num_threads must be at least 1 (or -1 to let OpenMP choose)");
-        return NULL;
+  if (num_threads <= 0 && num_threads != -1)
+    {
+      PyErr_SetString (
+          DokiError,
+          "num_threads must be at least 1 (or -1 to let OpenMP choose)");
+      return NULL;
     }
 
-    raw_state = PyCapsule_GetPointer(capsule, "qsimov.doki.state_vector");
-    if (raw_state == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to registry");
-        return NULL;
+  raw_state = PyCapsule_GetPointer (capsule, "qsimov.doki.state_vector");
+  if (raw_state == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry");
+      return NULL;
     }
-    state = (struct state_vector*) raw_state;
+  state = (struct state_vector *)raw_state;
 
-    if (num_threads != -1) {
-        omp_set_num_threads(num_threads);
+  if (num_threads != -1)
+    {
+      omp_set_num_threads (num_threads);
     }
-    return PyFloat_FromDouble(probability(state, id));
+  return PyFloat_FromDouble (probability (state, id));
 }
 
 static PyObject *
 doki_registry_density (PyObject *self, PyObject *args)
 {
-    PyObject *state_capsule;
-    void *raw_state;
-    FunctionalMatrix *densityMatrix;
-    int debug_enabled;
+  PyObject *state_capsule;
+  void *raw_state;
+  struct FMatrix *densityMatrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "Op", &state_capsule, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "Op", &state_capsule, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: registry_density(state, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError, "Syntax: registry_density(state, verbose)");
+      return NULL;
     }
 
-    raw_state = PyCapsule_GetPointer(state_capsule, "qsimov.doki.state_vector");
-    if (raw_state == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to registry");
-        return NULL;
+  raw_state = PyCapsule_GetPointer (state_capsule, "qsimov.doki.state_vector");
+  if (raw_state == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry");
+      return NULL;
     }
 
-    densityMatrix = densityMat((struct state_vector*) raw_state);
-    if (densityMatrix == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate density matrix");
-        return NULL;
+  densityMatrix = density_matrix (state_capsule);
+  if (densityMatrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[DENSITY] Failed to allocate density matrix");
+          break;
+        case 2:
+          PyErr_SetString (DokiError, "[DENSITY] The state is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[DENSITY] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) densityMatrix, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New ((void *)densityMatrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
-doki_funmatrix_get (PyObject *self, PyObject *args)
+doki_funmatrix_create (PyObject *self, PyObject *args)
 {
-    PyObject *capsule;
-    void *raw_matrix;
-    FunctionalMatrix *matrix;
-    NATURAL_TYPE i, j;
-    COMPLEX_TYPE val;
-    int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "OKKp", &capsule, &i, &j, &debug_enabled))
+  PyObject *list, *row, *raw_val;
+  unsigned int num_rows, num_cols;
+  NATURAL_TYPE size, i, j;
+  COMPLEX_TYPE val, *matrix_2d;
+  struct FMatrix *funmatrix;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "Op", &list, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_get(funmatrix, i, j, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError, "Syntax: funmatrix_create(matrix, verbose)");
+      return NULL;
     }
-
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix");
-        return NULL;
+  if (!PyList_Check (list))
+    {
+      PyErr_SetString (DokiError, "matrix must be a list of lists (matrix)");
+      return NULL;
     }
-    matrix = (FunctionalMatrix*) raw_matrix;
 
-    if (i < 0 || j < 0 || i >= matrix->r || j >= matrix->c) {
-        PyErr_SetString(DokiError, "Out of bounds");
-        return NULL;
+  num_rows = PyList_Size (list);
+  if (num_rows == 0)
+    {
+      PyErr_SetString (DokiError, "there are no rows");
+      return NULL;
+    }
+  row = PyList_GetItem (list, 0);
+  if (!PyList_Check (row))
+    {
+      PyErr_SetString (DokiError, "rows must be lists");
+      return NULL;
+    }
+  num_cols = PyList_Size (row);
+  if (num_cols == 0)
+    {
+      PyErr_SetString (DokiError, "there are no columns");
+      return NULL;
     }
 
-    val = COMPLEX_ZERO;
-    if (!getitem(matrix, i, j, &val)) {
-        PyErr_SetString(DokiError, "Error getting element");
-        return NULL;
+  size = (NATURAL_TYPE)num_rows * num_cols;
+  matrix_2d = MALLOC_TYPE (size, COMPLEX_TYPE);
+  if (matrix_2d == NULL)
+    {
+      PyErr_SetString (DokiError, "failed to allocate 2D matrix");
+      return NULL;
     }
 
-    if (isnan(RE(val)) || isnan(IM(val))) {
-        PyErr_SetString(DokiError, "Error calculating element");
-        return NULL;
+  for (i = 0; i < num_rows; ++i)
+    {
+      row = PyList_GetItem (list, i);
+      if (!PyList_Check (row) || (NATURAL_TYPE)PyList_Size (row) != num_cols)
+        {
+          PyErr_SetString (DokiError, "rows must be lists of the same size");
+          free (matrix_2d);
+          return NULL;
+        }
+      for (j = 0; j < num_cols; ++j)
+        {
+          raw_val = PyList_GetItem (row, j);
+          if (PyComplex_Check (raw_val))
+            {
+              val = COMPLEX_INIT (PyComplex_RealAsDouble (raw_val),
+                                  PyComplex_ImagAsDouble (raw_val));
+            }
+          else if (PyFloat_Check (raw_val))
+            {
+              val = COMPLEX_INIT (PyFloat_AsDouble (raw_val), 0.0);
+            }
+          else if (PyLong_Check (raw_val))
+            {
+              val = COMPLEX_INIT ((double)PyLong_AsLong (raw_val), 0.0);
+            }
+          else
+            {
+              PyErr_SetString (DokiError,
+                               "matrix elements must be complex numbers");
+              free (matrix_2d);
+              return NULL;
+            }
+          matrix_2d[i * num_rows + j] = val;
+        }
+    }
+  funmatrix = CustomMat (matrix_2d, size, num_rows, num_cols);
+  if (funmatrix == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to matrix");
+      return NULL;
     }
 
-    return PyComplex_FromDoubles(RE(val), IM(val));
+  return PyCapsule_New ((void *)funmatrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
-doki_funmatrix_add (PyObject *self, PyObject *args)
+doki_funmatrix_identity (PyObject *self, PyObject *args)
 {
-    PyObject *capsule1, *capsule2;
-    void *raw_matrix1, *raw_matrix2;
-    FunctionalMatrix *matrix1, *matrix2, *result;
-    int debug_enabled;
+  unsigned int num_qubits;
+  struct FMatrix *funmatrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "OOp", &capsule1, &capsule2, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "Ip", &num_qubits, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_add(funmatrix1, funmatrix2, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_identity(num_qubits, verbose)");
+      return NULL;
     }
+  funmatrix = Identity (num_qubits);
 
-    raw_matrix1 = PyCapsule_GetPointer(capsule1, "qsimov.doki.funmatrix");
-    if (raw_matrix1 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 1");
-        return NULL;
-    }
-    matrix1 = (FunctionalMatrix*) raw_matrix1;
+  return PyCapsule_New ((void *)funmatrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
+}
 
-    raw_matrix2 = PyCapsule_GetPointer(capsule2, "qsimov.doki.funmatrix");
-    if (raw_matrix2 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 2");
-        return NULL;
-    }
-    matrix2 = (FunctionalMatrix*) raw_matrix2;
+static PyObject *
+doki_funmatrix_hadamard (PyObject *self, PyObject *args)
+{
+  unsigned int num_qubits;
+  struct FMatrix *funmatrix;
+  int debug_enabled;
 
-    result = madd(matrix1, matrix2);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  if (!PyArg_ParseTuple (args, "Ip", &num_qubits, &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_hadamard(num_qubits, verbose)");
+      return NULL;
+    }
+  funmatrix = Hadamard (num_qubits);
+  if (funmatrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError, "[H] Failed to allocate result matrix");
+          break;
+        case 5:
+          PyErr_SetString (DokiError, "[H] Failed to allocate data pointer");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[H] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New ((void *)funmatrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
-doki_funmatrix_sub (PyObject *self, PyObject *args)
+doki_funmatrix_statezero (PyObject *self, PyObject *args)
 {
-    PyObject *capsule1, *capsule2;
-    void *raw_matrix1, *raw_matrix2;
-    FunctionalMatrix *matrix1, *matrix2, *result;
-    int debug_enabled;
+  unsigned int num_qubits;
+  struct FMatrix *funmatrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "OOp", &capsule1, &capsule2, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "Ip", &num_qubits, &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_statezero(num_qubits, verbose)");
+      return NULL;
+    }
+  funmatrix = StateZero (num_qubits);
+  if (funmatrix == NULL)
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_sub(funmatrix1, funmatrix2, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError, "NULL pointer to matrix");
+      return NULL;
     }
 
-    raw_matrix1 = PyCapsule_GetPointer(capsule1, "qsimov.doki.funmatrix");
-    if (raw_matrix1 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 1");
-        return NULL;
+  return PyCapsule_New ((void *)funmatrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
+}
+
+static PyObject *
+doki_funmatrix_densityzero (PyObject *self, PyObject *args)
+{
+  unsigned int num_qubits;
+  struct FMatrix *funmatrix;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "Ip", &num_qubits, &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_densityzero(num_qubits, verbose)");
+      return NULL;
+    }
+  funmatrix = DensityZero (num_qubits);
+  if (funmatrix == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to matrix");
+      return NULL;
     }
-    matrix1 = (FunctionalMatrix*) raw_matrix1;
 
-    raw_matrix2 = PyCapsule_GetPointer(capsule2, "qsimov.doki.funmatrix");
-    if (raw_matrix2 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 2");
-        return NULL;
+  return PyCapsule_New ((void *)funmatrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
+}
+
+static PyObject *
+doki_funmatrix_addcontrol (PyObject *self, PyObject *args)
+{
+  PyObject *capsule;
+  void *funmatrix;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "Op", &capsule, &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_addcontrol(funmatrix, verbose)");
+      return NULL;
     }
-    matrix2 = (FunctionalMatrix*) raw_matrix2;
 
-    result = msub(matrix1, matrix2);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  funmatrix = (void *)CU (capsule);
+  if (funmatrix == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to matrix");
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New ((void *)funmatrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
-doki_funmatrix_scalar_mul (PyObject *self, PyObject *args)
+doki_funmatrix_get (PyObject *self, PyObject *args)
 {
-    PyObject *capsule, *raw_scalar;
-    void *raw_matrix;
-    FunctionalMatrix *matrix, *result;
-    COMPLEX_TYPE scalar;
-    int debug_enabled;
+  PyObject *capsule;
+  void *raw_matrix;
+  struct FMatrix *matrix;
+  NATURAL_TYPE i, j;
+  COMPLEX_TYPE val;
+  int debug_enabled, res;
 
-    if (!PyArg_ParseTuple(args, "OOp", &capsule, &raw_scalar, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "OKKp", &capsule, &i, &j, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_mul(funmatrix, scalar, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_get(funmatrix, i, j, verbose)");
+      return NULL;
     }
 
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix");
-        return NULL;
+  raw_matrix = PyCapsule_GetPointer (capsule, "qsimov.doki.funmatrix");
+  if (raw_matrix == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to matrix");
+      return NULL;
     }
-    matrix = (FunctionalMatrix*) raw_matrix;
+  matrix = (struct FMatrix *)raw_matrix;
 
-    if (PyComplex_Check(raw_scalar)) {
-        scalar = complex_init(PyComplex_RealAsDouble(raw_scalar), PyComplex_ImagAsDouble(raw_scalar));
+  if (i < 0 || j < 0 || i >= matrix->r || j >= matrix->c)
+    {
+      PyErr_SetString (DokiError, "Out of bounds");
+      return NULL;
     }
-    else if(PyFloat_Check(raw_scalar)) {
-        scalar = complex_init(PyFloat_AsDouble(raw_scalar), 0.0);
+
+  val = COMPLEX_ZERO;
+  res = getitem (matrix, i, j, &val);
+  if (res != 0)
+    {
+      switch (res)
+        {
+        case 1:
+          PyErr_SetString (DokiError, "[GET] Error adding parent matrices");
+          break;
+        case 2:
+          PyErr_SetString (DokiError,
+                           "[GET] Error substracting parent matrices");
+          break;
+        case 3:
+          PyErr_SetString (DokiError,
+                           "[GET] Error multiplying parent matrices");
+          break;
+        case 4:
+          PyErr_SetString (
+              DokiError,
+              "[GET] Error multiplying entity-wise parent matrices");
+          break;
+        case 5:
+          PyErr_SetString (
+              DokiError,
+              "[GET] Error calculating Kronecker product of parent matrices");
+          break;
+        case 6:
+          PyErr_SetString (DokiError,
+                           "[GET] Unknown operation between parent matrices");
+          break;
+        case 7:
+          PyErr_SetString (DokiError, "[GET] Element out of bounds");
+          break;
+        case 8:
+          PyErr_SetString (DokiError, "[GET] f returned NAN");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[GET] Unknown error code");
+        }
+      return NULL;
     }
-    else if(PyLong_Check(raw_scalar)) {
-        scalar = complex_init((double) PyLong_AsLong(raw_scalar), 0.0);
+
+  if (isnan (RE (val)) || isnan (IM (val)))
+    {
+      PyErr_SetString (DokiError, "[GET] Unexpected NAN value");
+      return NULL;
     }
-    else {
-        PyErr_SetString(DokiError, "scalar is not a number");
-        return NULL;
+
+  return PyComplex_FromDoubles (RE (val), IM (val));
+}
+
+static PyObject *
+doki_funmatrix_add (PyObject *self, PyObject *args)
+{
+  PyObject *capsule1, *capsule2;
+  void *raw_matrix;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OOp", &capsule1, &capsule2, &debug_enabled))
+    {
+      PyErr_SetString (
+          DokiError, "Syntax: funmatrix_add(funmatrix1, funmatrix2, verbose)");
+      return NULL;
     }
 
-    result = mprod(scalar, matrix);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  raw_matrix = (void *)madd (capsule1, capsule2);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[ADD] Failed to allocate result matrix");
+          break;
+        case 2:
+          PyErr_SetString (DokiError, "[ADD] The operands are misalligned");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[ADD] The first operand is NULL");
+          break;
+        case 4:
+          PyErr_SetString (DokiError, "[ADD] The second operand is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[ADD] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
-doki_funmatrix_scalar_div (PyObject *self, PyObject *args)
+doki_funmatrix_sub (PyObject *self, PyObject *args)
 {
-    PyObject *capsule, *raw_scalar;
-    void *raw_matrix;
-    FunctionalMatrix *matrix, *result;
-    COMPLEX_TYPE scalar;
-    int debug_enabled;
+  PyObject *capsule1, *capsule2;
+  void *raw_matrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "OOp", &capsule, &raw_scalar, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "OOp", &capsule1, &capsule2, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_div(funmatrix, scalar, verbose)");
-        return NULL;
+      PyErr_SetString (
+          DokiError, "Syntax: funmatrix_sub(funmatrix1, funmatrix2, verbose)");
+      return NULL;
     }
 
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix");
-        return NULL;
+  raw_matrix = (void *)msub (capsule1, capsule2);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[SUB] Failed to allocate result matrix");
+          break;
+        case 2:
+          PyErr_SetString (DokiError, "[SUB] The operands are misalligned");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[SUB] The first operand is NULL");
+          break;
+        case 4:
+          PyErr_SetString (DokiError, "[SUB] The second operand is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[SUB] Unknown error");
+        }
+      return NULL;
+    }
+
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
+}
+
+static PyObject *
+doki_funmatrix_scalar_mul (PyObject *self, PyObject *args)
+{
+  PyObject *capsule, *raw_scalar;
+  void *raw_matrix;
+  COMPLEX_TYPE scalar;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OOp", &capsule, &raw_scalar, &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_mul(funmatrix, scalar, verbose)");
+      return NULL;
     }
-    matrix = (FunctionalMatrix*) raw_matrix;
 
-    if (PyComplex_Check(raw_scalar)) {
-        scalar = complex_init(PyComplex_RealAsDouble(raw_scalar), PyComplex_ImagAsDouble(raw_scalar));
+  if (PyComplex_Check (raw_scalar))
+    {
+      scalar = COMPLEX_INIT (PyComplex_RealAsDouble (raw_scalar),
+                             PyComplex_ImagAsDouble (raw_scalar));
     }
-    else if(PyFloat_Check(raw_scalar)) {
-        scalar = complex_init(PyFloat_AsDouble(raw_scalar), 0.0);
+  else if (PyFloat_Check (raw_scalar))
+    {
+      scalar = COMPLEX_INIT (PyFloat_AsDouble (raw_scalar), 0.0);
     }
-    else if(PyLong_Check(raw_scalar)) {
-        scalar = complex_init((double) PyLong_AsLong(raw_scalar), 0.0);
+  else if (PyLong_Check (raw_scalar))
+    {
+      scalar = COMPLEX_INIT ((double)PyLong_AsLong (raw_scalar), 0.0);
     }
-    else {
-        PyErr_SetString(DokiError, "scalar is not a number");
-        return NULL;
+  else
+    {
+      PyErr_SetString (DokiError, "scalar is not a number");
+      return NULL;
     }
 
-    result = mdiv(scalar, matrix);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  raw_matrix = (void *)mprod (scalar, capsule);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[SPROD] Failed to allocate result matrix");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[SPROD] The matrix operand is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[SPROD] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
-doki_funmatrix_matmul (PyObject *self, PyObject *args)
+doki_funmatrix_scalar_div (PyObject *self, PyObject *args)
 {
-    PyObject *capsule1, *capsule2;
-    void *raw_matrix1, *raw_matrix2;
-    FunctionalMatrix *matrix1, *matrix2, *result;
-    int debug_enabled;
+  PyObject *capsule, *raw_scalar;
+  void *raw_matrix;
+  COMPLEX_TYPE scalar;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "OOp", &capsule1, &capsule2, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "OOp", &capsule, &raw_scalar, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_matmul(funmatrix1, funmatrix2, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_div(funmatrix, scalar, verbose)");
+      return NULL;
     }
 
-    raw_matrix1 = PyCapsule_GetPointer(capsule1, "qsimov.doki.funmatrix");
-    if (raw_matrix1 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 1");
-        return NULL;
+  if (PyComplex_Check (raw_scalar))
+    {
+      scalar = COMPLEX_INIT (PyComplex_RealAsDouble (raw_scalar),
+                             PyComplex_ImagAsDouble (raw_scalar));
     }
-    matrix1 = (FunctionalMatrix*) raw_matrix1;
-
-    raw_matrix2 = PyCapsule_GetPointer(capsule2, "qsimov.doki.funmatrix");
-    if (raw_matrix2 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 2");
-        return NULL;
+  else if (PyFloat_Check (raw_scalar))
+    {
+      scalar = COMPLEX_INIT (PyFloat_AsDouble (raw_scalar), 0.0);
+    }
+  else if (PyLong_Check (raw_scalar))
+    {
+      scalar = COMPLEX_INIT ((double)PyLong_AsLong (raw_scalar), 0.0);
+    }
+  else
+    {
+      PyErr_SetString (DokiError, "scalar is not a number");
+      return NULL;
     }
-    matrix2 = (FunctionalMatrix*) raw_matrix2;
 
-    result = matmul(matrix1, matrix2);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  if (RE (scalar) == 0 && IM (scalar) == 0)
+    {
+      PyErr_SetString (DokiError, "Dividing by zero");
+      return NULL;
+    }
+  raw_matrix = (void *)mdiv (scalar, capsule);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[SDIV] Failed to allocate result matrix");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[SDIV] The matrix operand is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[SDIV] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
-doki_funmatrix_ewmul (PyObject *self, PyObject *args)
+doki_funmatrix_matmul (PyObject *self, PyObject *args)
 {
-    PyObject *capsule1, *capsule2;
-    void *raw_matrix1, *raw_matrix2;
-    FunctionalMatrix *matrix1, *matrix2, *result;
-    int debug_enabled;
+  PyObject *capsule1, *capsule2;
+  void *raw_matrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "OOp", &capsule1, &capsule2, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "OOp", &capsule1, &capsule2, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_ewmul(funmatrix1, funmatrix2, verbose)");
-        return NULL;
+      PyErr_SetString (
+          DokiError,
+          "Syntax: funmatrix_matmul(funmatrix1, funmatrix2, verbose)");
+      return NULL;
     }
 
-    raw_matrix1 = PyCapsule_GetPointer(capsule1, "qsimov.doki.funmatrix");
-    if (raw_matrix1 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 1");
-        return NULL;
+  raw_matrix = (void *)matmul (capsule1, capsule2);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[MATMUL] Failed to allocate result matrix");
+          break;
+        case 2:
+          PyErr_SetString (DokiError, "[MATMUL] The operands are misalligned");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[MATMUL] The first operand is NULL");
+          break;
+        case 4:
+          PyErr_SetString (DokiError, "[MATMUL] The second operand is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[MATMUL] Unknown error");
+        }
+      return NULL;
     }
-    matrix1 = (FunctionalMatrix*) raw_matrix1;
 
-    raw_matrix2 = PyCapsule_GetPointer(capsule2, "qsimov.doki.funmatrix");
-    if (raw_matrix2 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 2");
-        return NULL;
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
+}
+
+static PyObject *
+doki_funmatrix_ewmul (PyObject *self, PyObject *args)
+{
+  PyObject *capsule1, *capsule2;
+  void *raw_matrix;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OOp", &capsule1, &capsule2, &debug_enabled))
+    {
+      PyErr_SetString (
+          DokiError,
+          "Syntax: funmatrix_ewmul(funmatrix1, funmatrix2, verbose)");
+      return NULL;
     }
-    matrix2 = (FunctionalMatrix*) raw_matrix2;
 
-    result = ewmul(matrix1, matrix2);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  raw_matrix = (void *)ewmul (capsule1, capsule2);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[EWMUL] Failed to allocate result matrix");
+          break;
+        case 2:
+          PyErr_SetString (DokiError, "[EWMUL] The operands are misalligned");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[EWMUL] The first operand is NULL");
+          break;
+        case 4:
+          PyErr_SetString (DokiError, "[EWMUL] The second operand is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[EWMUL] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
 doki_funmatrix_kron (PyObject *self, PyObject *args)
 {
-    PyObject *capsule1, *capsule2;
-    void *raw_matrix1, *raw_matrix2;
-    FunctionalMatrix *matrix1, *matrix2, *result;
-    int debug_enabled;
+  PyObject *capsule1, *capsule2;
+  void *raw_matrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "OOp", &capsule1, &capsule2, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "OOp", &capsule1, &capsule2, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_kron(funmatrix1, funmatrix2, verbose)");
-        return NULL;
+      PyErr_SetString (
+          DokiError,
+          "Syntax: funmatrix_kron(funmatrix1, funmatrix2, verbose)");
+      return NULL;
     }
 
-    raw_matrix1 = PyCapsule_GetPointer(capsule1, "qsimov.doki.funmatrix");
-    if (raw_matrix1 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 1");
-        return NULL;
-    }
-    matrix1 = (FunctionalMatrix*) raw_matrix1;
+  raw_matrix = (void *)kron (capsule1, capsule2);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[KRON] Failed to allocate result matrix");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[KRON] The first operand is NULL");
+          break;
+        case 4:
+          PyErr_SetString (DokiError, "[KRON] The second operand is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[KRON] Unknown error");
+        }
+      return NULL;
+    }
+
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
+}
 
-    raw_matrix2 = PyCapsule_GetPointer(capsule2, "qsimov.doki.funmatrix");
-    if (raw_matrix2 == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix 2");
-        return NULL;
+static PyObject *
+doki_funmatrix_eyekron (PyObject *self, PyObject *args)
+{
+  PyObject *capsule;
+  unsigned int left, right;
+  void *raw_matrix;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OIIp", &capsule, &left, &right,
+                         &debug_enabled))
+    {
+      PyErr_SetString (DokiError, "Syntax: funmatrix_eyekron(funmatrix, "
+                                  "leftQubits, rightQubits, verbose)");
+      return NULL;
     }
-    matrix2 = (FunctionalMatrix*) raw_matrix2;
 
-    result = kron(matrix1, matrix2);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  raw_matrix = (void *)eyeKron (capsule, left, right);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[EYEKRON] Failed to allocate result matrix");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[EYEKRON] The matrix is NULL");
+          break;
+        case 5:
+          PyErr_SetString (DokiError,
+                           "[EYEKRON] Could not allocate data array");
+          break;
+        case 6:
+          PyErr_SetString (DokiError,
+                           "[EYEKRON] Could not allocate data struct");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[EYEKRON] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
 doki_funmatrix_transpose (PyObject *self, PyObject *args)
 {
-    PyObject *capsule;
-    void *raw_matrix;
-    FunctionalMatrix *matrix, *result;
-    int debug_enabled;
+  PyObject *capsule;
+  void *raw_matrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "Op", &capsule, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "Op", &capsule, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_transpose(funmatrix, verbose)");
-        return NULL;
-    }
-
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix");
-        return NULL;
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_transpose(funmatrix, verbose)");
+      return NULL;
     }
-    matrix = (FunctionalMatrix*) raw_matrix;
 
-    result = transpose(matrix);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  raw_matrix = (void *)transpose (capsule);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[TRANS] Failed to allocate result matrix");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[TRANS] The matrix is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[TRANS] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
 doki_funmatrix_dagger (PyObject *self, PyObject *args)
 {
-    PyObject *capsule;
-    void *raw_matrix;
-    FunctionalMatrix *matrix, *result;
-    int debug_enabled;
+  PyObject *capsule;
+  void *raw_matrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "Op", &capsule, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "Op", &capsule, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_dagger(funmatrix, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_dagger(funmatrix, verbose)");
+      return NULL;
     }
 
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix");
-        return NULL;
+  raw_matrix = (void *)dagger (capsule);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[HTRANS] Failed to allocate result matrix");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[HTRANS] The matrix is NULL");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[HTRANS] Unknown error");
+        }
+      return NULL;
+    }
+
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
+}
+
+static PyObject *
+doki_funmatrix_projection (PyObject *self, PyObject *args)
+{
+  PyObject *capsule;
+  unsigned int qubitId;
+  void *raw_matrix;
+  bool value, debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OIpp", &capsule, &qubitId, &value,
+                         &debug_enabled))
+    {
+      PyErr_SetString (
+          DokiError,
+          "Syntax: funmatrix_projection(funmatrix, qubit_id, value, verbose)");
+      return NULL;
     }
-    matrix = (FunctionalMatrix*) raw_matrix;
 
-    result = dagger(matrix);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  raw_matrix = (void *)projection (capsule, qubitId, value);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[PROJ] Failed to allocate result matrix");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[PROJ] The matrix is NULL");
+          break;
+        case 5:
+          PyErr_SetString (DokiError, "[PROJ] Could not allocate data struct");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[PROJ] Unknown error");
+        }
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
 doki_funmatrix_shape (PyObject *self, PyObject *args)
 {
-    PyObject *capsule;
-    void *raw_matrix;
-    FunctionalMatrix *matrix;
-    int debug_enabled;
+  PyObject *capsule;
+  void *raw_matrix;
+  struct FMatrix *matrix;
+  int debug_enabled;
 
-    if (!PyArg_ParseTuple(args, "Op", &capsule, &debug_enabled))
+  if (!PyArg_ParseTuple (args, "Op", &capsule, &debug_enabled))
     {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_shape(funmatrix, verbose)");
-        return NULL;
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_shape(funmatrix, verbose)");
+      return NULL;
     }
 
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix");
-        return NULL;
+  raw_matrix = PyCapsule_GetPointer (capsule, "qsimov.doki.funmatrix");
+  if (raw_matrix == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to matrix");
+      return NULL;
     }
-    matrix = (FunctionalMatrix*) raw_matrix;
+  matrix = (struct FMatrix *)raw_matrix;
 
-    return PyTuple_Pack(2, PyLong_FromUnsignedLongLong(rows(matrix)),
-                           PyLong_FromUnsignedLongLong(columns(matrix)));
+  return PyTuple_Pack (2, PyLong_FromUnsignedLongLong (rows (matrix)),
+                       PyLong_FromUnsignedLongLong (columns (matrix)));
 }
 
 static PyObject *
 doki_funmatrix_partialtrace (PyObject *self, PyObject *args)
 {
-    PyObject *capsule;
-    unsigned int id;
-    void *raw_matrix;
-    FunctionalMatrix *matrix, *result;
-    int debug_enabled;
-
-    if (!PyArg_ParseTuple(args, "OIp", &capsule, &id, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_partialtrace(funmatrix, id, verbose)");
-        return NULL;
-    }
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix");
-        return NULL;
-    }
-    matrix = (FunctionalMatrix*) raw_matrix;
-    result = partial_trace(matrix, id);
-    if (result == NULL) {
-        PyErr_SetString(DokiError, "Failed to allocate result");
-        return NULL;
+  PyObject *capsule;
+  unsigned int id;
+  void *raw_matrix;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OIp", &capsule, &id, &debug_enabled))
+    {
+      PyErr_SetString (
+          DokiError, "Syntax: funmatrix_partialtrace(funmatrix, id, verbose)");
+      return NULL;
     }
 
-    return PyCapsule_New((void*) result, "qsimov.doki.funmatrix", &doki_funmatrix_destroy);
+  raw_matrix = (void *)partial_trace (capsule, id);
+  if (raw_matrix == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError,
+                           "[PTRACE] Failed to allocate result matrix");
+          break;
+        case 2:
+          PyErr_SetString (DokiError,
+                           "[PTRACE] The matrix is not a square matrix");
+          break;
+        case 3:
+          PyErr_SetString (DokiError, "[PTRACE] The matrix is NULL");
+          break;
+        case 5:
+          PyErr_SetString (DokiError,
+                           "[PTRACE] Could not allocate argv struct");
+          break;
+        case 6:
+          PyErr_SetString (DokiError, "[PTRACE] elem id has to be >= 0");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[PTRACE] Unknown error");
+        }
+      return NULL;
+    }
+
+  return PyCapsule_New (raw_matrix, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
 
 static PyObject *
 doki_funmatrix_trace (PyObject *self, PyObject *args)
 {
-    PyObject *capsule;
-    void *raw_matrix;
-    FunctionalMatrix *matrix;
-    COMPLEX_TYPE result, aux;
-    NATURAL_TYPE i, min_shape;
-    int debug_enabled;
-
-    if (!PyArg_ParseTuple(args, "Op", &capsule, &debug_enabled)) {
-        PyErr_SetString(DokiError, "Syntax: funmatrix_trace(funmatrix, verbose)");
-        return NULL;
-    }
-    raw_matrix = PyCapsule_GetPointer(capsule, "qsimov.doki.funmatrix");
-    if (raw_matrix == NULL) {
-        PyErr_SetString(DokiError, "NULL pointer to matrix");
-        return NULL;
-    }
-    matrix = (FunctionalMatrix*) raw_matrix;
-    result = COMPLEX_ZERO;
-    min_shape = matrix->r <= matrix->c ? matrix->r : matrix->c;
-
-    aux = COMPLEX_ZERO;
-    for (i = 0; i < min_shape; i++) {
-        if (!getitem(matrix, i, i, &aux)) {
-            PyErr_SetString(DokiError, "Failed to get matrix element");
-            return NULL;
+  PyObject *capsule;
+  void *raw_matrix;
+  struct FMatrix *matrix;
+  COMPLEX_TYPE result, aux;
+  NATURAL_TYPE i, min_shape;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "Op", &capsule, &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_trace(funmatrix, verbose)");
+      return NULL;
+    }
+  raw_matrix = PyCapsule_GetPointer (capsule, "qsimov.doki.funmatrix");
+  if (raw_matrix == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to matrix");
+      return NULL;
+    }
+  matrix = (struct FMatrix *)raw_matrix;
+  result = COMPLEX_ZERO;
+  min_shape = matrix->r <= matrix->c ? matrix->r : matrix->c;
+
+  aux = COMPLEX_ZERO;
+  for (i = 0; i < min_shape; i++)
+    {
+      int res = getitem (matrix, i, i, &aux);
+      if (res != 0)
+        {
+          switch (res)
+            {
+            case 1:
+              PyErr_SetString (DokiError,
+                               "[TRACE] Error adding parent matrices");
+              break;
+            case 2:
+              PyErr_SetString (DokiError,
+                               "[TRACE] Error substracting parent matrices");
+              break;
+            case 3:
+              PyErr_SetString (DokiError,
+                               "[TRACE] Error multiplying parent matrices");
+              break;
+            case 4:
+              PyErr_SetString (
+                  DokiError,
+                  "[TRACE] Error multiplying entity-wise parent matrices");
+              break;
+            case 5:
+              PyErr_SetString (DokiError,
+                               "[TRACE] Error calculating Kronecker product "
+                               "of parent matrices");
+              break;
+            case 6:
+              PyErr_SetString (
+                  DokiError,
+                  "[TRACE] Unknown operation between parent matrices");
+              break;
+            case 7:
+              PyErr_SetString (DokiError, "[TRACE] Element out of bounds");
+              break;
+            case 8:
+              PyErr_SetString (DokiError, "[TRACE] f returned NAN");
+              break;
+            default:
+              PyErr_SetString (DokiError, "[TRACE] Unknown error code");
+            }
+          return NULL;
+        }
+
+      if (isnan (RE (aux)) || isnan (IM (aux)))
+        {
+          PyErr_SetString (DokiError, "[TRACE] Unexpected NAN value");
+          return NULL;
+        }
+      result = COMPLEX_ADD (result, aux);
+    }
+
+  return PyComplex_FromDoubles (RE (result), IM (result));
+}
+
+static PyObject *
+doki_funmatrix_apply (PyObject *self, PyObject *args)
+{
+  PyObject *raw_val, *state_capsule, *gate_capsule, *target_list, *control_set,
+      *acontrol_set, *aux;
+  void *raw_state, *raw_gate;
+  struct FMatrix *state, *new_state, *gate;
+  unsigned int num_targets, num_controls, num_anticontrols, num_qubits,
+      num_qb_gate, i;
+  unsigned int *targets, *controls, *anticontrols;
+  bool debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "OOOOOp", &state_capsule, &gate_capsule,
+                         &target_list, &control_set, &acontrol_set,
+                         &debug_enabled))
+    {
+      PyErr_SetString (DokiError,
+                       "Syntax: funmatrix_apply(registry, gate, target_list, "
+                       "control_set, anticontrol_set, verbose)");
+      return NULL;
+    }
+
+  raw_state = PyCapsule_GetPointer (state_capsule, "qsimov.doki.funmatrix");
+  if (raw_state == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry");
+      return NULL;
+    }
+  state = (struct FMatrix *)raw_state;
+
+  raw_gate = PyCapsule_GetPointer (gate_capsule, "qsimov.doki.funmatrix");
+  if (raw_gate == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to gate");
+      return NULL;
+    }
+  gate = (struct FMatrix *)raw_gate;
+
+  if (state->c > 1)
+    {
+      PyErr_SetString (DokiError, "registry is not a column vector");
+      return NULL;
+    }
+
+  if (gate->c != gate->r)
+    {
+      PyErr_SetString (DokiError, "gates have to be square matrices");
+      return NULL;
+    }
+
+  if (gate->r > state->r)
+    {
+      PyErr_SetString (DokiError, "gate is too big for this state vector");
+      return NULL;
+    }
+
+  num_qubits = log2_64 (state->r);
+  if (state->r != NATURAL_ONE << num_qubits)
+    {
+      PyErr_SetString (DokiError, "registry needs 2^n rows");
+      return NULL;
+    }
+
+  num_qb_gate = log2_64 (gate->r);
+  if (gate->r != NATURAL_ONE << num_qb_gate)
+    {
+      PyErr_SetString (DokiError, "gates need 2^n x 2^n elements");
+      return NULL;
+    }
+
+  if (!PyList_Check (target_list))
+    {
+      PyErr_SetString (DokiError, "target_list must be a list");
+      return NULL;
+    }
+
+  num_targets = (unsigned int)PyList_Size (target_list);
+  if (num_targets != num_qb_gate)
+    {
+      PyErr_SetString (DokiError,
+                       "Wrong number of targets specified for that gate");
+      return NULL;
+    }
+
+  num_controls = 0;
+  if (PySet_Check (control_set))
+    {
+      num_controls = (unsigned int)PySet_Size (control_set);
+    }
+  else if (control_set != Py_None)
+    {
+      PyErr_SetString (DokiError, "control_set must be a set or None");
+      return NULL;
+    }
+
+  num_anticontrols = 0;
+  if (PySet_Check (acontrol_set))
+    {
+      num_anticontrols = (unsigned int)PySet_Size (acontrol_set);
+    }
+  else if (acontrol_set != Py_None)
+    {
+      PyErr_SetString (DokiError, "anticontrol_set must be a set or None");
+      return NULL;
+    }
+
+  targets = MALLOC_TYPE (num_targets, unsigned int);
+  if (targets == NULL)
+    {
+      PyErr_SetString (DokiError, "Failed to allocate target array");
+      return NULL;
+    }
+  controls = NULL;
+  if (num_controls > 0)
+    {
+      controls = MALLOC_TYPE (num_controls, unsigned int);
+      if (controls == NULL)
+        {
+          PyErr_SetString (DokiError, "Failed to allocate control array");
+          return NULL;
+        }
+    }
+  anticontrols = NULL;
+  if (num_anticontrols > 0)
+    {
+      anticontrols = MALLOC_TYPE (num_anticontrols, unsigned int);
+      if (anticontrols == NULL)
+        {
+          PyErr_SetString (DokiError, "Failed to allocate anticontrol array");
+          return NULL;
+        }
+    }
+
+  if (num_controls > 0)
+    {
+      aux = PySet_New (control_set);
+      for (i = 0; i < num_controls; i++)
+        {
+          raw_val = PySet_Pop (aux);
+          if (!PyLong_Check (raw_val))
+            {
+              PyErr_SetString (
+                  DokiError,
+                  "control_set must be a set qubit ids (unsigned integers)");
+              return NULL;
+            }
+          controls[i] = PyLong_AsLong (raw_val);
+          if (controls[i] >= num_qubits)
+            {
+              PyErr_SetString (DokiError, "Control qubit out of range");
+              return NULL;
+            }
+        }
+    }
+
+  if (num_anticontrols > 0)
+    {
+      aux = PySet_New (acontrol_set);
+      for (i = 0; i < num_anticontrols; i++)
+        {
+          raw_val = PySet_Pop (aux);
+          if (!PyLong_Check (raw_val))
+            {
+              PyErr_SetString (DokiError, "anticontrol_set must be a set "
+                                          "qubit ids (unsigned integers)");
+              return NULL;
+            }
+          if (PySet_Contains (control_set, raw_val))
+            {
+              PyErr_SetString (DokiError,
+                               "A control cannot also be an anticontrol");
+              return NULL;
+            }
+          anticontrols[i] = PyLong_AsLong (raw_val);
+          if (anticontrols[i] >= num_qubits)
+            {
+              PyErr_SetString (DokiError, "Anticontrol qubit out of range");
+              return NULL;
+            }
+        }
+    }
+
+  for (i = 0; i < num_targets; i++)
+    {
+      raw_val = PyList_GetItem (target_list, i);
+      if (!PyLong_Check (raw_val))
+        {
+          PyErr_SetString (
+              DokiError,
+              "target_list must be a list of qubit ids (unsigned integers)");
+          return NULL;
+        }
+      if ((num_controls > 0 && PySet_Contains (control_set, raw_val))
+          || (num_anticontrols > 0 && PySet_Contains (acontrol_set, raw_val)))
+        {
+          PyErr_SetString (
+              DokiError,
+              "A target cannot also be a control or an anticontrol");
+          return NULL;
+        }
+      targets[i] = PyLong_AsLong (raw_val);
+      if (targets[i] >= num_qubits)
+        {
+          PyErr_SetString (DokiError, "Target qubit out of range");
+          return NULL;
+        }
+    }
+
+  new_state = apply_gate_fmat (state_capsule, gate_capsule, targets,
+                               num_targets, controls, num_controls,
+                               anticontrols, num_anticontrols);
+
+  if (new_state == NULL)
+    {
+      switch (errno)
+        {
+        case 1:
+          PyErr_SetString (DokiError, "[FMAPPLY] Failed to allocate matrix");
+          break;
+        case 5:
+          PyErr_SetString (DokiError,
+                           "[FMAPPLY] Failed to allocate data struct");
+          break;
+        default:
+          PyErr_SetString (DokiError, "[FMAPPLY] Unknown error code");
+        }
+      free (targets);
+      if (num_controls > 0)
+        {
+          free (controls);
+        }
+      if (num_anticontrols > 0)
+        {
+          free (anticontrols);
         }
-        result = complex_sum(result, aux);
+      return NULL;
     }
 
-    return PyComplex_FromDoubles(RE(result), IM(result));
+  return PyCapsule_New ((void *)new_state, "qsimov.doki.funmatrix",
+                        &doki_funmatrix_destroy);
 }
```

### Comparing `doki-Mowstyl-1.4.0/src/doki/qops.h` & `doki-Mowstyl-1.5.0/src/doki/qops.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,56 @@
-#ifndef __QOPS_H
-#define __QOPS_H
+#pragma once
+#ifndef QOPS_H_
+#define QOPS_H_
 
 #include "arraylist.h"
-#include "qstate.h"
-#include "qgate.h"
 #include "funmatrix.h"
+#include "qgate.h"
+#include "qstate.h"
+#include <Python.h>
 
-unsigned char
-join(struct state_vector *r, struct state_vector *s1, struct state_vector *s2);
+unsigned char join (struct state_vector *r, struct state_vector *s1,
+                    struct state_vector *s2);
 
-unsigned char
-measure(struct state_vector *state, _Bool *result, unsigned int target,
-        struct state_vector *new_state, REAL_TYPE roll);
+unsigned char measure (struct state_vector *state, _Bool *result,
+                       unsigned int target, struct state_vector *new_state,
+                       REAL_TYPE roll);
 
 REAL_TYPE
-probability(struct state_vector *state, unsigned int target_id);
+probability (struct state_vector *state, unsigned int target_id);
 
 REAL_TYPE
-get_global_phase(struct state_vector *state);
+get_global_phase (struct state_vector *state);
 
-unsigned char
-collapse(struct state_vector *state, unsigned int id, _Bool value,
-         struct state_vector *new_state);
-
-unsigned char
-apply_gate(struct state_vector *state, struct qgate *gate,
-           unsigned int *targets, unsigned int num_targets,
-           unsigned int *controls, unsigned int num_controls,
-           unsigned int *anticontrols, unsigned int num_anticontrols,
-           struct state_vector *new_state);
+unsigned char collapse (struct state_vector *state, unsigned int id,
+                        _Bool value, struct state_vector *new_state);
 
-unsigned char
-copy_and_index(struct state_vector *state, struct state_vector *new_state,
-               unsigned int *controls, unsigned int num_controls,
-               unsigned int *anticontrols, unsigned int num_anticontrols,
-               REAL_TYPE *norm_const, struct array_list_e *not_copy);
+unsigned char apply_gate (struct state_vector *state, struct qgate *gate,
+                          unsigned int *targets, unsigned int num_targets,
+                          unsigned int *controls, unsigned int num_controls,
+                          unsigned int *anticontrols,
+                          unsigned int num_anticontrols,
+                          struct state_vector *new_state);
 
 unsigned char
-calculate_empty(struct state_vector *state, struct qgate *gate,
-                unsigned int *targets, unsigned int num_targets,
+copy_and_index (struct state_vector *state, struct state_vector *new_state,
                 unsigned int *controls, unsigned int num_controls,
                 unsigned int *anticontrols, unsigned int num_anticontrols,
-                struct state_vector *new_state, struct array_list_e *not_copy,
-                REAL_TYPE *norm_const);
+                REAL_TYPE *norm_const, struct array_list_e *not_copy);
+
+unsigned char
+calculate_empty (struct state_vector *state, struct qgate *gate,
+                 unsigned int *targets, unsigned int num_targets,
+                 unsigned int *controls, unsigned int num_controls,
+                 unsigned int *anticontrols, unsigned int num_anticontrols,
+                 struct state_vector *new_state, struct array_list_e *not_copy,
+                 REAL_TYPE *norm_const);
 
-#ifndef _MSC_VER
-__attribute__ ((const))
-#endif
-COMPLEX_TYPE
-_densityFun(NATURAL_TYPE i, NATURAL_TYPE j,
-            #ifndef _MSC_VER
-            NATURAL_TYPE unused1 __attribute__((unused)), NATURAL_TYPE unused2 __attribute__((unused)),
-            #else
-            NATURAL_TYPE unused1, NATURAL_TYPE unused2,
-            #endif
-            void *rawstate);
+struct FMatrix *
+apply_gate_fmat (PyObject *state_capsule, PyObject *gate_capsule,
+                 unsigned int *targets, unsigned int num_targets,
+                 unsigned int *controls, unsigned int num_controls,
+                 unsigned int *anticontrols, unsigned int num_anticontrols);
 
-FunctionalMatrix*
-densityMat(struct state_vector *state);
+struct FMatrix *density_matrix (PyObject *state_capsule);
 
-#endif
+#endif /* QOPS_H_ */
```

### Comparing `doki-Mowstyl-1.4.0/src/doki/qstate.c` & `doki-Mowstyl-1.5.0/src/doki/qstate.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,139 @@
-#include "platform.h"
 #include "qstate.h"
-
+#include "platform.h"
 
 unsigned char
-state_init(struct state_vector *this, unsigned int num_qubits, int init)
+state_init (struct state_vector *this, unsigned int num_qubits, int init)
 {
-    size_t i, offset, errored_chunk;
-    _Bool errored;
+  size_t i, offset, errored_chunk;
+  _Bool errored;
 
-    if (num_qubits > MAX_NUM_QUBITS) {
-        return 3;
-    }
-    this->size = NATURAL_ONE << num_qubits;
-    this->fcarg_init = 0;
-    this->fcarg = -10.0;
-    this->num_qubits = num_qubits;
-    this->norm_const = 1;
-    this->num_chunks = this->size / COMPLEX_ARRAY_SIZE;
-    offset = this->size % COMPLEX_ARRAY_SIZE;
-    if (offset > 0) {
-        this->num_chunks++;
-    }
-    else {
-        offset = COMPLEX_ARRAY_SIZE;
-    }
-    this->vector = MALLOC_TYPE(this->num_chunks, COMPLEX_TYPE*);
-    if (this->vector == NULL) {
-        return 1;
-    }
-    errored = 0;
-    for (i = 0; i < this->num_chunks - 1; i++) {
-        if (init) {
-            this->vector[i] = CALLOC_TYPE(COMPLEX_ARRAY_SIZE, COMPLEX_TYPE);
-        }
-        else {
-            this->vector[i] = MALLOC_TYPE(COMPLEX_ARRAY_SIZE, COMPLEX_TYPE);
-        }
-        if (this->vector[i] == NULL) {
-            errored_chunk = i;
-            errored = 1;
-            break;
-        }
-    }
-    if (!errored) {
-        if (init) {
-            this->vector[this->num_chunks-1] = CALLOC_TYPE(offset, COMPLEX_TYPE);
-        }
-        else {
-            this->vector[this->num_chunks-1] = MALLOC_TYPE(offset, COMPLEX_TYPE);
-        }
-        if (this->vector[this->num_chunks-1] == NULL) {
-            errored = 1;
-            errored_chunk = this->num_chunks-1;
-        }
-    }
-    if (errored) {
-        for (i = 0; i < errored_chunk; i++) {
-            free(this->vector[i]);
-        }
-        free(this->vector);
-        return 2;
-    }
-    if (init) {
-        this->vector[0][0] = COMPLEX_ONE;
+  if (num_qubits > MAX_NUM_QUBITS)
+    {
+      return 3;
+    }
+  this->size = NATURAL_ONE << num_qubits;
+  this->fcarg_init = 0;
+  this->fcarg = -10.0;
+  this->num_qubits = num_qubits;
+  this->norm_const = 1;
+  this->num_chunks = this->size / COMPLEX_ARRAY_SIZE;
+  offset = this->size % COMPLEX_ARRAY_SIZE;
+  if (offset > 0)
+    {
+      this->num_chunks++;
+    }
+  else
+    {
+      offset = COMPLEX_ARRAY_SIZE;
+    }
+  this->vector = MALLOC_TYPE (this->num_chunks, COMPLEX_TYPE *);
+  if (this->vector == NULL)
+    {
+      return 1;
+    }
+  errored = 0;
+  for (i = 0; i < this->num_chunks - 1; i++)
+    {
+      if (init)
+        {
+          this->vector[i] = CALLOC_TYPE (COMPLEX_ARRAY_SIZE, COMPLEX_TYPE);
+        }
+      else
+        {
+          this->vector[i] = MALLOC_TYPE (COMPLEX_ARRAY_SIZE, COMPLEX_TYPE);
+        }
+      if (this->vector[i] == NULL)
+        {
+          errored_chunk = i;
+          errored = 1;
+          break;
+        }
+    }
+  if (!errored)
+    {
+      if (init)
+        {
+          this->vector[this->num_chunks - 1]
+              = CALLOC_TYPE (offset, COMPLEX_TYPE);
+        }
+      else
+        {
+          this->vector[this->num_chunks - 1]
+              = MALLOC_TYPE (offset, COMPLEX_TYPE);
+        }
+      if (this->vector[this->num_chunks - 1] == NULL)
+        {
+          errored = 1;
+          errored_chunk = this->num_chunks - 1;
+        }
+    }
+  if (errored)
+    {
+      for (i = 0; i < errored_chunk; i++)
+        {
+          free (this->vector[i]);
+        }
+      free (this->vector);
+      return 2;
+    }
+  if (init)
+    {
+      this->vector[0][0] = COMPLEX_ONE;
     }
 
-    return 0;
+  return 0;
 }
 
-
 unsigned char
-state_clone(struct state_vector *dest, struct state_vector *source)
+state_clone (struct state_vector *dest, struct state_vector *source)
 {
-    NATURAL_TYPE i;
-    unsigned char exit_code;
-    exit_code = state_init(dest, source->num_qubits, 0);
-    if (exit_code != 0) {
-        return exit_code;
-    }
-    #pragma omp parallel for default(none) \
-                             shared (source, dest, exit_code) \
-                             private (i)
-    for (i = 0; i < source->size; i++) {
-        dest->vector[i/COMPLEX_ARRAY_SIZE][i%COMPLEX_ARRAY_SIZE] = state_get(source, i);
+  NATURAL_TYPE i;
+  unsigned char exit_code;
+  exit_code = state_init (dest, source->num_qubits, 0);
+  if (exit_code != 0)
+    {
+      return exit_code;
+    }
+#pragma omp parallel for default(none)                                        \
+    shared(source, dest, exit_code) private(i)
+  for (i = 0; i < source->size; i++)
+    {
+      dest->vector[i / COMPLEX_ARRAY_SIZE][i % COMPLEX_ARRAY_SIZE]
+          = state_get (source, i);
     }
-    return 0;
+  return 0;
 }
 
-
 void
-state_clear(struct state_vector *this)
+state_clear (struct state_vector *this)
 {
-    size_t i;
-    if (this->vector != NULL) {
-        for (i = 0; i < this->num_chunks; i++) {
-            free(this->vector[i]);
-        }
-        free(this->vector);
-    }
-    this->vector = NULL;
-    this->num_chunks = 0;
-    this->num_qubits = 0;
-    this->size = 0;
-    this->norm_const = 0.0;
+  size_t i;
+  if (this->vector != NULL)
+    {
+      for (i = 0; i < this->num_chunks; i++)
+        {
+          free (this->vector[i]);
+        }
+      free (this->vector);
+    }
+  this->vector = NULL;
+  this->num_chunks = 0;
+  this->num_qubits = 0;
+  this->size = 0;
+  this->norm_const = 0.0;
 }
 
 void
-state_set(struct state_vector *this, NATURAL_TYPE i, COMPLEX_TYPE value)
+state_set (struct state_vector *this, NATURAL_TYPE i, COMPLEX_TYPE value)
 {
-    this->vector[i/COMPLEX_ARRAY_SIZE][i%COMPLEX_ARRAY_SIZE] = value;
+  this->vector[i / COMPLEX_ARRAY_SIZE][i % COMPLEX_ARRAY_SIZE] = value;
 }
 
-
 COMPLEX_TYPE
-state_get(struct state_vector *this, NATURAL_TYPE i)
+state_get (struct state_vector *this, NATURAL_TYPE i)
 {
-    COMPLEX_TYPE val;
-    val = complex_div_r(this->vector[i/COMPLEX_ARRAY_SIZE][i%COMPLEX_ARRAY_SIZE], this->norm_const);
-    return fix_value(val, -1, -1, 1, 1);
+  COMPLEX_TYPE val = COMPLEX_DIV_R (
+      this->vector[i / COMPLEX_ARRAY_SIZE][i % COMPLEX_ARRAY_SIZE],
+      this->norm_const);
+  return fix_value (val, -1, -1, 1, 1);
 }
```

### Comparing `doki-Mowstyl-1.4.0/src/doki/qstate.h` & `doki-Mowstyl-1.5.0/src/doki/qstate.h`

 * *Files 7% similar despite different names*

```diff
@@ -12,59 +12,60 @@
  */
 
 /** \struct array_list qstate.h "qstate.h"
  *  \brief List of complex number arrays.
  *  A list of complex number arrays (chunks).
  */
 
-#ifndef __QSTATE_H
-#define __QSTATE_H
+#pragma once
+#ifndef QSTATE_H_
+#define QSTATE_H_
 
 #include "platform.h"
 
 struct state_vector
 {
-    /* total size of the vector */
-    NATURAL_TYPE   size;
-    /* number of chunks */
-    size_t         num_chunks;
-    /* number of qubits in this quantum system */
-    unsigned int   num_qubits;
-    /* partial vector */
-    COMPLEX_TYPE **vector;
-    /* normalization constant */
-    REAL_TYPE      norm_const;
-    /* fcarg initialized */
-    _Bool          fcarg_init;
-    /* first complex argument */
-    REAL_TYPE      fcarg;
+  /* total size of the vector */
+  NATURAL_TYPE size;
+  /* number of chunks */
+  size_t num_chunks;
+  /* number of qubits in this quantum system */
+  unsigned int num_qubits;
+  /* partial vector */
+  COMPLEX_TYPE **vector;
+  /* normalization constant */
+  REAL_TYPE norm_const;
+  /* fcarg initialized */
+  _Bool fcarg_init;
+  /* first complex argument */
+  REAL_TYPE fcarg;
 };
 
-/** \fn unsigned char state_init(struct state_vector *this, unsigned int num_qubits, int init);
- *  \brief Initialize a state vector structure.
- *  \param this Pointer to an already allocated state_vector structure.
- *  \param num_qubits The number of qubits represented by this state (a maximum of MAX_NUM_QUBITS).
- *  \param init Whether to initialize to {1, 0, ..., 0} or not.
- *  \return 0 if ok, 1 if failed to allocate vector, 2 if failed to allocate any chunk, 3 if num_qubits > MAX_NUM_QUBITS.
+/** \fn unsigned char state_init(struct state_vector *this, unsigned int
+ * num_qubits, int init); \brief Initialize a state vector structure. \param
+ * this Pointer to an already allocated state_vector structure. \param
+ * num_qubits The number of qubits represented by this state (a maximum of
+ * MAX_NUM_QUBITS). \param init Whether to initialize to {1, 0, ..., 0} or not.
+ *  \return 0 if ok, 1 if failed to allocate vector, 2 if failed to allocate
+ * any chunk, 3 if num_qubits > MAX_NUM_QUBITS.
  */
-unsigned char
-state_init(struct state_vector *this, unsigned int num_qubits, int init);
+unsigned char state_init (struct state_vector *this, unsigned int num_qubits,
+                          int init);
 
-/** \fn unsigned char state_clone(struct state_vector *dest, struct state_vector *source);
- *  \brief Clone a state vector structure.
- *  \param dest Pointer to an already allocated state_vector structure i which the copy will be stored.
- *  \param source Pointer to the state_vector structure that has to be cloned.
- *  \return 0 if ok, 1 if failed to allocate dest vector, 2 if failed to allocate any chunk.
+/** \fn unsigned char state_clone(struct state_vector *dest, struct
+ * state_vector *source); \brief Clone a state vector structure. \param dest
+ * Pointer to an already allocated state_vector structure i which the copy will
+ * be stored. \param source Pointer to the state_vector structure that has to
+ * be cloned. \return 0 if ok, 1 if failed to allocate dest vector, 2 if failed
+ * to allocate any chunk.
  */
-unsigned char
-state_clone(struct state_vector *dest, struct state_vector *source);
+unsigned char state_clone (struct state_vector *dest,
+                           struct state_vector *source);
 
-void
-state_clear(struct state_vector *this);
+void state_clear (struct state_vector *this);
 
-void
-state_set(struct state_vector *this, NATURAL_TYPE i, COMPLEX_TYPE value);
+void state_set (struct state_vector *this, NATURAL_TYPE i, COMPLEX_TYPE value);
 
 COMPLEX_TYPE
-state_get(struct state_vector *this, NATURAL_TYPE i);
+state_get (struct state_vector *this, NATURAL_TYPE i);
 
-#endif
+#endif /* QSTATE_H_ */
```

