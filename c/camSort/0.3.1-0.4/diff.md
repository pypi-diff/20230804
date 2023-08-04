# Comparing `tmp/camSort-0.3.1.tar.gz` & `tmp/camSort-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/camSort-0.3.1.tar", last modified: Thu Aug  3 14:36:08 2023, max compression
+gzip compressed data, was "dist/camSort-0.4.tar", last modified: Fri Aug  4 10:43:05 2023, max compression
```

## Comparing `camSort-0.3.1.tar` & `camSort-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 14:36:08.000000 camSort-0.3.1/
--rw-r--r--   0 macbook    (501) staff       (20)     3079 2023-08-03 14:36:08.000000 camSort-0.3.1/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     2064 2023-08-03 14:34:20.000000 camSort-0.3.1/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 14:36:08.000000 camSort-0.3.1/camSort/
--rw-r--r--   0 macbook    (501) staff       (20)   347097 2023-08-03 14:36:07.000000 camSort-0.3.1/camSort/stringSort.c
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 14:36:08.000000 camSort-0.3.1/camSort.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     3079 2023-08-03 14:36:07.000000 camSort-0.3.1/camSort.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      208 2023-08-03 14:36:07.000000 camSort-0.3.1/camSort.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-03 14:36:07.000000 camSort-0.3.1/camSort.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       24 2023-08-03 14:36:07.000000 camSort-0.3.1/camSort.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-03 14:36:07.000000 camSort-0.3.1/camSort.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       99 2023-08-02 08:57:15.000000 camSort-0.3.1/pyproject.toml
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-03 14:36:08.000000 camSort-0.3.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1073 2023-08-03 14:34:29.000000 camSort-0.3.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-04 10:43:05.000000 camSort-0.4/
+-rw-r--r--   0 macbook    (501) staff       (20)     4024 2023-08-04 10:43:05.000000 camSort-0.4/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     2875 2023-08-04 10:38:00.000000 camSort-0.4/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-04 10:43:05.000000 camSort-0.4/camSort/
+-rw-r--r--   0 macbook    (501) staff       (20)   337230 2023-08-04 10:43:04.000000 camSort-0.4/camSort/stringSort.c
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-04 10:43:05.000000 camSort-0.4/camSort.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     4024 2023-08-04 10:43:05.000000 camSort-0.4/camSort.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      208 2023-08-04 10:43:05.000000 camSort-0.4/camSort.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-04 10:43:05.000000 camSort-0.4/camSort.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       24 2023-08-04 10:43:05.000000 camSort-0.4/camSort.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-04 10:43:05.000000 camSort-0.4/camSort.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       99 2023-08-02 08:57:15.000000 camSort-0.4/pyproject.toml
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-04 10:43:05.000000 camSort-0.4/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1071 2023-08-04 10:42:58.000000 camSort-0.4/setup.py
```

### Comparing `camSort-0.3.1/README.md` & `camSort-0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# camSort 0.3.1!
+# camSort 0.4!
 
 Working on `python 3.7.3`! (at least I think.)
 
 `camSort` is a Python library that makes sorted() look slow while also using sorted(). It's built on Cython, and provides preallocation to string sorting by using a custom key calculation for each string. Normal key calculation and object creation are often computationally expensive—but here we optimize that with Cython >:)!
 
 ## Overview
 
 The `camSort` library sorts a list of strings by creating a custom object for each string. This custom object, `StringWithKey`, holds the string and a unique key calculated from it. The key is a long integer derived from the sum of Unicode code points of the characters in the string, and the string's length.
 
 The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
 
-The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
+The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance.
 
 ## Installation
 
 ```pip install camSort```, or build locally :)
 
 ## Usage
 
@@ -28,24 +28,41 @@
 # By alphabetically
 sortedStringsCam = stringSort.byAlphabet(myList)
 # By sorting alphabetically and length
 sortedStringsCam = stringSort.byLengthAndAlphabet(myList)
 # Reversing! (This is the exact same as Python's)
 # Please read the demo.py file for an explaination.
 sortedStringsCam = stringSort.byLength(myList).reverse()
+# Returns a list of strings that contain a given substring/key, this is list comprehension.
+# Speed increase will be looked at in future.
+filteredStrings = sortedStringsCam.filterWithSubstring('hello'))
 
 ```
 
 ## Performance
 
 Try out the demo.py file!
 
 Average output on my 2017 macbook pro:
     (1 million strings, with a random legnth of 1 to 1000 chararacters)
 
 ```
-Time taken by Python sorted():               57.62033486366272 seconds
+Time taken by Python sorted():               56.833308935165405 seconds
     Using camSort!
-Time taken sorting by length:                7.040294170379639 seconds
-By sorting alphabetically:                   3.804348945617676 seconds
-By sorting alphabetically and length:        7.213421821594238 seconds
+Time taken sorting by length:                5.0397491455078125 seconds
+By sorting alphabetically:                   4.070678949356079 seconds
+By sorting alphabetically and length:        5.39140510559082 seconds
+
+Results on 0.4.
+
+Python reverse:                              5.470452070236206 seconds
+Camsort Reverse:                             5.303014755249023 seconds
+Using python list comprehension:             0.5422248840332031 seconds
+Using filterWithSubstring:                   0.6661787033081055 seconds
+
+Results pre 0.4.
+
+Python reverse:                              5.526482105255127 seconds
+Camsort reverse:                             5.083630084991455 seconds
+Using Python's list comprehension:           0.4732799530029297 seconds
+Using filterWithSubstring:                   0.38806891441345215 seconds
 ```
```

### Comparing `camSort-0.3.1/camSort/stringSort.c` & `camSort-0.4/camSort/stringSort.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 /* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "depends": [],
         "name": "camSort.stringSort",
         "sources": [
             "camSort/stringSort.pyx"
         ]
     },
     "module_name": "camSort.stringSort"
 }
@@ -614,16 +613,14 @@
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
 #define __PYX_HAVE__camSort__stringSort
 #define __PYX_HAVE_API__camSort__stringSort
 /* Early includes */
-#include <string.h>
-#include <stdlib.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -832,46 +829,45 @@
   "stringsource",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7camSort_10stringSort_StringWithKey;
 struct __pyx_obj_7camSort_10stringSort_SortedList;
 
-/* "camSort/stringSort.pyx":7
+/* "camSort/stringSort.pyx":5
  * cimport cython
  * 
  * cdef class StringWithKey:             # <<<<<<<<<<<<<<
  *     cdef public:
  *         str str
  */
 struct __pyx_obj_7camSort_10stringSort_StringWithKey {
   PyObject_HEAD
   struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *__pyx_vtab;
   PyObject *str;
   PyObject *key;
 };
 
 
-/* "camSort/stringSort.pyx":36
+/* "camSort/stringSort.pyx":34
  * 
  * 
  * cdef class SortedList:             # <<<<<<<<<<<<<<
  *     cdef:
- *         char **str_list
+ *         list str_list
  */
 struct __pyx_obj_7camSort_10stringSort_SortedList {
   PyObject_HEAD
   struct __pyx_vtabstruct_7camSort_10stringSort_SortedList *__pyx_vtab;
-  char **str_list;
-  size_t size;
+  PyObject *str_list;
 };
 
 
 
-/* "camSort/stringSort.pyx":7
+/* "camSort/stringSort.pyx":5
  * cimport cython
  * 
  * cdef class StringWithKey:             # <<<<<<<<<<<<<<
  *     cdef public:
  *         str str
  */
 
@@ -879,24 +875,25 @@
   PY_LONG_LONG (*calculate_key)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
   PyObject *(*calculate_key_alpha)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
   PY_LONG_LONG (*calculate_key_length_alpha)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
 };
 static struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *__pyx_vtabptr_7camSort_10stringSort_StringWithKey;
 
 
-/* "camSort/stringSort.pyx":36
+/* "camSort/stringSort.pyx":34
  * 
  * 
  * cdef class SortedList:             # <<<<<<<<<<<<<<
  *     cdef:
- *         char **str_list
+ *         list str_list
  */
 
 struct __pyx_vtabstruct_7camSort_10stringSort_SortedList {
   struct __pyx_obj_7camSort_10stringSort_SortedList *(*reverse)(struct __pyx_obj_7camSort_10stringSort_SortedList *, int __pyx_skip_dispatch);
+  PyObject *(*filterWithSubstring)(struct __pyx_obj_7camSort_10stringSort_SortedList *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_7camSort_10stringSort_SortedList *__pyx_vtabptr_7camSort_10stringSort_SortedList;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
@@ -978,23 +975,33 @@
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
+/* unicode_iter.proto */
+static CYTHON_INLINE int __Pyx_init_unicode_iteration(
+    PyObject* ustring, Py_ssize_t *length, void** data, int *kind);
+
 /* UnicodeAsUCS4.proto */
 static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject*);
 
 /* object_ord.proto */
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyObject_Ord(c)\
     (likely(PyUnicode_Check(c)) ? (long)__Pyx_PyUnicode_AsPy_UCS4(c) : __Pyx__PyObject_Ord(c))
@@ -1153,19 +1160,25 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* ArgTypeTest.proto */
-#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
-        __Pyx__ArgTypeTest(obj, type, name, exact))
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+/* SliceTupleAndList.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_GetSlice(PyObject* src, Py_ssize_t start, Py_ssize_t stop);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_GetSlice(PyObject* src, Py_ssize_t start, Py_ssize_t stop);
+#else
+#define __Pyx_PyList_GetSlice(seq, start, stop)   PySequence_GetSlice(seq, start, stop)
+#define __Pyx_PyTuple_GetSlice(seq, start, stop)  PySequence_GetSlice(seq, start, stop)
+#endif
+
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
@@ -1181,19 +1194,29 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
+/* ObjectGetItem.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
+#else
+#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
+#endif
+
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
 
 /* ListCompAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
@@ -1204,43 +1227,23 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
 
-/* decode_c_string_utf16.proto */
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = 0;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = -1;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16BE(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = 1;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-
-/* decode_c_string.proto */
-static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
-         const char* cstring, Py_ssize_t start, Py_ssize_t stop,
-         const char* encoding, const char* errors,
-         PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
-
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
@@ -1289,27 +1292,21 @@
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
-/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
-
-/* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
@@ -1326,204 +1323,179 @@
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
 static PyObject *__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_alpha(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
 static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_length_alpha(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
 static struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_f_7camSort_10stringSort_10SortedList_reverse(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
-
-/* Module declarations from 'libc.string' */
-
-/* Module declarations from 'libc.stdlib' */
+static PyObject *__pyx_f_7camSort_10stringSort_10SortedList_filterWithSubstring(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_substring, int __pyx_skip_dispatch); /* proto*/
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'camSort.stringSort' */
 static PyTypeObject *__pyx_ptype_7camSort_10stringSort_StringWithKey = 0;
 static PyTypeObject *__pyx_ptype_7camSort_10stringSort_SortedList = 0;
 static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_StringWithKey__set_state(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *); /*proto*/
+static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_SortedList__set_state(struct __pyx_obj_7camSort_10stringSort_SortedList *, PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "camSort.stringSort"
 extern int __pyx_module_is_main_camSort__stringSort;
 int __pyx_module_is_main_camSort__stringSort = 0;
 
 /* Implementation of 'camSort.stringSort' */
-static PyObject *__pyx_builtin_MemoryError;
-static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_IndexError;
-static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_sorted;
-static const char __pyx_k_n[] = "n";
 static const char __pyx_k_s[] = "s";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_str[] = "str";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
-static const char __pyx_k_step[] = "step";
-static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_alpha[] = "alpha";
 static const char __pyx_k_array[] = "array";
+static const char __pyx_k_byKey[] = "byKey";
 static const char __pyx_k_lower[] = "lower";
-static const char __pyx_k_range[] = "range";
-static const char __pyx_k_start[] = "start";
-static const char __pyx_k_utf_8[] = "utf-8";
-static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_length[] = "length";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_sorted[] = "sorted";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_py_list[] = "py_list";
 static const char __pyx_k_reverse[] = "reverse";
 static const char __pyx_k_byLength[] = "byLength";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_key_type[] = "key_type";
 static const char __pyx_k_operator[] = "operator";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
-static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
-static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_SortedList[] = "SortedList";
 static const char __pyx_k_attrgetter[] = "attrgetter";
 static const char __pyx_k_byAlphabet[] = "byAlphabet";
 static const char __pyx_k_input_list[] = "input_list";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
-static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_sorted_array[] = "sorted_array";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_StringWithKey[] = "StringWithKey";
-static const char __pyx_k_decode_string[] = "__decode_string";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_length_and_alpha[] = "length_and_alpha";
 static const char __pyx_k_camSort_stringSort[] = "camSort.stringSort";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_byLengthAndAlphabet[] = "byLengthAndAlphabet";
-static const char __pyx_k_Invalid_argument_type[] = "Invalid argument type.";
+static const char __pyx_k_filterWithSubstring[] = "filterWithSubstring";
 static const char __pyx_k_camSort_stringSort_pyx[] = "camSort/stringSort.pyx";
+static const char __pyx_k_pyx_unpickle_SortedList[] = "__pyx_unpickle_SortedList";
 static const char __pyx_k_pyx_unpickle_StringWithKey[] = "__pyx_unpickle_StringWithKey";
-static const char __pyx_k_PyStringList_index_out_of_range[] = "PyStringList index out of range";
+static const char __pyx_k_Incompatible_checksums_s_vs_0x2c[] = "Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0xef[] = "Incompatible checksums (%s vs 0xef4e75e = (key, str))";
-static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
+static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x2c;
 static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xef;
-static PyObject *__pyx_n_s_IndexError;
-static PyObject *__pyx_kp_u_Invalid_argument_type;
-static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_n_s_PickleError;
-static PyObject *__pyx_kp_u_PyStringList_index_out_of_range;
 static PyObject *__pyx_n_s_SortedList;
 static PyObject *__pyx_n_s_StringWithKey;
-static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_u_alpha;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_attrgetter;
 static PyObject *__pyx_n_s_byAlphabet;
+static PyObject *__pyx_n_s_byKey;
 static PyObject *__pyx_n_s_byLength;
 static PyObject *__pyx_n_s_byLengthAndAlphabet;
 static PyObject *__pyx_n_s_camSort_stringSort;
 static PyObject *__pyx_kp_s_camSort_stringSort_pyx;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_decode_string;
 static PyObject *__pyx_n_s_dict;
-static PyObject *__pyx_n_s_encode;
+static PyObject *__pyx_n_s_filterWithSubstring;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_input_list;
 static PyObject *__pyx_n_s_key;
 static PyObject *__pyx_n_u_key;
 static PyObject *__pyx_n_s_key_type;
 static PyObject *__pyx_n_u_length;
 static PyObject *__pyx_n_u_length_and_alpha;
 static PyObject *__pyx_n_s_lower;
 static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_n;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_new;
-static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_operator;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_py_list;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
+static PyObject *__pyx_n_s_pyx_unpickle_SortedList;
 static PyObject *__pyx_n_s_pyx_unpickle_StringWithKey;
 static PyObject *__pyx_n_s_pyx_vtable;
-static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_reverse;
 static PyObject *__pyx_n_s_s;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_sorted;
 static PyObject *__pyx_n_s_sorted_array;
-static PyObject *__pyx_n_s_start;
-static PyObject *__pyx_n_s_step;
-static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_n_s_str;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_update;
-static PyObject *__pyx_kp_u_utf_8;
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str, PyObject *__pyx_v_key_type); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3str___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3key___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_2__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_4__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_7camSort_10stringSort_10SortedList___cinit__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_py_list); /* proto */
-static void __pyx_pf_7camSort_10stringSort_10SortedList_2__dealloc__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_4reverse(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_6to_list(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_8__decode_string(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, int __pyx_v_i); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_10__getitem__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
-static Py_ssize_t __pyx_pf_7camSort_10stringSort_10SortedList_12__len__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_byLength(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_2byLengthAndAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_4byAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_6__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_7camSort_10stringSort_10SortedList___init__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_py_list); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_2reverse(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_4to_list(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_6__getitem__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
+static Py_ssize_t __pyx_pf_7camSort_10stringSort_10SortedList_8__len__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_10filterWithSubstring(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_substring); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_12__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_14__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_byKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list, PyObject *__pyx_v_key_type); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_2byLength(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_4byLengthAndAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_6byAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_8__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10__pyx_unpickle_SortedList(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_7camSort_10stringSort_StringWithKey(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_7camSort_10stringSort_SortedList(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_int_0;
+static PyObject *__pyx_int_46947008;
 static PyObject *__pyx_int_250931038;
 static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_codeobj__2;
+static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__6;
 static PyObject *__pyx_codeobj__8;
 static PyObject *__pyx_codeobj__10;
 static PyObject *__pyx_codeobj__12;
 /* Late includes */
 
-/* "camSort/stringSort.pyx":12
+/* "camSort/stringSort.pyx":10
  *         object key
  * 
- *     def __init__(self, str, key_type='length'):             # <<<<<<<<<<<<<<
+ *     def __init__(self, str str, key_type='length'):             # <<<<<<<<<<<<<<
  *         self.str = str
  *         if key_type == 'alpha':
  */
 
 /* Python wrapper */
 static int __pyx_pw_7camSort_10stringSort_13StringWithKey_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7camSort_10stringSort_13StringWithKey_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -1559,323 +1531,297 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_key_type);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 12, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 10, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_str = values[0];
+    __pyx_v_str = ((PyObject*)values[0]);
     __pyx_v_key_type = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 12, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 10, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_str), (&PyUnicode_Type), 1, "str", 1))) __PYX_ERR(0, 10, __pyx_L1_error)
   __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self), __pyx_v_str, __pyx_v_key_type);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = -1;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str, PyObject *__pyx_v_key_type) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "camSort/stringSort.pyx":13
