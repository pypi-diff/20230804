# Comparing `tmp/vaal-1.4.1-py3-none-any.whl.zip` & `tmp/vaal-1.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11905 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      464 b- defN 23-Jul-27 05:09 deepview/vaal/__init__.py
--rw-rw-r--  2.0 unx     1513 b- defN 23-Jul-27 05:09 deepview/vaal/camera.py
--rw-rw-r--  2.0 unx    12893 b- defN 23-Jul-27 05:09 deepview/vaal/context.py
--rw-rw-r--  2.0 unx     9004 b- defN 23-Jul-27 05:09 deepview/vaal/library.py
--rw-rw-r--  2.0 unx    11710 b- defN 23-Jul-27 05:12 vaal-1.4.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      229 b- defN 23-Jul-27 05:12 vaal-1.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-27 05:12 vaal-1.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-27 05:12 vaal-1.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      698 b- defN 23-Jul-27 05:12 vaal-1.4.1.dist-info/RECORD
-9 files, 36612 bytes uncompressed, 10711 bytes compressed:  70.7%
+Zip file size: 12026 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      464 b- defN 23-Aug-04 16:25 deepview/vaal/__init__.py
+-rw-rw-r--  2.0 unx     1829 b- defN 23-Aug-04 16:25 deepview/vaal/camera.py
+-rw-rw-r--  2.0 unx    13008 b- defN 23-Aug-04 16:25 deepview/vaal/context.py
+-rw-rw-r--  2.0 unx     9004 b- defN 23-Aug-04 16:25 deepview/vaal/library.py
+-rw-rw-r--  2.0 unx    11710 b- defN 23-Aug-04 16:30 vaal-1.4.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      229 b- defN 23-Aug-04 16:30 vaal-1.4.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-04 16:30 vaal-1.4.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Aug-04 16:30 vaal-1.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      698 b- defN 23-Aug-04 16:30 vaal-1.4.2.dist-info/RECORD
+9 files, 37043 bytes uncompressed, 10832 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: deepview/vaal/context.py
 Comment: 
 
 Filename: deepview/vaal/library.py
 Comment: 
 
-Filename: vaal-1.4.1.dist-info/LICENSE.txt
+Filename: vaal-1.4.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vaal-1.4.1.dist-info/METADATA
+Filename: vaal-1.4.2.dist-info/METADATA
 Comment: 
 
-Filename: vaal-1.4.1.dist-info/WHEEL
+Filename: vaal-1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: vaal-1.4.1.dist-info/top_level.txt
+Filename: vaal-1.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: vaal-1.4.1.dist-info/RECORD
+Filename: vaal-1.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deepview/vaal/camera.py

```diff
@@ -12,29 +12,35 @@
 class CameraType(Enum):
     Image = 0
     Video = 1
     Stream = 2
 
 
 class Camera:
-    def __init__(self, source, source_type):
+    def __init__(self, source, source_type, width=None, height=None):
         self.source = source
         self.source_type = source_type
         self.video_capture = None
         self.image_index = -1
+        self.width = width
+        self.height = height
 
         if isinstance(self.source, str) and \
                 self.source_type == CameraType.Image:
             self.source = [self.source]
 
     def __iter__(self):
         import cv2
 
         if self.source_type in [CameraType.Video, CameraType.Stream]:
             self.video_capture = cv2.VideoCapture(self.source)
+            if self.width is not None:
+                self.video_capture.set(cv2.CAP_PROP_FRAME_WIDTH, self.width)
+            if self.height is not None:
+                self.video_capture.set(cv2.CAP_PROP_FRAME_HEIGHT, self.height)
         return self
 
     def __next__(self):
         import cv2
         if self.source_type == CameraType.Image:
             self.image_index += 1
             if self.image_index >= len(self.source):
```

## deepview/vaal/context.py

