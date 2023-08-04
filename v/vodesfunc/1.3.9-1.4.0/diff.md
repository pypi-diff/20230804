# Comparing `tmp/vodesfunc-1.3.9.tar.gz` & `tmp/vodesfunc-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodesfunc-1.3.9.tar", last modified: Wed Jun 21 22:02:38 2023, max compression
+gzip compressed data, was "vodesfunc-1.4.0.tar", last modified: Fri Aug  4 17:01:22 2023, max compression
```

## Comparing `vodesfunc-1.3.9.tar` & `vodesfunc-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 22:02:38.430460 vodesfunc-1.3.9/
--rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.9/LICENSE
--rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1196 2023-06-21 22:02:38.430460 vodesfunc-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.9/README.md
--rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 22:02:38.430460 vodesfunc-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 22:02:38.417457 vodesfunc-1.3.9/vodesfunc/
--rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.9/vodesfunc/__init__.py
--rw-rw-rw-   0        0        0      362 2023-06-21 22:02:18.000000 vodesfunc-1.3.9/vodesfunc/_metadata.py
--rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.9/vodesfunc/aa.py
-drwxrwxrwx   0        0        0        0 2023-06-21 22:02:38.429459 vodesfunc-1.3.9/vodesfunc/auto/
--rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.9/vodesfunc/auto/convert.py
--rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.9/vodesfunc/auto/download.py
--rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.9/vodesfunc/auto/fonts.py
--rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.9/vodesfunc/auto/muxing.py
--rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.9/vodesfunc/auto/parsing.py
--rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.9/vodesfunc/auto/webhook.py
--rw-rw-rw-   0        0        0    32395 2023-05-13 20:45:39.000000 vodesfunc-1.3.9/vodesfunc/automation.py
--rw-rw-rw-   0        0        0     4742 2023-05-05 21:25:21.000000 vodesfunc-1.3.9/vodesfunc/denoise.py
--rw-rw-rw-   0        0        0    12864 2023-05-13 20:45:35.000000 vodesfunc-1.3.9/vodesfunc/descale.py
--rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.9/vodesfunc/misc.py
--rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.9/vodesfunc/noise.py
--rw-rw-rw-   0        0        0    14058 2023-05-24 12:07:39.000000 vodesfunc-1.3.9/vodesfunc/scale.py
--rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.9/vodesfunc/types.py
--rw-rw-rw-   0        0        0     6942 2023-06-21 22:00:50.000000 vodesfunc-1.3.9/vodesfunc/util.py
-drwxrwxrwx   0        0        0        0 2023-06-21 22:02:38.425459 vodesfunc-1.3.9/vodesfunc.egg-info/
--rw-rw-rw-   0        0        0     1196 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-21 22:02:38.000000 vodesfunc-1.3.9/vodesfunc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 17:01:22.015873 vodesfunc-1.4.0/
+-rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1196 2023-08-04 17:01:22.015873 vodesfunc-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.4.0/README.md
+-rw-rw-rw-   0        0        0      360 2023-08-04 16:59:46.000000 vodesfunc-1.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 17:01:22.015873 vodesfunc-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:01:22.002872 vodesfunc-1.4.0/vodesfunc/
+-rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.4.0/vodesfunc/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-08-04 17:00:02.000000 vodesfunc-1.4.0/vodesfunc/_metadata.py
+-rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.4.0/vodesfunc/aa.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:01:22.014874 vodesfunc-1.4.0/vodesfunc/auto/
+-rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.4.0/vodesfunc/auto/convert.py
+-rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.4.0/vodesfunc/auto/download.py
+-rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.4.0/vodesfunc/auto/fonts.py
+-rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.4.0/vodesfunc/auto/muxing.py
+-rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.4.0/vodesfunc/auto/parsing.py
+-rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.4.0/vodesfunc/auto/webhook.py
+-rw-rw-rw-   0        0        0    32395 2023-05-13 20:45:39.000000 vodesfunc-1.4.0/vodesfunc/automation.py
+-rw-rw-rw-   0        0        0     4742 2023-05-05 21:25:21.000000 vodesfunc-1.4.0/vodesfunc/denoise.py
+-rw-rw-rw-   0        0        0    13895 2023-08-04 16:58:40.000000 vodesfunc-1.4.0/vodesfunc/descale.py
+-rw-rw-rw-   0        0        0     3358 2023-08-04 16:23:12.000000 vodesfunc-1.4.0/vodesfunc/misc.py
+-rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.4.0/vodesfunc/noise.py
+-rw-rw-rw-   0        0        0    14058 2023-05-24 12:07:39.000000 vodesfunc-1.4.0/vodesfunc/scale.py
+-rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.4.0/vodesfunc/types.py
+-rw-rw-rw-   0        0        0     6942 2023-06-26 15:52:20.000000 vodesfunc-1.4.0/vodesfunc/util.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:01:22.010871 vodesfunc-1.4.0/vodesfunc.egg-info/
+-rw-rw-rw-   0        0        0     1196 2023-08-04 17:01:21.000000 vodesfunc-1.4.0/vodesfunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-08-04 17:01:21.000000 vodesfunc-1.4.0/vodesfunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 17:01:21.000000 vodesfunc-1.4.0/vodesfunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-04 17:01:21.000000 vodesfunc-1.4.0/vodesfunc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 17:01:21.000000 vodesfunc-1.4.0/vodesfunc.egg-info/top_level.txt
```

### Comparing `vodesfunc-1.3.9/LICENSE` & `vodesfunc-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/PKG-INFO` & `vodesfunc-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.9
+Version: 1.4.0
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.9/setup.py` & `vodesfunc-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/aa.py` & `vodesfunc-1.4.0/vodesfunc/aa.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/auto/convert.py` & `vodesfunc-1.4.0/vodesfunc/auto/convert.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/auto/download.py` & `vodesfunc-1.4.0/vodesfunc/auto/download.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/auto/fonts.py` & `vodesfunc-1.4.0/vodesfunc/auto/fonts.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/auto/muxing.py` & `vodesfunc-1.4.0/vodesfunc/auto/muxing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/auto/parsing.py` & `vodesfunc-1.4.0/vodesfunc/auto/parsing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/auto/webhook.py` & `vodesfunc-1.4.0/vodesfunc/auto/webhook.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/automation.py` & `vodesfunc-1.4.0/vodesfunc/automation.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/denoise.py` & `vodesfunc-1.4.0/vodesfunc/denoise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/descale.py` & `vodesfunc-1.4.0/vodesfunc/descale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from vstools import vs, core, get_w, get_y, depth, iterate, ColorRange, join, get_depth
 from vskernels import Scaler, ScalerT, Kernel, KernelT, Catrom