+  /* "camSort/stringSort.pyx":11
  * 
- *     def __init__(self, str, key_type='length'):
+ *     def __init__(self, str str, key_type='length'):
  *         self.str = str             # <<<<<<<<<<<<<<
  *         if key_type == 'alpha':
  *             self.key = self.calculate_key_alpha(str)
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_str))||((__pyx_v_str) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_str)->tp_name), 0))) __PYX_ERR(0, 13, __pyx_L1_error)
-  __pyx_t_1 = __pyx_v_str;
-  __Pyx_INCREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_v_str);
+  __Pyx_GIVEREF(__pyx_v_str);
   __Pyx_GOTREF(__pyx_v_self->str);
   __Pyx_DECREF(__pyx_v_self->str);
-  __pyx_v_self->str = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_v_self->str = __pyx_v_str;
 
-  /* "camSort/stringSort.pyx":14
- *     def __init__(self, str, key_type='length'):
+  /* "camSort/stringSort.pyx":12
+ *     def __init__(self, str str, key_type='length'):
  *         self.str = str
  *         if key_type == 'alpha':             # <<<<<<<<<<<<<<
  *             self.key = self.calculate_key_alpha(str)
  *         elif key_type == 'length_and_alpha':
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_key_type, __pyx_n_u_alpha, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 14, __pyx_L1_error)
-  if (__pyx_t_2) {
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_key_type, __pyx_n_u_alpha, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (__pyx_t_1) {
 
-    /* "camSort/stringSort.pyx":15
+    /* "camSort/stringSort.pyx":13
  *         self.str = str
  *         if key_type == 'alpha':
  *             self.key = self.calculate_key_alpha(str)             # <<<<<<<<<<<<<<
  *         elif key_type == 'length_and_alpha':
  *             self.key = self.calculate_key_length_alpha(str)
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key_alpha(__pyx_v_self, __pyx_v_str); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_1);
+    __pyx_t_2 = ((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key_alpha(__pyx_v_self, __pyx_v_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->key);
     __Pyx_DECREF(__pyx_v_self->key);
-    __pyx_v_self->key = __pyx_t_1;
-    __pyx_t_1 = 0;
+    __pyx_v_self->key = __pyx_t_2;
+    __pyx_t_2 = 0;
 
-    /* "camSort/stringSort.pyx":14
- *     def __init__(self, str, key_type='length'):
+    /* "camSort/stringSort.pyx":12
+ *     def __init__(self, str str, key_type='length'):
  *         self.str = str
  *         if key_type == 'alpha':             # <<<<<<<<<<<<<<
  *             self.key = self.calculate_key_alpha(str)
  *         elif key_type == 'length_and_alpha':
  */
     goto __pyx_L3;
   }
 
-  /* "camSort/stringSort.pyx":16
+  /* "camSort/stringSort.pyx":14
  *         if key_type == 'alpha':
  *             self.key = self.calculate_key_alpha(str)
  *         elif key_type == 'length_and_alpha':             # <<<<<<<<<<<<<<
  *             self.key = self.calculate_key_length_alpha(str)
  *         else:
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_key_type, __pyx_n_u_length_and_alpha, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 16, __pyx_L1_error)
-  if (__pyx_t_2) {
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_key_type, __pyx_n_u_length_and_alpha, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (__pyx_t_1) {
 
-    /* "camSort/stringSort.pyx":17
+    /* "camSort/stringSort.pyx":15
  *             self.key = self.calculate_key_alpha(str)
  *         elif key_type == 'length_and_alpha':
  *             self.key = self.calculate_key_length_alpha(str)             # <<<<<<<<<<<<<<
  *         else:
  *             self.key = self.calculate_key(str)
  */
-    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key_length_alpha(__pyx_v_self, __pyx_v_str)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key_length_alpha(__pyx_v_self, __pyx_v_str)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->key);
     __Pyx_DECREF(__pyx_v_self->key);
-    __pyx_v_self->key = __pyx_t_1;
-    __pyx_t_1 = 0;
+    __pyx_v_self->key = __pyx_t_2;
+    __pyx_t_2 = 0;
 
-    /* "camSort/stringSort.pyx":16
+    /* "camSort/stringSort.pyx":14
  *         if key_type == 'alpha':
  *             self.key = self.calculate_key_alpha(str)
  *         elif key_type == 'length_and_alpha':             # <<<<<<<<<<<<<<
  *             self.key = self.calculate_key_length_alpha(str)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "camSort/stringSort.pyx":19
+  /* "camSort/stringSort.pyx":17
  *             self.key = self.calculate_key_length_alpha(str)
  *         else:
  *             self.key = self.calculate_key(str)             # <<<<<<<<<<<<<<
  * 
- *     cdef long long calculate_key(self, str):
+ *     cdef long long calculate_key(self, str str):
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->key);
     __Pyx_DECREF(__pyx_v_self->key);
-    __pyx_v_self->key = __pyx_t_1;
-    __pyx_t_1 = 0;
+    __pyx_v_self->key = __pyx_t_2;
+    __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "camSort/stringSort.pyx":12
+  /* "camSort/stringSort.pyx":10
  *         object key
  * 
- *     def __init__(self, str, key_type='length'):             # <<<<<<<<<<<<<<
+ *     def __init__(self, str str, key_type='length'):             # <<<<<<<<<<<<<<
  *         self.str = str
  *         if key_type == 'alpha':
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":21
+/* "camSort/stringSort.pyx":19
  *             self.key = self.calculate_key(str)
  * 
- *     cdef long long calculate_key(self, str):             # <<<<<<<<<<<<<<
+ *     cdef long long calculate_key(self, str str):             # <<<<<<<<<<<<<<
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  */
 
 static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
   int __pyx_v_length;
   PY_LONG_LONG __pyx_v_sum;
   PyObject *__pyx_v_c = NULL;
   PY_LONG_LONG __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  long __pyx_t_5;
+  Py_ssize_t __pyx_t_3;
+  void *__pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  long __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_key", 0);
 
-  /* "camSort/stringSort.pyx":22
+  /* "camSort/stringSort.pyx":20
  * 
- *     cdef long long calculate_key(self, str):
+ *     cdef long long calculate_key(self, str str):
  *         cdef int length = len(str)             # <<<<<<<<<<<<<<
  *         cdef long long sum = 0
  *         for c in str:
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_str); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (unlikely(__pyx_v_str == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 20, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_str); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 20, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "camSort/stringSort.pyx":23
- *     cdef long long calculate_key(self, str):
+  /* "camSort/stringSort.pyx":21
+ *     cdef long long calculate_key(self, str str):
  *         cdef int length = len(str)
  *         cdef long long sum = 0             # <<<<<<<<<<<<<<
  *         for c in str:
  *             sum += ord(c)
  */
   __pyx_v_sum = 0;
 
-  /* "camSort/stringSort.pyx":24
+  /* "camSort/stringSort.pyx":22
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  *         for c in str:             # <<<<<<<<<<<<<<
  *             sum += ord(c)
  *         return length * 10000 + sum
  */
