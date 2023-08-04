# Comparing `tmp/anydyce-0.4.0-py3-none-any.whl.zip` & `tmp/anydyce-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 20628 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1049 b- defN 22-Oct-25 12:10 anydyce/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 22-Oct-25 12:11 anydyce/_version.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-25 12:10 anydyce/py.typed
--rw-r--r--  2.0 unx    55368 b- defN 22-Oct-25 12:10 anydyce/viz.py
--rw-r--r--  2.0 unx     2118 b- defN 22-Oct-25 12:11 anydyce-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    15580 b- defN 22-Oct-25 12:11 anydyce-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-25 12:11 anydyce-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Oct-25 12:11 anydyce-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      678 b- defN 22-Oct-25 12:11 anydyce-0.4.0.dist-info/RECORD
-9 files, 74941 bytes uncompressed, 19468 bytes compressed:  74.0%
+Zip file size: 21342 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1049 b- defN 22-Oct-27 18:18 anydyce/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 22-Oct-27 18:18 anydyce/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Oct-27 18:18 anydyce/py.typed
+-rw-r--r--  2.0 unx    58977 b- defN 22-Oct-27 18:18 anydyce/viz.py
+-rw-r--r--  2.0 unx     2118 b- defN 22-Oct-27 18:18 anydyce-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15580 b- defN 22-Oct-27 18:18 anydyce-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Oct-27 18:18 anydyce-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 22-Oct-27 18:18 anydyce-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      678 b- defN 22-Oct-27 18:18 anydyce-0.4.1.dist-info/RECORD
+9 files, 78550 bytes uncompressed, 20182 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: anydyce/py.typed
 Comment: 
 
 Filename: anydyce/viz.py
 Comment: 
 
-Filename: anydyce-0.4.0.dist-info/LICENSE
+Filename: anydyce-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: anydyce-0.4.0.dist-info/METADATA
+Filename: anydyce-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: anydyce-0.4.0.dist-info/WHEEL
+Filename: anydyce-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: anydyce-0.4.0.dist-info/top_level.txt
+Filename: anydyce-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: anydyce-0.4.0.dist-info/RECORD
+Filename: anydyce-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anydyce/_version.py

```diff
@@ -1,3 +1,3 @@
-__vers_str__ = "0.4.0"
-__version__ = (0, 4, 0)
+__vers_str__ = "0.4.1"
+__version__ = (0, 4, 1)
```

## anydyce/viz.py