-from typing import Callable
+from vsmasktools import EdgeDetectT, EdgeDetect
+from typing import Callable, Sequence, Union
 from math import floor
 from dataclasses import dataclass
 
 from .scale import Doubler, NNEDI_Doubler
 
 __all__ = ['DescaleTarget', 'MixedRescale', 'DT']
 
@@ -42,28 +43,31 @@
         :param width:           Width to be descaled to. (will be calculated if None)
         :param base_width:      Needed for fractional descales. (will be calculated if None)
         :param do_post_double:  A function that's called on the doubled clip. Can be used to do sensitive processing on a bigger clip. (e. g. Dehaloing)
         :param credit_mask:     Can be used to pass a mask that'll be used or False to disable error masking.
         :param credit_mask_thr: The error threshold of the automatically generated credit mask.
         :param credit_mask_bh:  Generates an error mask based on a descale using the baseheight. For some reason had better results with this on some shows.
         :param line_mask:       Can be used to pass a mask that'll be used or False to disable line masking.
+                                You can also pass a list containing edgemask function, scaler and thresholds to generate the mask on the doubled clip.
+                                Which may or may not result in something better.
+                                For example: line_mask=(KirschTCanny, Bilinear, 50 / 250, 150 / 250)
         :param bbmod_masks:     Specify rows to be bbmod'ed for a clip to generate the masks on. Will probably be useful for the new border param in descale.
     """
     height: float
     kernel: KernelT = Catrom
     upscaler: Doubler | ScalerT = NNEDI_Doubler()
     downscaler: ScalerT = Catrom
     base_height: int | None = None
     width: float | None = None
     base_width: int | None = None
     do_post_double: Callable[[vs.VideoNode], vs.VideoNode] | None = None
     credit_mask: vs.VideoNode | bool | None = None
     credit_mask_thr: float = 0.04
     credit_mask_bh: bool = False
-    line_mask: vs.VideoNode | bool | None = None
+    line_mask: vs.VideoNode | bool | Sequence[Union[EdgeDetectT, ScalerT, float]] | None = None
     bbmod_masks: int | list[int] = 0 # Not actually implemented yet lol
 
     def generate_clips(self, clip: vs.VideoNode) -> 'DescaleTarget':
         """
             Generates descaled and rescaled clips of the given input clip
 
             :param clip:    Clip to descale and rescale
@@ -94,15 +98,15 @@
                 .std.CopyFrameProps(clip).std.SetFrameProp('Rescale', self.index + 1)
             if self.credit_mask_bh:
                 base_height_desc = self.kernel.descale(clip, self.base_height * (clip.width / clip.height), self.base_height)
                 ref_y = self.kernel.scale(base_height_desc, clip.width, clip.height)
             else:
                 ref_y = self.rescale
             