-  if (likely(PyList_CheckExact(__pyx_v_str)) || PyTuple_CheckExact(__pyx_v_str)) {
-    __pyx_t_2 = __pyx_v_str; __Pyx_INCREF(__pyx_t_2); __pyx_t_1 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_1 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_2)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 24, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 24, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      }
-    } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_2);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 24, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_4);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_c, __pyx_t_4);
-    __pyx_t_4 = 0;
+  if (unlikely(__pyx_v_str == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
+    __PYX_ERR(0, 22, __pyx_L1_error)
+  }
+  __Pyx_INCREF(__pyx_v_str);
+  __pyx_t_2 = __pyx_v_str;
+  __pyx_t_6 = __Pyx_init_unicode_iteration(__pyx_t_2, (&__pyx_t_3), (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 22, __pyx_L1_error)
+  for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_3; __pyx_t_7++) {
+    __pyx_t_1 = __pyx_t_7;
+    __pyx_t_8 = PyUnicode_FromOrdinal(__Pyx_PyUnicode_READ(__pyx_t_5, __pyx_t_4, __pyx_t_1)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 22, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_XDECREF_SET(__pyx_v_c, __pyx_t_8);
+    __pyx_t_8 = 0;
 
-    /* "camSort/stringSort.pyx":25
+    /* "camSort/stringSort.pyx":23
  *         cdef long long sum = 0
  *         for c in str:
  *             sum += ord(c)             # <<<<<<<<<<<<<<
  *         return length * 10000 + sum
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_Ord(__pyx_v_c); if (unlikely(__pyx_t_5 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 25, __pyx_L1_error)
-    __pyx_v_sum = (__pyx_v_sum + __pyx_t_5);
-
-    /* "camSort/stringSort.pyx":24
- *         cdef int length = len(str)
- *         cdef long long sum = 0
- *         for c in str:             # <<<<<<<<<<<<<<
- *             sum += ord(c)
- *         return length * 10000 + sum
- */
+    __pyx_t_9 = __Pyx_PyObject_Ord(__pyx_v_c); if (unlikely(__pyx_t_9 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 23, __pyx_L1_error)
+    __pyx_v_sum = (__pyx_v_sum + __pyx_t_9);
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":26
+  /* "camSort/stringSort.pyx":24
  *         for c in str:
  *             sum += ord(c)
  *         return length * 10000 + sum             # <<<<<<<<<<<<<<
  * 
- *     cdef object calculate_key_alpha(self, str):
+ *     cdef object calculate_key_alpha(self, str str):
  */
   __pyx_r = ((__pyx_v_length * 0x2710) + __pyx_v_sum);
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":21
+  /* "camSort/stringSort.pyx":19
  *             self.key = self.calculate_key(str)
  * 
- *     cdef long long calculate_key(self, str):             # <<<<<<<<<<<<<<
+ *     cdef long long calculate_key(self, str str):             # <<<<<<<<<<<<<<
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_WriteUnraisable("camSort.stringSort.StringWithKey.calculate_key", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_c);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":28
+/* "camSort/stringSort.pyx":26
  *         return length * 10000 + sum
  * 
- *     cdef object calculate_key_alpha(self, str):             # <<<<<<<<<<<<<<
+ *     cdef object calculate_key_alpha(self, str str):             # <<<<<<<<<<<<<<
  *         return str.lower()
  * 
  */
 
 static PyObject *__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_alpha(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -1883,47 +1829,47 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_key_alpha", 0);
 
-  /* "camSort/stringSort.pyx":29
+  /* "camSort/stringSort.pyx":27
  * 
- *     cdef object calculate_key_alpha(self, str):
+ *     cdef object calculate_key_alpha(self, str str):
  *         return str.lower()             # <<<<<<<<<<<<<<
  * 
- *     cdef long long calculate_key_length_alpha(self, str):
+ *     cdef long long calculate_key_length_alpha(self, str str):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_str, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_str, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":28
+  /* "camSort/stringSort.pyx":26
  *         return length * 10000 + sum
  * 
- *     cdef object calculate_key_alpha(self, str):             # <<<<<<<<<<<<<<
+ *     cdef object calculate_key_alpha(self, str str):             # <<<<<<<<<<<<<<
  *         return str.lower()
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -1933,70 +1879,74 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":31
+/* "camSort/stringSort.pyx":29
  *         return str.lower()
  * 
- *     cdef long long calculate_key_length_alpha(self, str):             # <<<<<<<<<<<<<<
+ *     cdef long long calculate_key_length_alpha(self, str str):             # <<<<<<<<<<<<<<
  *         cdef int length = len(str)
  *         return length * 10000 + self.calculate_key(str)
  */
 
 static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_length_alpha(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
   int __pyx_v_length;
   PY_LONG_LONG __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_key_length_alpha", 0);
 
-  /* "camSort/stringSort.pyx":32
+  /* "camSort/stringSort.pyx":30
  * 
- *     cdef long long calculate_key_length_alpha(self, str):
+ *     cdef long long calculate_key_length_alpha(self, str str):
  *         cdef int length = len(str)             # <<<<<<<<<<<<<<
  *         return length * 10000 + self.calculate_key(str)
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_str); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (unlikely(__pyx_v_str == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 30, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_str); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 30, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "camSort/stringSort.pyx":33
- *     cdef long long calculate_key_length_alpha(self, str):
+  /* "camSort/stringSort.pyx":31
+ *     cdef long long calculate_key_length_alpha(self, str str):
  *         cdef int length = len(str)
  *         return length * 10000 + self.calculate_key(str)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((__pyx_v_length * 0x2710) + ((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str));
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":31
+  /* "camSort/stringSort.pyx":29
  *         return str.lower()
  * 
- *     cdef long long calculate_key_length_alpha(self, str):             # <<<<<<<<<<<<<<
+ *     cdef long long calculate_key_length_alpha(self, str str):             # <<<<<<<<<<<<<<
  *         cdef int length = len(str)
  *         return length * 10000 + self.calculate_key(str)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("camSort.stringSort.StringWithKey.calculate_key_length_alpha", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":9
+/* "camSort/stringSort.pyx":7
  * cdef class StringWithKey:
  *     cdef public:
  *         str str             # <<<<<<<<<<<<<<
  *         object key
  * 
  */
 
@@ -2046,15 +1996,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 7, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->str);
   __Pyx_DECREF(__pyx_v_self->str);
   __pyx_v_self->str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -2096,20 +2046,20 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":10
+/* "camSort/stringSort.pyx":8
  *     cdef public:
  *         str str
  *         object key             # <<<<<<<<<<<<<<
  * 
- *     def __init__(self, str, key_type='length'):
+ *     def __init__(self, str str, key_type='length'):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3key_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3key_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2498,32 +2448,32 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":41
- *         size_t size
+/* "camSort/stringSort.pyx":38
+ *         list str_list
+ * 
+ *     def __init__(self, list py_list):             # <<<<<<<<<<<<<<
+ *         self.str_list = py_list[:]
  * 
- *     def __cinit__(self, list py_list):             # <<<<<<<<<<<<<<
- *         self.size = len(py_list)
- *         self.str_list = <char **> malloc(sizeof(char *) * self.size)
  */
 
 /* Python wrapper */
-static int __pyx_pw_7camSort_10stringSort_10SortedList_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_7camSort_10stringSort_10SortedList_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_7camSort_10stringSort_10SortedList_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_10SortedList_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_py_list = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
+  __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_py_list,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
@@ -2535,318 +2485,142 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_py_list)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 41, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 38, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_py_list = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 41, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 38, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("camSort.stringSort.SortedList.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_py_list), (&PyList_Type), 1, "py_list", 1))) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList___cinit__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), __pyx_v_py_list);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_py_list), (&PyList_Type), 1, "py_list", 1))) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList___init__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), __pyx_v_py_list);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7camSort_10stringSort_10SortedList___cinit__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_py_list) {
-  size_t __pyx_v_i;
-  PyObject *__pyx_v_s = NULL;
+static int __pyx_pf_7camSort_10stringSort_10SortedList___init__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_py_list) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  Py_ssize_t __pyx_t_1;
-  int __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  size_t __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  char const *__pyx_t_9;
+  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__cinit__", 0);
+  __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "camSort/stringSort.pyx":42
+  /* "camSort/stringSort.pyx":39
  * 
- *     def __cinit__(self, list py_list):
- *         self.size = len(py_list)             # <<<<<<<<<<<<<<
- *         self.str_list = <char **> malloc(sizeof(char *) * self.size)
- *         if not self.str_list:
+ *     def __init__(self, list py_list):
+ *         self.str_list = py_list[:]             # <<<<<<<<<<<<<<
+ * 
+ *     cpdef SortedList reverse(self):
  */
   if (unlikely(__pyx_v_py_list == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 42, __pyx_L1_error)
-  }
-  __pyx_t_1 = PyList_GET_SIZE(__pyx_v_py_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 42, __pyx_L1_error)
-  __pyx_v_self->size = __pyx_t_1;
-
-  /* "camSort/stringSort.pyx":43
- *     def __cinit__(self, list py_list):
- *         self.size = len(py_list)
- *         self.str_list = <char **> malloc(sizeof(char *) * self.size)             # <<<<<<<<<<<<<<
- *         if not self.str_list:
- *             # bye bye
- */
-  __pyx_v_self->str_list = ((char **)malloc(((sizeof(char *)) * __pyx_v_self->size)));
-
-  /* "camSort/stringSort.pyx":44
- *         self.size = len(py_list)
- *         self.str_list = <char **> malloc(sizeof(char *) * self.size)
- *         if not self.str_list:             # <<<<<<<<<<<<<<
- *             # bye bye
- *             raise MemoryError()
- */
-  __pyx_t_2 = ((!(__pyx_v_self->str_list != 0)) != 0);
-  if (unlikely(__pyx_t_2)) {
-
-    /* "camSort/stringSort.pyx":46
- *         if not self.str_list:
- *             # bye bye
- *             raise MemoryError()             # <<<<<<<<<<<<<<
- * 
- *         for i in range(self.size):
- */
-    PyErr_NoMemory(); __PYX_ERR(0, 46, __pyx_L1_error)
-
-    /* "camSort/stringSort.pyx":44
- *         self.size = len(py_list)
- *         self.str_list = <char **> malloc(sizeof(char *) * self.size)
- *         if not self.str_list:             # <<<<<<<<<<<<<<
- *             # bye bye
- *             raise MemoryError()
- */
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(0, 39, __pyx_L1_error)
   }
+  __pyx_t_1 = __Pyx_PyList_GetSlice(__pyx_v_py_list, 0, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->str_list);
+  __Pyx_DECREF(__pyx_v_self->str_list);
+  __pyx_v_self->str_list = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "camSort/stringSort.pyx":48
- *             raise MemoryError()
- * 
- *         for i in range(self.size):             # <<<<<<<<<<<<<<
- *             s = py_list[i].encode('utf-8')
- *             self.str_list[i] = strdup(s)
- */
-  __pyx_t_3 = __pyx_v_self->size;
-  __pyx_t_4 = __pyx_t_3;
-  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
-    __pyx_v_i = __pyx_t_5;
-
-    /* "camSort/stringSort.pyx":49
- * 
- *         for i in range(self.size):
- *             s = py_list[i].encode('utf-8')             # <<<<<<<<<<<<<<
- *             self.str_list[i] = strdup(s)
- * 
- */
-    if (unlikely(__pyx_v_py_list == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 49, __pyx_L1_error)
-    }
-    __pyx_t_7 = __Pyx_GetItemInt_List(__pyx_v_py_list, __pyx_v_i, size_t, 0, __Pyx_PyInt_FromSize_t, 1, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 49, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 49, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_7);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-      }
-    }
-    __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u_utf_8);
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 49, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_s, __pyx_t_6);
-    __pyx_t_6 = 0;
-
-    /* "camSort/stringSort.pyx":50
- *         for i in range(self.size):
- *             s = py_list[i].encode('utf-8')
- *             self.str_list[i] = strdup(s)             # <<<<<<<<<<<<<<
+  /* "camSort/stringSort.pyx":38
+ *         list str_list
  * 
- *     def __dealloc__(self):
- */
-    __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_v_s); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L1_error)
-    (__pyx_v_self->str_list[__pyx_v_i]) = strdup(__pyx_t_9);
-  }
-
-  /* "camSort/stringSort.pyx":41
- *         size_t size
+ *     def __init__(self, list py_list):             # <<<<<<<<<<<<<<
+ *         self.str_list = py_list[:]
  * 
- *     def __cinit__(self, list py_list):             # <<<<<<<<<<<<<<
- *         self.size = len(py_list)
- *         self.str_list = <char **> malloc(sizeof(char *) * self.size)
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("camSort.stringSort.SortedList.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_s);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":52
- *             self.str_list[i] = strdup(s)
- * 
- *     def __dealloc__(self):             # <<<<<<<<<<<<<<
- *         for i in range(self.size):
- *             free(self.str_list[i])
- */
-
-/* Python wrapper */
-static void __pyx_pw_7camSort_10stringSort_10SortedList_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_7camSort_10stringSort_10SortedList_3__dealloc__(PyObject *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_7camSort_10stringSort_10SortedList_2__dealloc__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-static void __pyx_pf_7camSort_10stringSort_10SortedList_2__dealloc__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
-  size_t __pyx_v_i;
-  __Pyx_RefNannyDeclarations
-  size_t __pyx_t_1;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
-
-  /* "camSort/stringSort.pyx":53
- * 
- *     def __dealloc__(self):
- *         for i in range(self.size):             # <<<<<<<<<<<<<<
- *             free(self.str_list[i])
- *         free(self.str_list)
- */
-  __pyx_t_1 = __pyx_v_self->size;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
-
-    /* "camSort/stringSort.pyx":54
- *     def __dealloc__(self):
- *         for i in range(self.size):
- *             free(self.str_list[i])             # <<<<<<<<<<<<<<
- *         free(self.str_list)
- * 
- */
-    free((__pyx_v_self->str_list[__pyx_v_i]));
-  }
-
-  /* "camSort/stringSort.pyx":55
- *         for i in range(self.size):
- *             free(self.str_list[i])
- *         free(self.str_list)             # <<<<<<<<<<<<<<
- * 
- *     cpdef SortedList reverse(self):
- */
-  free(__pyx_v_self->str_list);
-
-  /* "camSort/stringSort.pyx":52
- *             self.str_list[i] = strdup(s)
- * 
- *     def __dealloc__(self):             # <<<<<<<<<<<<<<
- *         for i in range(self.size):
- *             free(self.str_list[i])
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "camSort/stringSort.pyx":57
- *         free(self.str_list)
+/* "camSort/stringSort.pyx":41
+ *         self.str_list = py_list[:]
  * 
  *     cpdef SortedList reverse(self):             # <<<<<<<<<<<<<<
- *         cdef:
- *             size_t i
+ *         self.str_list.reverse()
+ *         return self
  */
 
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_5reverse(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_3reverse(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_f_7camSort_10stringSort_10SortedList_reverse(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, int __pyx_skip_dispatch) {
-  size_t __pyx_v_i;
-  char *__pyx_v_temp;
   struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  size_t __pyx_t_5;
-  size_t __pyx_t_6;
-  size_t __pyx_t_7;
+  int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reverse", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reverse); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reverse); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7camSort_10stringSort_10SortedList_5reverse)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7camSort_10stringSort_10SortedList_3reverse)) {
         __Pyx_XDECREF(((PyObject *)__pyx_r));
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_7camSort_10stringSort_SortedList))))) __PYX_ERR(0, 57, __pyx_L1_error)
+        if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_7camSort_10stringSort_SortedList))))) __PYX_ERR(0, 41, __pyx_L1_error)
         __pyx_r = ((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -2857,72 +2631,45 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "camSort/stringSort.pyx":62
- *             char* temp
- * 
- *         for i in range(self.size // 2):             # <<<<<<<<<<<<<<
- *             temp = self.str_list[i]
- *             self.str_list[i] = self.str_list[self.size - i - 1]
- */
-  __pyx_t_5 = (__pyx_v_self->size / 2);
-  __pyx_t_6 = __pyx_t_5;
-  for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
-    __pyx_v_i = __pyx_t_7;
-
-    /* "camSort/stringSort.pyx":63
- * 
- *         for i in range(self.size // 2):
- *             temp = self.str_list[i]             # <<<<<<<<<<<<<<
- *             self.str_list[i] = self.str_list[self.size - i - 1]
- *             self.str_list[self.size - i - 1] = temp
- */
-    __pyx_v_temp = (__pyx_v_self->str_list[__pyx_v_i]);
-
-    /* "camSort/stringSort.pyx":64
- *         for i in range(self.size // 2):
- *             temp = self.str_list[i]
- *             self.str_list[i] = self.str_list[self.size - i - 1]             # <<<<<<<<<<<<<<
- *             self.str_list[self.size - i - 1] = temp
- * 
- */
-    (__pyx_v_self->str_list[__pyx_v_i]) = (__pyx_v_self->str_list[((__pyx_v_self->size - __pyx_v_i) - 1)]);
-
-    /* "camSort/stringSort.pyx":65
- *             temp = self.str_list[i]
- *             self.str_list[i] = self.str_list[self.size - i - 1]
- *             self.str_list[self.size - i - 1] = temp             # <<<<<<<<<<<<<<
+  /* "camSort/stringSort.pyx":42
  * 
+ *     cpdef SortedList reverse(self):
+ *         self.str_list.reverse()             # <<<<<<<<<<<<<<
  *         return self
+ * 
  */
-    (__pyx_v_self->str_list[((__pyx_v_self->size - __pyx_v_i) - 1)]) = __pyx_v_temp;
+  if (unlikely(__pyx_v_self->str_list == Py_None)) {
+    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "reverse");
+    __PYX_ERR(0, 42, __pyx_L1_error)
   }
+  __pyx_t_5 = PyList_Reverse(__pyx_v_self->str_list); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 42, __pyx_L1_error)
 
-  /* "camSort/stringSort.pyx":67
- *             self.str_list[self.size - i - 1] = temp
- * 
+  /* "camSort/stringSort.pyx":43
+ *     cpdef SortedList reverse(self):
+ *         self.str_list.reverse()
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def to_list(self):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = __pyx_v_self;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":57
- *         free(self.str_list)
+  /* "camSort/stringSort.pyx":41
+ *         self.str_list = py_list[:]
  * 
  *     cpdef SortedList reverse(self):             # <<<<<<<<<<<<<<
- *         cdef:
- *             size_t i
+ *         self.str_list.reverse()
+ *         return self
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -2932,36 +2679,36 @@
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_5reverse(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_5reverse(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_3reverse(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_3reverse(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("reverse (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_4reverse(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_2reverse(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_4reverse(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_2reverse(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reverse", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_7camSort_10stringSort_10SortedList_reverse(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7camSort_10stringSort_10SortedList_reverse(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2970,1506 +2717,1359 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":69
+/* "camSort/stringSort.pyx":45
  *         return self
  * 
  *     def to_list(self):             # <<<<<<<<<<<<<<
- *         return [self.str_list[i].decode('utf-8') for i in range(self.size)]
+ *         return self.str_list[:]
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_7to_list(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_7to_list(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_5to_list(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_5to_list(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("to_list (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_6to_list(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_4to_list(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_6to_list(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
-  size_t __pyx_7genexpr__pyx_v_i;
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_4to_list(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  char *__pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("to_list", 0);
 
-  /* "camSort/stringSort.pyx":70
+  /* "camSort/stringSort.pyx":46
  * 
  *     def to_list(self):
- *         return [self.str_list[i].decode('utf-8') for i in range(self.size)]             # <<<<<<<<<<<<<<
+ *         return self.str_list[:]             # <<<<<<<<<<<<<<
  * 
- *     def __decode_string(self, int i):
+ *     def __getitem__(self, item):
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __pyx_v_self->size;
-    __pyx_t_3 = __pyx_t_2;
-    for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-      __pyx_7genexpr__pyx_v_i = __pyx_t_4;
-      __pyx_t_5 = (__pyx_v_self->str_list[__pyx_7genexpr__pyx_v_i]);
-      __pyx_t_6 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 70, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    }
-  } /* exit inner scope */
+  if (unlikely(__pyx_v_self->str_list == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(0, 46, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_PyList_GetSlice(__pyx_v_self->str_list, 0, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":69
+  /* "camSort/stringSort.pyx":45
  *         return self
  * 
  *     def to_list(self):             # <<<<<<<<<<<<<<
- *         return [self.str_list[i].decode('utf-8') for i in range(self.size)]
+ *         return self.str_list[:]
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("camSort.stringSort.SortedList.to_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":72
- *         return [self.str_list[i].decode('utf-8') for i in range(self.size)]
+/* "camSort/stringSort.pyx":48
+ *         return self.str_list[:]
  * 
- *     def __decode_string(self, int i):             # <<<<<<<<<<<<<<
- *         return self.str_list[i].decode('utf-8')
+ *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
+ *         return self.str_list[item]
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_9__decode_string(PyObject *__pyx_v_self, PyObject *__pyx_arg_i); /*proto*/
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_9__decode_string(PyObject *__pyx_v_self, PyObject *__pyx_arg_i) {
-  int __pyx_v_i;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_7__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_item); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_7__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_item) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__decode_string (wrapper)", 0);
-  assert(__pyx_arg_i); {
-    __pyx_v_i = __Pyx_PyInt_As_int(__pyx_arg_i); if (unlikely((__pyx_v_i == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("camSort.stringSort.SortedList.__decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_8__decode_string(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((int)__pyx_v_i));
+  __Pyx_RefNannySetupContext("__getitem__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_6__getitem__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((PyObject *)__pyx_v_item));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_8__decode_string(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, int __pyx_v_i) {
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_6__getitem__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_item) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  char *__pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__decode_string", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "camSort/stringSort.pyx":73
- * 
- *     def __decode_string(self, int i):
- *         return self.str_list[i].decode('utf-8')             # <<<<<<<<<<<<<<
+  /* "camSort/stringSort.pyx":49
  * 
  *     def __getitem__(self, item):
+ *         return self.str_list[item]             # <<<<<<<<<<<<<<
+ * 
+ *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = (__pyx_v_self->str_list[__pyx_v_i]);
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_t_2);
-  __pyx_r = __pyx_t_2;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(__pyx_v_self->str_list == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(0, 49, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->str_list, __pyx_v_item); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":72
- *         return [self.str_list[i].decode('utf-8') for i in range(self.size)]
+  /* "camSort/stringSort.pyx":48
+ *         return self.str_list[:]
  * 
- *     def __decode_string(self, int i):             # <<<<<<<<<<<<<<
- *         return self.str_list[i].decode('utf-8')
+ *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
+ *         return self.str_list[item]
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("camSort.stringSort.SortedList.__decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":75
- *         return self.str_list[i].decode('utf-8')
+/* "camSort/stringSort.pyx":51
+ *         return self.str_list[item]
  * 
- *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
- *         cdef int start, stop, step, length
+ *     def __len__(self):             # <<<<<<<<<<<<<<
+ *         return len(self.str_list)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_11__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_item); /*proto*/
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_11__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_item) {
-  PyObject *__pyx_r = 0;
+static Py_ssize_t __pyx_pw_7camSort_10stringSort_10SortedList_9__len__(PyObject *__pyx_v_self); /*proto*/
+static Py_ssize_t __pyx_pw_7camSort_10stringSort_10SortedList_9__len__(PyObject *__pyx_v_self) {
+  Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__getitem__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_10__getitem__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((PyObject *)__pyx_v_item));
+  __Pyx_RefNannySetupContext("__len__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_8__len__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_10__getitem__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_item) {
-  int __pyx_v_start;
-  int __pyx_v_stop;
-  int __pyx_v_step;
-  int __pyx_8genexpr1__pyx_v_i;
-  PyObject *__pyx_r = NULL;
+static Py_ssize_t __pyx_pf_7camSort_10stringSort_10SortedList_8__len__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+  Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  int __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  Py_ssize_t __pyx_t_10;
-  PyObject *(*__pyx_t_11)(PyObject *);
-  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "camSort/stringSort.pyx":78
- *         cdef int start, stop, step, length
+  /* "camSort/stringSort.pyx":52
  * 
- *         if isinstance(item, slice):             # <<<<<<<<<<<<<<
- *             start = item.start if item.start is not None else 0
- *             stop = item.stop if item.stop is not None else self.size
- */
-  __pyx_t_1 = PySlice_Check(__pyx_v_item); 
-  __pyx_t_2 = (__pyx_t_1 != 0);
-  if (__pyx_t_2) {
-
-    /* "camSort/stringSort.pyx":79
+ *     def __len__(self):
+ *         return len(self.str_list)             # <<<<<<<<<<<<<<
  * 
- *         if isinstance(item, slice):
- *             start = item.start if item.start is not None else 0             # <<<<<<<<<<<<<<
- *             stop = item.stop if item.stop is not None else self.size
- *             step = item.step if item.step is not None else 1
+ *     cpdef list filterWithSubstring(self, str substring):
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_item, __pyx_n_s_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = (__pyx_t_4 != Py_None);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if ((__pyx_t_2 != 0)) {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_item, __pyx_n_s_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_3 = __pyx_t_5;
-    } else {
-      __pyx_t_3 = 0;
-    }
-    __pyx_v_start = __pyx_t_3;
+  __pyx_t_1 = __pyx_v_self->str_list;
+  __Pyx_INCREF(__pyx_t_1);
+  if (unlikely(__pyx_t_1 == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 52, __pyx_L1_error)
+  }
+  __pyx_t_2 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_2;
+  goto __pyx_L0;
 
-    /* "camSort/stringSort.pyx":80
- *         if isinstance(item, slice):
- *             start = item.start if item.start is not None else 0
- *             stop = item.stop if item.stop is not None else self.size             # <<<<<<<<<<<<<<
- *             step = item.step if item.step is not None else 1
+  /* "camSort/stringSort.pyx":51
+ *         return self.str_list[item]
  * 
- */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_item, __pyx_n_s_stop); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = (__pyx_t_4 != Py_None);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if ((__pyx_t_2 != 0)) {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_item, __pyx_n_s_stop); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_3 = __pyx_t_5;
-    } else {
-      __pyx_t_3 = __pyx_v_self->size;
-    }
-    __pyx_v_stop = __pyx_t_3;
-
-    /* "camSort/stringSort.pyx":81
- *             start = item.start if item.start is not None else 0
- *             stop = item.stop if item.stop is not None else self.size
- *             step = item.step if item.step is not None else 1             # <<<<<<<<<<<<<<
+ *     def __len__(self):             # <<<<<<<<<<<<<<
+ *         return len(self.str_list)
  * 
- *             return [self.__decode_string(i) for i in range(start, stop, step)]
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_item, __pyx_n_s_step); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = (__pyx_t_4 != Py_None);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if ((__pyx_t_2 != 0)) {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_item, __pyx_n_s_step); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_3 = __pyx_t_5;
-    } else {
-      __pyx_t_3 = 1;
-    }
-    __pyx_v_step = __pyx_t_3;
 
-    /* "camSort/stringSort.pyx":83
- *             step = item.step if item.step is not None else 1
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":54
+ *         return len(self.str_list)
+ * 
+ *     cpdef list filterWithSubstring(self, str substring):             # <<<<<<<<<<<<<<
+ *         return [s for s in self.str_list if substring in s]
  * 
- *             return [self.__decode_string(i) for i in range(start, stop, step)]             # <<<<<<<<<<<<<<
- *         elif isinstance(item, int):
- *             if item < 0 or item >= self.size:
  */
-    __Pyx_XDECREF(__pyx_r);
-    { /* enter inner scope */
-      __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 83, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_stop); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_step); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GIVEREF(__pyx_t_6);
-      PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_6);
-      __Pyx_GIVEREF(__pyx_t_7);
-      PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_7);
-      __Pyx_GIVEREF(__pyx_t_8);
-      PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_8);
-      __pyx_t_6 = 0;
-      __pyx_t_7 = 0;
-      __pyx_t_8 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (likely(PyList_CheckExact(__pyx_t_8)) || PyTuple_CheckExact(__pyx_t_8)) {
-        __pyx_t_9 = __pyx_t_8; __Pyx_INCREF(__pyx_t_9); __pyx_t_10 = 0;
-        __pyx_t_11 = NULL;
-      } else {
-        __pyx_t_10 = -1; __pyx_t_9 = PyObject_GetIter(__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_11 = Py_TYPE(__pyx_t_9)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 83, __pyx_L1_error)
-      }
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      for (;;) {
-        if (likely(!__pyx_t_11)) {
-          if (likely(PyList_CheckExact(__pyx_t_9))) {
-            if (__pyx_t_10 >= PyList_GET_SIZE(__pyx_t_9)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_8 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_8); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 83, __pyx_L1_error)
-            #else
-            __pyx_t_8 = PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_8);
-            #endif
-          } else {
-            if (__pyx_t_10 >= PyTuple_GET_SIZE(__pyx_t_9)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_8); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 83, __pyx_L1_error)
-            #else
-            __pyx_t_8 = PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_8);
-            #endif
-          }
-        } else {
-          __pyx_t_8 = __pyx_t_11(__pyx_t_9);
-          if (unlikely(!__pyx_t_8)) {
-            PyObject* exc_type = PyErr_Occurred();
-            if (exc_type) {
-              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 83, __pyx_L1_error)
-            }
-            break;
-          }
-          __Pyx_GOTREF(__pyx_t_8);
-        }
-        __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_8); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_8genexpr1__pyx_v_i = __pyx_t_3;
-        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_12 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_7);
-          if (likely(__pyx_t_12)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-            __Pyx_INCREF(__pyx_t_12);
+
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_11filterWithSubstring(PyObject *__pyx_v_self, PyObject *__pyx_v_substring); /*proto*/
+static PyObject *__pyx_f_7camSort_10stringSort_10SortedList_filterWithSubstring(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_substring, int __pyx_skip_dispatch) {
+  PyObject *__pyx_7genexpr__pyx_v_s = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_t_6;
+  int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("filterWithSubstring", 0);
+  /* Check if called by wrapper */
+  if (unlikely(__pyx_skip_dispatch)) ;
+  /* Check if overridden in Python */
+  else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
+    #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+    static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
+    if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
+      PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      #endif
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_filterWithSubstring); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7camSort_10stringSort_10SortedList_11filterWithSubstring)) {
+        __Pyx_XDECREF(__pyx_r);
+        __Pyx_INCREF(__pyx_t_1);
+        __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_4)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_7, function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
-        __pyx_t_8 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_12, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
-        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 83, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_substring) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_substring);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (!(likely(PyList_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 54, __pyx_L1_error)
+        __pyx_r = ((PyObject*)__pyx_t_2);
+        __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        goto __pyx_L0;
       }
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    } /* exit inner scope */
-    __pyx_r = __pyx_t_4;
-    __pyx_t_4 = 0;
-    goto __pyx_L0;
-
-    /* "camSort/stringSort.pyx":78
- *         cdef int start, stop, step, length
- * 
- *         if isinstance(item, slice):             # <<<<<<<<<<<<<<
- *             start = item.start if item.start is not None else 0
- *             stop = item.stop if item.stop is not None else self.size
- */
+      #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+      __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      __pyx_obj_dict_version = __Pyx_get_object_dict_version(((PyObject *)__pyx_v_self));
+      if (unlikely(__pyx_type_dict_guard != __pyx_tp_dict_version)) {
+        __pyx_tp_dict_version = __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
+      }
+      #endif
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+    }
+    #endif
   }
 
