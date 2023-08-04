# Comparing `tmp/pyevspace-0.14.0.tar.gz` & `tmp/pyevspace-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevspace-0.14.0.tar", last modified: Mon Jul 31 05:57:22 2023, max compression
+gzip compressed data, was "pyevspace-0.14.1.tar", last modified: Fri Aug  4 02:36:04 2023, max compression
```

## Comparing `pyevspace-0.14.0.tar` & `pyevspace-0.14.1.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.650717 pyevspace-0.14.0/
--rw-rw-rw-   0        0        0     1090 2023-07-31 05:39:21.000000 pyevspace-0.14.0/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-01-13 04:56:37.000000 pyevspace-0.14.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3525 2023-07-31 05:57:22.649719 pyevspace-0.14.0/PKG-INFO
--rw-rw-rw-   0        0        0     2551 2023-07-31 05:39:21.000000 pyevspace-0.14.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 05:57:22.650717 pyevspace-0.14.0/setup.cfg
--rw-rw-rw-   0        0        0     1578 2023-07-31 05:39:21.000000 pyevspace-0.14.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.617137 pyevspace-0.14.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.632765 pyevspace-0.14.0/src/pyevspace/
--rw-rw-rw-   0        0        0      152 2023-07-31 05:39:21.000000 pyevspace-0.14.0/src/pyevspace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.630772 pyevspace-0.14.0/src/pyevspace/src/
--rw-rw-rw-   0        0        0    25597 2023-07-31 05:39:21.000000 pyevspace-0.14.0/src/pyevspace/src/evspacemodule.c
-drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.644732 pyevspace-0.14.0/src/pyevspace.egg-info/
--rw-rw-rw-   0        0        0     3525 2023-07-31 05:57:22.000000 pyevspace-0.14.0/src/pyevspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-31 05:57:22.000000 pyevspace-0.14.0/src/pyevspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 05:57:22.000000 pyevspace-0.14.0/src/pyevspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 05:57:22.000000 pyevspace-0.14.0/src/pyevspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 02:35:56.000000 pyevspace-0.14.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 02:35:56.000000 pyevspace-0.14.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-04 02:36:04.067542 pyevspace-0.14.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-04 02:35:56.000000 pyevspace-0.14.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 02:36:04.071542 pyevspace-0.14.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-04 02:35:56.000000 pyevspace-0.14.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/pyevspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/pyevspace/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_angles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25681 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_refframe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_rotation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23275 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspace_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/include/evspacemodule.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/pyevspace/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-08-04 02:35:56.000000 pyevspace-0.14.1/src/pyevspace/src/evspacemodule.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:36:04.067542 pyevspace-0.14.1/src/pyevspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-04 02:36:04.000000 pyevspace-0.14.1/src/pyevspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-04 02:36:04.000000 pyevspace-0.14.1/src/pyevspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:36:04.000000 pyevspace-0.14.1/src/pyevspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 02:36:04.000000 pyevspace-0.14.1/src/pyevspace.egg-info/top_level.txt
```

### Comparing `pyevspace-0.14.0/PKG-INFO` & `pyevspace-0.14.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,131 +1,135 @@
-Metadata-Version: 2.1
-Name: pyevspace
-Version: 0.14.0
-Summary: A Python 3-dimensional Euclidean vector space.
-Home-page: https://github.com/qbizzle68/pyevspace
-Author: Quinton Barnes
-Author-email: devqbizzle68@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PyEVSpace 0.14.0
-
-PyEVSpace is a Python Euclidean vector space package containing types
-and methods for representing vector quantites and fasilitating rotating
-them between reference frames. PyEVSpace is designed for 3-dimensional
-space only, which allows for optimum speed since size checks do not
-occur.
-
-
-## Documentation
-
-The full documentation of this project with both Python and C APIs can
-be found [here](https://qbizzle68.github.io/pyevspace/html/index.html).
-
-## Install
-
-The python module can be installed with
-```python
-pip install pyevspace
-```
-
-Alternatively the repository can be downloaded or cloned using:
-```bash
-git clone https://github.com/qbizzle68/pyevspace.git
-```
-It can be used as is within Visual Studio, or built inplace using the
-*setup.py* if needed.
-
-## Usage
-
-To use the module simply import the pyevspace module into your project:
-```python
-import pyevspace as evs
-from math import pi
-
-vec = evs.Vector(1, 2, 3)
-
-rotatedVec = evs.rotateAxisTo(evs.X_AXIS, pi/2)
-```
-
-Matrices can be created from iterables, where each iterable represents
-a row of the matrix
-```python
-import pyevspace as evs
-
-mat = evs.Matrix((0, 0, 1), (0, -1, 0), (1, 0, 0))
-
-rotatedVec = evs.rotateMatrixFrom(mat, Vector(1, 1, 1))
-```
-
-The Order and Angles types can be used to create an Euler rotation 
-matrix. All twelve Euler rotations are already defined in the module,
-so you shouldn't need to instantiate an Order object. The Angles
-object holds the angles for each rotation in the Euler rotation, in
-the order of the axis rotations (in radians).
-```python
-import pyevspace as evs
-
-angs = Angles(1.1, 4.5, 3.14)
-mat = getMatrixEuler(XYZ, angs)
-
-rotatedVec = mat * Vector(1, 0, 2)
-```
-
-There are many methods that handle the rotations for you, check the
-official documentation to learn more about them.
-
-## Examples
-
-### Examples of numeric operators
-```python
-v1 = Vector(1, 2, 3)
-v2 = Vector(4, 5, 6)
-
-print(v1 * 2)
-# prints [2, 4, 6]
-
-print(v1 + v2)
-# prints [5, 7, 9]
-
-print(v1 - v2)
-# prints [-3, -3, -3]
-```
-
-### Examples of vector and matrix operators
-```python
-v1 = Vector(1, 2, 3)
-v2 = Vector(4, 5, 6)
-m1 = Matrix(Vector(4, 2, 3), Vector(8, 5, 2), Vector(4, 2, 1))
-
-print(dot(v1, v2))
-# prints 32.0
-
-print(cross(v1, v2))
-# prints [ -3.00000, 6.00000, -3.00000 ]
-
-print(det(m1))
-# prints -8.0
-
-print(transpose(m1))
-# prints 
-# ([4, 2, 3],
-# [8, 5, 2],
-# [4, 2, 1])
-```
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: pyevspace
+Version: 0.14.1
+Summary: A Python 3-dimensional Euclidean vector space.
+Home-page: https://github.com/qbizzle68/pyevspace
+Author: Quinton Barnes
+Author-email: devqbizzle68@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# PyEVSpace 0.14.1
+
+This version of PyEVSpace is no functionally different than 0.14.0.
+This version was published to pypi using automated scripting workflows,
+and its existence means everything works!!
+
+PyEVSpace is a Python Euclidean vector space package containing types
+and methods for representing vector quantites and fasilitating rotating
+them between reference frames. PyEVSpace is designed for 3-dimensional
+space only, which allows for optimum speed since size checks do not
+occur.
+
+
+## Documentation
+
+The full documentation of this project with both Python and C APIs can
+be found [here](https://qbizzle68.github.io/pyevspace/html/index.html).
+
+## Install
+
+The python module can be installed with
+```python
+pip install pyevspace
+```
+
+Alternatively the repository can be downloaded or cloned using:
+```bash
+git clone https://github.com/qbizzle68/pyevspace.git
+```
+It can be used as is within Visual Studio, or built inplace using the
+*setup.py* if needed.
+
+## Usage
+
+To use the module simply import the pyevspace module into your project:
+```python
+import pyevspace as evs
+from math import pi
+
+vec = evs.Vector(1, 2, 3)
+
+rotatedVec = evs.rotateAxisTo(evs.X_AXIS, pi/2)
+```
+
+Matrices can be created from iterables, where each iterable represents
+a row of the matrix
+```python
+import pyevspace as evs
+
+mat = evs.Matrix((0, 0, 1), (0, -1, 0), (1, 0, 0))
+
+rotatedVec = evs.rotateMatrixFrom(mat, Vector(1, 1, 1))
+```
+
+The Order and Angles types can be used to create an Euler rotation 
+matrix. All twelve Euler rotations are already defined in the module,
+so you shouldn't need to instantiate an Order object. The Angles
+object holds the angles for each rotation in the Euler rotation, in
+the order of the axis rotations (in radians).
+```python
+import pyevspace as evs
+
+angs = Angles(1.1, 4.5, 3.14)
+mat = getMatrixEuler(XYZ, angs)
+
+rotatedVec = mat * Vector(1, 0, 2)
+```
+
+There are many methods that handle the rotations for you, check the
+official documentation to learn more about them.
+
+## Examples
+
+### Examples of numeric operators
+```python
+v1 = Vector(1, 2, 3)
+v2 = Vector(4, 5, 6)
+
+print(v1 * 2)
+# prints [2, 4, 6]
+
+print(v1 + v2)
+# prints [5, 7, 9]
+
+print(v1 - v2)
+# prints [-3, -3, -3]
+```
+
+### Examples of vector and matrix operators
+```python
+v1 = Vector(1, 2, 3)
+v2 = Vector(4, 5, 6)
+m1 = Matrix(Vector(4, 2, 3), Vector(8, 5, 2), Vector(4, 2, 1))
+
+print(dot(v1, v2))
+# prints 32.0
+
+print(cross(v1, v2))
+# prints [ -3.00000, 6.00000, -3.00000 ]
+
+print(det(m1))
+# prints -8.0
+
+print(transpose(m1))
+# prints 
+# ([4, 2, 3],
+# [8, 5, 2],
+# [4, 2, 1])
+```
+
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `pyevspace-0.14.0/src/pyevspace/src/evspacemodule.c` & `pyevspace-0.14.1/src/pyevspace/src/evspacemodule.c`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,706 +1,706 @@
-﻿#define PY_SSIZE_T_CLEAN
-#include <Python.h>
-#include <structmember.h> // PyMemberDef
-
-/* don't need the extra's for the C API */
-#define _EVSPACE_IMPL
-#include <evspacemodule.h>
-#include <evspace_vector.h>
-#include <evspace_matrix.h>
-#include <evspace_angles.h>
-#include <evspace_rotation.h>
-#include <evspace_refframe.h>
-
-
-/* EVSpace_VectorType definition */
-
-static PyNumberMethods vector_as_number = {
-    .nb_add                 = (binaryfunc)vector_add,
-    .nb_subtract            = (binaryfunc)vector_subtract,
-    .nb_multiply            = (binaryfunc)vector_multiply,
-    .nb_negative            = (unaryfunc)vector_negative,
-    .nb_inplace_add         = (binaryfunc)vector_iadd,
-    .nb_inplace_subtract    = (binaryfunc)vector_isubtract,
-    .nb_inplace_multiply    = (binaryfunc)vector_imultiply,
-    .nb_true_divide         = (binaryfunc)vector_divide,
-    .nb_inplace_true_divide = (binaryfunc)vector_idivide,
-    .nb_matrix_multiply     = (binaryfunc)vector_multiply_matrix,
-    .nb_inplace_matrix_multiply = (binaryfunc)vector_mat_imultiply
-};
-
-static PySequenceMethods vector_as_sequence = {
-    .sq_length      = (lenfunc)vector_length,
-    .sq_item        = (ssizeargfunc)vector_get_item,
-    .sq_ass_item    = (ssizeobjargproc)vector_set_item
-};
-
-static PyBufferProcs vector_buffer = {
-    .bf_getbuffer       = (getbufferproc)vector_get_buffer,
-    .bf_releasebuffer   = (releasebufferproc)release_buffer
-};
-
-PyDoc_STRVAR(vector_mag2_doc, "mag() -> float\n\
-\n\
-Computes the square of the magnitude of a vector. Eliminates\n\
-round-off error when squaring the result of mag().");
-
-PyDoc_STRVAR(vector_norm_doc, "normalize() -> Vector\n\
-\n\
-Modifies the vector to a length of 1, while preserving\n\
-its direction.");
-
-PyDoc_STRVAR(vector_reduce_doc, "__reduce__() -> (cls, (x, y, z))\n\
-\n\
-Allows pickling of the Vector type by returning the constructor\n\
-and arguments to recreate the Vector.");
-
-static PyMethodDef vector_methods[] = {
-
-    /* instance methods */
-
-    {"mag",         (PyCFunction)vector_magnitude, METH_NOARGS,
-     PyDoc_STR("mag() -> float\n\nComputes the magnitude of a vector.")},
-
-    {"mag2",        (PyCFunction)vector_magnitude_square, METH_NOARGS, 
-     vector_mag2_doc},
-
-    {"normalize",   (PyCFunction)vector_normalize, METH_NOARGS,
-     vector_norm_doc},
-
-    {"__reduce__",  (PyCFunction)vector_reduce, METH_NOARGS, 
-     vector_reduce_doc},
-
-    {NULL}
-};
-
-PyDoc_STRVAR(vector_doc, "Vector([{x, y, z | iterable}])\n\
-\n\
-The Vector can be constructed with an iterable of length 3, or\n\
-directly with the x, y and z components. All components must be\n\
-numeric types. Alternatively the components will default to zero\n\
-if no argument is specified.");
-
-static PyTypeObject EVSpace_VectorType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name        = "pyevspace.Vector",
-    .tp_basicsize   = sizeof(EVSpace_Vector),
-    .tp_itemsize    = 0,
-    .tp_repr        = (reprfunc)vector_repr,
-    .tp_as_number   = &vector_as_number,
-    .tp_as_sequence = &vector_as_sequence,
-    .tp_str         = (reprfunc)vector_str,
-    .tp_as_buffer   = &vector_buffer,
-#if PY_VERSION_HEX >= 0x03100000
-    .tp_flags       = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_SEQUENCE,
-#else
-    .tp_flags       = Py_TPFLAGS_DEFAULT,
-#endif
-    .tp_doc         = vector_doc,
-    .tp_richcompare = (richcmpfunc)&vector_richcompare,
-    .tp_iter        = (getiterfunc)vector_iter,
-    .tp_methods     = vector_methods,
-    .tp_new         = (newfunc)vector_new,
-    .tp_free        = (freefunc)vector_free
-};
-
-
-/* EVSpace_MatrixType definition*/
-
-static PyNumberMethods matrix_as_number = {
-    .nb_add             = (binaryfunc)matrix_add,
-    .nb_subtract        = (binaryfunc)matrix_subtract,
-    .nb_multiply        = (binaryfunc)matrix_multiply,
-    .nb_negative        = (unaryfunc)matrix_negative,
-    .nb_inplace_add     = (binaryfunc)matrix_iadd,
-    .nb_inplace_subtract = (binaryfunc)matrix_isubtract,
-    .nb_inplace_multiply = (binaryfunc)matrix_imultiply,
-    .nb_true_divide     = (binaryfunc)matrix_divide,
-    .nb_inplace_true_divide = (binaryfunc)matrix_idivide,
-    .nb_matrix_multiply = (binaryfunc)matrix_mat_multiply,
-    .nb_inplace_matrix_multiply = (binaryfunc)matrix_mat_imultiply
-};
-
-static PyMappingMethods matrix_as_mapping = {
-    .mp_subscript       = (binaryfunc)matrix_get_item,
-    .mp_ass_subscript   = (objobjargproc)matrix_set_item
-};
-
-static PyBufferProcs matrix_buffer = {
-    .bf_getbuffer       = (getbufferproc)matrix_get_buffer,
-    .bf_releasebuffer   = (releasebufferproc)release_buffer
-};
-
-PyDoc_STRVAR(matrix_reduce_doc, "__reduce__() -> (cls, state)\n\
-\n\
-Allows pickling of the Matrix type by returning the constructor\n\
-and arguments to recreate the Matrix.");
-
-static PyMethodDef matrix_methods[] = {
-    {"__reduce__", (PyCFunction)matrix_reduce, METH_NOARGS, 
-     matrix_reduce_doc},
-
-    {NULL}
-};
-
-PyDoc_STRVAR(matrix_doc, "Matrix([row0, row1, row2])\n\
-\n\
-The Matrix can be constructed with three iterables, all of length\n\
-three, whose components are numeric types. Each iterable represents\n\
-a row of the matrix and are all required. Alternatively if no arguments\n\
-are present each component is defaulted to zero.");
-
-static PyTypeObject EVSpace_MatrixType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name        = "pyevspace.Matrix",
-    .tp_basicsize   = sizeof(EVSpace_Matrix),
-    .tp_itemsize    = 0,
-    .tp_repr        = (reprfunc)matrix_repr,
-    .tp_as_number   = &matrix_as_number,
-    .tp_as_mapping  = &matrix_as_mapping,
-    .tp_str         = (reprfunc)matrix_str,
-    .tp_as_buffer   = &matrix_buffer,
-#if PY_VERSION_HEX >= 0x03100000
-    .tp_flags       = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_MAPPING,
-#else
-    .tp_flags       = Py_TPFLAGS_DEFAULT,
-#endif
-    .tp_doc         = matrix_doc,
-    .tp_richcompare = (richcmpfunc)&matrix_richcompare,
-    .tp_methods     = matrix_methods,
-    .tp_new         = (newfunc)matrix_new,
-    .tp_free        = (freefunc)matrix_free
-};
-
-static PySequenceMethods angles_as_sequence = {
-    .sq_length      = (lenfunc)vector_length,
-    .sq_item        = (ssizeargfunc)angles_get_item,
-    .sq_ass_item    = (ssizeobjargproc)angles_set_item
-};
-
-static PyGetSetDef angles_getset[] = {
-    {"alpha", (getter)angles_getter, (setter)angles_setter,
-     PyDoc_STR("first angle of a rotation"), (void*)ROTATION_ANGLE_ALPHA},
-    {"beta", (getter)angles_getter, (setter)angles_setter,
-     PyDoc_STR("second angle of a rotation"), (void*)ROTATION_ANGLE_BETA},
-    {"gamma", (getter)angles_getter, (setter)angles_setter,
-     PyDoc_STR("third angle of a rotation"), (void*)ROTATION_ANGLE_GAMMA},
-
-    {NULL}
-};
-
-PyDoc_STRVAR(angles_reduce_doc, "__reduce__() -> (cls, state)\n\
-\n\
-Allows pickling of the Angles type by returning the constructor\n\
-and state of the object to recreate later.");
-
-static PyMethodDef angles_methods[] = {
-    {"__reduce__", (PyCFunction)angles_reduce, METH_NOARGS,
-     angles_reduce_doc},
-
-    {NULL}
-};
-
-PyDoc_STRVAR(angles_doc, "Angles(alpha, beta, gamma)\n\
-\n\
-The angles are all required, unneeded angles should be set to zero.");
-
-static PyTypeObject EVSpace_AnglesType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name        = "pyevspace.Angles",
-    .tp_basicsize   = sizeof(EVSpace_Angles),
-    .tp_itemsize    = 0,
-    .tp_repr        = (reprfunc)angles_repr,
-    .tp_as_sequence = &angles_as_sequence,
-    .tp_str         = (reprfunc)angles_str,
-#if PY_VERSION_HEX >= 0x03100000
-    .tp_flags       = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_SEQUENCE,
-#else
-    .tp_flags       = Py_TPFLAGS_DEFAULT,
-#endif
-    .tp_doc         = angles_doc,
-    .tp_methods     = angles_methods,
-    .tp_getset      = angles_getset,
-    .tp_new         = (newfunc)angles_new
-};
-
-static PySequenceMethods order_as_sequence = {
-    .sq_length      = (lenfunc)vector_length,
-    .sq_item        = (ssizeargfunc)order_get_item,
-    .sq_ass_item    = (ssizeobjargproc)order_set_item
-};
-
-static PyMemberDef order_members[] = {
-    {"first", T_INT, offsetof(EVSpace_Order, first), READONLY,
-     PyDoc_STR("first axis of a rotation")},
-
-    {"second", T_INT, offsetof(EVSpace_Order, second), READONLY,
-     PyDoc_STR("second axis of a rotation")},
-
-    {"third", T_INT, offsetof(EVSpace_Order, third), READONLY,
-     PyDoc_STR("third axis of a rotation")},
-
-    {NULL}
-};
-
-PyDoc_STRVAR(order_reduce_doc, "__reduce__() -> (cls, state)\n\
-\n\
-Allows pickling of the Order type by returning the constructor\n\
-and state of the object to recreate later.");
-
-static PyMethodDef order_methods[] = {
-    {"__reduce__", (PyCFunction)order_reduce, METH_NOARGS, order_reduce_doc},
-    {NULL}
-};
-
-PyDoc_STRVAR(order_doc, "Order(axis1, axis2, axis3)\n\
-\n\
-All axes are required and should be one of the three eunmerated\n\
-axis types X_AXIS, Y_AXIS or Z_AXIS.");
-
-static PyTypeObject EVSpace_OrderType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name        = "pyevspace.Order",
-    .tp_basicsize   = sizeof(EVSpace_Order),
-    .tp_itemsize    = 0,
-    .tp_repr        = (reprfunc)order_repr,
-    .tp_as_sequence = &order_as_sequence,
-    .tp_str         = (reprfunc)order_str,
-#if PY_VERSION_HEX >= 0x03100000
-    .tp_flags       = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_SEQUENCE,
-#else
-    .tp_flags       = Py_TPFLAGS_DEFAULT,
-#endif
-    .tp_doc         = order_doc,
-    .tp_methods     = order_methods,
-    .tp_members     = order_members,
-    .tp_new         = (newfunc)order_new
-};
-
-static PyMemberDef reference_frame_members[] = {
-    {"order", T_OBJECT_EX, offsetof(EVSpace_ReferenceFrame, order), READONLY,
-     PyDoc_STR("order of axes in the rotation")},
-
-    {"matrix", T_OBJECT_EX, offsetof(EVSpace_ReferenceFrame, matrix), READONLY,
-     PyDoc_STR("internal matrix describing the rotation")},
-
-    {NULL}
-};
-
-static PyGetSetDef reference_frame_getset[] = {
-    {"angles", (getter)refframe_angles_getter,
-     (setter)refframe_angles_setter,
-     PyDoc_STR("angles of the rotations"), NULL},
-
-    {"offset", (getter)refframe_offset_getter,
-     (setter)refframe_offset_setter,
-     PyDoc_STR("offset of the reference frame origin"), NULL},
-
-    {NULL}
-};
-
-static PyMethodDef reference_frame_methods[] = {
-    {"rotateTo", (PyCFunction)refframe_rotate_to, METH_O,
-     PyDoc_STR("rotateTo(vector) -> Vector\n\nRotate vector from an "
-               "inertial frame to this reference frame.")},
-
-    {"rotateFrom", (PyCFunction)refframe_rotate_from, METH_O,
-     PyDoc_STR("rotateFrom(vector) -> Vector\n\nRotate vector to an inertial "
-               "frame from this reference frame.")},
-
-    {"rotateToFrame", (PyCFunction)refframe_to_frame, METH_FASTCALL,
-     PyDoc_STR("rotateToFrame(frame, vector) -> Vector\n\nRotate vector from "
-               "this reference frame to frame.")},
-
-    {"rotateFromFrame", (PyCFunction)refframe_from_frame, METH_FASTCALL,
-     PyDoc_STR("rotateFromFrame(frame, vector) -> Vector\n\nRotate vector "
-               "from frame to this reference frame")},
-
-    {NULL}
-};
-
-PyDoc_STRVAR(reference_frame_doc, "ReferenceFrame(order, angles[, *, offset])\n\
-\n\
-The order and angles parameters are required and order should be\n\
-one of the default Order type instances provided by pyevspace.\n\
-Angles needs to be in radians and offset is an optional vector that\n\
-points from an inertial origin to the reference frames origin.");
-
-static PyTypeObject EVSpace_ReferenceFrameType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name        = "pyevspace.ReferenceFrame",
-    .tp_basicsize   = sizeof(EVSpace_ReferenceFrame),
-    .tp_itemsize    = 0,
-    .tp_flags       = Py_TPFLAGS_DEFAULT,
-    .tp_doc         = reference_frame_doc,
-    .tp_methods     = reference_frame_methods,
-    .tp_members     = reference_frame_members,
-    .tp_getset      = reference_frame_getset,
-    .tp_new         = (newfunc)refframe_new
-};
-
-
-/* capsule definition */
-
-static inline 
-EVSpace_CAPI* get_evspace_capi(void) 
-{
-    EVSpace_CAPI* capi = malloc(sizeof(EVSpace_CAPI));
-    if (!capi) {
-        PyErr_NoMemory();
-        return NULL;
-    }
-
-    capi->VectorType    = &EVSpace_VectorType;
-    capi->MatrixType    = &EVSpace_MatrixType;
-    capi->AnglesType    = &EVSpace_AnglesType;
-    capi->OrderType     = &EVSpace_OrderType;
-    capi->RefFrameType  = &EVSpace_ReferenceFrameType;
-
-    capi->Vector_FromArray  = _vector_from_array;
-    capi->Vector_StealArray = _vector_steal_array;
-    capi->Matrix_FromArray  = _matrix_from_array;
-    capi->Matrix_StealArray = _matrix_steal_array;
-    capi->Angles_New        = _angles_new;
-    capi->Order_New         = _order_new;
-    capi->RefFrame_New      = _reference_frame_new;
-
-    capi->Vector_add        = _vector_add;
-    capi->Vector_subtract   = _vector_subtract;
-    capi->Vector_multiply   = _vector_multiply;
-    capi->Vector_multiply_m = _vector_multiply_matrix;
-    capi->Vector_divide     = _vector_divide;
-    capi->Vector_iadd       = _vector_iadd;
-    capi->Vector_isubtract  = _vector_isubtract;
-    capi->Vector_imultiply  = _vector_imultiply;
-    capi->Vector_idivide    = _vector_idivide;
-    capi->Vector_negative   = _vector_negative;
-
-    capi->Matrix_add        = _matrix_add;
-    capi->Matrix_subtract   = _matrix_subtract;
-    capi->Matrix_multiply_v = _matrix_multiply_v;
-    capi->Matrix_multiply_m = _matrix_multiply_m;
-    capi->Matrix_multiply_s = _matrix_multiply_s;
-    capi->Matrix_divide     = _matrix_divide;
-    capi->Matrix_iadd       = _matrix_iadd;
-    capi->Matrix_isubtract  = _matrix_isubtract;
-    capi->Matrix_imultiply  = _matrix_imultiply_s;
-    capi->Matrix_idivide    = _matrix_idivide;
-    capi->Matrix_negative   = _matrix_negative;
-
-    capi->Vector_mag        = _vector_magnitude;
-    capi->Vector_mag2       = _vector_magnitude2;
-    capi->Vector_normalize  = _vector_normalize;
-
-    capi->Vector_dot        = _vector_dot;
-    capi->Vector_cross      = _vector_cross;
-    capi->Vector_norm       = _vector_norm;
-    capi->Vector_vang       = _vector_angle;
-    capi->Vector_vxcl       = _vector_exclude;
-    capi->Vector_proj       = _vector_projection;
-    capi->Matrix_det        = _matrix_determinate;
-    capi->Matrix_transpose  = _matrix_transpose;
-
-    capi->Get_matrix        = _get_rotation_matrix;
-    capi->Get_euler         = _get_euler_matrix;
-    capi->Get_from_to       = _get_matrix_from_to;
-
-    capi->Rotate_axis_to       = _rotate_axis_to;
-    capi->Rotate_axis_from     = _rotate_axis_from;
-    capi->Rotate_euler_to      = _rotate_euler_to;
-    capi->Rotate_euler_from    = _rotate_euler_from;
-    capi->Rotate_matrix_to     = _rotate_matrix_to;
-    capi->Rotate_matrix_from   = _rotate_matrix_from;
-    capi->Rotate_offset_to     = _rotate_offset_to;
-    capi->Rotate_offset_from   = _rotate_offset_from;
-
-    capi->Rotate_ref_to        = _refframe_rotate_to;
-    capi->Rotate_ref_from      = _refframe_rotate_from;
-    capi->Rotate_ref_to_ref    = _refframe_to_frame;
-    capi->Rotate_ref_from_ref  = _refframe_from_frame;
-
-    return capi;
-}
-
-
-/* module definition */
-
-static void 
-evspace_destructor(PyObject* capi) 
-{
-    void* ptr = PyCapsule_GetPointer(capi, Evs_CAPSULE_NAME);
-    free(ptr);
-}
-
-PyDoc_STRVAR(norm_doc, "norm(vector) -> Vector\n\
-\n\
-Creates a normalized version of a Vector. Differs from\n\
-vector.normalize() by returning a new Vector and 'vector'\n\
-remains unchanged.");
-
-PyDoc_STRVAR(vang_doc, "vang(from, to) -> float\n\
-\n\
-Determines the shortest angle between two vectors. The arguments\n\
-are commutative i.e. vang(from, to) == vang(to, from).");
-
-PyDoc_STRVAR(vxcl_doc, "vxcl(vector, exclude) -> Vector\n\
-\n\
-Removes all portions of exclude from vector. This is the same as\n\
-projecting vector onto the plane whose normal vector is exclude.");
-
-PyDoc_STRVAR(transpose_doc, "transpose(matrix) -> Matrix\n\
-\n\
-Returns the transpose of matrix, where the returned matrix is\n\
-the rows and columns of matrix are inverted.");
-
-PyDoc_STRVAR(matrix_euler_doc, "getMatrixEuler(order, angles) -> Matrix\n\
-\n\
-Creates the rotation matrix that represents the Euler rotation\n\
-defined by order and angles.");
-
-PyDoc_STRVAR(matrix_fromto_doc,
-"getMatrixFromTo(orderFrom, anglesFrom, orderTo, anglesTo) -> Matrix\n\
-\n\
-Creates the rotation matrix between two reference frames, both\n\
-defined by a particular Euler order and the corresponding angles.");
-
-PyDoc_STRVAR(axisto_doc, "rotateAxisTo(axis, angle, vector) -> Vector\n\
-\n\
-Rotates a vector to the reference frame defined by a rotation\n\
-around axis by angle radians.");
-
-PyDoc_STRVAR(axisfrom_doc, "rotateAxisFrom(axis, angle, vector) -> Vector\n\
-\n\
-Rotates a vector from the reference frame defined by a rotation\n\
-around axis by angle radians.");
-
-PyDoc_STRVAR(eulerto_doc, "rotateEulerTo(order, angles, vector) -> Vector\n\
-\n\
-Rotates a vector to the reference frame defined by an Euler\n\
-rotation.");
-
-PyDoc_STRVAR(eulerfrom_doc, "rotateEulerFrom(order, angles, vector) -> Vector\n\
-\n\
-Rotates a vector from the reference frame defined by an Euler\n\
-rotation.");
-
-static PyMethodDef evspace_methods[] = {
-    {"dot", (PyCFunction)vector_dot, METH_FASTCALL,
-     PyDoc_STR("dot(lhs, rhs) -> float\n\nCompute the dot product of "
-               "two Vectors.")},
-
-    {"cross", (PyCFunction)vector_cross, METH_FASTCALL,
-     PyDoc_STR("cross(lhs, rhs) -> Vector\n\nCompute the cross product of "
-               "two Vectors using the right-hand rule.")},
-
-    {"norm", (PyCFunction)vector_norm, METH_FASTCALL, norm_doc},
-
-    {"vang", (PyCFunction)vector_angle, METH_FASTCALL, vang_doc},
-
-    {"vxcl", (PyCFunction)vector_exclude, METH_FASTCALL, vxcl_doc},
-
-    {"proj", (PyCFunction)vector_proj, METH_FASTCALL,
-     PyDoc_STR("proj(proj, onto) -> Vector\n\nProjects the vector proj onto "
-               "the vector onto.")},
-
-    {"det", (PyCFunction)matrix_determinate, METH_FASTCALL,
-     PyDoc_STR("det(matrix) -> float\n\nComputes the determinate of a "
-               "Matrix.")},
-
-    {"transpose", (PyCFunction)matrix_transpose, METH_FASTCALL, transpose_doc},
-
-    {"getMatrixAxis", (PyCFunction)get_rotation_matrix, METH_VARARGS,
-     PyDoc_STR("getMatrixAxis(axis, angle) -> Matrix\n\nGenerates a rotation "
-               "matrix for a rotation around axis by angle radians.")},
-
-    {"getMatrixEuler", (PyCFunction)get_euler_matrix, METH_FASTCALL,
-     matrix_euler_doc},
-
-    {"getMatrixFromTo", (PyCFunction)get_matrix_from_to, METH_FASTCALL,
-     matrix_fromto_doc},
-
-    {"rotateAxisTo", (PyCFunction)rotate_axis_to, METH_VARARGS, axisto_doc},
-
-    {"rotateAxisFrom", (PyCFunction)rotate_axis_from, METH_VARARGS,
-     axisfrom_doc},
-
-    {"rotateEulerTo", (PyCFunction)rotate_euler_to, METH_FASTCALL, eulerto_doc},
-
-    {"rotateEulerFrom", (PyCFunction)rotate_euler_from, METH_FASTCALL,
-     eulerfrom_doc},
-
-    {"rotateMatrixTo", (PyCFunction)rotate_matrix_to, METH_FASTCALL,
-     PyDoc_STR("rotateMatrixTo(matrix, vector) -> Vector\n\nRotates a vector "
-               "to the reference frame defined by matrix.")},
-
-    {"rotateMatrixFrom", (PyCFunction)rotate_matrix_from, METH_FASTCALL,
-     PyDoc_STR("rotateMatrixFrom(matrix, vector) -> Vector\n\nRotates a vector "
-               "from the reference frame defined by matrix.")},
-
-    {"rotateOffsetTo", (PyCFunction)rotate_offset_to, METH_FASTCALL,
-     PyDoc_STR("rotateOffsetTo(matrix, offset, vector) -> Vector\n\nRotates "
-               "a vector to an offset reference frame defined by matrix.")},
-
-    {"rotateOffsetFrom", (PyCFunction)rotate_offset_from, METH_FASTCALL,
-     PyDoc_STR("rotateOffsetFrom(matrix, offset, vector) -> Vector\n\nRotates "
-               "a vector from an offset reference frame defined by matrix.")},
-
-    {NULL}
-};
-
-PyDoc_STRVAR(evspace_doc, "A 3-dimensional Euclidean vector space module with \
-a vector and matrix type as well as necessary methods to use them.");
-
-static PyModuleDef EVSpace_Module = {
-    PyModuleDef_HEAD_INIT,
-    .m_name     = "_pyevspace",
-    .m_doc      = evspace_doc,
-    .m_size     = -1,
-    .m_methods  = evspace_methods
-};
-
-#define PYEVSPACE_ADD_DICT(dict, name, value_expr)          \
-    {                                                       \
-        PyObject* value = (value_expr);                     \
-        if (!value) {                                       \
-            return -1;                                      \
-        }                                                   \
-                                                            \
-        if (PyDict_SetItemString(dict, name, value) < 0) {  \
-            Py_DECREF(value);                               \
-            return -1;                                      \
-        }                                                   \
-        Py_DECREF(value);                                   \
-    }
-
-#define PYEVSPACE_ADD_OBJECT(m, name, value_expr)       \
-    {                                                   \
-        PyObject* value = (value_expr);                 \
-        if (!value) {                                   \
-            return -1;                                  \
-        }                                               \
-                                                        \
-        if (PyModule_AddObject(m, name, value) < 0) {   \
-            Py_DECREF(value);                           \
-            return -1;                                  \
-        }                                               \
-    }
-
-#define PYEVSPACE_ADD_ORDER(m, cap, order, f, s, l)         \
-    {                                                       \
-        PyObject* val = (PyObject*)new_order(f, s, l);      \
-        PYEVSPACE_ADD_OBJECT(m, #order, val);               \
-        cap->Order_##order = (const EVSpace_Order*)val;   \
-    }
-
-static int
-_pyevspace_exec(PyObject* module)
-{
-    PyTypeObject* types[] = {
-        &EVSpace_VectorType,
-        &EVSpace_MatrixType,
-        &EVSpace_AnglesType,
-        &EVSpace_OrderType,
-        &EVSpace_ReferenceFrameType
-    };
-
-    for (int i = 0; i < Py_ARRAY_LENGTH(types); i++) {
-#if PY_VERSION_HEX >= 0x03090000
-        if (PyModule_AddType(module, types[i]) < 0) {
-            return -1;
-        }
-#else
-        char* names[] = {
-            "Vector",
-            "Matrix",
-            "Angles",
-            "Order",
-            "ReferenceFrame"
-        };
-
-        if (PyType_Ready(types[i]) < 0) {
-            for (int j = 0; j < i; j++) {
-                Py_DECREF(types[j]);
-            }
-            return -1;
-        }
-        if (PyModule_AddObject(module, names[i], (PyObject*)types[i]) < 0) {
-            for (int j = 0; j < i; j++) {
-                Py_DECREF(types[j]);
-            }
-            return -1;
-        }
-#endif
-    }
-
-    double arr[3] = { 1.0, 0.0, 0.0 };
-    PyObject* dict = EVSpace_VectorType.tp_dict;
-    PYEVSPACE_ADD_DICT(dict, "e1", (PyObject*)new_vector(arr));
-    arr[0] = 0.0, arr[1] = 1.0;
-    PYEVSPACE_ADD_DICT(dict, "e2", (PyObject*)new_vector(arr));
-    arr[1] = 0.0, arr[2] = 1.0;
-    PYEVSPACE_ADD_DICT(dict, "e3", (PyObject*)new_vector(arr));
-
-    double mat[9] = { 1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0 };
-    dict = EVSpace_MatrixType.tp_dict;
-    PYEVSPACE_ADD_DICT(dict, "id", (PyObject*)new_matrix(mat));
-
-    if (PyModule_AddIntConstant(module, "X_AXIS", X_AXIS) < 0) {
-        return -1;
-    }
-
-    if (PyModule_AddIntConstant(module, "Y_AXIS", Y_AXIS) < 0) {
-        return -1;
-    }
-
-    if (PyModule_AddIntConstant(module, "Z_AXIS", Z_AXIS) < 0) {
-        return -1;
-    }
-
-    EVSpace_CAPI* capi = get_evspace_capi();
-    if (!capi) {
-        return -1;
-    }
-
-    PYEVSPACE_ADD_ORDER(module, capi, XYZ, X_AXIS, Y_AXIS, Z_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, XZY, X_AXIS, Z_AXIS, Y_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, YXZ, Y_AXIS, X_AXIS, Z_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, YZX, Y_AXIS, Z_AXIS, X_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, ZXY, Z_AXIS, X_AXIS, Y_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, ZYX, Z_AXIS, Y_AXIS, X_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, XYX, X_AXIS, Y_AXIS, X_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, XZX, X_AXIS, Z_AXIS, X_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, YXY, Y_AXIS, X_AXIS, Y_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, YZY, Y_AXIS, Z_AXIS, Y_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, ZXZ, Z_AXIS, X_AXIS, Z_AXIS);
-    PYEVSPACE_ADD_ORDER(module, capi, ZYZ, Z_AXIS, Y_AXIS, Z_AXIS);
-
-    PyObject* capsule = PyCapsule_New(capi, Evs_CAPSULE_NAME, 
-                                      evspace_destructor);
-    if (!capsule) {
-        free(capi);
-        return -1;
-    }
-
-    if (PyModule_AddObject(module, "evspace_CAPI", capsule) < 0) {
-        Py_DECREF(capsule);
-        return -1;
-    }
-
-    return 0;
-}
-
-PyMODINIT_FUNC
-PyInit_core(void)
-{
-    PyObject* module = PyModule_Create(&EVSpace_Module);
-    if (!module) {
-        return NULL;
-    }
-
-    if (_pyevspace_exec(module) < 0) {
-        Py_DECREF(module);
-        return NULL;
-    }
-
-    return module;
+﻿#define PY_SSIZE_T_CLEAN
+#include <Python.h>
+#include <structmember.h> // PyMemberDef
+
+/* don't need the extra's for the C API */
+#define _EVSPACE_IMPL
+#include <evspacemodule.h>
+#include <evspace_vector.h>
+#include <evspace_matrix.h>
+#include <evspace_angles.h>
+#include <evspace_rotation.h>
+#include <evspace_refframe.h>
+
+
+/* EVSpace_VectorType definition */
+
+static PyNumberMethods vector_as_number = {
+    .nb_add                 = (binaryfunc)vector_add,
+    .nb_subtract            = (binaryfunc)vector_subtract,
+    .nb_multiply            = (binaryfunc)vector_multiply,
+    .nb_negative            = (unaryfunc)vector_negative,
+    .nb_inplace_add         = (binaryfunc)vector_iadd,
+    .nb_inplace_subtract    = (binaryfunc)vector_isubtract,
+    .nb_inplace_multiply    = (binaryfunc)vector_imultiply,
+    .nb_true_divide         = (binaryfunc)vector_divide,
+    .nb_inplace_true_divide = (binaryfunc)vector_idivide,
+    .nb_matrix_multiply     = (binaryfunc)vector_multiply_matrix,
+    .nb_inplace_matrix_multiply = (binaryfunc)vector_mat_imultiply
+};
+
+static PySequenceMethods vector_as_sequence = {
+    .sq_length      = (lenfunc)vector_length,
+    .sq_item        = (ssizeargfunc)vector_get_item,
+    .sq_ass_item    = (ssizeobjargproc)vector_set_item
+};
+
+static PyBufferProcs vector_buffer = {
+    .bf_getbuffer       = (getbufferproc)vector_get_buffer,
+    .bf_releasebuffer   = (releasebufferproc)release_buffer
+};
+
+PyDoc_STRVAR(vector_mag2_doc, "mag() -> float\n\
+\n\
+Computes the square of the magnitude of a vector. Eliminates\n\
+round-off error when squaring the result of mag().");
+
+PyDoc_STRVAR(vector_norm_doc, "normalize() -> Vector\n\
+\n\
+Modifies the vector to a length of 1, while preserving\n\
+its direction.");
+
+PyDoc_STRVAR(vector_reduce_doc, "__reduce__() -> (cls, (x, y, z))\n\
+\n\
+Allows pickling of the Vector type by returning the constructor\n\
+and arguments to recreate the Vector.");
+
+static PyMethodDef vector_methods[] = {
+
+    /* instance methods */
+
+    {"mag",         (PyCFunction)vector_magnitude, METH_NOARGS,
+     PyDoc_STR("mag() -> float\n\nComputes the magnitude of a vector.")},
+
+    {"mag2",        (PyCFunction)vector_magnitude_square, METH_NOARGS, 
+     vector_mag2_doc},
+
+    {"normalize",   (PyCFunction)vector_normalize, METH_NOARGS,
+     vector_norm_doc},
+
+    {"__reduce__",  (PyCFunction)vector_reduce, METH_NOARGS, 
+     vector_reduce_doc},
+
+    {NULL}
+};
+
+PyDoc_STRVAR(vector_doc, "Vector([{x, y, z | iterable}])\n\
+\n\
+The Vector can be constructed with an iterable of length 3, or\n\
+directly with the x, y and z components. All components must be\n\
+numeric types. Alternatively the components will default to zero\n\
+if no argument is specified.");
+
+static PyTypeObject EVSpace_VectorType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_name        = "pyevspace.Vector",
+    .tp_basicsize   = sizeof(EVSpace_Vector),
+    .tp_itemsize    = 0,
+    .tp_repr        = (reprfunc)vector_repr,
+    .tp_as_number   = &vector_as_number,
+    .tp_as_sequence = &vector_as_sequence,
+    .tp_str         = (reprfunc)vector_str,
+    .tp_as_buffer   = &vector_buffer,
+#if PY_VERSION_HEX >= 0x03100000
+    .tp_flags       = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_SEQUENCE,
+#else
+    .tp_flags       = Py_TPFLAGS_DEFAULT,
+#endif
+    .tp_doc         = vector_doc,
+    .tp_richcompare = (richcmpfunc)&vector_richcompare,
+    .tp_iter        = (getiterfunc)vector_iter,
+    .tp_methods     = vector_methods,
+    .tp_new         = (newfunc)vector_new,
+    .tp_free        = (freefunc)vector_free
+};
+
+
+/* EVSpace_MatrixType definition*/
+
+static PyNumberMethods matrix_as_number = {
+    .nb_add             = (binaryfunc)matrix_add,
+    .nb_subtract        = (binaryfunc)matrix_subtract,
+    .nb_multiply        = (binaryfunc)matrix_multiply,
+    .nb_negative        = (unaryfunc)matrix_negative,
+    .nb_inplace_add     = (binaryfunc)matrix_iadd,
+    .nb_inplace_subtract = (binaryfunc)matrix_isubtract,
+    .nb_inplace_multiply = (binaryfunc)matrix_imultiply,
+    .nb_true_divide     = (binaryfunc)matrix_divide,
+    .nb_inplace_true_divide = (binaryfunc)matrix_idivide,
+    .nb_matrix_multiply = (binaryfunc)matrix_mat_multiply,
+    .nb_inplace_matrix_multiply = (binaryfunc)matrix_mat_imultiply
+};
+
+static PyMappingMethods matrix_as_mapping = {
+    .mp_subscript       = (binaryfunc)matrix_get_item,
+    .mp_ass_subscript   = (objobjargproc)matrix_set_item
+};
+
+static PyBufferProcs matrix_buffer = {
+    .bf_getbuffer       = (getbufferproc)matrix_get_buffer,
+    .bf_releasebuffer   = (releasebufferproc)release_buffer
+};
+
+PyDoc_STRVAR(matrix_reduce_doc, "__reduce__() -> (cls, state)\n\
+\n\
+Allows pickling of the Matrix type by returning the constructor\n\
+and arguments to recreate the Matrix.");
+
+static PyMethodDef matrix_methods[] = {
+    {"__reduce__", (PyCFunction)matrix_reduce, METH_NOARGS, 
+     matrix_reduce_doc},
+
+    {NULL}
+};
+
+PyDoc_STRVAR(matrix_doc, "Matrix([row0, row1, row2])\n\
+\n\
+The Matrix can be constructed with three iterables, all of length\n\
+three, whose components are numeric types. Each iterable represents\n\
+a row of the matrix and are all required. Alternatively if no arguments\n\
+are present each component is defaulted to zero.");
+
+static PyTypeObject EVSpace_MatrixType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_name        = "pyevspace.Matrix",
+    .tp_basicsize   = sizeof(EVSpace_Matrix),
+    .tp_itemsize    = 0,
+    .tp_repr        = (reprfunc)matrix_repr,
+    .tp_as_number   = &matrix_as_number,
+    .tp_as_mapping  = &matrix_as_mapping,
+    .tp_str         = (reprfunc)matrix_str,
+    .tp_as_buffer   = &matrix_buffer,
+#if PY_VERSION_HEX >= 0x03100000
+    .tp_flags       = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_MAPPING,
+#else
+    .tp_flags       = Py_TPFLAGS_DEFAULT,
+#endif
+    .tp_doc         = matrix_doc,
+    .tp_richcompare = (richcmpfunc)&matrix_richcompare,
+    .tp_methods     = matrix_methods,
+    .tp_new         = (newfunc)matrix_new,
+    .tp_free        = (freefunc)matrix_free
+};
+
+static PySequenceMethods angles_as_sequence = {
+    .sq_length      = (lenfunc)vector_length,
+    .sq_item        = (ssizeargfunc)angles_get_item,
+    .sq_ass_item    = (ssizeobjargproc)angles_set_item
+};
+
+static PyGetSetDef angles_getset[] = {
+    {"alpha", (getter)angles_getter, (setter)angles_setter,
+     PyDoc_STR("first angle of a rotation"), (void*)ROTATION_ANGLE_ALPHA},
+    {"beta", (getter)angles_getter, (setter)angles_setter,
+     PyDoc_STR("second angle of a rotation"), (void*)ROTATION_ANGLE_BETA},
+    {"gamma", (getter)angles_getter, (setter)angles_setter,
+     PyDoc_STR("third angle of a rotation"), (void*)ROTATION_ANGLE_GAMMA},
+
+    {NULL}
+};
+
+PyDoc_STRVAR(angles_reduce_doc, "__reduce__() -> (cls, state)\n\
+\n\
+Allows pickling of the Angles type by returning the constructor\n\
+and state of the object to recreate later.");
+
+static PyMethodDef angles_methods[] = {
+    {"__reduce__", (PyCFunction)angles_reduce, METH_NOARGS,
+     angles_reduce_doc},
+
+    {NULL}
+};
+
+PyDoc_STRVAR(angles_doc, "Angles(alpha, beta, gamma)\n\
+\n\
+The angles are all required, unneeded angles should be set to zero.");
+
+static PyTypeObject EVSpace_AnglesType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_name        = "pyevspace.Angles",
+    .tp_basicsize   = sizeof(EVSpace_Angles),
+    .tp_itemsize    = 0,
+    .tp_repr        = (reprfunc)angles_repr,
+    .tp_as_sequence = &angles_as_sequence,
+    .tp_str         = (reprfunc)angles_str,
+#if PY_VERSION_HEX >= 0x03100000
+    .tp_flags       = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_SEQUENCE,
+#else
+    .tp_flags       = Py_TPFLAGS_DEFAULT,
+#endif
+    .tp_doc         = angles_doc,
+    .tp_methods     = angles_methods,
+    .tp_getset      = angles_getset,
+    .tp_new         = (newfunc)angles_new
+};
+
+static PySequenceMethods order_as_sequence = {
+    .sq_length      = (lenfunc)vector_length,
+    .sq_item        = (ssizeargfunc)order_get_item,
+    .sq_ass_item    = (ssizeobjargproc)order_set_item
+};
+
+static PyMemberDef order_members[] = {
+    {"first", T_INT, offsetof(EVSpace_Order, first), READONLY,
+     PyDoc_STR("first axis of a rotation")},
+
+    {"second", T_INT, offsetof(EVSpace_Order, second), READONLY,
+     PyDoc_STR("second axis of a rotation")},
+
+    {"third", T_INT, offsetof(EVSpace_Order, third), READONLY,
+     PyDoc_STR("third axis of a rotation")},
+
+    {NULL}
+};
+
+PyDoc_STRVAR(order_reduce_doc, "__reduce__() -> (cls, state)\n\
+\n\
+Allows pickling of the Order type by returning the constructor\n\
+and state of the object to recreate later.");
+
+static PyMethodDef order_methods[] = {
+    {"__reduce__", (PyCFunction)order_reduce, METH_NOARGS, order_reduce_doc},
+    {NULL}
+};
+
+PyDoc_STRVAR(order_doc, "Order(axis1, axis2, axis3)\n\
+\n\
+All axes are required and should be one of the three eunmerated\n\
+axis types X_AXIS, Y_AXIS or Z_AXIS.");
+
+static PyTypeObject EVSpace_OrderType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_name        = "pyevspace.Order",
+    .tp_basicsize   = sizeof(EVSpace_Order),
+    .tp_itemsize    = 0,
+    .tp_repr        = (reprfunc)order_repr,
+    .tp_as_sequence = &order_as_sequence,
+    .tp_str         = (reprfunc)order_str,
+#if PY_VERSION_HEX >= 0x03100000
+    .tp_flags       = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_SEQUENCE,
+#else
+    .tp_flags       = Py_TPFLAGS_DEFAULT,
+#endif
+    .tp_doc         = order_doc,
+    .tp_methods     = order_methods,
+    .tp_members     = order_members,
+    .tp_new         = (newfunc)order_new
+};
+
+static PyMemberDef reference_frame_members[] = {
+    {"order", T_OBJECT_EX, offsetof(EVSpace_ReferenceFrame, order), READONLY,
+     PyDoc_STR("order of axes in the rotation")},
+
+    {"matrix", T_OBJECT_EX, offsetof(EVSpace_ReferenceFrame, matrix), READONLY,
+     PyDoc_STR("internal matrix describing the rotation")},
+
+    {NULL}
+};
+
+static PyGetSetDef reference_frame_getset[] = {
+    {"angles", (getter)refframe_angles_getter,
+     (setter)refframe_angles_setter,
+     PyDoc_STR("angles of the rotations"), NULL},
+
+    {"offset", (getter)refframe_offset_getter,
+     (setter)refframe_offset_setter,
+     PyDoc_STR("offset of the reference frame origin"), NULL},
+
+    {NULL}
+};
+
+static PyMethodDef reference_frame_methods[] = {
+    {"rotateTo", (PyCFunction)refframe_rotate_to, METH_O,
+     PyDoc_STR("rotateTo(vector) -> Vector\n\nRotate vector from an "
+               "inertial frame to this reference frame.")},
+
+    {"rotateFrom", (PyCFunction)refframe_rotate_from, METH_O,
+     PyDoc_STR("rotateFrom(vector) -> Vector\n\nRotate vector to an inertial "
+               "frame from this reference frame.")},
+
+    {"rotateToFrame", (PyCFunction)refframe_to_frame, METH_FASTCALL,
+     PyDoc_STR("rotateToFrame(frame, vector) -> Vector\n\nRotate vector from "
+               "this reference frame to frame.")},
+
+    {"rotateFromFrame", (PyCFunction)refframe_from_frame, METH_FASTCALL,
+     PyDoc_STR("rotateFromFrame(frame, vector) -> Vector\n\nRotate vector "
+               "from frame to this reference frame")},
+
+    {NULL}
+};
+
+PyDoc_STRVAR(reference_frame_doc, "ReferenceFrame(order, angles[, *, offset])\n\
+\n\
+The order and angles parameters are required and order should be\n\
+one of the default Order type instances provided by pyevspace.\n\
+Angles needs to be in radians and offset is an optional vector that\n\
+points from an inertial origin to the reference frames origin.");
+
+static PyTypeObject EVSpace_ReferenceFrameType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_name        = "pyevspace.ReferenceFrame",
+    .tp_basicsize   = sizeof(EVSpace_ReferenceFrame),
+    .tp_itemsize    = 0,
+    .tp_flags       = Py_TPFLAGS_DEFAULT,
+    .tp_doc         = reference_frame_doc,
+    .tp_methods     = reference_frame_methods,
+    .tp_members     = reference_frame_members,
+    .tp_getset      = reference_frame_getset,
+    .tp_new         = (newfunc)refframe_new
+};
+
+
+/* capsule definition */
+
+static inline 
+EVSpace_CAPI* get_evspace_capi(void) 
+{
+    EVSpace_CAPI* capi = malloc(sizeof(EVSpace_CAPI));
+    if (!capi) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+
+    capi->VectorType    = &EVSpace_VectorType;
+    capi->MatrixType    = &EVSpace_MatrixType;
+    capi->AnglesType    = &EVSpace_AnglesType;
+    capi->OrderType     = &EVSpace_OrderType;
+    capi->RefFrameType  = &EVSpace_ReferenceFrameType;
+
+    capi->Vector_FromArray  = _vector_from_array;
+    capi->Vector_StealArray = _vector_steal_array;
+    capi->Matrix_FromArray  = _matrix_from_array;
+    capi->Matrix_StealArray = _matrix_steal_array;
+    capi->Angles_New        = _angles_new;
+    capi->Order_New         = _order_new;
+    capi->RefFrame_New      = _reference_frame_new;
+
+    capi->Vector_add        = _vector_add;
+    capi->Vector_subtract   = _vector_subtract;
+    capi->Vector_multiply   = _vector_multiply;
+    capi->Vector_multiply_m = _vector_multiply_matrix;
+    capi->Vector_divide     = _vector_divide;
+    capi->Vector_iadd       = _vector_iadd;
+    capi->Vector_isubtract  = _vector_isubtract;
+    capi->Vector_imultiply  = _vector_imultiply;
+    capi->Vector_idivide    = _vector_idivide;
+    capi->Vector_negative   = _vector_negative;
+
+    capi->Matrix_add        = _matrix_add;
+    capi->Matrix_subtract   = _matrix_subtract;
+    capi->Matrix_multiply_v = _matrix_multiply_v;
+    capi->Matrix_multiply_m = _matrix_multiply_m;
+    capi->Matrix_multiply_s = _matrix_multiply_s;
+    capi->Matrix_divide     = _matrix_divide;
+    capi->Matrix_iadd       = _matrix_iadd;
+    capi->Matrix_isubtract  = _matrix_isubtract;
+    capi->Matrix_imultiply  = _matrix_imultiply_s;
+    capi->Matrix_idivide    = _matrix_idivide;
+    capi->Matrix_negative   = _matrix_negative;
+
+    capi->Vector_mag        = _vector_magnitude;
+    capi->Vector_mag2       = _vector_magnitude2;
+    capi->Vector_normalize  = _vector_normalize;
+
+    capi->Vector_dot        = _vector_dot;
+    capi->Vector_cross      = _vector_cross;
+    capi->Vector_norm       = _vector_norm;
+    capi->Vector_vang       = _vector_angle;
+    capi->Vector_vxcl       = _vector_exclude;
+    capi->Vector_proj       = _vector_projection;
+    capi->Matrix_det        = _matrix_determinate;
+    capi->Matrix_transpose  = _matrix_transpose;
+
+    capi->Get_matrix        = _get_rotation_matrix;
+    capi->Get_euler         = _get_euler_matrix;
+    capi->Get_from_to       = _get_matrix_from_to;
+
+    capi->Rotate_axis_to       = _rotate_axis_to;
+    capi->Rotate_axis_from     = _rotate_axis_from;
+    capi->Rotate_euler_to      = _rotate_euler_to;
+    capi->Rotate_euler_from    = _rotate_euler_from;
+    capi->Rotate_matrix_to     = _rotate_matrix_to;
+    capi->Rotate_matrix_from   = _rotate_matrix_from;
+    capi->Rotate_offset_to     = _rotate_offset_to;
+    capi->Rotate_offset_from   = _rotate_offset_from;
+
+    capi->Rotate_ref_to        = _refframe_rotate_to;
+    capi->Rotate_ref_from      = _refframe_rotate_from;
+    capi->Rotate_ref_to_ref    = _refframe_to_frame;
+    capi->Rotate_ref_from_ref  = _refframe_from_frame;
+
+    return capi;
+}
+
+
+/* module definition */
+
+static void 
+evspace_destructor(PyObject* capi) 
+{
+    void* ptr = PyCapsule_GetPointer(capi, Evs_CAPSULE_NAME);
+    free(ptr);
+}
+
+PyDoc_STRVAR(norm_doc, "norm(vector) -> Vector\n\
+\n\
+Creates a normalized version of a Vector. Differs from\n\
+vector.normalize() by returning a new Vector and 'vector'\n\
+remains unchanged.");
+
+PyDoc_STRVAR(vang_doc, "vang(from, to) -> float\n\
+\n\
+Determines the shortest angle between two vectors. The arguments\n\
+are commutative i.e. vang(from, to) == vang(to, from).");
+
+PyDoc_STRVAR(vxcl_doc, "vxcl(vector, exclude) -> Vector\n\
+\n\
+Removes all portions of exclude from vector. This is the same as\n\
+projecting vector onto the plane whose normal vector is exclude.");
+
+PyDoc_STRVAR(transpose_doc, "transpose(matrix) -> Matrix\n\
+\n\
+Returns the transpose of matrix, where the returned matrix is\n\
+the rows and columns of matrix are inverted.");
+
+PyDoc_STRVAR(matrix_euler_doc, "getMatrixEuler(order, angles) -> Matrix\n\
+\n\
+Creates the rotation matrix that represents the Euler rotation\n\
+defined by order and angles.");
+
+PyDoc_STRVAR(matrix_fromto_doc,
+"getMatrixFromTo(orderFrom, anglesFrom, orderTo, anglesTo) -> Matrix\n\
+\n\
+Creates the rotation matrix between two reference frames, both\n\
+defined by a particular Euler order and the corresponding angles.");
+
+PyDoc_STRVAR(axisto_doc, "rotateAxisTo(axis, angle, vector) -> Vector\n\
+\n\
+Rotates a vector to the reference frame defined by a rotation\n\
+around axis by angle radians.");
+
+PyDoc_STRVAR(axisfrom_doc, "rotateAxisFrom(axis, angle, vector) -> Vector\n\
+\n\
+Rotates a vector from the reference frame defined by a rotation\n\
+around axis by angle radians.");
+
+PyDoc_STRVAR(eulerto_doc, "rotateEulerTo(order, angles, vector) -> Vector\n\
+\n\
+Rotates a vector to the reference frame defined by an Euler\n\
+rotation.");
+
+PyDoc_STRVAR(eulerfrom_doc, "rotateEulerFrom(order, angles, vector) -> Vector\n\
+\n\
+Rotates a vector from the reference frame defined by an Euler\n\
+rotation.");
+
+static PyMethodDef evspace_methods[] = {
+    {"dot", (PyCFunction)vector_dot, METH_FASTCALL,
+     PyDoc_STR("dot(lhs, rhs) -> float\n\nCompute the dot product of "
+               "two Vectors.")},
+
+    {"cross", (PyCFunction)vector_cross, METH_FASTCALL,
+     PyDoc_STR("cross(lhs, rhs) -> Vector\n\nCompute the cross product of "
+               "two Vectors using the right-hand rule.")},
+
+    {"norm", (PyCFunction)vector_norm, METH_FASTCALL, norm_doc},
+
+    {"vang", (PyCFunction)vector_angle, METH_FASTCALL, vang_doc},
+
+    {"vxcl", (PyCFunction)vector_exclude, METH_FASTCALL, vxcl_doc},
+
+    {"proj", (PyCFunction)vector_proj, METH_FASTCALL,
+     PyDoc_STR("proj(proj, onto) -> Vector\n\nProjects the vector proj onto "
+               "the vector onto.")},
+
+    {"det", (PyCFunction)matrix_determinate, METH_FASTCALL,
+     PyDoc_STR("det(matrix) -> float\n\nComputes the determinate of a "
+               "Matrix.")},
+
+    {"transpose", (PyCFunction)matrix_transpose, METH_FASTCALL, transpose_doc},
+
+    {"getMatrixAxis", (PyCFunction)get_rotation_matrix, METH_VARARGS,
+     PyDoc_STR("getMatrixAxis(axis, angle) -> Matrix\n\nGenerates a rotation "
+               "matrix for a rotation around axis by angle radians.")},
+
+    {"getMatrixEuler", (PyCFunction)get_euler_matrix, METH_FASTCALL,
+     matrix_euler_doc},
+
+    {"getMatrixFromTo", (PyCFunction)get_matrix_from_to, METH_FASTCALL,
+     matrix_fromto_doc},
+
+    {"rotateAxisTo", (PyCFunction)rotate_axis_to, METH_VARARGS, axisto_doc},
+
+    {"rotateAxisFrom", (PyCFunction)rotate_axis_from, METH_VARARGS,
+     axisfrom_doc},
+
+    {"rotateEulerTo", (PyCFunction)rotate_euler_to, METH_FASTCALL, eulerto_doc},
+
+    {"rotateEulerFrom", (PyCFunction)rotate_euler_from, METH_FASTCALL,
+     eulerfrom_doc},
+
+    {"rotateMatrixTo", (PyCFunction)rotate_matrix_to, METH_FASTCALL,
+     PyDoc_STR("rotateMatrixTo(matrix, vector) -> Vector\n\nRotates a vector "
+               "to the reference frame defined by matrix.")},
+
+    {"rotateMatrixFrom", (PyCFunction)rotate_matrix_from, METH_FASTCALL,
+     PyDoc_STR("rotateMatrixFrom(matrix, vector) -> Vector\n\nRotates a vector "
+               "from the reference frame defined by matrix.")},
+
+    {"rotateOffsetTo", (PyCFunction)rotate_offset_to, METH_FASTCALL,
+     PyDoc_STR("rotateOffsetTo(matrix, offset, vector) -> Vector\n\nRotates "
+               "a vector to an offset reference frame defined by matrix.")},
+
+    {"rotateOffsetFrom", (PyCFunction)rotate_offset_from, METH_FASTCALL,
+     PyDoc_STR("rotateOffsetFrom(matrix, offset, vector) -> Vector\n\nRotates "
+               "a vector from an offset reference frame defined by matrix.")},
+
+    {NULL}
+};
+
+PyDoc_STRVAR(evspace_doc, "A 3-dimensional Euclidean vector space module with \
+a vector and matrix type as well as necessary methods to use them.");
+
+static PyModuleDef EVSpace_Module = {
+    PyModuleDef_HEAD_INIT,
+    .m_name     = "_pyevspace",
+    .m_doc      = evspace_doc,
+    .m_size     = -1,
+    .m_methods  = evspace_methods
+};
+
+#define PYEVSPACE_ADD_DICT(dict, name, value_expr)          \
+    {                                                       \
+        PyObject* value = (value_expr);                     \
+        if (!value) {                                       \
+            return -1;                                      \
+        }                                                   \
+                                                            \
+        if (PyDict_SetItemString(dict, name, value) < 0) {  \
+            Py_DECREF(value);                               \
+            return -1;                                      \
+        }                                                   \
+        Py_DECREF(value);                                   \
+    }
+
+#define PYEVSPACE_ADD_OBJECT(m, name, value_expr)       \
+    {                                                   \
+        PyObject* value = (value_expr);                 \
+        if (!value) {                                   \
+            return -1;                                  \
+        }                                               \
+                                                        \
+        if (PyModule_AddObject(m, name, value) < 0) {   \
+            Py_DECREF(value);                           \
+            return -1;                                  \
+        }                                               \
+    }
+
+#define PYEVSPACE_ADD_ORDER(m, cap, order, f, s, l)         \
+    {                                                       \
+        PyObject* val = (PyObject*)new_order(f, s, l);      \
+        PYEVSPACE_ADD_OBJECT(m, #order, val);               \
+        cap->Order_##order = (const EVSpace_Order*)val;   \
+    }
+
+static int
+_pyevspace_exec(PyObject* module)
+{
+    PyTypeObject* types[] = {
+        &EVSpace_VectorType,
+        &EVSpace_MatrixType,
+        &EVSpace_AnglesType,
+        &EVSpace_OrderType,
+        &EVSpace_ReferenceFrameType
+    };
+
+    for (int i = 0; i < Py_ARRAY_LENGTH(types); i++) {
+#if PY_VERSION_HEX >= 0x03090000
+        if (PyModule_AddType(module, types[i]) < 0) {
+            return -1;
+        }
+#else
+        char* names[] = {
+            "Vector",
+            "Matrix",
+            "Angles",
+            "Order",
+            "ReferenceFrame"
+        };
+
+        if (PyType_Ready(types[i]) < 0) {
+            for (int j = 0; j < i; j++) {
+                Py_DECREF(types[j]);
+            }
+            return -1;
+        }
+        if (PyModule_AddObject(module, names[i], (PyObject*)types[i]) < 0) {
+            for (int j = 0; j < i; j++) {
+                Py_DECREF(types[j]);
+            }
+            return -1;
+        }
+#endif
+    }
+
+    double arr[3] = { 1.0, 0.0, 0.0 };
+    PyObject* dict = EVSpace_VectorType.tp_dict;
+    PYEVSPACE_ADD_DICT(dict, "e1", (PyObject*)new_vector(arr));
+    arr[0] = 0.0, arr[1] = 1.0;
+    PYEVSPACE_ADD_DICT(dict, "e2", (PyObject*)new_vector(arr));
+    arr[1] = 0.0, arr[2] = 1.0;
+    PYEVSPACE_ADD_DICT(dict, "e3", (PyObject*)new_vector(arr));
+
+    double mat[9] = { 1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0 };
+    dict = EVSpace_MatrixType.tp_dict;
+    PYEVSPACE_ADD_DICT(dict, "id", (PyObject*)new_matrix(mat));
+
+    if (PyModule_AddIntConstant(module, "X_AXIS", X_AXIS) < 0) {
+        return -1;
+    }
+
+    if (PyModule_AddIntConstant(module, "Y_AXIS", Y_AXIS) < 0) {
+        return -1;
+    }
+
+    if (PyModule_AddIntConstant(module, "Z_AXIS", Z_AXIS) < 0) {
+        return -1;
+    }
+
+    EVSpace_CAPI* capi = get_evspace_capi();
+    if (!capi) {
+        return -1;
+    }
+
+    PYEVSPACE_ADD_ORDER(module, capi, XYZ, X_AXIS, Y_AXIS, Z_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, XZY, X_AXIS, Z_AXIS, Y_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, YXZ, Y_AXIS, X_AXIS, Z_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, YZX, Y_AXIS, Z_AXIS, X_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, ZXY, Z_AXIS, X_AXIS, Y_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, ZYX, Z_AXIS, Y_AXIS, X_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, XYX, X_AXIS, Y_AXIS, X_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, XZX, X_AXIS, Z_AXIS, X_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, YXY, Y_AXIS, X_AXIS, Y_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, YZY, Y_AXIS, Z_AXIS, Y_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, ZXZ, Z_AXIS, X_AXIS, Z_AXIS);
+    PYEVSPACE_ADD_ORDER(module, capi, ZYZ, Z_AXIS, Y_AXIS, Z_AXIS);
+
+    PyObject* capsule = PyCapsule_New(capi, Evs_CAPSULE_NAME, 
+                                      evspace_destructor);
+    if (!capsule) {
+        free(capi);
+        return -1;
+    }
+
+    if (PyModule_AddObject(module, "evspace_CAPI", capsule) < 0) {
+        Py_DECREF(capsule);
+        return -1;
+    }
+
+    return 0;
+}
+
+PyMODINIT_FUNC
+PyInit_core(void)
+{
+    PyObject* module = PyModule_Create(&EVSpace_Module);
+    if (!module) {
+        return NULL;
+    }
+
+    if (_pyevspace_exec(module) < 0) {
+        Py_DECREF(module);
+        return NULL;
+    }
+
+    return module;
 }
```

### Comparing `pyevspace-0.14.0/src/pyevspace.egg-info/PKG-INFO` & `pyevspace-0.14.1/src/pyevspace.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,131 +1,135 @@
-Metadata-Version: 2.1
-Name: pyevspace
-Version: 0.14.0
-Summary: A Python 3-dimensional Euclidean vector space.
-Home-page: https://github.com/qbizzle68/pyevspace
-Author: Quinton Barnes
-Author-email: devqbizzle68@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PyEVSpace 0.14.0
-
-PyEVSpace is a Python Euclidean vector space package containing types
-and methods for representing vector quantites and fasilitating rotating
-them between reference frames. PyEVSpace is designed for 3-dimensional
-space only, which allows for optimum speed since size checks do not
-occur.
-
-
-## Documentation
-
-The full documentation of this project with both Python and C APIs can
-be found [here](https://qbizzle68.github.io/pyevspace/html/index.html).
-
-## Install
-
-The python module can be installed with
-```python
-pip install pyevspace
-```
-
-Alternatively the repository can be downloaded or cloned using:
-```bash
-git clone https://github.com/qbizzle68/pyevspace.git
-```
-It can be used as is within Visual Studio, or built inplace using the
-*setup.py* if needed.
-
-## Usage
-
-To use the module simply import the pyevspace module into your project:
-```python
-import pyevspace as evs
-from math import pi
-
-vec = evs.Vector(1, 2, 3)
-
-rotatedVec = evs.rotateAxisTo(evs.X_AXIS, pi/2)
-```
-
-Matrices can be created from iterables, where each iterable represents
-a row of the matrix
-```python
-import pyevspace as evs
-
-mat = evs.Matrix((0, 0, 1), (0, -1, 0), (1, 0, 0))
-
-rotatedVec = evs.rotateMatrixFrom(mat, Vector(1, 1, 1))
-```
-
-The Order and Angles types can be used to create an Euler rotation 
-matrix. All twelve Euler rotations are already defined in the module,
-so you shouldn't need to instantiate an Order object. The Angles
-object holds the angles for each rotation in the Euler rotation, in
-the order of the axis rotations (in radians).
-```python
-import pyevspace as evs
-
-angs = Angles(1.1, 4.5, 3.14)
-mat = getMatrixEuler(XYZ, angs)
-
-rotatedVec = mat * Vector(1, 0, 2)
-```
-
-There are many methods that handle the rotations for you, check the
-official documentation to learn more about them.
-
-## Examples
-
-### Examples of numeric operators
-```python
-v1 = Vector(1, 2, 3)
-v2 = Vector(4, 5, 6)
-
-print(v1 * 2)
-# prints [2, 4, 6]
-
-print(v1 + v2)
-# prints [5, 7, 9]
-
-print(v1 - v2)
-# prints [-3, -3, -3]
-```
-
-### Examples of vector and matrix operators
-```python
-v1 = Vector(1, 2, 3)
-v2 = Vector(4, 5, 6)
-m1 = Matrix(Vector(4, 2, 3), Vector(8, 5, 2), Vector(4, 2, 1))
-
-print(dot(v1, v2))
-# prints 32.0
-
-print(cross(v1, v2))
-# prints [ -3.00000, 6.00000, -3.00000 ]
-
-print(det(m1))
-# prints -8.0
-
-print(transpose(m1))
-# prints 
-# ([4, 2, 3],
-# [8, 5, 2],
-# [4, 2, 1])
-```
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: pyevspace
+Version: 0.14.1
+Summary: A Python 3-dimensional Euclidean vector space.
+Home-page: https://github.com/qbizzle68/pyevspace
+Author: Quinton Barnes
+Author-email: devqbizzle68@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# PyEVSpace 0.14.1
+
+This version of PyEVSpace is no functionally different than 0.14.0.
+This version was published to pypi using automated scripting workflows,
+and its existence means everything works!!
+
+PyEVSpace is a Python Euclidean vector space package containing types
+and methods for representing vector quantites and fasilitating rotating
+them between reference frames. PyEVSpace is designed for 3-dimensional
+space only, which allows for optimum speed since size checks do not
+occur.
+
+
+## Documentation
+
+The full documentation of this project with both Python and C APIs can
+be found [here](https://qbizzle68.github.io/pyevspace/html/index.html).
+
+## Install
+
+The python module can be installed with
+```python
+pip install pyevspace
+```
+
+Alternatively the repository can be downloaded or cloned using:
+```bash
+git clone https://github.com/qbizzle68/pyevspace.git
+```
+It can be used as is within Visual Studio, or built inplace using the
+*setup.py* if needed.
+
+## Usage
+
+To use the module simply import the pyevspace module into your project:
+```python
+import pyevspace as evs
+from math import pi
+
+vec = evs.Vector(1, 2, 3)
+
+rotatedVec = evs.rotateAxisTo(evs.X_AXIS, pi/2)
+```
+
+Matrices can be created from iterables, where each iterable represents
+a row of the matrix
+```python
+import pyevspace as evs
+
+mat = evs.Matrix((0, 0, 1), (0, -1, 0), (1, 0, 0))
+
+rotatedVec = evs.rotateMatrixFrom(mat, Vector(1, 1, 1))
+```
+
+The Order and Angles types can be used to create an Euler rotation 
+matrix. All twelve Euler rotations are already defined in the module,
+so you shouldn't need to instantiate an Order object. The Angles
+object holds the angles for each rotation in the Euler rotation, in
+the order of the axis rotations (in radians).
+```python
+import pyevspace as evs
+
+angs = Angles(1.1, 4.5, 3.14)
+mat = getMatrixEuler(XYZ, angs)
+
+rotatedVec = mat * Vector(1, 0, 2)
+```
+
+There are many methods that handle the rotations for you, check the
+official documentation to learn more about them.
+
+## Examples
+
+### Examples of numeric operators
+```python
+v1 = Vector(1, 2, 3)
+v2 = Vector(4, 5, 6)
+
+print(v1 * 2)
+# prints [2, 4, 6]
+
+print(v1 + v2)
+# prints [5, 7, 9]
+
+print(v1 - v2)
+# prints [-3, -3, -3]
+```
+
+### Examples of vector and matrix operators
+```python
+v1 = Vector(1, 2, 3)
+v2 = Vector(4, 5, 6)
+m1 = Matrix(Vector(4, 2, 3), Vector(8, 5, 2), Vector(4, 2, 1))
+
+print(dot(v1, v2))
+# prints 32.0
+
+print(cross(v1, v2))
+# prints [ -3.00000, 6.00000, -3.00000 ]
+
+print(det(m1))
+# prints -8.0
+
+print(transpose(m1))
+# prints 
+# ([4, 2, 3],
+# [8, 5, 2],
+# [4, 2, 1])
+```
+
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
```