-        if self.line_mask != False:
+        if self.line_mask != False and not isinstance(self.line_mask, Sequence):
             if not isinstance(self.line_mask, vs.VideoNode):
                 try:
                     from vsmasktools.edge import KirschTCanny
                     try:
                         # Scaling was changed so I abuse the new param to check if its the newer version
                         self.line_mask = KirschTCanny().edgemask(clip, lthr=80 / 255, hthr=150 / 255, planes=(0, True))
                     except:
@@ -165,14 +169,21 @@
         else:
             self.upscale = self.downscaler.scale(self.doubled, clip.width, clip.height)
 
         self.upscale = depth(self.upscale, 16)
         self.rescale = depth(self.rescale, 16)
 
         if self.line_mask != False:
+            if isinstance(self.line_mask, Sequence):
+                if len(self.line_mask) < 4:
+                    raise ValueError("DescaleTarget line_mask must contain an Edgemask, Downscaler, lthr and hthr if you passed a list.")
+                mask_fun = EdgeDetect.ensure_obj(self.line_mask[0])
+                mask = mask_fun.edgemask(self.doubled, self.line_mask[2], self.line_mask[3], planes=0)
+                self.line_mask = Scaler.ensure_obj(self.line_mask[1]).scale(mask, clip.width, clip.height)
+                
             self.upscale = y.std.MaskedMerge(self.upscale, self.line_mask)
 
         if self.credit_mask != False or self.credit_mask_thr <= 0:
             self.upscale = self.upscale.std.MaskedMerge(y, self.credit_mask)
 
         self.upscale = depth(self.upscale, get_depth(clip))
         self.upscale = self.upscale if clip.format.color_family == vs.GRAY else join(self.upscale, clip)
```

### Comparing `vodesfunc-1.3.9/vodesfunc/misc.py` & `vodesfunc-1.4.0/vodesfunc/misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,34 @@
 import vapoursynth as vs
 core = vs.core
 
-from vstools import depth, get_y
+from vstools import KwargsT, depth, get_y
 from functools import partial
 from typing import Callable
 
 
 def lehmer_merge(*clips: vs.VideoNode, 
-        lowpass: Callable[[vs.VideoNode], vs.VideoNode]=lambda i: core.std.BoxBlur(i, hradius=3, vradius=3, hpasses=2, vpasses=2)):
+        lowpass: Callable[[vs.VideoNode], vs.VideoNode]=lambda i: core.std.BoxBlur(i, hradius=3, vradius=3, hpasses=2, vpasses=2), 
+        **kwargs: KwargsT):
     """
         Perform a lehmer merge using a bunch of clips with the goal of getting the detail from each.
         Credits to Zewia
 
         :param clips:       However many clips
         :param lowpass:     Callable used to perform the lowpass
 
         :return:            Merged clip
     """
-    clips = list(clips)
-    count = len(clips)
-    expr = ""
-
-    for i in range(count):
-        expr += f"src{i} src{count + i} - D{i}! "
-
-    for v in range(2):
-        for i in range(count):
-            expr += f"D{i}@ {v + 2} pow "
-        expr += "+ " * (count - 1) + f"P{v}! "
-
-    for i in range(count):
-        expr += f"src{count + i} "
-    expr += "+ " * (count - 1) + f"{count} / "
-
-    expr += "P0@ 0 = 0 P1@ P0@ / ? +"
-
-    blur = [lowpass(i) for i in clips]
-    return core.akarin.Expr(clips + blur, expr)
+    print("vodesfunc.lehmer_merge is deprecated. Please use vsdenoise.frequency_merge!")
+    from vsdenoise import frequency_merge
+    args = KwargsT(
+        lowpass=lowpass
+    )
+    args.update(**kwargs)
+    return frequency_merge(clips, **args)
 
 
 def dirty_prop_set(clip: vs.VideoNode, threshold: int = 1100, luma_scaling: int = 24, prop_name: str = None,
                    src_prop_val: any = None, bbm_prop_val: any = None, debug_output: bool = False
                    ) -> list[vs.VideoNode]:
     """
     Dirty-edge-based frameprop setting function using bbm, a brightness difference check and a brightness scaling
```

### Comparing `vodesfunc-1.3.9/vodesfunc/noise.py` & `vodesfunc-1.4.0/vodesfunc/noise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/scale.py` & `vodesfunc-1.4.0/vodesfunc/scale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/types.py` & `vodesfunc-1.4.0/vodesfunc/types.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc/util.py` & `vodesfunc-1.4.0/vodesfunc/util.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.9/vodesfunc.egg-info/PKG-INFO` & `vodesfunc-1.4.0/vodesfunc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.9
+Version: 1.4.0
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.9/vodesfunc.egg-info/SOURCES.txt` & `vodesfunc-1.4.0/vodesfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