-  /* "camSort/stringSort.pyx":84
+  /* "camSort/stringSort.pyx":55
  * 
- *             return [self.__decode_string(i) for i in range(start, stop, step)]
- *         elif isinstance(item, int):             # <<<<<<<<<<<<<<
- *             if item < 0 or item >= self.size:
- *                 raise IndexError("PyStringList index out of range")
- */
-  __pyx_t_2 = PyInt_Check(__pyx_v_item); 
-  __pyx_t_1 = (__pyx_t_2 != 0);
-  if (likely(__pyx_t_1)) {
-
-    /* "camSort/stringSort.pyx":85
- *             return [self.__decode_string(i) for i in range(start, stop, step)]
- *         elif isinstance(item, int):
- *             if item < 0 or item >= self.size:             # <<<<<<<<<<<<<<
- *                 raise IndexError("PyStringList index out of range")
- *             return self.__decode_string(item)
- */
-    __pyx_t_4 = PyObject_RichCompare(__pyx_v_item, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_self->size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = PyObject_RichCompare(__pyx_v_item, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 85, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_1 = __pyx_t_2;
-    __pyx_L7_bool_binop_done:;
-    if (unlikely(__pyx_t_1)) {
-
-      /* "camSort/stringSort.pyx":86
- *         elif isinstance(item, int):
- *             if item < 0 or item >= self.size:
- *                 raise IndexError("PyStringList index out of range")             # <<<<<<<<<<<<<<
- *             return self.__decode_string(item)
- *         else:
- */
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_Raise(__pyx_t_9, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __PYX_ERR(0, 86, __pyx_L1_error)
-
-      /* "camSort/stringSort.pyx":85
- *             return [self.__decode_string(i) for i in range(start, stop, step)]
- *         elif isinstance(item, int):
- *             if item < 0 or item >= self.size:             # <<<<<<<<<<<<<<
- *                 raise IndexError("PyStringList index out of range")
- *             return self.__decode_string(item)
+ *     cpdef list filterWithSubstring(self, str substring):
+ *         return [s for s in self.str_list if substring in s]             # <<<<<<<<<<<<<<
+ * 
+ * def byKey(list input_list, str key_type):
  */
+  __Pyx_XDECREF(__pyx_r);
+  { /* enter inner scope */
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (unlikely(__pyx_v_self->str_list == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+      __PYX_ERR(0, 55, __pyx_L5_error)
     }
-
-    /* "camSort/stringSort.pyx":87
- *             if item < 0 or item >= self.size:
- *                 raise IndexError("PyStringList index out of range")
- *             return self.__decode_string(item)             # <<<<<<<<<<<<<<
- *         else:
- *             raise TypeError("Invalid argument type.")
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_8);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
+    __pyx_t_2 = __pyx_v_self->str_list; __Pyx_INCREF(__pyx_t_2); __pyx_t_5 = 0;
+    for (;;) {
+      if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_2)) break;
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 55, __pyx_L5_error)
+      #else
+      __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      #endif
+      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_s, __pyx_t_3);
+      __pyx_t_3 = 0;
+      __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_v_substring, __pyx_7genexpr__pyx_v_s, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 55, __pyx_L5_error)
+      __pyx_t_7 = (__pyx_t_6 != 0);
+      if (__pyx_t_7) {
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_s))) __PYX_ERR(0, 55, __pyx_L5_error)
       }
     }
-    __pyx_t_9 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_v_item) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_item);
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 87, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_r = __pyx_t_9;
-    __pyx_t_9 = 0;
-    goto __pyx_L0;
-
-    /* "camSort/stringSort.pyx":84
- * 
- *             return [self.__decode_string(i) for i in range(start, stop, step)]
- *         elif isinstance(item, int):             # <<<<<<<<<<<<<<
- *             if item < 0 or item >= self.size:
- *                 raise IndexError("PyStringList index out of range")
- */
-  }
-
-  /* "camSort/stringSort.pyx":89
- *             return self.__decode_string(item)
- *         else:
- *             raise TypeError("Invalid argument type.")             # <<<<<<<<<<<<<<
- * 
- *     def __len__(self):
- */
-  /*else*/ {
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 89, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_Raise(__pyx_t_9, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __PYX_ERR(0, 89, __pyx_L1_error)
-  }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s); __pyx_7genexpr__pyx_v_s = 0;
+    goto __pyx_L9_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s); __pyx_7genexpr__pyx_v_s = 0;
+    goto __pyx_L1_error;
+    __pyx_L9_exit_scope:;
+  } /* exit inner scope */
+  __pyx_r = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":75
- *         return self.str_list[i].decode('utf-8')
+  /* "camSort/stringSort.pyx":54
+ *         return len(self.str_list)
  * 
- *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
- *         cdef int start, stop, step, length
+ *     cpdef list filterWithSubstring(self, str substring):             # <<<<<<<<<<<<<<
+ *         return [s for s in self.str_list if substring in s]
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_AddTraceback("camSort.stringSort.SortedList.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.filterWithSubstring", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":91
- *             raise TypeError("Invalid argument type.")
- * 
- *     def __len__(self):             # <<<<<<<<<<<<<<
- *         return self.size
- * 
- */
-
 /* Python wrapper */
-static Py_ssize_t __pyx_pw_7camSort_10stringSort_10SortedList_13__len__(PyObject *__pyx_v_self); /*proto*/
-static Py_ssize_t __pyx_pw_7camSort_10stringSort_10SortedList_13__len__(PyObject *__pyx_v_self) {
-  Py_ssize_t __pyx_r;
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_11filterWithSubstring(PyObject *__pyx_v_self, PyObject *__pyx_v_substring); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_11filterWithSubstring(PyObject *__pyx_v_self, PyObject *__pyx_v_substring) {
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__len__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_12__len__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+  __Pyx_RefNannySetupContext("filterWithSubstring (wrapper)", 0);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_substring), (&PyUnicode_Type), 1, "substring", 1))) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_10filterWithSubstring(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((PyObject*)__pyx_v_substring));
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static Py_ssize_t __pyx_pf_7camSort_10stringSort_10SortedList_12__len__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
-  Py_ssize_t __pyx_r;
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_10filterWithSubstring(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_substring) {
+  PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__len__", 0);
-
-  /* "camSort/stringSort.pyx":92
- * 
- *     def __len__(self):
- *         return self.size             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_self->size;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("filterWithSubstring", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __pyx_f_7camSort_10stringSort_10SortedList_filterWithSubstring(__pyx_v_self, __pyx_v_substring, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":91
- *             raise TypeError("Invalid argument type.")
- * 
- *     def __len__(self):             # <<<<<<<<<<<<<<
- *         return self.size
- * 
- */
-
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.filterWithSubstring", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
+ *     cdef tuple state
+ *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_13__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_13__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_14__reduce_cython__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_12__reduce_cython__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_12__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v__dict = 0;
+  int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
-  /* "(tree fragment)":2
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+  /* "(tree fragment)":5
+ *     cdef object _dict
+ *     cdef bint use_setstate
+ *     state = (self.str_list,)             # <<<<<<<<<<<<<<
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_v_self->str_list);
+  __Pyx_GIVEREF(__pyx_v_self->str_list);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_self->str_list);
+  __pyx_v_state = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":6
+ *     cdef bint use_setstate
+ *     state = (self.str_list,)
+ *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
+ *     if _dict is not None:
+ *         state += (_dict,)
+ */
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v__dict = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":7
+ *     state = (self.str_list,)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+  __pyx_t_2 = (__pyx_v__dict != Py_None);
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":8
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ *         state += (_dict,)             # <<<<<<<<<<<<<<
+ *         use_setstate = True
+ *     else:
+ */
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_v__dict);
+    __Pyx_GIVEREF(__pyx_v__dict);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict);
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_4));
+    __pyx_t_4 = 0;
+
+    /* "(tree fragment)":9
+ *     if _dict is not None:
+ *         state += (_dict,)
+ *         use_setstate = True             # <<<<<<<<<<<<<<
+ *     else:
+ *         use_setstate = self.str_list is not None
+ */
+    __pyx_v_use_setstate = 1;
+
+    /* "(tree fragment)":7
+ *     state = (self.str_list,)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+    goto __pyx_L3;
+  }
+
+  /* "(tree fragment)":11
+ *         use_setstate = True
+ *     else:
+ *         use_setstate = self.str_list is not None             # <<<<<<<<<<<<<<
+ *     if use_setstate:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state
+ */
+  /*else*/ {
+    __pyx_t_3 = (__pyx_v_self->str_list != ((PyObject*)Py_None));
+    __pyx_v_use_setstate = __pyx_t_3;
+  }
+  __pyx_L3:;
+
+  /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self.str_list is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state
+ *     else:
+ */
+  __pyx_t_3 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":13
+ *         use_setstate = self.str_list is not None
+ *     if use_setstate:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state             # <<<<<<<<<<<<<<
+ *     else:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_SortedList); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_46947008);
+    __Pyx_GIVEREF(__pyx_int_46947008);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_46947008);
+    __Pyx_INCREF(Py_None);
+    __Pyx_GIVEREF(Py_None);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None);
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
+    __pyx_t_4 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
+    goto __pyx_L0;
+
+    /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self.str_list is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state
+ *     else:
+ */
+  }
+
+  /* "(tree fragment)":15
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state
+ *     else:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_SortedList__set_state(self, __pyx_state)
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_SortedList); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_46947008);
+    __Pyx_GIVEREF(__pyx_int_46947008);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_46947008);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_5 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
+    goto __pyx_L0;
+  }
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
+ *     cdef tuple state
+ *     cdef object _dict
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("camSort.stringSort.SortedList.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_state);
+  __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "(tree fragment)":3
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+/* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     __pyx_unpickle_SortedList__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_15__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_15__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_16__setstate_cython__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_14__setstate_cython__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_14__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
-  /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+  /* "(tree fragment)":17
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_SortedList__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7camSort_10stringSort___pyx_unpickle_SortedList__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 4, __pyx_L1_error)
 
-  /* "(tree fragment)":3
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     __pyx_unpickle_SortedList__set_state(self, __pyx_state)
  */
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("camSort.stringSort.SortedList.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":95
- * 
+/* "camSort/stringSort.pyx":57
+ *         return [s for s in self.str_list if substring in s]
  * 
- * def byLength(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s) for s in input_list]
+ * def byKey(list input_list, str key_type):             # <<<<<<<<<<<<<<
+ *     cdef list array = [StringWithKey(s, key_type) for s in input_list]
+ *     sorted_array = sorted(array, key=attrgetter('key'))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_1byLength(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_10stringSort_1byLength = {"byLength", (PyCFunction)__pyx_pw_7camSort_10stringSort_1byLength, METH_O, 0};
-static PyObject *__pyx_pw_7camSort_10stringSort_1byLength(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+static PyObject *__pyx_pw_7camSort_10stringSort_1byKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_1byKey = {"byKey", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7camSort_10stringSort_1byKey, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_1byKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_input_list = 0;
+  PyObject *__pyx_v_key_type = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("byLength (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_byLength(__pyx_self, ((PyObject *)__pyx_v_input_list));
+  __Pyx_RefNannySetupContext("byKey (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_input_list,&__pyx_n_s_key_type,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_input_list)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_key_type)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("byKey", 1, 2, 2, 1); __PYX_ERR(0, 57, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "byKey") < 0)) __PYX_ERR(0, 57, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_input_list = ((PyObject*)values[0]);
+    __pyx_v_key_type = ((PyObject*)values[1]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("byKey", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 57, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("camSort.stringSort.byKey", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_input_list), (&PyList_Type), 1, "input_list", 1))) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key_type), (&PyUnicode_Type), 1, "key_type", 1))) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7camSort_10stringSort_byKey(__pyx_self, __pyx_v_input_list, __pyx_v_key_type);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_byLength(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
-  CYTHON_UNUSED int __pyx_v_n;
+static PyObject *__pyx_pf_7camSort_10stringSort_byKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list, PyObject *__pyx_v_key_type) {
   PyObject *__pyx_v_array = 0;
   PyObject *__pyx_v_sorted_array = NULL;
+  PyObject *__pyx_8genexpr1__pyx_v_s = NULL;
   PyObject *__pyx_8genexpr2__pyx_v_s = NULL;
-  PyObject *__pyx_8genexpr3__pyx_v_s = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *(*__pyx_t_4)(PyObject *);
+  Py_ssize_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
+  PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("byLength", 0);
-
-  /* "camSort/stringSort.pyx":96
- * 
- * def byLength(input_list):
- *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
- *     cdef list array = [StringWithKey(s) for s in input_list]
- * 
- */
-  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 96, __pyx_L1_error)
-  __pyx_v_n = __pyx_t_1;
+  __Pyx_RefNannySetupContext("byKey", 0);
 