```diff
@@ -1,22 +1,23 @@
 # ======================================================================================
-# Copyright and other protections apply. Please see the accompanying LICENSE file for
+# Copyright other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
 from __future__ import annotations
 
 import asyncio
 import base64
 import csv
 import io
 import math
+import urllib.parse
 import warnings
 from abc import abstractmethod, abstractproperty
 from collections import Counter
 from dataclasses import dataclass, field, fields
 from enum import Enum
 from fractions import Fraction
 from functools import partial, wraps
@@ -66,31 +67,38 @@
 ColorT = Sequence[float]
 ColorListT = Iterable[ColorT]
 HLikeT = Union[H, HableT]
 HFormatterT = Callable[[RealLike, Fraction, H], str]
 HPlotterFactoryT = Callable[[], "HPlotter"]
 
 
+class ImageType(str, Enum):
+    PNG = "PNG"
+    SVG = "SVG"
+
+
 class TraditionalPlotType(str, Enum):
     NORMAL = "Normal"
     AT_MOST = "At Most"
     AT_LEAST = "At Least"
 
 
 class SettingsDict(TypedDict):
     alpha: float
     burst_cmap_inner: str
     burst_cmap_link: bool
     burst_cmap_outer: str
     burst_color_bg: str
+    burst_color_bg_trnsp: bool
     burst_color_text: str
     burst_swap: bool
     burst_zero_fill_normalize: bool
     enable_cutoff: bool
     graph_type: TraditionalPlotType
+    img_type: ImageType
     markers: str
     plot_style: str
     scale: int
     show_shadow: bool
 
 
 # ---- Data ----------------------------------------------------------------------------
@@ -199,43 +207,60 @@
 
     return _decorator(f) if callable(f) else _decorator
 
 
 # ---- Classes -------------------------------------------------------------------------
 
 
+class Image:
+    @beartype
+    def __init__(self, file_name: str, file_type: ImageType, data: bytes):
+        if file_type is ImageType.PNG:
+            self._data = base64.b64encode(data).decode()
+            self._mime_pfx = "data:image/png;base64,"
+        elif file_type is ImageType.SVG:
+            self._data = data.decode()
+            self._mime_pfx = "data:image/svg+xml,"
+        else:
+            assert False, f"unrecognized file type {file_type}"
+
+        if file_name.lower().endswith(file_type.lower()):
+            self._file_name = file_name
+        else:
+            self._file_name = file_name + "." + file_type.lower()
+
+        self._file_type = file_type
+
+    @beartype
+    def _repr_png_(self):
+        return self._data if self._file_type is ImageType.PNG else None
+
+    @beartype
+    def _repr_svg_(self):
+        return self._data if self._file_type is ImageType.SVG else None
+
+    @beartype
+    def download_link(self) -> str:
+        return f'<a download="{self._file_name}" href="{self._mime_pfx}{urllib.parse.quote(self._data)}" target="_blank">Download {self._file_type} image</a>'
+
+
 @dataclass(frozen=True)
 class _PlotWidgetsDataclass:
 
     # Widget to trigger updates (hack)
     _rev_no: widgets.IntText = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.IntText,
             value=0,
             layout={"display": "none"},
         ),
     )
 
-    # Generic display widgets
-    scale: widgets.FloatLogSlider = field(
-        init=False,
-        repr=False,
-        default_factory=partial(
-            widgets.IntSlider,
-            value=12,
-            min=8,
-            max=16,
-            step=1,
-            continuous_update=False,
-            description="Scale",
-        ),
-    )
-
     # Data culling widgets
     cutoff: widgets.FloatLogSlider = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.FloatLogSlider,
             value=_CUTOFF_BASE ** -(_CUTOFF_EXP - 2),
@@ -254,14 +279,41 @@
         repr=False,
         default_factory=partial(
             widgets.Checkbox,
             description="Hide Small Outcomes",
         ),
     )
 
+    # Generic display widgets
+    scale: widgets.FloatLogSlider = field(
+        init=False,
+        repr=False,
+        default_factory=partial(
+            widgets.IntSlider,
+            value=12,
+            min=8,
+            max=16,
+            step=1,
+            continuous_update=False,
+            description="Scale",
+        ),
+    )
+
+    img_type: widgets.ToggleButtons = field(
+        init=False,
+        repr=False,
+        default_factory=partial(
+            widgets.ToggleButtons,
+            value=next(iter(ImageType)),
+            options=[(img_type.value, img_type) for img_type in ImageType],
+            description="Image Format",
+            rows=min(len(ImageType), 5),
+        ),
+    )
+
     # Burst plot widgets
     burst_cmap_inner: widgets.Dropdown = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.Dropdown,
             value=next(iter(matplotlib.colormaps)),
@@ -286,25 +338,36 @@
             widgets.Dropdown,
             value=next(iter(matplotlib.colormaps)),
             options=sorted(matplotlib.colormaps.keys()),
             description="Outer Colors",
         ),
     )
 
-    burst_color_bg: widgets.Dropdown = field(
+    burst_color_bg: widgets.ColorPicker = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.ColorPicker,
             value="white",
             # options=sorted(sorted(matplotlib.colors.CSS4_COLORS.keys())),
             concise=False,
             description="Background",
         ),
     )
+
+    burst_color_bg_trnsp: widgets.Checkbox = field(
+        init=False,
+        repr=False,
+        default_factory=partial(
+            widgets.Checkbox,
+            value=False,
+            description="Transparent",
+        ),
+    )
+
     burst_color_text: widgets.ColorPicker = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.ColorPicker,
             value="black",
             # options=sorted(sorted(matplotlib.colors.CSS4_COLORS.keys())),
@@ -354,14 +417,15 @@
         default_factory=partial(
             widgets.Select,
             value=next(iter(TraditionalPlotType)),
             options=[
                 (graph_type.value, graph_type) for graph_type in TraditionalPlotType
             ],
             description="Plot Type",
+            rows=min(len(TraditionalPlotType), 5),
         ),
     )
 
     markers: widgets.Text = field(
         init=False,
         repr=False,
         default_factory=partial(
@@ -401,27 +465,30 @@
     r"""
     !!! warning "Experimental"
 
         This class should be considered experimental and may change or disappear in
         future versions.
     """
 
+    @beartype
     def __init__(
         self,
         *,
         initial_alpha: float = DEFAULT_ALPHA,
         initial_burst_cmap_inner: str = DEFAULT_CMAP_BURST_INNER,
         initial_burst_cmap_link: bool = True,
         initial_burst_cmap_outer: str = DEFAULT_CMAP_BURST_OUTER,
         initial_burst_color_bg: str = "white",
+        initial_burst_color_bg_trnsp: bool = False,
         initial_burst_color_text: str = DEFAULT_COLOR_TEXT,
         initial_burst_swap: bool = False,
         initial_burst_zero_fill_normalize: bool = False,
         initial_enable_cutoff: bool = False,
         initial_graph_type: TraditionalPlotType = TraditionalPlotType.NORMAL,
+        initial_img_type: ImageType = ImageType.PNG,
         initial_markers: str = "oX^v><dP",
         initial_plot_style: str = "bmh",
         initial_show_shadow: bool = False,
     ):
         super().__init__()
 
         if initial_plot_style not in matplotlib.style.available:
@@ -433,34 +500,42 @@
 
         self.alpha.value = initial_alpha
         self.burst_cmap_inner.value = initial_burst_cmap_inner
         self.burst_cmap_link.value = initial_burst_cmap_link
         self.burst_cmap_outer.disabled = initial_burst_cmap_link
         self.burst_cmap_outer.value = initial_burst_cmap_outer
         self.burst_color_bg.value = initial_burst_color_bg
+        self.burst_color_bg_trnsp.value = initial_burst_color_bg_trnsp
         self.burst_color_text.value = initial_burst_color_text
         self.burst_swap.value = initial_burst_swap
         self.burst_zero_fill_normalize.value = initial_burst_zero_fill_normalize
         self.cutoff.disabled = not initial_enable_cutoff
         self.enable_cutoff.value = initial_enable_cutoff
         self.graph_type.value = initial_graph_type
+        self.img_type.value = initial_img_type
         self.markers.value = initial_markers
         self.plot_style.value = initial_plot_style
         self.show_shadow.value = initial_show_shadow
 
         def _handle_burst_cmap_link(change) -> None:
             self.burst_cmap_outer.disabled = change["new"]
 
         self.burst_cmap_link.observe(_handle_burst_cmap_link, names="value")
 
+        def _handle_burst_color_bg_trnsp(change) -> None:
+            self.burst_color_bg.disabled = change["new"]
+
+        self.burst_color_bg_trnsp.observe(_handle_burst_color_bg_trnsp, names="value")
+
         def _handle_cutoff(change) -> None:
             self.cutoff.disabled = not change["new"]
 
         self.enable_cutoff.observe(_handle_cutoff, names="value")
 
+    @beartype
     def asdict(self) -> Dict[str, Any]:
         return dict((field.name, getattr(self, field.name)) for field in fields(self))
 
 
 class HPlotter:
     r"""
     !!! warning "Experimental"
@@ -484,38 +559,46 @@
     def layout(self, plot_widgets: PlotWidgets) -> widgets.Widget:
         r"""
         Takes a set of widgets (*plot_widgets*) and returns a container (layout) widget
         selecting those needed by the plotter.
         """
         return widgets.VBox(
             [
-                plot_widgets.scale,
                 plot_widgets.enable_cutoff,
                 plot_widgets.cutoff,
+                plot_widgets.img_type,
+                plot_widgets.scale,
             ]
         )
 
     @abstractmethod
     def plot(
         self,
-        fig: Figure,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ):
         r"""
         Creates and displays a visualization of the provided histograms. *fig* is the
         [``#!python
         matplotlib.figure.Figure``](https://matplotlib.org/stable/api/figure_api.html#matplotlib.figure.Figure)
         in which the visualization should be constructed. *hs* is a sequence of
         three-tuples, a name, a primary histogram, and an optional secondary histogram
         (``#!python None`` if omitted). Plotters should implement this function to
         display at least the primary histogram and visually associate it with the name.
         """
         raise NotImplementedError
 
+    @beartype
+    def transparent(self, requested: bool) -> bool:
+        r"""
+        Returns whether this plotter produces plots which support transparency if
+        *requested*. The default implementation always returns ``#!python False``.
+        """
+        return False
+
 
 class BarHPlotter(HPlotter):
     r"""
     !!! warning "Experimental"
 
         This class should be considered experimental and may change or disappear in
         future versions.
@@ -547,20 +630,24 @@
                 ),
             ]
         )
 
     @beartype
     def plot(
         self,
-        fig: Figure,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
-        xmin, ymin, dx, dy = 0, 0, 1, 1
-        ax = fig.add_axes((xmin, ymin, dx, dy))
+        _, ax = matplotlib.pyplot.subplots(
+            figsize=(
+                settings["scale"],
+                settings["scale"] / 16 * 9,
+            )
+        )
+
         plot_bar(
             ax,
             tuple((label, h) for label, h, _ in hs),
             alpha=settings["alpha"],
             graph_type=settings["graph_type"],
             shadow=settings["show_shadow"],
         )
@@ -590,57 +677,58 @@
         return widgets.VBox(
             [
                 widgets.HBox(
                     [
                         widgets.VBox(
                             [
                                 cutoff_layout_widget,
-                                plot_widgets.burst_swap,
-                                plot_widgets.burst_zero_fill_normalize,
                             ]
                         ),
                         widgets.VBox(
                             [
+                                plot_widgets.burst_swap,
+                                plot_widgets.burst_zero_fill_normalize,
                                 plot_widgets.burst_cmap_inner,
                                 plot_widgets.burst_cmap_outer,
                                 plot_widgets.burst_cmap_link,
                             ]
                         ),
                         widgets.VBox(
                             [
                                 plot_widgets.alpha,
                                 plot_widgets.burst_color_text,
                                 plot_widgets.burst_color_bg,
+                                plot_widgets.burst_color_bg_trnsp,
                             ]
                         ),
                     ]
                 ),
             ]
         )
 
     @beartype
     def plot(
         self,
-        fig: Figure,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
         cols = 3
         logical_rows = len(hs) // cols + (len(hs) % cols != 0)
         # Height of row gaps in relation to height of figs
-        gap_size_ratio = Fraction(2, 5)
+        gap_size_ratio = Fraction(1, 5)
         total_gaps = max(0, logical_rows - 1)
-        fig.set_figwidth(settings["scale"])
-        fig.set_figheight(
-            settings["scale"] / 16 * 5 * (logical_rows + total_gaps * gap_size_ratio)
-        )
-        fig.set_facecolor(settings["burst_color_bg"])
-
-        actual_rows_per_fig = gap_size_ratio.denominator**2
-        actual_rows_per_gap = gap_size_ratio.numerator * gap_size_ratio.denominator
+        figsize = (
+            settings["scale"],
+            float(
+                settings["scale"] * (logical_rows + total_gaps * gap_size_ratio) / cols
+            ),
+        )
+        matplotlib.pyplot.figure(facecolor=settings["burst_color_bg"], figsize=figsize)
+        actual_rows_per_fig = gap_size_ratio.denominator
+        actual_rows_per_gap = gap_size_ratio.numerator
         total_actual_rows = (
             logical_rows * actual_rows_per_fig + total_gaps * actual_rows_per_gap
         )
 
         def _zero_fill_normalize():
             unique_outcomes: Set[RealLike] = set()
 
@@ -672,30 +760,31 @@
             )
 
             if h_outer is not None:
                 if settings["burst_swap"]:
                     h_inner, h_outer = h_outer, h_inner
 
             logical_row = i // cols
-            actual_fig_row_start = logical_row * (
-                actual_rows_per_gap + actual_rows_per_fig
-            )
-
+            actual_row_start = logical_row * (actual_rows_per_gap + actual_rows_per_fig)
             ax = matplotlib.pyplot.subplot2grid(
                 (total_actual_rows, cols),
-                (actual_fig_row_start, i % cols),
+                (actual_row_start, i % cols),
                 rowspan=actual_rows_per_fig,
             )
             plot_burst(
                 ax,
                 h_inner,
                 h_outer,
                 **plot_burst_kw,
             )
 
+    @beartype
+    def transparent(self, requested: bool) -> bool:
+        return requested
+
 
 class HorizontalBarHPlotter(BarHPlotter):
     r"""
     !!! warning "Experimental"
 
         This class should be considered experimental and may change or disappear in
         future versions.
@@ -705,28 +794,27 @@
     """
 
     NAME = "Horizontal Bar Plots"
 
     @beartype
     def plot(
         self,
-        fig: Figure,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
         total_outcomes = sum(
             1 for _ in chain.from_iterable(h.outcomes() for _, h, _ in hs)
         )
         total_height = total_outcomes + 1  # one extra to accommodate the axis
         inches_per_height_unit = settings["scale"] / 64
-        fig.set_figwidth(settings["scale"])
-        fig.set_figheight(total_height * inches_per_height_unit)
-        grid = (total_height, 1)
-        top = 0
-        ax = first_ax = None
+        figsize = (
+            settings["scale"],
+            total_height * inches_per_height_unit,
+        )
+        matplotlib.pyplot.figure(figsize=figsize)
         barh_kw: Dict[str, Any] = dict(alpha=settings["alpha"])
 
         if settings["show_shadow"]:
             barh_kw.update(
                 dict(
                     path_effects=[
                         matplotlib.patheffects.withSimplePatchShadow(),
@@ -745,35 +833,36 @@
             # Our current style has a cycler with colors, so use it
             cycler = matplotlib.style.library[plot_style]["axes.prop_cycle"]
         else:
             # Revert to the global default
             cycler = matplotlib.rcParams["axes.prop_cycle"]
 
         color_iter = cycle(cycler.by_key().get("color", (None,)))
+        row_start = 0
+        first_ax = ax = None
 
         for i, (label, h, _) in enumerate(hs):
             outcomes, values = values_xy_for_graph_type(h, settings["graph_type"])
-            loc = (top, 0)
             rowspan = len(outcomes)
-            top += rowspan
 
             if first_ax is None:
                 first_ax = ax = matplotlib.pyplot.subplot2grid(
-                    grid, loc, rowspan=rowspan
+                    (total_height, 1), (row_start, 0), rowspan=rowspan
                 )
             else:
                 ax = matplotlib.pyplot.subplot2grid(
-                    grid, loc, rowspan=rowspan, sharex=first_ax
+                    (total_height, 1), (row_start, 0), rowspan=rowspan, sharex=first_ax
                 )
 
             ax.set_yticks(outcomes)
             ax.tick_params(labelbottom=False)
             ax.set_ylim((max(outcomes) + 0.5, min(outcomes) - 0.5))
             ax.barh(outcomes, values, color=next(color_iter), label=label, **barh_kw)
             ax.legend(loc="upper right")
+            row_start += rowspan
 
         if ax is not None:
             ax.tick_params(labelbottom=True)
             ax.xaxis.set_major_formatter(matplotlib.ticker.PercentFormatter(xmax=1))
 
 
 class LineHPlotter(HPlotter):
@@ -811,20 +900,24 @@
                 ),
             ]
         )
 
     @beartype
     def plot(
         self,
-        fig: Figure,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
-        xmin, ymin, dx, dy = 0, 0, 1, 1
-        ax = fig.add_axes((xmin, ymin, dx, dy))
+        _, ax = matplotlib.pyplot.subplots(
+            figsize=(
+                settings["scale"],
+                settings["scale"] / 16 * 9,
+            )
+        )
+
         plot_line(
             ax,
             tuple((label, h) for label, h, _ in hs),
             alpha=settings["alpha"],
             graph_type=settings["graph_type"],
             markers=settings["markers"],
             shadow=settings["show_shadow"],
@@ -847,20 +940,24 @@
     """
 
     NAME = "Scatter Plot"
 
     @beartype
     def plot(
         self,
-        fig: Figure,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
-        xmin, ymin, dx, dy = 0, 0, 1, 1
-        ax = fig.add_axes((xmin, ymin, dx, dy))
+        _, ax = matplotlib.pyplot.subplots(
+            figsize=(
+                settings["scale"],
+                settings["scale"] / 16 * 9,
+            )
+        )
+
         plot_scatter(
             ax,
             tuple((label, h) for label, h, _ in hs),
             alpha=settings["alpha"],
             graph_type=settings["graph_type"],
             markers=settings["markers"],
             shadow=settings["show_shadow"],
@@ -965,15 +1062,15 @@
 
         for plotter_name, plotter in self._plotters_by_name.items():
             self._layouts_by_name[plotter_name] = plotter.layout(plot_widgets)
 
         self._hs: Tuple[Tuple[str, H, Optional[H]], ...] = ()
         self._hs_culled: Tuple[Tuple[str, H, Optional[H]], ...] = ()
         self._cutoff: Optional[float] = None
-        self._csv_download_link = HTML()
+        self._csv_download_link = ""
         self.update_hs(histogram_specs)
 
         self._selected_plotter: Optional[HPlotter]
 
         tab_names = tuple(self._plotters_by_name.keys())
 
         chooser_tab = widgets.Tab(
@@ -1013,44 +1110,53 @@
         r"""
         Displays the container responsible for selecting which plotter is used.
         """
         display(self._out)
 
     @beartype
     # @debounce
-    def plot(self, **settings) -> None:
+    def plot(self, **kw) -> None:
         r"""
         Callback for updating the visualization in response to configuration or data
         changes. *settings* are the current values from all control widgets. (See
         [``PlotWidgets``][anydyce.viz.PlotWidgets].)
         """
+        settings = cast(SettingsDict, kw)
         cutoff = (
             self._plot_widgets.cutoff.value
             if self._plot_widgets.enable_cutoff.value
             else None
         )
 
         if self._cutoff != cutoff:
             self._cutoff = cutoff
             self._cull_data()
 
-        display(self._csv_download_link)
-        matplotlib.rcParams.update(matplotlib.rcParamsDefault)
-
         with matplotlib.style.context(settings["plot_style"]):
-            fig = matplotlib.pyplot.figure(
-                figsize=(settings["scale"], settings["scale"] / 16 * 9)
-            )
-
             if self._selected_plotter is not None:
-                self._selected_plotter.plot(
-                    fig, self._hs_culled, cast(SettingsDict, settings)
+                self._selected_plotter.plot(self._hs_culled, settings)
+                transparent = self._selected_plotter.transparent(
+                    settings["burst_color_bg_trnsp"]
                 )
+            else:
+                transparent = False
 
-            matplotlib.pyplot.show()
+            buf = io.BytesIO()
+            matplotlib.pyplot.savefig(
+                buf,
+                bbox_inches="tight",
+                format=settings["img_type"],
+                transparent=transparent,
+            )
+            img_name = "-".join(label for label, _, _ in self._hs)
+            img = Image(img_name, settings["img_type"], buf.getvalue())
+            display(HTML(f"{self._csv_download_link} | {img.download_link()}"))
+            display(img)
+            matplotlib.pyplot.clf()
+            matplotlib.pyplot.close()
 
     @beartype
     def update_hs(
         self,
         histogram_specs: Iterable[
             Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
         ],
@@ -1603,19 +1709,21 @@
     *,
     controls_expanded: bool = True,
     initial_alpha: float = DEFAULT_ALPHA,
     initial_burst_cmap_inner: str = DEFAULT_CMAP_BURST_INNER,
     initial_burst_cmap_link: bool = True,
     initial_burst_cmap_outer: str = DEFAULT_CMAP_BURST_OUTER,
     initial_burst_color_bg: str = "white",
+    initial_burst_color_bg_trnsp: bool = False,
     initial_burst_color_text: str = DEFAULT_COLOR_TEXT,
     initial_burst_swap: bool = False,
     initial_burst_zero_fill_normalize: bool = False,
     initial_enable_cutoff: bool = False,
     initial_graph_type: TraditionalPlotType = TraditionalPlotType.NORMAL,
+    initial_img_type: ImageType = ImageType.PNG,
     initial_markers: str = "oX^v><dP",
     initial_plot_style: str = "bmh",
     initial_show_shadow: bool = False,
     selected_name: Optional[str] = None,
 ):
     r"""
     !!! warning "Experimental"
@@ -1646,31 +1754,33 @@
         histogram_specs,
         plot_widgets=PlotWidgets(
             initial_alpha=initial_alpha,
             initial_burst_cmap_inner=initial_burst_cmap_inner,
             initial_burst_cmap_link=initial_burst_cmap_link,
             initial_burst_cmap_outer=initial_burst_cmap_outer,
             initial_burst_color_bg=initial_burst_color_bg,
+            initial_burst_color_bg_trnsp=initial_burst_color_bg_trnsp,
             initial_burst_color_text=initial_burst_color_text,
             initial_burst_swap=initial_burst_swap,
             initial_burst_zero_fill_normalize=initial_burst_zero_fill_normalize,
             initial_enable_cutoff=initial_enable_cutoff,
             initial_graph_type=initial_graph_type,
+            initial_img_type=initial_img_type,
             initial_markers=initial_markers,
             initial_plot_style=initial_plot_style,
             initial_show_shadow=initial_show_shadow,
         ),
         selected_name=selected_name,
     )
 
     plotter_chooser.interact()
 
 
 @beartype
-def _csv_download_link(hs: Sequence[Tuple[str, H, Optional[H]]]) -> HTML:
+def _csv_download_link(hs: Sequence[Tuple[str, H, Optional[H]]]) -> str:
     unique_outcomes = sorted(set(chain.from_iterable(h.outcomes() for _, h, _ in hs)))
     labels = [label for label, _, _ in hs]
     raw_buffer = io.BytesIO()
     csv_buffer = io.TextIOWrapper(
         raw_buffer, encoding="utf-8", newline="", write_through=True
     )
     csv_writer = csv.DictWriter(csv_buffer, fieldnames=["Outcome"] + labels)
@@ -1678,25 +1788,19 @@
 
     for outcome in unique_outcomes:
         row = {"Outcome": outcome}
         row.update({label: h[outcome] / h.total for label, h, _ in hs if outcome in h})
         csv_writer.writerow(row)
 
     # Inspiration: <https://medium.com/@charles2588/how-to-upload-download-files-to-from-notebook-in-my-local-machine-6a4e65a15767>
-    csv_name = ", ".join(labels)
+    csv_name = "-".join(labels)
     csv_name = csv_name if len(labels) <= 32 else (csv_name[:29] + "...")
     payload = base64.standard_b64encode(raw_buffer.getvalue()).decode()
 
-    return HTML(
-        f"""
-<a download="{csv_name}.csv" href="data:text/csv;base64,{payload}" target="_blank">
-Download raw data as CSV
-</a>
-"""
-    )
+    return f'<a download="{csv_name}.csv" href="data:text/csv;base64,{payload}" target="_blank">Download raw data as CSV</a>'
 
 
 @beartype
 def _histogram_specs_to_h_tuples(
     histogram_specs: Iterable[
         Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
     ],
```