```diff
@@ -4,33 +4,32 @@
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from ctypes import \
     cast, c_void_p, c_int, c_int32, c_uint32, c_float, c_size_t, \
-    c_char_p, create_string_buffer, byref
+    create_string_buffer, byref
 from deepview.vaal.library import VAALBox, VAALKeypoint, VAALEuler, \
     lib, strerror, Type, ModelType
 from enum import Enum
-import os
 
 
 class Context:
     """
     DeepView VAAL Context is used to manage DeepViewRT models with VisionPack.
     """
 
     def __init__(self, engine="npu", model_type=ModelType.NONE):
         if model_type != ModelType.NONE:
             c_model_type = c_uint32(model_type.value)
-            self._handle = lib.vaal_model_probe(engine.encode('utf-8'), c_model_type)
+            self._handle = lib.vaal_model_probe(
+                engine.encode('utf-8'), c_model_type)
         else:
             self._handle = lib.vaal_context_create(engine.encode('utf-8'))
-        
 
     def __del__(self):
         if self._handle is not None:
             lib.vaal_context_release(self._handle)
             self._handle = None
 
     def __getitem__(self, key):
@@ -171,19 +170,23 @@
             if res is not None:
                 outputs.append(res)
                 i += 1
             else:
                 break
         return outputs
 
-    def label(self, index):
+    def label(self, index, nofail=True):
         lbl = lib.vaal_label(self._handle, index)
-        if lbl is None:
-            raise ValueError('No label found with index %d' % index)
-        return lbl.decode('utf-8')
+        lbl = lbl.decode('utf-8') if lbl is not None else ''
+        if lbl == '':
+            if nofail:
+                return str(index)
+            else:
+                raise ValueError('no label at index %d' % index)
+        return lbl
 
     def tensor(self, name):
         try:
             ptr = lib.vaal_get_tensor_by_name(
                 self._handle, name.encode('utf-8'))
         except Exception:
             raise ValueError("Unable to find tensor with name: %s" % name)
```

## Comparing `vaal-1.4.1.dist-info/LICENSE.txt` & `vaal-1.4.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vaal-1.4.1.dist-info/RECORD` & `vaal-1.4.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 deepview/vaal/__init__.py,sha256=PiYF_oAd7xGaa1JvOChOIaTFkFHh35un5sbF8xbSEew,464
-deepview/vaal/camera.py,sha256=Q_uoNMQi9Oz7XHlDsQRfExUjjrwdxDr2NzLXOzEXX4c,1513
-deepview/vaal/context.py,sha256=Eflo8Nyf7OifJMCnj0Z0Zrq7CVNL0SupuVsy7gruun0,12893
+deepview/vaal/camera.py,sha256=G0waR6jglgB3IY212GbzJILdM0L_0g9kaL2e4bJPKE8,1829
+deepview/vaal/context.py,sha256=v6Rc7imf_zBAf2OxYw-rfp7m-6P4mbTvAHWneYIuRpk,13008
 deepview/vaal/library.py,sha256=ANcCL_u2guAeHD6mKABWwpBu0fmDVDvCARfr4d_sFTs,9004
-vaal-1.4.1.dist-info/LICENSE.txt,sha256=tRF0H4BBjc7hxfxRe2Y573C-tye_wJQBFdZu_wG_rLQ,11710
-vaal-1.4.1.dist-info/METADATA,sha256=PY1ukwdRbnrfnqki2l9_0NHHvA57CF4M6SDtCzBveRI,229
-vaal-1.4.1.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
-vaal-1.4.1.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
-vaal-1.4.1.dist-info/RECORD,,
+vaal-1.4.2.dist-info/LICENSE.txt,sha256=tRF0H4BBjc7hxfxRe2Y573C-tye_wJQBFdZu_wG_rLQ,11710
+vaal-1.4.2.dist-info/METADATA,sha256=AjBl9Ql1dmzbhsAE639PqIrvEmmNiSrP_3FqrTj2ovI,229
+vaal-1.4.2.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
+vaal-1.4.2.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
+vaal-1.4.2.dist-info/RECORD,,
```