-  /* "camSort/stringSort.pyx":97
- * def byLength(input_list):
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s) for s in input_list]             # <<<<<<<<<<<<<<
+  /* "camSort/stringSort.pyx":58
  * 
+ * def byKey(list input_list, str key_type):
+ *     cdef list array = [StringWithKey(s, key_type) for s in input_list]             # <<<<<<<<<<<<<<
  *     sorted_array = sorted(array, key=attrgetter('key'))
+ *     return SortedList([s.str for s in sorted_array])
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
-      __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
-      __pyx_t_4 = NULL;
-    } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (unlikely(__pyx_v_input_list == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+      __PYX_ERR(0, 58, __pyx_L5_error)
     }
+    __pyx_t_2 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     for (;;) {
-      if (likely(!__pyx_t_4)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 97, __pyx_L5_error)
-          #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          #endif
-        } else {
-          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 97, __pyx_L5_error)
-          #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          #endif
-        }
-      } else {
-        __pyx_t_5 = __pyx_t_4(__pyx_t_3);
-        if (unlikely(!__pyx_t_5)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 97, __pyx_L5_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_5);
-      }
-      __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_s, __pyx_t_5);
-      __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_8genexpr2__pyx_v_s); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L5_error)
+      if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 58, __pyx_L5_error)
+      #else
+      __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      #endif
+      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_s, __pyx_t_4);
+      __pyx_t_4 = 0;
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_INCREF(__pyx_8genexpr1__pyx_v_s);
+      __Pyx_GIVEREF(__pyx_8genexpr1__pyx_v_s);
+      PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_8genexpr1__pyx_v_s);
+      __Pyx_INCREF(__pyx_v_key_type);
+      __Pyx_GIVEREF(__pyx_v_key_type);
+      PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_key_type);
+      __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 97, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 58, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s); __pyx_8genexpr2__pyx_v_s = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s); __pyx_8genexpr1__pyx_v_s = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s); __pyx_8genexpr2__pyx_v_s = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s); __pyx_8genexpr1__pyx_v_s = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
-  __pyx_v_array = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __pyx_v_array = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "camSort/stringSort.pyx":99
- *     cdef list array = [StringWithKey(s) for s in input_list]
- * 
+  /* "camSort/stringSort.pyx":59
+ * def byKey(list input_list, str key_type):
+ *     cdef list array = [StringWithKey(s, key_type) for s in input_list]
  *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
  *     return SortedList([s.str for s in sorted_array])
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_array);
   __Pyx_GIVEREF(__pyx_v_array);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 99, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_array);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_n_u_key);
-  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_u_key);
+  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_sorted_array = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "camSort/stringSort.pyx":100
- * 
+  /* "camSort/stringSort.pyx":60
+ *     cdef list array = [StringWithKey(s, key_type) for s in input_list]
  *     sorted_array = sorted(array, key=attrgetter('key'))
  *     return SortedList([s.str for s in sorted_array])             # <<<<<<<<<<<<<<
  * 
- * def byLengthAndAlphabet(input_list):
+ * def byLength(list input_list):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L11_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
-      __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
-      __pyx_t_4 = NULL;
+      __pyx_t_2 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+      __pyx_t_7 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L11_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 60, __pyx_L11_error)
     }
     for (;;) {
-      if (likely(!__pyx_t_4)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
+      if (likely(!__pyx_t_7)) {
+        if (likely(PyList_CheckExact(__pyx_t_2))) {
+          if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 100, __pyx_L11_error)
+          __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 60, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L11_error)
-          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L11_error)
+          __Pyx_GOTREF(__pyx_t_1);
           #endif
         } else {
-          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+          if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 100, __pyx_L11_error)
+          __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 60, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L11_error)
-          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L11_error)
+          __Pyx_GOTREF(__pyx_t_1);
           #endif
         }
       } else {
-        __pyx_t_2 = __pyx_t_4(__pyx_t_3);
-        if (unlikely(!__pyx_t_2)) {
+        __pyx_t_1 = __pyx_t_7(__pyx_t_2);
+        if (unlikely(!__pyx_t_1)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 100, __pyx_L11_error)
+            else __PYX_ERR(0, 60, __pyx_L11_error)
           }
           break;
         }
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_GOTREF(__pyx_t_1);
       }
-      __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_s, __pyx_t_2);
-      __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr3__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 100, __pyx_L11_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_s, __pyx_t_1);
+      __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 60, __pyx_L11_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s); __pyx_8genexpr3__pyx_v_s = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s); __pyx_8genexpr2__pyx_v_s = 0;
     goto __pyx_L14_exit_scope;
     __pyx_L11_error:;
-    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s); __pyx_8genexpr3__pyx_v_s = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s); __pyx_8genexpr2__pyx_v_s = 0;
     goto __pyx_L1_error;
     __pyx_L14_exit_scope:;
   } /* exit inner scope */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":95
