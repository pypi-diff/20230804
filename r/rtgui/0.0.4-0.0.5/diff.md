# Comparing `tmp/rtgui-0.0.4.tar.gz` & `tmp/rtgui-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtgui-0.0.4.tar", last modified: Wed Jul 19 21:57:42 2023, max compression
+gzip compressed data, was "rtgui-0.0.5.tar", last modified: Fri Aug  4 19:13:25 2023, max compression
```

## Comparing `rtgui-0.0.4.tar` & `rtgui-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 antonioprado   (504) staff       (20)        0 2023-07-19 21:57:42.284790 rtgui-0.0.4/
--rw-r--r--   0 antonioprado   (504) staff       (20)     1070 2023-07-06 21:19:44.000000 rtgui-0.0.4/LICENSE
--rw-r--r--   0 antonioprado   (504) staff       (20)      488 2023-07-19 21:57:42.284477 rtgui-0.0.4/PKG-INFO
--rw-r--r--   0 antonioprado   (504) staff       (20)      443 2023-07-11 18:08:08.000000 rtgui-0.0.4/README.md
-drwxr-xr-x   0 antonioprado   (504) staff       (20)        0 2023-07-19 21:57:42.280645 rtgui-0.0.4/rtgui/
--rw-r--r--   0 antonioprado   (504) staff       (20)    37471 2023-07-19 21:54:01.000000 rtgui-0.0.4/rtgui/__init__.py
-drwxr-xr-x   0 antonioprado   (504) staff       (20)        0 2023-07-19 21:57:42.284022 rtgui-0.0.4/rtgui.egg-info/
--rw-r--r--   0 antonioprado   (504) staff       (20)      488 2023-07-19 21:57:42.000000 rtgui-0.0.4/rtgui.egg-info/PKG-INFO
--rw-r--r--   0 antonioprado   (504) staff       (20)      188 2023-07-19 21:57:42.000000 rtgui-0.0.4/rtgui.egg-info/SOURCES.txt
--rw-r--r--   0 antonioprado   (504) staff       (20)        1 2023-07-19 21:57:42.000000 rtgui-0.0.4/rtgui.egg-info/dependency_links.txt
--rw-r--r--   0 antonioprado   (504) staff       (20)       30 2023-07-19 21:57:42.000000 rtgui-0.0.4/rtgui.egg-info/requires.txt
--rw-r--r--   0 antonioprado   (504) staff       (20)        6 2023-07-19 21:57:42.000000 rtgui-0.0.4/rtgui.egg-info/top_level.txt
--rw-r--r--   0 antonioprado   (504) staff       (20)       38 2023-07-19 21:57:42.284884 rtgui-0.0.4/setup.cfg
--rw-r--r--   0 antonioprado   (504) staff       (20)     1188 2023-07-19 21:54:57.000000 rtgui-0.0.4/setup.py
+drwxr-xr-x   0 antonioprado   (504) staff       (20)        0 2023-08-04 19:13:25.158188 rtgui-0.0.5/
+-rw-r--r--   0 antonioprado   (504) staff       (20)     1070 2023-07-06 21:19:44.000000 rtgui-0.0.5/LICENSE
+-rw-r--r--   0 antonioprado   (504) staff       (20)      488 2023-08-04 19:13:25.157718 rtgui-0.0.5/PKG-INFO
+-rw-r--r--   0 antonioprado   (504) staff       (20)      443 2023-07-11 18:08:08.000000 rtgui-0.0.5/README.md
+drwxr-xr-x   0 antonioprado   (504) staff       (20)        0 2023-08-04 19:13:25.151864 rtgui-0.0.5/rtgui/
+-rw-r--r--   0 antonioprado   (504) staff       (20)    38604 2023-08-04 18:55:09.000000 rtgui-0.0.5/rtgui/__init__.py
+drwxr-xr-x   0 antonioprado   (504) staff       (20)        0 2023-08-04 19:13:25.156888 rtgui-0.0.5/rtgui/communication/
+-rw-r--r--   0 antonioprado   (504) staff       (20)     6023 2023-08-02 21:55:52.000000 rtgui-0.0.5/rtgui/communication/__init__.py
+drwxr-xr-x   0 antonioprado   (504) staff       (20)        0 2023-08-04 19:13:25.156406 rtgui-0.0.5/rtgui.egg-info/
+-rw-r--r--   0 antonioprado   (504) staff       (20)      488 2023-08-04 19:13:25.000000 rtgui-0.0.5/rtgui.egg-info/PKG-INFO
+-rw-r--r--   0 antonioprado   (504) staff       (20)      220 2023-08-04 19:13:25.000000 rtgui-0.0.5/rtgui.egg-info/SOURCES.txt
+-rw-r--r--   0 antonioprado   (504) staff       (20)        1 2023-08-04 19:13:25.000000 rtgui-0.0.5/rtgui.egg-info/dependency_links.txt
+-rw-r--r--   0 antonioprado   (504) staff       (20)       39 2023-08-04 19:13:25.000000 rtgui-0.0.5/rtgui.egg-info/requires.txt
+-rw-r--r--   0 antonioprado   (504) staff       (20)        6 2023-08-04 19:13:25.000000 rtgui-0.0.5/rtgui.egg-info/top_level.txt
+-rw-r--r--   0 antonioprado   (504) staff       (20)       38 2023-08-04 19:13:25.158306 rtgui-0.0.5/setup.cfg
+-rw-r--r--   0 antonioprado   (504) staff       (20)     1188 2023-08-04 19:11:33.000000 rtgui-0.0.5/setup.py
```

### Comparing `rtgui-0.0.4/LICENSE` & `rtgui-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rtgui-0.0.4/rtgui/__init__.py` & `rtgui-0.0.5/rtgui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         # self.ax = ax
         if len(color) != len(names):
             color = [color[0]] * len(names)
         if defaultVal is None:
             dV = [0] * len(names)
         else:
             if len(defaultVal) is not len(names):