## Comparing `anydyce-0.4.0.dist-info/LICENSE` & `anydyce-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anydyce-0.4.0.dist-info/METADATA` & `anydyce-0.4.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydyce
-Version: 0.4.0
+Version: 0.4.1
 Summary: Visualization tools for dyce
 Home-page: https://posita.github.io/anydyce/
 Author: Matt Bogosian
 Author-email: matt@bogosian.net
 License: MIT License
 Project-URL: Source Repository, https://github.com/posita/anydyce/
 Classifier: Topic :: Education
@@ -51,19 +51,19 @@
 
 *Copyright and other protections apply.
 Please see the accompanying ``LICENSE`` file for rights and restrictions governing use of this software.
 All rights not expressly waived or licensed are reserved.
 If that file is missing or appears to be modified from its original, then please contact the author before viewing or using this software in any capacity.*
 
 [![Tests](https://github.com/posita/anydyce/actions/workflows/on-push.yaml/badge.svg)](https://github.com/posita/anydyce/actions/workflows/on-push.yaml)
-[![Version](https://img.shields.io/pypi/v/anydyce/0.4.0.svg)](https://pypi.org/project/anydyce/0.4.0/)
-[![Development Stage](https://img.shields.io/pypi/status/anydyce/0.4.0.svg)](https://pypi.org/project/anydyce/0.4.0/)
-[![License](https://img.shields.io/pypi/l/anydyce/0.4.0.svg)](http://opensource.org/licenses/MIT)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/anydyce/0.4.0.svg)](https://pypi.org/project/anydyce/0.4.0/)
-[![Supported Python Implementations](https://img.shields.io/pypi/implementation/anydyce/0.4.0.svg)](https://pypi.org/project/anydyce/0.4.0/)
+[![Version](https://img.shields.io/pypi/v/anydyce/0.4.1.svg)](https://pypi.org/project/anydyce/0.4.1/)
+[![Development Stage](https://img.shields.io/pypi/status/anydyce/0.4.1.svg)](https://pypi.org/project/anydyce/0.4.1/)
+[![License](https://img.shields.io/pypi/l/anydyce/0.4.1.svg)](http://opensource.org/licenses/MIT)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/anydyce/0.4.1.svg)](https://pypi.org/project/anydyce/0.4.1/)
+[![Supported Python Implementations](https://img.shields.io/pypi/implementation/anydyce/0.4.1.svg)](https://pypi.org/project/anydyce/0.4.1/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![``dyce``-powered!](https://raw.githubusercontent.com/posita/dyce/latest/docs/dyce-powered.svg)](https://posita.github.io/dyce/)
 [![``numerary``-encumbered](https://raw.githubusercontent.com/posita/numerary/latest/docs/numerary-encumbered.svg)](https://posita.github.io/numerary/)
 [![Bear-ified™](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.rtfd.io/)
 
 # ``anydyce`` – visualization tools for [``dyce``](https://posita.github.io/dyce/)
 
@@ -112,15 +112,15 @@
     Notebooks can also be downloaded and shared as ``.ipynb`` files.
 
 ### Interactive quick start
 
 Probably the _easiest_ way to start tinkering with ``anydyce`` is with [JupyterLite](https://jupyterlite.readthedocs.io/):
 [![Try dyce](https://jupyterlite.readthedocs.io/en/latest/_static/badge.svg)](https://posita.github.io/anydyce/0.4/jupyter/lab/?path=anydyce_intro.ipynb)
 
-The [``quickstart-local.sh`` script](https://github.com/posita/anydyce/blob/v0.4.0/quickstart-local.sh) will create a local [virtual environment](https://docs.python.org/3/library/venv.html) to bootstrap a local Jupyter server with ``anydyce`` installed and open a web browser to the [introduction notebook](https://github.com/posita/anydyce/blob/v0.4.0/docs/notebooks/anydyce_intro-ipynb).
+The [``quickstart-local.sh`` script](https://github.com/posita/anydyce/blob/v0.4.1/quickstart-local.sh) will create a local [virtual environment](https://docs.python.org/3/library/venv.html) to bootstrap a local Jupyter server with ``anydyce`` installed and open a web browser to the [introduction notebook](https://github.com/posita/anydyce/blob/v0.4.1/docs/notebooks/anydyce_intro-ipynb).
 
 [Binder](https://mybinder.org/) is another great resource that you can use to share notebooks from your Git repositories (including [Gists](https://gist.github.com/)):
 [![Try dyce](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/posita/anydyce/HEAD?labpath=docs%2Fnotebooks%2Fanydyce_intro.ipynb)
 
 !!! danger "JupyterLite and Binder may not save your work!"
 
     JupyterLite attempts to make use of your browser’s local storage for saving notebook changes.
@@ -160,20 +160,20 @@
 >>> plot_burst(ax, 2@H(6))
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_1_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: Basic plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_1_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_1_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_1_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: Basic plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_1_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_1_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_1.py"><code>plot_burst_1.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_1.py"><code>plot_burst_1.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_1.py"
 ```
 </details>
 
 The outer ring can also be used to compare two histograms directly.
@@ -193,20 +193,20 @@
 ... )
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_2_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: 2d6 vs. 4dF plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_2_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_2_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_2_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: 2d6 vs. 4dF plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_2_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_2_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_2.py"><code>plot_burst_2.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_2.py"><code>plot_burst_2.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_2.py"
 ```
 </details>
 
 Labels can even be overridden for interesting, at-a-glance displays.
@@ -232,20 +232,20 @@
 ... }), inner_cmap="RdYlBu_r", outer_formatter=d20formatter)
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_3_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: Advanced plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_3_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_3_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_3_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: Advanced plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_3_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_3_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.0/docs/assets/plot_burst_3.py"><code>plot_burst_3.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.1/docs/assets/plot_burst_3.py"><code>plot_burst_3.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_3.py"
 ```
 </details>
 
 ### Requirements
```

## Comparing `anydyce-0.4.0.dist-info/RECORD` & `anydyce-0.4.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 anydyce/__init__.py,sha256=PdvwQvTYEPurA7Jw9D8Igzg5kJrdzrTPLBd9auZ-fFs,1049
-anydyce/_version.py,sha256=pKZrBWLg9JpiEeQf6dMBubeGmux88mkk46QAcA5SK-I,48
+anydyce/_version.py,sha256=GO1phFiWTn_hFn1R3eyJjs4M9itmF1X6FmfWknT-E68,48
 anydyce/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-anydyce/viz.py,sha256=qzcVmZTV1OkMfKu1Rgl3luKvSNpHwhBSi9FwD6Vf0so,55368
-anydyce-0.4.0.dist-info/LICENSE,sha256=6WaQmeuKAR5YS6y5aX0B9aj94xteomlJ_xjuW8rc6Uo,2118
-anydyce-0.4.0.dist-info/METADATA,sha256=PRhXnaOqNxvyI2FCHnrDjGP71fxXP4J1LpJF01SqTXQ,15580
-anydyce-0.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-anydyce-0.4.0.dist-info/top_level.txt,sha256=DiuY4cmvZIdl2Tc2SI-fYfLfRr_gkQP529FQPLng2LM,8
-anydyce-0.4.0.dist-info/RECORD,,
+anydyce/viz.py,sha256=ds_7ilGVaWw9eO6UKlNPKv7i8J68TD7Pcr94jWmAwfE,58977
+anydyce-0.4.1.dist-info/LICENSE,sha256=6WaQmeuKAR5YS6y5aX0B9aj94xteomlJ_xjuW8rc6Uo,2118
+anydyce-0.4.1.dist-info/METADATA,sha256=fsOKFfcZWK-WRPc7aaxESYSLDW_5dHiJt3_Qm07rCwY,15580
+anydyce-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+anydyce-0.4.1.dist-info/top_level.txt,sha256=DiuY4cmvZIdl2Tc2SI-fYfLfRr_gkQP529FQPLng2LM,8
+anydyce-0.4.1.dist-info/RECORD,,
```

