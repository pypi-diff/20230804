# Comparing `tmp/fileformats-0.8.4.tar.gz` & `tmp/fileformats-0.8.5.tar.gz`

## Comparing `fileformats-0.8.4.tar` & `fileformats-0.8.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/archive/__init__.py
--rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/_version.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/converter.py
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/datatype.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/field.py
--rw-r--r--   0        0        0    46197 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/fileset.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/mark.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/mixin.py
--rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/utils.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_test_extras.py
--rw-r--r--   0        0        0    12335 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/document/__init__.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/image/base.py
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/image/notclassifiedyet.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/image/vector.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/misc/medical.py
--rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/misc/unclassified.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/model/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/testing/classifiers.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/testing/headers.py
--rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/text/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.4/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.4/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.4/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.4/LICENSE
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.4/README.rst
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/converter.py
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/datatype.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/field.py
+-rw-r--r--   0        0        0    46547 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/mark.py
+-rw-r--r--   0        0        0    27183 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/mixin.py
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/utils.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_test_extras.py
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/base.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/notclassifiedyet.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/vector.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/misc/medical.py
+-rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/misc/unclassified.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/model/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/testing/headers.py
+-rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/text/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.5/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.5/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.5/LICENSE
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.5/README.rst
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.5/PKG-INFO
```

### Comparing `fileformats-0.8.4/fileformats/archive/__init__.py` & `fileformats-0.8.5/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/audio/__init__.py` & `fileformats-0.8.5/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/converter.py` & `fileformats-0.8.5/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/datatype.py` & `fileformats-0.8.5/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/exceptions.py` & `fileformats-0.8.5/fileformats/core/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     "No converters exist between formats"
 
 
 class FormatRecognitionError(KeyError, FileFormatsError):
     "Did not find a format class corresponding to a MIME, or MIME-like, type string"
 
 
+class UnconstrainedExtensionException(FileFormatsError):
+    "Did not find a format class corresponding to a MIME, or MIME-like, type string"
+
+
 class FileFormatsExtrasError(FileFormatsError):
     """If there is an "extras hook" in the datatype class but no methods have been
     registered on it"""
 
 
 class FileFormatsExtrasPkgUninstalledError(FileFormatsExtrasError):
     """If there is an "extras hook" in the datatype class and a extras package on PyPI
```

### Comparing `fileformats-0.8.4/fileformats/core/field.py` & `fileformats-0.8.5/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/fileset.py` & `fileformats-0.8.5/fileformats/core/fileset.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     describe_task,
     import_extras_module,
 )
 from .converter import SubtypeVar
 from .exceptions import (
     FileFormatsError,
     FormatMismatchError,
+    UnconstrainedExtensionException,
     FormatConversionError,
     FileFormatsExtrasError,
     FileFormatsExtrasPkgUninstalledError,
     FileFormatsExtrasPkgNotCheckedError,
 )
 from .datatype import DataType
 from . import mark
@@ -449,15 +450,15 @@
                     f"'{cls.mime_like}' formats"
                 )
                 extras_imported, extras_pkg, extras_pypi = import_extras_module(cls)
                 if not extras_imported:
                     msg += (
                         f'. Was not able to import "extras" module, {extras_pkg}, '
                         f"you may want to try installing the '{extras_pypi}' package "
-                        f"from PyPI (e.g. pip install {extras_pypi})"
+                        f"from PyPI (e.g. pip install {extras_pypi}) or check it isn't broken"
                     )
                 raise FormatConversionError(msg) from None
             converter_tuple = available_converters[0]
             # Store mapping for future reference
             converters[source_format] = converter_tuple
         converter, conv_kwargs = converter_tuple
         if kwargs:
@@ -888,15 +889,23 @@
             self.required_paths()
             if required_only and self.required_paths()
             else self.fspaths
         )
         nested = self.nested_filesets()
         for fileset in [self] + nested:
             if isinstance(fileset, File):
-                decomposed = (fileset.fspath.parent, fileset.stem, fileset.actual_ext)
+                try:
+                    decomposed = (
+                        fileset.fspath.parent,
+                        fileset.stem,
+                        fileset.actual_ext,
+                    )
+                except UnconstrainedExtensionException:
+                    implicit.add(fileset.fspath)
+                    continue
                 if fileset.fspath in implicit:
                     decomposed_fspaths.append(decomposed)
                     implicit.remove(fileset.fspath)
                 elif decomposed not in decomposed_fspaths:
                     previous_fileset = next(
                         f for f in nested if f.fspath == fileset.fspath
                     )
@@ -1089,14 +1098,16 @@
         extension_decomposition : FileSet.ExtensionDecomposition, optional
             whether to consider file extensions to start from the first '.' (multiple) or the
             last (single) or be empty (none), when the extension of a fspath in the
             FileSet isn't explicitly defined by the FileSet class. Only relevant when
             collation mode is set to "adjacent". By default True
         """
         mode = self.CopyMode[mode] if isinstance(mode, str) else mode