-                if len(defaultVal) is 1:
+                if len(defaultVal) == 1:
                     dV = defaultVal * len(names)
                 else:
                     warnings.warn('Default values should be 1 or equal to the number of names')
                     dV = defaultVal + [''] * (len(names) - len(defaultVal))
             else:
                 dV = defaultVal
         if len(color) is not len(names):
@@ -92,18 +92,18 @@
         :type parseCMD: function
         """
         super(ConsoleFrame, self).__init__(parent, **kwargs)
         self.parseCMD = parseCMD
         self.nLines = nLines
         self.consoleVar = tk.StringVar()
         self.consoleList = []
-        tk.Label(self, text='Console').pack(fill=tk.BOTH)
+        tk.Label(self, text='Console').pack(side=tk.TOP)
         self.console = tk.Message(self, textvariable=self.consoleVar, relief=tk.SUNKEN)
-        self.console.pack()
-        tk.Button(self, text='Clear', command=self.clearConsole).pack()
+        self.console.pack(expand=tk.YES, side=tk.TOP)
+        tk.Button(self, text='Clear', command=self.clearConsole).pack(expand=tk.YES, side=tk.TOP)
 
     def __append2console(self, text):
         self.consoleList.append(text)
         if len(self.consoleList) >= self.nLines:
             self.consoleList.pop(0)
         console = ''
         for t in self.consoleList:
@@ -133,15 +133,15 @@
 
 
 class PlotPanel(tk.Frame):
     def __init__(self, parent, title, titles, names, plotColor, timestamp, allValsList, color=None, number2Plot=500,
                  shareAxis=None, showTime=False, useScale=True, figsize=(5, 2), useCheckFn=False, **kwargs):
         """
         This widget has checkboxes with variables and a matplot figure the label goes to the left
-        :param parent: parent frome
+        :param parent: parent frame
         :type parent: tk.Frame
         :param title: Title of the widget
         :type title: str
         :param titles: List with title of each of the checkbox control widget
         :type titles: list
         :param names: A list of list containing the name of each signal to plot
         :type names: list
@@ -212,39 +212,43 @@
         self.canvas.get_tk_widget().pack(side=tk.LEFT, fill=tk.BOTH, expand=True)
         # self.canvas.get_tk_widget().grid(row=0,column=2)
         self.toolbar = NavigationToolbar2Tk(self.canvas, self)
         self.toolbar.update()
         # self.canvas._tkcanvas.grid()
         self.canvas._tkcanvas.pack(side=tk.BOTTOM, fill=tk.BOTH, expand=True)
 
-    def plotControlFromChecks(self):
+    def plotControlFromChecks(self, t_in_ms=False):
         """
         This function plots all the values that have an active checkbox
         """
         #
         self.axis.clear()
         useScale = self.useScale
         s = self.s
         i = 0
         if self.showTime:
+            if t_in_ms:
+                ms_scale = 1000.0
+            else:
+                ms_scale = 1.0
             if type(self.timestamp[0]) is list:
-                t = self.timestamp[0][-1] / 1000.0
+                t = self.timestamp[0][-1] / ms_scale
             else:
-                t = self.timestamp[-1] / 1000.0
+                t = self.timestamp[-1] / ms_scale
             self.consoleVar.set(self.title + '\n %.1fs' % t)
         for ch, col in zip(self.checks, self.plotColor):
             vals = ch.getAllValues()
             for v, c1 in zip(vals, col):
                 if v == 1:
                     if type(self.timestamp[0]) is list:
 
-                        t = np.array(self.timestamp[i][-s:]) / 1000.0
+                        t = np.array(self.timestamp[i][-s:]) / ms_scale
                         # print(t.shape)
                     else:
-                        t = np.array(self.timestamp[-s:]) / 1000.0
+                        t = np.array(self.timestamp[-s:]) / ms_scale
                     y = np.array(self.all[i])
                     if y.size > t.size:
                         y = y[:t.size]
                     if y.size < t.size:
                         t = t[:y.size]
                     # divAux = FACTOR
                     # ymin = SCALE_MIN
@@ -262,33 +266,37 @@
                     except ValueError:
                         a = 1
                 i = i + 1
         if useScale:
             self.axis.set_ylim(-0.1, 1.1)
         self.canvas.draw()
 
-    def plotControlFromChecksTime(self, tV, extraT=2):
+    def plotControlFromChecksTime(self, tV, extraT=2, t_in_ms=False):
         """
         This function plots all the values that have an active checkbox and display the timestamp
         :param tV: time to show in seconds
         :type tV: float
         :param extraT: extra time (empty) to show for visualization
         :type float
         """
         if len(self.all[0]) < 2:
             return
         useScale = self.useScale
         self.axis.clear()
         i = 0
         if self.showTime:
+            if t_in_ms:
+                ms_scale = 1000.0
+            else:
+                ms_scale = 1.0
             if type(self.timestamp[0]) is list:
-                t = self.timestamp[0][-1] / 1000.0
+                t = self.timestamp[0][-1] / ms_scale
                 # print(t.shape)
             else:
-                t = self.timestamp[-1] / 1000.0
+                t = self.timestamp[-1] / ms_scale
             self.consoleVar.set(self.title + '\n %.1fs' % t)
         # t = np.array(t1) / 1000
         for ch, col in zip(self.checks, self.plotColor):
             vals = ch.getAllValues()
             for v, c1 in zip(vals, col):
                 if v == 1:
                     # plot that var