- * 
+  /* "camSort/stringSort.pyx":57
+ *         return [s for s in self.str_list if substring in s]
  * 
- * def byLength(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s) for s in input_list]
+ * def byKey(list input_list, str key_type):             # <<<<<<<<<<<<<<
+ *     cdef list array = [StringWithKey(s, key_type) for s in input_list]
+ *     sorted_array = sorted(array, key=attrgetter('key'))
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("camSort.stringSort.byLength", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.byKey", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_array);
   __Pyx_XDECREF(__pyx_v_sorted_array);
+  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s);
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s);
-  __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":102
+/* "camSort/stringSort.pyx":62
  *     return SortedList([s.str for s in sorted_array])
  * 
- * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ * def byLength(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'length')
+ * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_3byLengthAndAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_10stringSort_3byLengthAndAlphabet = {"byLengthAndAlphabet", (PyCFunction)__pyx_pw_7camSort_10stringSort_3byLengthAndAlphabet, METH_O, 0};
-static PyObject *__pyx_pw_7camSort_10stringSort_3byLengthAndAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+static PyObject *__pyx_pw_7camSort_10stringSort_3byLength(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_3byLength = {"byLength", (PyCFunction)__pyx_pw_7camSort_10stringSort_3byLength, METH_O, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_3byLength(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("byLengthAndAlphabet (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_2byLengthAndAlphabet(__pyx_self, ((PyObject *)__pyx_v_input_list));
+  __Pyx_RefNannySetupContext("byLength (wrapper)", 0);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_input_list), (&PyList_Type), 1, "input_list", 1))) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7camSort_10stringSort_2byLength(__pyx_self, ((PyObject*)__pyx_v_input_list));
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_2byLengthAndAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
-  CYTHON_UNUSED int __pyx_v_n;
-  PyObject *__pyx_v_array = 0;
-  PyObject *__pyx_v_sorted_array = NULL;
-  PyObject *__pyx_8genexpr4__pyx_v_s = NULL;
-  PyObject *__pyx_8genexpr5__pyx_v_s = NULL;
+static PyObject *__pyx_pf_7camSort_10stringSort_2byLength(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyObject *(*__pyx_t_4)(PyObject *);
+  int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("byLengthAndAlphabet", 0);
+  __Pyx_RefNannySetupContext("byLength", 0);
 
-  /* "camSort/stringSort.pyx":103
+  /* "camSort/stringSort.pyx":63
  * 
- * def byLengthAndAlphabet(input_list):
- *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
- *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ * def byLength(list input_list):
+ *     return byKey(input_list, 'length')             # <<<<<<<<<<<<<<
  * 
+ * def byLengthAndAlphabet(list input_list):
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 103, __pyx_L1_error)
-  __pyx_v_n = __pyx_t_1;
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_byKey); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_input_list, __pyx_n_u_length};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_input_list, __pyx_n_u_length};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+  } else
+  #endif
+  {
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (__pyx_t_3) {
+      __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
+    }
+    __Pyx_INCREF(__pyx_v_input_list);
+    __Pyx_GIVEREF(__pyx_v_input_list);
+    PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_input_list);
+    __Pyx_INCREF(__pyx_n_u_length);
+    __Pyx_GIVEREF(__pyx_n_u_length);
+    PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_n_u_length);
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":104
- * def byLengthAndAlphabet(input_list):
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]             # <<<<<<<<<<<<<<
+  /* "camSort/stringSort.pyx":62
+ *     return SortedList([s.str for s in sorted_array])
+ * 
+ * def byLength(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'length')
  * 
- *     sorted_array = sorted(array, key=attrgetter('key'))
  */
-  { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
-      __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
-      __pyx_t_4 = NULL;
-    } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L5_error)
-    }
-    for (;;) {
-      if (likely(!__pyx_t_4)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 104, __pyx_L5_error)
-          #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 104, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          #endif
-        } else {
-          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 104, __pyx_L5_error)
-          #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 104, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          #endif
-        }
-      } else {
-        __pyx_t_5 = __pyx_t_4(__pyx_t_3);
-        if (unlikely(!__pyx_t_5)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 104, __pyx_L5_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_5);
-      }
-      __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_s, __pyx_t_5);
-      __pyx_t_5 = 0;
-      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 104, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_INCREF(__pyx_8genexpr4__pyx_v_s);
-      __Pyx_GIVEREF(__pyx_8genexpr4__pyx_v_s);
-      PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_8genexpr4__pyx_v_s);
-      __Pyx_INCREF(__pyx_n_u_length_and_alpha);
-      __Pyx_GIVEREF(__pyx_n_u_length_and_alpha);
-      PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_length_and_alpha);
-      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 104, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 104, __pyx_L5_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_s); __pyx_8genexpr4__pyx_v_s = 0;
-    goto __pyx_L8_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_s); __pyx_8genexpr4__pyx_v_s = 0;
-    goto __pyx_L1_error;
-    __pyx_L8_exit_scope:;
-  } /* exit inner scope */
-  __pyx_v_array = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":106
- *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("camSort.stringSort.byLength", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":65
+ *     return byKey(input_list, 'length')
  * 
- *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
- *     return SortedList([s.str for s in sorted_array])
+ * def byLengthAndAlphabet(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'length_and_alpha')
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_v_array);
-  __Pyx_GIVEREF(__pyx_v_array);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_7);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-    }
-  }
-  __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_u_key);
-  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_sorted_array = __pyx_t_6;
-  __pyx_t_6 = 0;
 
-  /* "camSort/stringSort.pyx":107
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_5byLengthAndAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_5byLengthAndAlphabet = {"byLengthAndAlphabet", (PyCFunction)__pyx_pw_7camSort_10stringSort_5byLengthAndAlphabet, METH_O, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_5byLengthAndAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("byLengthAndAlphabet (wrapper)", 0);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_input_list), (&PyList_Type), 1, "input_list", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7camSort_10stringSort_4byLengthAndAlphabet(__pyx_self, ((PyObject*)__pyx_v_input_list));
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_4byLengthAndAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("byLengthAndAlphabet", 0);
+
+  /* "camSort/stringSort.pyx":66
  * 
- *     sorted_array = sorted(array, key=attrgetter('key'))
- *     return SortedList([s.str for s in sorted_array])             # <<<<<<<<<<<<<<
+ * def byLengthAndAlphabet(list input_list):
+ *     return byKey(input_list, 'length_and_alpha')             # <<<<<<<<<<<<<<
  * 
- * def byAlphabet(input_list):
+ * def byAlphabet(list input_list):
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L11_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
-      __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
-      __pyx_t_4 = NULL;
-    } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L11_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_byKey); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
-    for (;;) {
-      if (likely(!__pyx_t_4)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 107, __pyx_L11_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L11_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        } else {
-          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 107, __pyx_L11_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L11_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        }
-      } else {
-        __pyx_t_2 = __pyx_t_4(__pyx_t_3);
-        if (unlikely(!__pyx_t_2)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 107, __pyx_L11_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_2);
-      }
-      __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_s, __pyx_t_2);
-      __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr5__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 107, __pyx_L11_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_input_list, __pyx_n_u_length_and_alpha};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_input_list, __pyx_n_u_length_and_alpha};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+  } else
+  #endif
+  {
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (__pyx_t_3) {
+      __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_s); __pyx_8genexpr5__pyx_v_s = 0;
-    goto __pyx_L14_exit_scope;
-    __pyx_L11_error:;
-    __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_s); __pyx_8genexpr5__pyx_v_s = 0;
-    goto __pyx_L1_error;
-    __pyx_L14_exit_scope:;
-  } /* exit inner scope */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
+    __Pyx_INCREF(__pyx_v_input_list);
+    __Pyx_GIVEREF(__pyx_v_input_list);
+    PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_input_list);
+    __Pyx_INCREF(__pyx_n_u_length_and_alpha);
+    __Pyx_GIVEREF(__pyx_n_u_length_and_alpha);
+    PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_n_u_length_and_alpha);
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":102
- *     return SortedList([s.str for s in sorted_array])
+  /* "camSort/stringSort.pyx":65
+ *     return byKey(input_list, 'length')
+ * 
+ * def byLengthAndAlphabet(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'length_and_alpha')
  * 
- * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("camSort.stringSort.byLengthAndAlphabet", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_array);
-  __Pyx_XDECREF(__pyx_v_sorted_array);
-  __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_s);
-  __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":109
- *     return SortedList([s.str for s in sorted_array])
+/* "camSort/stringSort.pyx":68
+ *     return byKey(input_list, 'length_and_alpha')
  * 
- * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ * def byAlphabet(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'alpha')
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_5byAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_10stringSort_5byAlphabet = {"byAlphabet", (PyCFunction)__pyx_pw_7camSort_10stringSort_5byAlphabet, METH_O, 0};
-static PyObject *__pyx_pw_7camSort_10stringSort_5byAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+static PyObject *__pyx_pw_7camSort_10stringSort_7byAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_7byAlphabet = {"byAlphabet", (PyCFunction)__pyx_pw_7camSort_10stringSort_7byAlphabet, METH_O, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_7byAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("byAlphabet (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_10stringSort_4byAlphabet(__pyx_self, ((PyObject *)__pyx_v_input_list));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_input_list), (&PyList_Type), 1, "input_list", 1))) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7camSort_10stringSort_6byAlphabet(__pyx_self, ((PyObject*)__pyx_v_input_list));
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_4byAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
-  CYTHON_UNUSED int __pyx_v_n;
-  PyObject *__pyx_v_array = 0;
-  PyObject *__pyx_v_sorted_array = NULL;
-  PyObject *__pyx_8genexpr6__pyx_v_s = NULL;
-  PyObject *__pyx_8genexpr7__pyx_v_s = NULL;
+static PyObject *__pyx_pf_7camSort_10stringSort_6byAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyObject *(*__pyx_t_4)(PyObject *);
+  int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("byAlphabet", 0);
 
-  /* "camSort/stringSort.pyx":110
- * 
- * def byAlphabet(input_list):
- *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
- *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
- * 
- */
-  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 110, __pyx_L1_error)
-  __pyx_v_n = __pyx_t_1;
-
-  /* "camSort/stringSort.pyx":111
- * def byAlphabet(input_list):
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]             # <<<<<<<<<<<<<<
- * 
- *     sorted_array = sorted(array, key=attrgetter('key'))
- */
-  { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
-      __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
-      __pyx_t_4 = NULL;
-    } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L5_error)
-    }
-    for (;;) {
-      if (likely(!__pyx_t_4)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 111, __pyx_L5_error)
-          #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          #endif
-        } else {
-          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 111, __pyx_L5_error)
-          #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          #endif
-        }
-      } else {
-        __pyx_t_5 = __pyx_t_4(__pyx_t_3);
-        if (unlikely(!__pyx_t_5)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 111, __pyx_L5_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_5);
-      }
-      __Pyx_XDECREF_SET(__pyx_8genexpr6__pyx_v_s, __pyx_t_5);
-      __pyx_t_5 = 0;
-      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_INCREF(__pyx_8genexpr6__pyx_v_s);
-      __Pyx_GIVEREF(__pyx_8genexpr6__pyx_v_s);
-      PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_8genexpr6__pyx_v_s);
-      __Pyx_INCREF(__pyx_n_u_alpha);
-      __Pyx_GIVEREF(__pyx_n_u_alpha);
-      PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_alpha);
-      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 111, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 111, __pyx_L5_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_s); __pyx_8genexpr6__pyx_v_s = 0;
-    goto __pyx_L8_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_s); __pyx_8genexpr6__pyx_v_s = 0;
-    goto __pyx_L1_error;
-    __pyx_L8_exit_scope:;
-  } /* exit inner scope */
-  __pyx_v_array = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
-
-  /* "camSort/stringSort.pyx":113
- *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+  /* "camSort/stringSort.pyx":69
  * 
- *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
- *     return SortedList([s.str for s in sorted_array])
+ * def byAlphabet(list input_list):
+ *     return byKey(input_list, 'alpha')             # <<<<<<<<<<<<<<
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_byKey); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_v_array);
-  __Pyx_GIVEREF(__pyx_v_array);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_7);
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_u_key);
-  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_sorted_array = __pyx_t_6;
-  __pyx_t_6 = 0;
-
-  /* "camSort/stringSort.pyx":114
- * 
- *     sorted_array = sorted(array, key=attrgetter('key'))
- *     return SortedList([s.str for s in sorted_array])             # <<<<<<<<<<<<<<
- */
-  __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 114, __pyx_L11_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
-      __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
-      __pyx_t_4 = NULL;
-    } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L11_error)
-    }
-    for (;;) {
-      if (likely(!__pyx_t_4)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 114, __pyx_L11_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L11_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        } else {
-          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 114, __pyx_L11_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L11_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        }
-      } else {
-        __pyx_t_2 = __pyx_t_4(__pyx_t_3);
-        if (unlikely(!__pyx_t_2)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 114, __pyx_L11_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_2);
-      }
-      __Pyx_XDECREF_SET(__pyx_8genexpr7__pyx_v_s, __pyx_t_2);
-      __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr7__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 114, __pyx_L11_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_input_list, __pyx_n_u_alpha};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_input_list, __pyx_n_u_alpha};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+  } else
+  #endif
+  {
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (__pyx_t_3) {
+      __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_s); __pyx_8genexpr7__pyx_v_s = 0;
-    goto __pyx_L14_exit_scope;
-    __pyx_L11_error:;
-    __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_s); __pyx_8genexpr7__pyx_v_s = 0;
-    goto __pyx_L1_error;
-    __pyx_L14_exit_scope:;
-  } /* exit inner scope */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
+    __Pyx_INCREF(__pyx_v_input_list);
+    __Pyx_GIVEREF(__pyx_v_input_list);
+    PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_input_list);
+    __Pyx_INCREF(__pyx_n_u_alpha);
+    __Pyx_GIVEREF(__pyx_n_u_alpha);
+    PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_n_u_alpha);
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":109
- *     return SortedList([s.str for s in sorted_array])
+  /* "camSort/stringSort.pyx":68
+ *     return byKey(input_list, 'length_and_alpha')
  * 
- * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ * def byAlphabet(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'alpha')
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("camSort.stringSort.byAlphabet", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_array);
-  __Pyx_XDECREF(__pyx_v_sorted_array);
-  __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_s);
-  __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_7__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_10stringSort_7__pyx_unpickle_StringWithKey = {"__pyx_unpickle_StringWithKey", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7camSort_10stringSort_7__pyx_unpickle_StringWithKey, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7camSort_10stringSort_7__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7camSort_10stringSort_9__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_9__pyx_unpickle_StringWithKey = {"__pyx_unpickle_StringWithKey", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7camSort_10stringSort_9__pyx_unpickle_StringWithKey, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_9__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -4527,22 +4127,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_StringWithKey", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_StringWithKey", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7camSort_10stringSort_6__pyx_unpickle_StringWithKey(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_8__pyx_unpickle_StringWithKey(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_6__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7camSort_10stringSort_8__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -4860,14 +4460,412 @@
   __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_StringWithKey__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+
+/* "(tree fragment)":1
+ * def __pyx_unpickle_SortedList(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_11__pyx_unpickle_SortedList(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_11__pyx_unpickle_SortedList = {"__pyx_unpickle_SortedList", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7camSort_10stringSort_11__pyx_unpickle_SortedList, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_11__pyx_unpickle_SortedList(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v___pyx_type = 0;
+  long __pyx_v___pyx_checksum;
+  PyObject *__pyx_v___pyx_state = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__pyx_unpickle_SortedList (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_SortedList", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_SortedList", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_SortedList") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+    }
+    __pyx_v___pyx_type = values[0];
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+    __pyx_v___pyx_state = values[2];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_SortedList", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_SortedList", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10__pyx_unpickle_SortedList(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_10__pyx_unpickle_SortedList(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_v___pyx_PickleError = 0;
+  PyObject *__pyx_v___pyx_result = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_SortedList", 0);
+
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum != 0x2cc5ac0:             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ */
+  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x2cc5ac0) != 0);
+  if (__pyx_t_1) {
+
+    /* "(tree fragment)":5
+ *     cdef object __pyx_result
+ *     if __pyx_checksum != 0x2cc5ac0:
+ *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ */
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_n_s_PickleError);
+    __Pyx_GIVEREF(__pyx_n_s_PickleError);
+    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
+    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_t_2);
+    __pyx_v___pyx_PickleError = __pyx_t_2;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "(tree fragment)":6
+ *     if __pyx_checksum != 0x2cc5ac0:
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ */
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x2c, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_INCREF(__pyx_v___pyx_PickleError);
+    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
+      }
+    }
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __PYX_ERR(1, 6, __pyx_L1_error)
+
+    /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum != 0x2cc5ac0:             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ */
+  }
+
+  /* "(tree fragment)":7
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ *     __pyx_result = SortedList.__new__(__pyx_type)             # <<<<<<<<<<<<<<
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v___pyx_result = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_6 = (__pyx_t_1 != 0);
+  if (__pyx_t_6) {
+
+    /* "(tree fragment)":9
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
+ *     return __pyx_result
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ */
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_7camSort_10stringSort___pyx_unpickle_SortedList__set_state(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  }
+
+  /* "(tree fragment)":10
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result             # <<<<<<<<<<<<<<
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_list = __pyx_state[0]
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v___pyx_result);
+  __pyx_r = __pyx_v___pyx_result;
+  goto __pyx_L0;
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_SortedList(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_SortedList", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v___pyx_PickleError);
+  __Pyx_XDECREF(__pyx_v___pyx_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":11
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ */
+
+static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_SortedList__set_state(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_SortedList__set_state", 0);
+
+  /* "(tree fragment)":12
+ *     return __pyx_result
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_list = __pyx_state[0]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->str_list);
+  __Pyx_DECREF(__pyx_v___pyx_result->str_list);
+  __pyx_v___pyx_result->str_list = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":13
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(1, 13, __pyx_L1_error)
+  }
+  __pyx_t_3 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_4 = ((__pyx_t_3 > 1) != 0);
+  if (__pyx_t_4) {
+  } else {
+    __pyx_t_2 = __pyx_t_4;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_4 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
+  __pyx_t_2 = __pyx_t_5;
+  __pyx_L4_bool_binop_done:;
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":14
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[1])             # <<<<<<<<<<<<<<
+ */
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(__pyx_v___pyx_state == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(1, 14, __pyx_L1_error)
+    }
+    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "(tree fragment)":13
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  }
+
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_SortedList__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
 static struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey __pyx_vtable_7camSort_10stringSort_StringWithKey;
 
 static PyObject *__pyx_tp_new_7camSort_10stringSort_StringWithKey(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7camSort_10stringSort_StringWithKey *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -5017,81 +5015,91 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
 };
 static struct __pyx_vtabstruct_7camSort_10stringSort_SortedList __pyx_vtable_7camSort_10stringSort_SortedList;
 