+        if new_stem:
+            supported_modes -= self.CopyMode.leave
         selected_mode = mode & supported_modes
         if len(self.fspaths) == 1:
             # If there is only one path to copy, then collation isn't meaningful
             collation = self.CopyCollation.any
         else:
             collation = (
                 self.CopyCollation[collation]
@@ -1118,15 +1129,15 @@
         if not selected_mode:
             raise FileFormatsError(
                 f"Cannot copy {self} using {mode} mode as it is not supported by "
                 f"the {supported_modes} given the collation specification, {collation}"
             )
         if selected_mode & self.CopyMode.leave:
             return self  # Don't need to do anything
-        if collation == self.CopyCollation.adjacent:
+        if collation == self.CopyCollation.adjacent or new_stem:
             decomposed_fspaths = self.decomposed_fspaths(
                 required_only=trim, decomposition_mode=extension_decomposition
             )
             exts = [d[-1] for d in decomposed_fspaths]
             duplicate_exts = [n for n, c in Counter(exts).items() if c > 1]
             if duplicate_exts:
                 raise FileFormatsError(
@@ -1161,26 +1172,24 @@
         else:
             fspaths_to_copy = self.fspaths
         if not fspaths_to_copy:
             raise FileFormatsError(
                 f"Cannot copy {self} because none of the fspaths in the file-set are "
                 "required. Set trim=False to copy all file-paths"
             )
+        # Set default for new_stem if not provided and collating file-set to be adjacent
         if collation == self.CopyCollation.adjacent:
             if new_stem is None:
                 new_stem = sorted(decomposed_fspaths)[0][1]
-            # Warning we redefine fspaths_to_copy as list of tuples not Paths
+        # WARNING we redefine fspaths_to_copy as list of tuples not Paths
+        if new_stem:
             fspaths_to_copy = decomposed_fspaths
-        elif new_stem is not None:
-            raise FileFormatsError(
-                f"'stem' ({new_stem}) provided to FileSet.copy() method when collation is "
-                f"not set to 'adjacent' ({collation})"
-            )
+
         for fspath in fspaths_to_copy:
-            if collation == self.CopyCollation.adjacent:
+            if new_stem:
                 # fspath is a path decomposed into parent, stem, ext instead of a Path
                 parent_dir, old_stem, ext = fspath
                 fspath = parent_dir / (old_stem + ext)  # reconstruct into a Path
                 new_path = dest_dir / (new_stem + ext)
             elif collation == self.CopyCollation.siblings:
                 new_path = dest_dir / fspath.name
             else:
@@ -1230,7 +1239,10 @@
     def validate_fspaths(self, _, fspaths):
         pass
 
     @classproperty
     def _type_name(cls):
         assert cls.__name__.endswith("Mock")
         return cls.__name__[: -len("Mock")]
+
+    def __bytes_repr__(self, cache):
+        yield from (str(fspath).encode() for fspath in self.fspaths)
```

### Comparing `fileformats-0.8.4/fileformats/core/mark.py` & `fileformats-0.8.5/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/mixin.py` & `fileformats-0.8.5/fileformats/core/mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+import re
 import typing as ty
 from collections import Counter
 from . import mark
 from .fileset import FileSet
 from .utils import classproperty, describe_task, to_mime_format_name
 from .converter import SubtypeVar
 from .exceptions import FileFormatsError, FormatMismatchError, FormatRecognitionError
@@ -10,26 +11,28 @@
 
 class WithMagicNumber:
     """Mixin class for Files with magic numbers at the start of their
     contents.
 
     Class Attrs
     -----------
-    magic_number : str
-        the magic number/string to search for at the start of the file
+    magic_number : str or bytes
+        the magic number/string to search for at the start of the file. If a unicode
+        string then it is interpreted as the byte code in hex, if a bytes object, then
+        it is treated as the byte string directly.
     binary : bool
         if the file-format is a binary type then this flag needs to be set in order to
         read the contents properly
     magic_number_offset : int, optional
         the offset in bytes from the start of the file that the magic number is stored
     """
 
     magic_number_offset = 0
     binary: bool
-    magic_number: ty.Union[str, int]
+    magic_number: ty.Union[str, bytes]
 
     @mark.check
     def check_magic_number(self):
         if self.binary and isinstance(self.magic_number, str):
             magic_bytes = bytes.fromhex(self.magic_number)
         else:
             magic_bytes = self.magic_number
@@ -45,14 +48,62 @@
                 magic_str = self.magic_number
             raise FormatMismatchError(
                 f"Magic number of file {read_magic_str} doesn't match expected "
                 f"{magic_str}"
             )
 
 
+class WithMagicVersion:
+    """Mixin class for Files with version numbers embedded within "magic numbers"
+    the start of their contents.
+
+    Class Attrs
+    -----------
+    magic_pattern : bytes
+        the magic number/string to search for at the start of the file
+    magic_pattern_offset : int, optional
+        the offset in bytes from the start of the file that the magic pattern is read from
+    magic_pattern_maxlength : int, optional
+        the maximum length of the pattern, i.e. the length of the byte-string that will
+        be read from the file, by default it will be the length of the magic_pattern
+        string (which will probably be longer than the string it matches due to the
+        special characters in the regex)
+    """
+
+    binary: bool
+    magic_pattern: bytes
+    magic_pattern_offset = 0
+    magic_pattern_maxlength = None
+
+    @mark.required
+    @property
+    def version(self) -> ty.Union[str, ty.Tuple[str]]:
+        read_length = (
+            self.magic_pattern_length
+            if self.magic_pattern_length
+            else len(self.magic_pattern)
+        )
+        read_bytes = self.read_contents(read_length, offset=self.magic_pattern_offset)
+        match = re.match(self.magic_pattern, read_bytes)
+        if not match:
+            raise FormatMismatchError(
+                f"Byte-string of length {read_length} at {self.magic_pattern_offset} "
+                f"({read_bytes}), doesn't match expected pattern, {self.magic_pattern}"
+            )
+        version = tuple(b.decode("utf-8") for b in match.groups())
+        if not version:
+            raise FileFormatsError(
+                f"No version patterns found in magic pattern of {type(self).__name__} "
+                f"class, {self.magic_pattern}"
+            )
+        if len(version) == 1:
+            version = version[0]
+        return version
+
+
 class WithAdjacentFiles:
     """
     If only the main fspath is provided to the __init__ of the class, this mixin
     automatically includes any "adjacent files", i.e. any files with the same stem but
     different extensions
 
     Note that WithAdjacentFiles must come before the primary type in the method-resolution
```

### Comparing `fileformats-0.8.4/fileformats/core/utils.py` & `fileformats-0.8.5/fileformats/core/utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_classifiers.py` & `fileformats-0.8.5/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_converter.py` & `fileformats-0.8.5/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_detection.py` & `fileformats-0.8.5/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_general.py` & `fileformats-0.8.5/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_mime.py` & `fileformats-0.8.5/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_mixin.py` & `fileformats-0.8.5/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_subpackages.py` & `fileformats-0.8.5/fileformats/core/tests/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_test_extras.py` & `fileformats-0.8.5/fileformats/core/tests/test_test_extras.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/core/tests/test_utils.py` & `fileformats-0.8.5/fileformats/core/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,21 +195,14 @@
     fileset = FileSet(fspaths)
 
     cpy = fileset.copy(dest_dir=dest_dir, collation="adjacent", new_stem="newfile")
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert all(p.stem == "newfile" for p in cpy.fspaths)
 
 
-def test_copy_collation_with_stem_not_adjacent(luigi_file: Luigi, dest_dir):
-    with pytest.raises(
-        FileFormatsError, match="when collation is not set to 'adjacent'"
-    ):
-        luigi_file.copy(dest_dir, collation="any", new_stem="new")
-
-
 def test_copy_collation_leave_diff_dir(work_dir: Path, dest_dir: Path):
     a = work_dir / "a" / "file.x"
     b = work_dir / "b" / "file.y"
     c = work_dir / "c" / "file.z"
     fspaths = (a, b, c)
 
     for x in fspaths:
```

### Comparing `fileformats-0.8.4/fileformats/document/__init__.py` & `fileformats-0.8.5/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/field/__init__.py` & `fileformats-0.8.5/fileformats/field/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,44 +109,49 @@
         except ValueError as e:
             raise FormatMismatchError(str(e)) from None
     return value
 
 
 def array_converter(value):
     if isinstance(value, str):
-        if value.startswith("[") and value.endswith("]"):
+        if (value.startswith("[") and value.endswith("]")) or (
+            value.startswith("(") and value.endswith(")")
+        ):
             value = value[1:-1]
-        elif value.startswith("[") or value.endswith("]"):
+        elif (
+            value.startswith("[")
+            or value.endswith("]")
+            or value.startswith("(")
+            or value.endswith(")")
+        ):
             raise FormatMismatchError(f"Unmatched brackets in array field {value}")
         value = tuple(v.strip() for v in value.split(","))
     else:
         try:
             value = tuple(value)
         except ValueError as e:
             raise FormatMismatchError(str(e)) from None
     return value
 
 
 @attrs.define(repr=False)
 class Text(Singular):
-
     value: str = attrs.field(converter=text_converter)
 
     primitive = str
 
     def __hash__(self):
         return hash(self.value)
 
     def __repr__(self):
         return f'{self._type_name}("{self.value}")'
 
 
 @attrs.define(repr=False)
 class Integer(Singular, ScalarMixin):
-
     value: int = attrs.field(converter=integer_converter)
 
     primitive = int
 
     def __int__(self):
         return self.value
 
@@ -158,15 +163,14 @@
 
     def __hash__(self):
         return hash(self.value)
 
 
 @attrs.define(repr=False)
 class Decimal(Singular, ScalarMixin):
-
     value: decimal.Decimal = attrs.field(converter=decimal_converter)
 
     primitive = float
 
     def __float__(self):
         return float(self.value)
 
@@ -175,15 +179,14 @@
 
     def __hash__(self):
         return hash(self.value)
 
 
 @attrs.define(repr=False)
 class Boolean(Singular, LogicalMixin):
-
     primitive = bool
 
     value: bool = attrs.field(converter=boolean_converter)
 
     def __str__(self):
         return str(self.value).lower()
 
@@ -192,15 +195,14 @@
 
     def __hash__(self):
         return hash(self.value)
 
 
 @attrs.define(auto_attribs=False, repr=False)
 class Array(WithClassifiers, Field):
-
     # WithClassifiers class attrs
     classifiers_attr_name: str = "item_type"
     multiple_classifiers: bool = False
     allowed_classifiers: ty.Tuple[ty.Type[Singular]] = (Singular,)
     item_type: ty.Union[ty.Type[Singular], None] = None
 
     primitive = tuple
```

### Comparing `fileformats-0.8.4/fileformats/field/tests/test_fields.py` & `fileformats-0.8.5/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.8.5/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/generic/__init__.py` & `fileformats-0.8.5/fileformats/generic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import os
 import typing as ty
 from pathlib import Path
 import attrs
 from fileformats.core.fileset import FileSet
-from fileformats.core.exceptions import FormatMismatchError, FileFormatsError
+from fileformats.core.exceptions import (
+    FormatMismatchError,
+    FileFormatsError,
+    UnconstrainedExtensionException,
+)
 from fileformats.core import mark
 from fileformats.core.utils import classproperty
 from fileformats.core.mixin import WithClassifiers
 
 
 class FsObject(FileSet, os.PathLike):
     "Generic file-system object, can be either a file or a directory"
@@ -114,20 +118,23 @@
                 f.read(offset)
             contents = f.read(size)
         return contents
 
     @property
     def actual_ext(self):
         "The actual file extension (out of the primary  and alternate extensions possible)"
-        matching = [e for e in self.possible_exts if self.fspath.name.endswith(e)]
+        constrained_exts = [
+            e for e in self.possible_exts if e is not None
+        ]  # strip out unconstrained
+        matching = [e for e in constrained_exts if self.fspath.name.endswith(e)]
         if not matching:
-            assert False, (
-                f"extension of fspath {self.fspath} is not in possible extensions for "
-                f"{type(self)} class: {self.possible_exts}. This should have been "
-                "checked at initialisation"
+            raise UnconstrainedExtensionException(
+                f"Cannot determine actual extension of {self.fspath}, as it doesn't "
+                f"match any of the defined extensions {constrained_exts} "
+                "(i.e. matches the None extension)"
             )
         # Return the longest matching extension, useful for optional extensions
         return sorted(matching, key=len)[-1]
 
     @property
     def stem(self):
         if self.actual_ext:
```

### Comparing `fileformats-0.8.4/fileformats/image/__init__.py` & `fileformats-0.8.5/fileformats/image/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/image/notclassifiedyet.py` & `fileformats-0.8.5/fileformats/image/notclassifiedyet.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/image/raster.py` & `fileformats-0.8.5/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/image/tests/test_image_raster.py` & `fileformats-0.8.5/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/misc/__init__.py` & `fileformats-0.8.5/fileformats/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/misc/unclassified.py` & `fileformats-0.8.5/fileformats/misc/unclassified.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/model/__init__.py` & `fileformats-0.8.5/fileformats/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/serialization/__init__.py` & `fileformats-0.8.5/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/testing/classifiers.py` & `fileformats-0.8.5/fileformats/testing/classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/testing/headers.py` & `fileformats-0.8.5/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/text/__init__.py` & `fileformats-0.8.5/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/fileformats/video/__init__.py` & `fileformats-0.8.5/fileformats/video/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/LICENSE` & `fileformats-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/README.rst` & `fileformats-0.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/pyproject.toml` & `fileformats-0.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.4/PKG-INFO` & `fileformats-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.8.4
+Version: 0.8.5
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