@@ -389,66 +397,85 @@
         :type multiplier: int
         :param timerFrame: timerFrame to use to display the time
         :type timerFrame: PlotPanelTimer
         """
         super(PlotPanelPandas, self).__init__(parent, title, titles, names, plotColor, timestamp, allValsPandas,
                                               color=color, number2Plot=number2Plot, shareAxis=shareAxis,
                                               showTime=showTime, useScale=useScale, **kwargs)
-        self.button = ButtonPanel(self, [['Reset Scale']], [[self.resetScale]])
-        self.button.pack()
+        scale_frame = tk.Frame(self)
+        scale_frame.pack(fill=tk.BOTH, expand=tk.YES)
+        # self.button = ButtonPanel(scale_frame, [['Reset Scale']], [[self.resetScale]])
+        self.button = tk.Button(scale_frame, text='Reset Scale', command=self.resetScale)
+        self.button.pack(side=tk.LEFT, fill=tk.BOTH)
+        self._check_normal = CheckControl(scale_frame, "", ['Normalize'], self._normalize_option, color=['white'],
+                                          defaultVal=[useScale])
+        self._check_normal.pack(side=tk.LEFT)
         self.maxValsAux = None
         self.minValsAux = None
         self.dt = 0
         self.multiplier = multiplier
         self.counter = multiplier
         self.timerFrame = timerFrame
+        self._normalize_option()
+
+    def _normalize_option(self):
+        self.useScale = self._check_normal.getAllValues()[0]
+        if self.useScale:
+            self.button.configure(state='normal')
+        else:
+            self.button.configure(state='disabled')
+
 
     def plotControlFromChecks(self):
         warnings.warn('Please do not use this funciton with plotPanelPandas')
 
     def resetScale(self):
         """
         Resets the scale of the plot
         """
         self.maxValsAux = None
 
-    def plotControlFromChecksTime(self, tV, extraT=2.0, preprocess=None):
+    def plotControlFromChecksTime(self, tV, extraT=2.0, preprocess=None, t_in_ms=False):
         """
         This function plots all the values that have an active checkbox and display the timestamp
         :param tV: time to show in seconds
         :type tV: float
         :param extraT: extra time (empty) to show for visualization
         :type float
         :param preprocess: Function to use to preprocess the signals
         :type preprocess: function
         """
         # this function will plot all the values from all
-        if self.all.shape[0] is 0:
+        if self.all.shape[0] == 0:
             return
         if self.counter != 0:
             self.counter -= 1
             return
         # print(self.counter)
         self.counter = self.multiplier
         # i = 0
 
         # def _plotThread(self, tV, extraT, preprocess):
-        dt = 1000.0 / np.diff(self.all.index.values).mean()
+        if t_in_ms:
+            ms_scale = 1000.0
+        else:
+            ms_scale = 1.0
+        dt = ms_scale / np.diff(self.all.index.values).mean()
         if np.isnan(dt):
             return
         self.dt = dt
         if self.showTime:
-            t = self.all.index[-1] / 1000.0
+            t = self.all.index[-1] / ms_scale
             # print(self.all.columns)
             s_val = self.all['sync'].values[-1] == 1
             self.consoleVar.set(self.title + '\n %.1fs\n%.1fHz\n Sync: %d' % (t, dt, s_val))
             if self.timerFrame is not None:
                 self.timerFrame.setNewTime(t)
-        vals = np.array([ch.getAllValues() for ch in self.checks]).flatten()
-        if np.all(vals == 0):
+        vals = [ch.getAllValues() for ch in self.checks]
+        if all(v == 0 for vv in vals for v in vv):
             return
         self.axis.cla()
 
         # I'll plot only the new 500 values
 
         # t = np.array(t1) / 1000
         # timeS = int((self.all.index[-1] - tV * 1000 ) // self.all.index.get_values().mean())
@@ -469,15 +496,15 @@
                 self.minValsAux.loc[windowVals.min() < self.minValsAux] = windowVals.min().loc[
                     windowVals.min() < self.minValsAux]
             divAux = self.maxValsAux - self.minValsAux
             divAux[divAux == 0] = 1
             windowVals = (windowVals - self.minValsAux) / (divAux)
         # print(dt)
         # print(windowVals.shape[0])
-        windowVals.index /= 1000.0
+        windowVals.index /= ms_scale
         for ch, col, colNames in zip(self.checks, self.plotColor, self.names):
             vals = ch.getAllValues()
             for v, c1, na in zip(vals, col, colNames):
                 if na not in windowVals.columns:
                     continue
                 if v == 1:
                     # print(na)
@@ -559,15 +586,15 @@
         i = 0
         # t = np.array(t1) / 1000
         for ch, col in zip(self.checks, self.plotColor):
             vals = ch.getAllValues()
             for v, c1 in zip(vals, col):
                 if v == 1:
                     # Get the values of rotation
-                    if len(self.all[i][0]) is 0:
+                    if len(self.all[i][0]) == 0:
                         self.systs[i].rotateAndPlotSystem(H=self.Hs[i], clearAx=False)
                         continue
                     # self.all is a list of list with [rx, ry, rz]
                     eu = [x[-1] for x in self.all[i]]
                     self.Hs[i][:3, :3] = rot.from_euler(self._rotationOrder, eu, degrees=self._degrees).as_matrix()
                     self.systs[i].rotateAndPlotSystem(H=self.Hs[i], clearAx=False)
 
@@ -648,15 +675,15 @@
         i = 0
         # t = np.array(t1) / 1000
         for ch, col in zip(self.checks, self.plotColor):
             vals = ch.getAllValues()
             for v, c1 in zip(vals, col):
                 if v == 1:
                     # Get the values of rotation
-                    if self.all[i].shape[0] is 0:
+                    if self.all[i].shape[0] == 0:
                         self.systs[i].rotateAndPlotSystem(H=self.Hs[i], clearAx=False)
                         continue
                     eu = self.all.loc[self._angle_column_names].values[-1]
                     self.Hs[i][:3, :3] = rot.from_euler(self._rotationOrder, eu, degrees=self._degrees).as_matrix()
                     self.systs[i].rotateAndPlotSystem(H=self.Hs[i], clearAx=False)
 
                 i = i + 1
@@ -729,17 +756,17 @@
     def changeButtonColor(self, typeE):
         """
         Changes the color of the button
         :param typeE: 3 options:
         Error, Warn, Good
         :type typeE: str
         """
-        if typeE is 'Error':
+        if typeE == 'Error':
             c = 'red'
-        elif typeE is 'Warn':
+        elif typeE == 'Warn':
             c = 'yellow'
         else:
             c = 'green'
         self.exButton.config(bg=c)
 
 
 class ButtonPanel(tk.Frame):
@@ -806,15 +833,15 @@
         # names = ['Freq']
         self.allNames = names
         self._process_function = process_function
         if defaultVals is None:
             dV = [''] * len(names)
         else:
             if len(defaultVals) is not len(names):
-                if len(defaultVals) is 1:
+                if len(defaultVals) == 1:
                     dV = defaultVals * len(names)
                 else:
                     warnings.warn('Default values should be 1 or equal to the number of names')
                     dV = defaultVals + [''] * (len(names) - len(defaultVals))
             else:
                 dV = defaultVals
         for i, (n, d) in enumerate(zip(names, dV)):
```

### Comparing `rtgui-0.0.4/setup.py` & `rtgui-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return False
 
 
 def requirements_filter(fd):
     return list(filter(filter_lines, fd.read().split('\n')))
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Python package for signal plotting using tk'
 LONG_DESCRIPTION = 'Python package for signal plotting using tk with real time capabilities'
 with open('requirements.txt', 'r') as fd:
     requirements = requirements_filter(fd)
 install_requires = list(requirements)
 # Setting up
 setup(
```