-static PyObject *__pyx_tp_new_7camSort_10stringSort_SortedList(PyTypeObject *t, PyObject *a, PyObject *k) {
+static PyObject *__pyx_tp_new_7camSort_10stringSort_SortedList(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7camSort_10stringSort_SortedList *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_7camSort_10stringSort_SortedList *)o);
   p->__pyx_vtab = __pyx_vtabptr_7camSort_10stringSort_SortedList;
-  if (unlikely(__pyx_pw_7camSort_10stringSort_10SortedList_1__cinit__(o, a, k) < 0)) goto bad;
+  p->str_list = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
-  bad:
-  Py_DECREF(o); o = 0;
-  return NULL;
 }
 
 static void __pyx_tp_dealloc_7camSort_10stringSort_SortedList(PyObject *o) {
+  struct __pyx_obj_7camSort_10stringSort_SortedList *p = (struct __pyx_obj_7camSort_10stringSort_SortedList *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
-  {
-    PyObject *etype, *eval, *etb;
-    PyErr_Fetch(&etype, &eval, &etb);
-    __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_7camSort_10stringSort_10SortedList_3__dealloc__(o);
-    __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
-    PyErr_Restore(etype, eval, etb);
-  }
+  PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->str_list);
   (*Py_TYPE(o)->tp_free)(o);
 }
+
+static int __pyx_tp_traverse_7camSort_10stringSort_SortedList(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_7camSort_10stringSort_SortedList *p = (struct __pyx_obj_7camSort_10stringSort_SortedList *)o;
+  if (p->str_list) {
+    e = (*v)(p->str_list, a); if (e) return e;
+  }
+  return 0;
+}
+
+static int __pyx_tp_clear_7camSort_10stringSort_SortedList(PyObject *o) {
+  PyObject* tmp;
+  struct __pyx_obj_7camSort_10stringSort_SortedList *p = (struct __pyx_obj_7camSort_10stringSort_SortedList *)o;
+  tmp = ((PyObject*)p->str_list);
+  p->str_list = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  return 0;
+}
 static PyObject *__pyx_sq_item_7camSort_10stringSort_SortedList(PyObject *o, Py_ssize_t i) {
   PyObject *r;
   PyObject *x = PyInt_FromSsize_t(i); if(!x) return 0;
   r = Py_TYPE(o)->tp_as_mapping->mp_subscript(o, x);
   Py_DECREF(x);
   return r;
 }
 
 static PyMethodDef __pyx_methods_7camSort_10stringSort_SortedList[] = {
-  {"reverse", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_5reverse, METH_NOARGS, 0},
-  {"to_list", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_7to_list, METH_NOARGS, 0},
-  {"__decode_string", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_9__decode_string, METH_O, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_15__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_17__setstate_cython__, METH_O, 0},
+  {"reverse", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_3reverse, METH_NOARGS, 0},
+  {"to_list", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_5to_list, METH_NOARGS, 0},
+  {"filterWithSubstring", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_11filterWithSubstring, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_13__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_15__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static PySequenceMethods __pyx_tp_as_sequence_SortedList = {
-  __pyx_pw_7camSort_10stringSort_10SortedList_13__len__, /*sq_length*/
+  __pyx_pw_7camSort_10stringSort_10SortedList_9__len__, /*sq_length*/
   0, /*sq_concat*/
   0, /*sq_repeat*/
   __pyx_sq_item_7camSort_10stringSort_SortedList, /*sq_item*/
   0, /*sq_slice*/
   0, /*sq_ass_item*/
   0, /*sq_ass_slice*/
   0, /*sq_contains*/
   0, /*sq_inplace_concat*/
   0, /*sq_inplace_repeat*/
 };
 
 static PyMappingMethods __pyx_tp_as_mapping_SortedList = {
-  __pyx_pw_7camSort_10stringSort_10SortedList_13__len__, /*mp_length*/
-  __pyx_pw_7camSort_10stringSort_10SortedList_11__getitem__, /*mp_subscript*/
+  __pyx_pw_7camSort_10stringSort_10SortedList_9__len__, /*mp_length*/
+  __pyx_pw_7camSort_10stringSort_10SortedList_7__getitem__, /*mp_subscript*/
   0, /*mp_ass_subscript*/
 };
 
 static PyTypeObject __pyx_type_7camSort_10stringSort_SortedList = {
   PyVarObject_HEAD_INIT(0, 0)
   "camSort.stringSort.SortedList", /*tp_name*/
   sizeof(struct __pyx_obj_7camSort_10stringSort_SortedList), /*tp_basicsize*/
@@ -5117,31 +5125,31 @@
   &__pyx_tp_as_mapping_SortedList, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  0, /*tp_traverse*/
-  0, /*tp_clear*/
+  __pyx_tp_traverse_7camSort_10stringSort_SortedList, /*tp_traverse*/
+  __pyx_tp_clear_7camSort_10stringSort_SortedList, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_7camSort_10stringSort_SortedList, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
-  0, /*tp_init*/
+  __pyx_pw_7camSort_10stringSort_10SortedList_1__init__, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_7camSort_10stringSort_SortedList, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
@@ -5202,190 +5210,150 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
+  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x2c, __pyx_k_Incompatible_checksums_s_vs_0x2c, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x2c), 0, 0, 1, 0},
   {&__pyx_kp_s_Incompatible_checksums_s_vs_0xef, __pyx_k_Incompatible_checksums_s_vs_0xef, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xef), 0, 0, 1, 0},
-  {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Invalid_argument_type, __pyx_k_Invalid_argument_type, sizeof(__pyx_k_Invalid_argument_type), 0, 1, 0, 0},
-  {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-  {&__pyx_kp_u_PyStringList_index_out_of_range, __pyx_k_PyStringList_index_out_of_range, sizeof(__pyx_k_PyStringList_index_out_of_range), 0, 1, 0, 0},
   {&__pyx_n_s_SortedList, __pyx_k_SortedList, sizeof(__pyx_k_SortedList), 0, 0, 1, 1},
   {&__pyx_n_s_StringWithKey, __pyx_k_StringWithKey, sizeof(__pyx_k_StringWithKey), 0, 0, 1, 1},
-  {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_u_alpha, __pyx_k_alpha, sizeof(__pyx_k_alpha), 0, 1, 0, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_attrgetter, __pyx_k_attrgetter, sizeof(__pyx_k_attrgetter), 0, 0, 1, 1},
   {&__pyx_n_s_byAlphabet, __pyx_k_byAlphabet, sizeof(__pyx_k_byAlphabet), 0, 0, 1, 1},
+  {&__pyx_n_s_byKey, __pyx_k_byKey, sizeof(__pyx_k_byKey), 0, 0, 1, 1},
   {&__pyx_n_s_byLength, __pyx_k_byLength, sizeof(__pyx_k_byLength), 0, 0, 1, 1},
   {&__pyx_n_s_byLengthAndAlphabet, __pyx_k_byLengthAndAlphabet, sizeof(__pyx_k_byLengthAndAlphabet), 0, 0, 1, 1},
   {&__pyx_n_s_camSort_stringSort, __pyx_k_camSort_stringSort, sizeof(__pyx_k_camSort_stringSort), 0, 0, 1, 1},
   {&__pyx_kp_s_camSort_stringSort_pyx, __pyx_k_camSort_stringSort_pyx, sizeof(__pyx_k_camSort_stringSort_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_decode_string, __pyx_k_decode_string, sizeof(__pyx_k_decode_string), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-  {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
+  {&__pyx_n_s_filterWithSubstring, __pyx_k_filterWithSubstring, sizeof(__pyx_k_filterWithSubstring), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_input_list, __pyx_k_input_list, sizeof(__pyx_k_input_list), 0, 0, 1, 1},
   {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
   {&__pyx_n_u_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 1, 0, 1},
   {&__pyx_n_s_key_type, __pyx_k_key_type, sizeof(__pyx_k_key_type), 0, 0, 1, 1},
   {&__pyx_n_u_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 1, 0, 1},
   {&__pyx_n_u_length_and_alpha, __pyx_k_length_and_alpha, sizeof(__pyx_k_length_and_alpha), 0, 1, 0, 1},
   {&__pyx_n_s_lower, __pyx_k_lower, sizeof(__pyx_k_lower), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
-  {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_operator, __pyx_k_operator, sizeof(__pyx_k_operator), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_py_list, __pyx_k_py_list, sizeof(__pyx_k_py_list), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_unpickle_SortedList, __pyx_k_pyx_unpickle_SortedList, sizeof(__pyx_k_pyx_unpickle_SortedList), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_StringWithKey, __pyx_k_pyx_unpickle_StringWithKey, sizeof(__pyx_k_pyx_unpickle_StringWithKey), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_reverse, __pyx_k_reverse, sizeof(__pyx_k_reverse), 0, 0, 1, 1},
   {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_sorted, __pyx_k_sorted, sizeof(__pyx_k_sorted), 0, 0, 1, 1},
   {&__pyx_n_s_sorted_array, __pyx_k_sorted_array, sizeof(__pyx_k_sorted_array), 0, 0, 1, 1},
-  {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
-  {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
-  {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
-  {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 46, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 48, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 86, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 89, __pyx_L1_error)
-  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 59, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "camSort/stringSort.pyx":86
- *         elif isinstance(item, int):
- *             if item < 0 or item >= self.size:
- *                 raise IndexError("PyStringList index out of range")             # <<<<<<<<<<<<<<
- *             return self.__decode_string(item)
- *         else:
+  /* "camSort/stringSort.pyx":57
+ *         return [s for s in self.str_list if substring in s]
+ * 
+ * def byKey(list input_list, str key_type):             # <<<<<<<<<<<<<<
+ *     cdef list array = [StringWithKey(s, key_type) for s in input_list]
+ *     sorted_array = sorted(array, key=attrgetter('key'))
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_PyStringList_index_out_of_range); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_key_type, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byKey, 57, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 57, __pyx_L1_error)
 
-  /* "camSort/stringSort.pyx":89
- *             return self.__decode_string(item)
- *         else:
- *             raise TypeError("Invalid argument type.")             # <<<<<<<<<<<<<<
+  /* "camSort/stringSort.pyx":62
+ *     return SortedList([s.str for s in sorted_array])
+ * 
+ * def byLength(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'length')
  * 
- *     def __len__(self):
- */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Invalid_argument_type); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "(tree fragment)":2
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_input_list); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLength, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 62, __pyx_L1_error)
 
-  /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
-  /* "camSort/stringSort.pyx":95
+  /* "camSort/stringSort.pyx":65
+ *     return byKey(input_list, 'length')
  * 
+ * def byLengthAndAlphabet(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'length_and_alpha')
  * 
- * def byLength(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s) for s in input_list]
  */
-  __pyx_tuple__5 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_input_list); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLength, 95, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLengthAndAlphabet, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 65, __pyx_L1_error)
 
-  /* "camSort/stringSort.pyx":102
- *     return SortedList([s.str for s in sorted_array])
+  /* "camSort/stringSort.pyx":68
+ *     return byKey(input_list, 'length_and_alpha')
  * 
- * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ * def byAlphabet(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'alpha')
  */
-  __pyx_tuple__7 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_n_s_input_list); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLengthAndAlphabet, 102, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 102, __pyx_L1_error)
-
-  /* "camSort/stringSort.pyx":109
- *     return SortedList([s.str for s in sorted_array])
- * 
- * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
- */
-  __pyx_tuple__9 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byAlphabet, 109, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byAlphabet, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 68, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
+  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StringWithKey, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StringWithKey, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_SortedList, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_46947008 = PyInt_FromLong(46947008L); if (unlikely(!__pyx_int_46947008)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_250931038 = PyInt_FromLong(250931038L); if (unlikely(!__pyx_int_250931038)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -5427,37 +5395,38 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_7camSort_10stringSort_StringWithKey = &__pyx_vtable_7camSort_10stringSort_StringWithKey;
   __pyx_vtable_7camSort_10stringSort_StringWithKey.calculate_key = (PY_LONG_LONG (*)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *))__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key;
   __pyx_vtable_7camSort_10stringSort_StringWithKey.calculate_key_alpha = (PyObject *(*)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *))__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_alpha;
   __pyx_vtable_7camSort_10stringSort_StringWithKey.calculate_key_length_alpha = (PY_LONG_LONG (*)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *))__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_length_alpha;
-  if (PyType_Ready(&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7camSort_10stringSort_StringWithKey.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7camSort_10stringSort_StringWithKey.tp_dictoffset && __pyx_type_7camSort_10stringSort_StringWithKey.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7camSort_10stringSort_StringWithKey.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7camSort_10stringSort_StringWithKey.tp_dict, __pyx_vtabptr_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringWithKey, (PyObject *)&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7camSort_10stringSort_StringWithKey.tp_dict, __pyx_vtabptr_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringWithKey, (PyObject *)&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __pyx_ptype_7camSort_10stringSort_StringWithKey = &__pyx_type_7camSort_10stringSort_StringWithKey;
   __pyx_vtabptr_7camSort_10stringSort_SortedList = &__pyx_vtable_7camSort_10stringSort_SortedList;
   __pyx_vtable_7camSort_10stringSort_SortedList.reverse = (struct __pyx_obj_7camSort_10stringSort_SortedList *(*)(struct __pyx_obj_7camSort_10stringSort_SortedList *, int __pyx_skip_dispatch))__pyx_f_7camSort_10stringSort_10SortedList_reverse;
-  if (PyType_Ready(&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_vtable_7camSort_10stringSort_SortedList.filterWithSubstring = (PyObject *(*)(struct __pyx_obj_7camSort_10stringSort_SortedList *, PyObject *, int __pyx_skip_dispatch))__pyx_f_7camSort_10stringSort_10SortedList_filterWithSubstring;
+  if (PyType_Ready(&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7camSort_10stringSort_SortedList.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7camSort_10stringSort_SortedList.tp_dictoffset && __pyx_type_7camSort_10stringSort_SortedList.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7camSort_10stringSort_SortedList.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7camSort_10stringSort_SortedList.tp_dict, __pyx_vtabptr_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SortedList, (PyObject *)&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7camSort_10stringSort_SortedList.tp_dict, __pyx_vtabptr_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SortedList, (PyObject *)&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __pyx_ptype_7camSort_10stringSort_SortedList = &__pyx_type_7camSort_10stringSort_SortedList;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -5688,16 +5657,16 @@
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "camSort/stringSort.pyx":2
  * # cython: language_level=3
  * from operator import attrgetter             # <<<<<<<<<<<<<<
- * from libc.stdlib cimport malloc, free
- * from libc.string cimport strdup
+ * cimport cython
+ * 
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_attrgetter);
   __Pyx_GIVEREF(__pyx_n_s_attrgetter);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_attrgetter);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_operator, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
@@ -5705,64 +5674,87 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_attrgetter, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":95
- * 
+  /* "camSort/stringSort.pyx":57
+ *         return [s for s in self.str_list if substring in s]
  * 
- * def byLength(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s) for s in input_list]
+ * def byKey(list input_list, str key_type):             # <<<<<<<<<<<<<<
+ *     cdef list array = [StringWithKey(s, key_type) for s in input_list]
+ *     sorted_array = sorted(array, key=attrgetter('key'))
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_1byLength, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_1byKey, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLength, __pyx_t_2) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byKey, __pyx_t_2) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":102
+  /* "camSort/stringSort.pyx":62
  *     return SortedList([s.str for s in sorted_array])
  * 
- * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ * def byLength(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'length')
+ * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_3byLengthAndAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_3byLength, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLengthAndAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLength, __pyx_t_2) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":109
- *     return SortedList([s.str for s in sorted_array])
+  /* "camSort/stringSort.pyx":65
+ *     return byKey(input_list, 'length')
+ * 
+ * def byLengthAndAlphabet(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'length_and_alpha')
+ * 
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_5byLengthAndAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLengthAndAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "camSort/stringSort.pyx":68
+ *     return byKey(input_list, 'length_and_alpha')
  * 
- * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
- *     cdef int n = len(input_list)
- *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ * def byAlphabet(list input_list):             # <<<<<<<<<<<<<<
+ *     return byKey(input_list, 'alpha')
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_5byAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_7byAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_7__pyx_unpickle_StringWithKey, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_9__pyx_unpickle_StringWithKey, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_StringWithKey, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_StringWithKey__set_state(<StringWithKey> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_StringWithKey__set_state(StringWithKey __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.key = __pyx_state[0]; __pyx_result.str = __pyx_state[1]
+ *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_11__pyx_unpickle_SortedList, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_SortedList, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
   /* "camSort/stringSort.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * from operator import attrgetter
- * from libc.stdlib cimport malloc, free
+ * cimport cython
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
@@ -5974,14 +5966,35 @@
     }
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
+/* ArgTypeTest */
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+{
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    }
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
+        name, type->tp_name, Py_TYPE(obj)->tp_name);
+    return 0;
+}
+
 /* BytesEquals */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
 #if CYTHON_COMPILING_IN_PYPY
     return PyObject_RichCompareBool(s1, s2, equals);
 #else
     if (s1 == s2) {
         return (equals == Py_EQ);
@@ -6123,14 +6136,30 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
+/* unicode_iter */
+static CYTHON_INLINE int __Pyx_init_unicode_iteration(
+    PyObject* ustring, Py_ssize_t *length, void** data, int *kind) {
+#if CYTHON_PEP393_ENABLED
+    if (unlikely(__Pyx_PyUnicode_READY(ustring) < 0)) return -1;
+    *kind   = PyUnicode_KIND(ustring);
+    *length = PyUnicode_GET_LENGTH(ustring);
+    *data   = PyUnicode_DATA(ustring);
+#else
+    *kind   = 0;
+    *length = PyUnicode_GET_SIZE(ustring);
+    *data   = (void*)PyUnicode_AS_UNICODE(ustring);
+#endif
+    return 0;
+}
+
 /* UnicodeAsUCS4 */
 static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject* x) {
    Py_ssize_t length;
    #if CYTHON_PEP393_ENABLED
    length = PyUnicode_GET_LENGTH(x);
    if (likely(length == 1)) {
        return PyUnicode_READ_CHAR(x, 0);
@@ -6607,32 +6636,83 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* ArgTypeTest */
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
-{
+/* SliceTupleAndList */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_crop_slice(Py_ssize_t* _start, Py_ssize_t* _stop, Py_ssize_t* _length) {
+    Py_ssize_t start = *_start, stop = *_stop, length = *_length;
+    if (start < 0) {
+        start += length;
+        if (start < 0)
+            start = 0;
+    }
+    if (stop < 0)
+        stop += length;
+    else if (stop > length)
+        stop = length;
+    *_length = stop - start;
+    *_start = start;
+    *_stop = stop;
+}
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject** CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject* __Pyx_PyList_GetSlice(
+            PyObject* src, Py_ssize_t start, Py_ssize_t stop) {
+    PyObject* dest;
+    Py_ssize_t length = PyList_GET_SIZE(src);
+    __Pyx_crop_slice(&start, &stop, &length);
+    if (unlikely(length <= 0))
+        return PyList_New(0);
+    dest = PyList_New(length);
+    if (unlikely(!dest))
+        return NULL;
+    __Pyx_copy_object_array(
+        ((PyListObject*)src)->ob_item + start,
+        ((PyListObject*)dest)->ob_item,
+        length);
+    return dest;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_GetSlice(
+            PyObject* src, Py_ssize_t start, Py_ssize_t stop) {
+    PyObject* dest;
+    Py_ssize_t length = PyTuple_GET_SIZE(src);
+    __Pyx_crop_slice(&start, &stop, &length);
+    if (unlikely(length <= 0))
+        return PyTuple_New(0);
+    dest = PyTuple_New(length);
+    if (unlikely(!dest))
+        return NULL;
+    __Pyx_copy_object_array(
+        ((PyTupleObject*)src)->ob_item + start,
+        ((PyTupleObject*)dest)->ob_item,
+        length);
+    return dest;
+}
+#endif
+
+/* ExtTypeTest */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
-    else if (exact) {
-        #if PY_MAJOR_VERSION == 2
-        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
-        #endif
-    }
-    else {
-        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
-    }
-    PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
     return 0;
 }
 
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
@@ -6715,14 +6795,43 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* ObjectGetItem */
+#if CYTHON_USE_TYPE_SLOTS
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
+    PyObject *runerr;
+    Py_ssize_t key_value;
+    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
+    if (unlikely(!(m && m->sq_item))) {
+        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
+        return NULL;
+    }
+    key_value = __Pyx_PyIndex_AsSsize_t(index);
+    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
+        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
+    }
+    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        PyErr_Clear();
+        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
+    }
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
+    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
+    if (likely(m && m->mp_subscript)) {
+        return m->mp_subscript(obj, key);
+    }
+    return __Pyx_PyObject_GetIndex(obj, key);
+}
+#endif
+
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -6744,58 +6853,91 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
-/* ExtTypeTest */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
+/* Import */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *empty_list = 0;
+    PyObject *module = 0;
+    PyObject *global_dict = 0;
+    PyObject *empty_dict = 0;
+    PyObject *list;
+    #if PY_MAJOR_VERSION < 3
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (!py_import)
+        goto bad;
+    #endif
+    if (from_list)
+        list = from_list;
+    else {
+        empty_list = PyList_New(0);
+        if (!empty_list)
+            goto bad;
+        list = empty_list;
     }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
+    global_dict = PyModule_GetDict(__pyx_m);
+    if (!global_dict)
+        goto bad;
+    empty_dict = PyDict_New();
+    if (!empty_dict)
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                module = PyImport_ImportModuleLevelObject(
+                    name, global_dict, empty_dict, list, 1);
+                if (!module) {
+                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                        goto bad;
+                    PyErr_Clear();
+                }
+            }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_MAJOR_VERSION < 3
+            PyObject *py_level = PyInt_FromLong(level);
+            if (!py_level)
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+            Py_DECREF(py_level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, global_dict, empty_dict, list, level);
+            #endif
+        }
+    }
+bad:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_import);
+    #endif
+    Py_XDECREF(empty_list);
+    Py_XDECREF(empty_dict);
+    return module;
 }
 
-/* decode_c_string */
-static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
-         const char* cstring, Py_ssize_t start, Py_ssize_t stop,
-         const char* encoding, const char* errors,
-         PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
-    Py_ssize_t length;
-    if (unlikely((start < 0) | (stop < 0))) {
-        size_t slen = strlen(cstring);
-        if (unlikely(slen > (size_t) PY_SSIZE_T_MAX)) {
-            PyErr_SetString(PyExc_OverflowError,
-                            "c-string too long to convert to Python");
-            return NULL;
-        }
-        length = (Py_ssize_t) slen;
-        if (start < 0) {
-            start += length;
-            if (start < 0)
-                start = 0;
-        }
-        if (stop < 0)
-            stop += length;
-    }
-    if (unlikely(stop <= start))
-        return __Pyx_NewRef(__pyx_empty_unicode);
-    length = stop - start;
-    cstring += start;
-    if (decode_func) {
-        return decode_func(cstring, length, errors);
-    } else {
-        return PyUnicode_Decode(cstring, length, encoding, errors);
+/* ImportFrom */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
+    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        PyErr_Format(PyExc_ImportError,
+        #if PY_MAJOR_VERSION < 3
+            "cannot import name %.230s", PyString_AS_STRING(name));
+        #else
+            "cannot import name %S", name);
+        #endif
     }
+    return value;
 }
 
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
@@ -6949,93 +7091,14 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
-    PyObject *module = 0;
-    PyObject *global_dict = 0;
-    PyObject *empty_dict = 0;
-    PyObject *list;
-    #if PY_MAJOR_VERSION < 3
-    PyObject *py_import;
-    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
-        goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
-        empty_list = PyList_New(0);
-        if (!empty_list)
-            goto bad;
-        list = empty_list;
-    }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
-    empty_dict = PyDict_New();
-    if (!empty_dict)
-        goto bad;
-    {
-        #if PY_MAJOR_VERSION >= 3
-        if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
-                        goto bad;
-                    PyErr_Clear();
-                }
-            }
-            level = 0;
-        }
-        #endif
-        if (!module) {
-            #if PY_MAJOR_VERSION < 3
-            PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
-                goto bad;
-            module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
-            Py_DECREF(py_level);
-            #else
-            module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
-            #endif
-        }
-    }
-bad:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(py_import);
-    #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
-    return module;
-}
-
-/* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
-    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
-    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
-        PyErr_Format(PyExc_ImportError,
-        #if PY_MAJOR_VERSION < 3
-            "cannot import name %.230s", PyString_AS_STRING(name));
-        #else
-            "cannot import name %S", name);
-        #endif
-    }
-    return value;
-}
-
 /* HasAttr */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
@@ -7481,45 +7544,14 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(PY_LONG_LONG),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
     const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(long) <= sizeof(unsigned long)) {
@@ -7543,203 +7575,14 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (int) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (int) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if (sizeof(int) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            int val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (int) -1;
-        }
-    } else {
-        int val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (int) -1;
-        val = __Pyx_PyInt_As_int(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to int");
-    return (int) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to int");
-    return (int) -1;
-}
-
-/* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
     const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
@@ -7921,163 +7764,163 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
-    const size_t neg_one = (size_t) ((size_t) 0 - (size_t) 1), const_zero = (size_t) 0;
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(size_t) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
+        if (sizeof(int) < sizeof(long)) {
+            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (size_t) val;
+            return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(size_t, digit, digits[0])
+                case  0: return (int) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 2 * PyLong_SHIFT) {
-                            return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
+                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 3 * PyLong_SHIFT) {
-                            return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
+                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
-                            return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
+                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (size_t) -1;
+                    return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(size_t) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned long, PyLong_AsUnsignedLong(x))
+            if (sizeof(int) <= sizeof(unsigned long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(size_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(size_t,  digit, +digits[0])
+                case  0: return (int) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(size_t) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, long, PyLong_AsLong(x))
+            if (sizeof(int) <= sizeof(long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
 #if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
                             "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
 #else
-            size_t val;
+            int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -8089,32 +7932,32 @@
                                               bytes, sizeof(val),
                                               is_little, !is_unsigned);
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
 #endif
-            return (size_t) -1;
+            return (int) -1;
         }
     } else {
-        size_t val;
+        int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (size_t) -1;
-        val = __Pyx_PyInt_As_size_t(tmp);
+        if (!tmp) return (int) -1;
+        val = __Pyx_PyInt_As_int(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to size_t");
-    return (size_t) -1;
+        "value too large to convert to int");
+    return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to size_t");
-    return (size_t) -1;
+        "can't convert negative value to int");
+    return (int) -1;
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
```

### Comparing `camSort-0.3.1/setup.py` & `camSort-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
 
     name="camSort",
-    version="0.3.1",
+    version="0.4",
     install_requires=["setuptools", "wheel", "cython"],
 
     ext_modules = cythonize(['camSort/stringSort.pyx']),
 
     author=["cameronbae / cameron jay"],
     author_email="<contact@camjay.io>",
     description="make sorted() fast for strings",
```

