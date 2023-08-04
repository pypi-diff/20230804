# Comparing `tmp/pyjt-0.3.1.tar.gz` & `tmp/pyjt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.3.1.tar", last modified: Thu Aug  3 16:42:28 2023, max compression
+gzip compressed data, was "pyjt-0.4.0.tar", last modified: Fri Aug  4 08:55:48 2023, max compression
```

## Comparing `pyjt-0.3.1.tar` & `pyjt-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:42:28.684167 pyjt-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 16:41:47.000000 pyjt-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-03 16:42:28.684167 pyjt-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-03 16:41:47.000000 pyjt-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:42:28.684167 pyjt-0.3.1/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:42:28.684167 pyjt-0.3.1/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:42:28.684167 pyjt-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:42:28.684167 pyjt-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 16:41:47.000000 pyjt-0.3.1/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 16:41:47.000000 pyjt-0.3.1/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-03 16:41:47.000000 pyjt-0.3.1/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:55:48.321832 pyjt-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 08:55:16.000000 pyjt-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-04 08:55:48.321832 pyjt-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-04 08:55:16.000000 pyjt-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:55:48.317832 pyjt-0.4.0/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:55:48.317832 pyjt-0.4.0/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-04 08:55:48.000000 pyjt-0.4.0/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-04 08:55:48.000000 pyjt-0.4.0/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:55:48.000000 pyjt-0.4.0/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 08:55:48.000000 pyjt-0.4.0/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 08:55:48.000000 pyjt-0.4.0/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 08:55:16.000000 pyjt-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:55:48.321832 pyjt-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:55:48.317832 pyjt-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 08:55:16.000000 pyjt-0.4.0/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 08:55:16.000000 pyjt-0.4.0/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-04 08:55:16.000000 pyjt-0.4.0/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 08:55:16.000000 pyjt-0.4.0/tests/test_textfield.py
```

### Comparing `pyjt-0.3.1/LICENSE` & `pyjt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.3.1/PKG-INFO` & `pyjt-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.3.1
+Version: 0.4.0
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjt-0.3.1/README.md` & `pyjt-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjt-0.3.1/pyjt/ComponentFinder.py` & `pyjt-0.4.0/pyjt/ComponentFinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
 
 @staticmethod
 def _matches(cmpt, **kwargs):
     # log.debug(f"_matches({cmpt}, name={name}, text={text})")
     for name, value in kwargs.items():
         if name == 'role':
-            cc = cmpt.instance if isinstance(cmpt, Proxy) else cmpt
+            cc = cmpt.object if isinstance(cmpt, Proxy) else cmpt
             log.debug(f"\tcheck01 {name} {type(cc)}={value}")
             check = isinstance(cc, value)
             log.debug(f"\t\tcheck01: {check}")
             if not check:
                 return False
             continue
         fname = f"get{name[0].capitalize()}{name[1:]}"
```

### Comparing `pyjt-0.3.1/pyjt/Fixture.py` & `pyjt-0.4.0/pyjt/Fixture.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,30 +16,53 @@
         self._control = control
         self.robot = Robot()
 
     def locate(self, locator=None, **kwargs):
         """ Search a control as a sub-element of the control
             managed by this fixture.
 
-            Parameters
-            ----------
+            Args:
+                locator (Locator):  A locator object to find the sub-control
+                **kwargs:           Additional search parameters.
 
-            locator:    Locator
-                A locator object to find the sub-control
-            **kwargs:
-                Additional search parameters.
+            Returns:
+                Fixture:
+                    A fixture pointing to the first component
+                    matching the search criteria.
+
+            Raises:
+                ElementNotFoundError:
+                    No element was found matching the search criteria
         """
         log.debug(f"frame.find({locator}, {kwargs})")
         locator = locator if locator else Locator(**kwargs)
         control = ComponentFinder.findIn(self._control.getComponents, locator)
         if not control:
             raise ElementNotFoundError(f"Control({kwargs}) not found!")
         return Fixture(control)
 
     def find(self, role, **kwargs):
+        """ Search a control of type **role** as a sub-control of this control.
+
+            Args:
+                role (Class):
+                    The class type of the component to look for, e.g.
+                    javax.swing.JTextField
+                **kwargs:
+                    Search criteria for the component.
+
+            Returns:
+                Fixture:
+                    A fixture pointing to the first component
+                    matching the search criteria.
+
+            Raises:
+                ElementNotFoundError:
+                    No element was found matching the search criteria
+        """
         kwargs['role'] = role
         return self.locate(**kwargs)
 
     def click(self):
         """ Move the mouse over this control and execute a click. """
         log.debug(f"click({self._control})")
         self.robot.move(self._control)
@@ -73,12 +96,19 @@
             self.click()
             if clear:
                 self.robot.selectAll()
             self.robot.type(text)
         if mode == FillMode.SET:
             self._control.setText(text)
 
+    @property
+    def control(self):
+        """ Returns:
+                Proxy:  A reference to the control managed by this fixture.
+        """
+        return self._control
+
     def __getattr__(self, name):
         return getattr(self._control, name)
 
     def __repr__(self):
         return str(self._control)
```

### Comparing `pyjt-0.3.1/pyjt/Frame.py` & `pyjt-0.4.0/pyjt/Frame.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,55 +8,55 @@
 from pyjt.Inspector import Inspector
 from pyjt import Proxy
 
 log = logging.getLogger(__name__)
 
 
 class FrameFinder:
-    """ Helper class to find a frame in the list of application frames.
+    """ Find a frame in the list of application frames.
+
+        Example:
+
+        .. code:: python
+
+            frame = FrameFinder(title="Hello World")
+            frame.find(JTextField, name="first name")
     """
     @staticmethod
     def find(locator=None, **kwargs):
         """Find a frame by a locator or frame attributes.
 
-        Parameters
-        ----------
-        locator : Locator
-            Locator to find a frame.
-        **kwargs :
-            Search filters by keyword arguments.
-
-        Raises
-        ------
-
-        ElementNotFoundError
-            If the no frame was found matching the given search criteria.
-
-        Returns
-        -------
-        Frame
-            A Frame instance reflecting the frame window found by the find
-            operation.
+            Args:
+                locator (Locator):  Locator to find a frame.
+                **kwargs:           Search filters by keyword arguments.
+
+            Raises:
+                ElementNotFoundError:
+                         No frame was found matching the given search criteria.
+
+            Returns:
+                Frame:
+                    The first frame in the list of frames matching
+                    the search criteria.
         """
         from java.awt import Window
         locator = locator if locator else Locator(**kwargs)
         wp = Proxy(Window)
         for window in wp.getWindows():
             if locator.matches(window):
                 return Frame(window)
         raise ElementNotFoundError(f"Window {locator} not found!")
 
     @staticmethod
     def inspect():
-        """ Inspect a component
-
-            Returns
-            -------
+        """ Inspect a component.
 
-            dict    A dicitionary tree of all ui components of all available
+            Returns:
+                dict:
+                    A dicitionary tree of all ui components of all available
                     frames.
         """
         from java.awt import Window
         wp = Proxy(Window)
         result = []
         for window in wp.getWindows():
             result.append(Inspector.inspect(window))
@@ -68,8 +68,8 @@
     def dispose(self):
         """ Dispose this frame. """
         self._control.dispose()
 
     def close(self):
         """ Close this frame by sending a close message. """
         from java.awt.event import WindowEvent
-        self._control.instance.dispatchEvent(WindowEvent(self._component.instance, WindowEvent.WINDOW_CLOSING))
+        self._control.object.dispatchEvent(WindowEvent(self._component.instance, WindowEvent.WINDOW_CLOSING))
```

### Comparing `pyjt-0.3.1/pyjt/Inspector.py` & `pyjt-0.4.0/pyjt/Inspector.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,24 @@
 
 
 class Inspector:
     """ Helper class for inspecting the component tree of a specific component.
     """
     @staticmethod
     def inspect(component):
-        """ Inspects the component tree of a component and returns a dictionary
-            with test-relevant data.
+        """ Inspects the component tree of a component.
+
+            Args:
+                component (Fixture):
+                    The component to inspect.
+
+            Returns:
+                dict:
+                    A dictionary with information of all sub-components
+                    for this component.
         """
         result = {}
         result['name'] = str(component.getName())
         result['class'] = str(component.getClass())
         result['text'] = _getText(component)
         title = _getTitle(component)
         if title:
```

### Comparing `pyjt-0.3.1/pyjt/Robot.py` & `pyjt-0.4.0/pyjt/Robot.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 from pyjt import Proxy
 
 log = logging.getLogger(__name__)
 
 
 class Robot:
-    """ Smart robot features for controlling the application. """
+    """ Smart robot features for controlling the application.
+
+        Args:
+            robot (java.awt.Robot):
+                Use the given java.awt.Robot() object
+                If **robot** is None, create a own instance of the robot class.
+            typespeed (int):
+                The speed to type text in number of keystrokes per second.
+    """
     _robot = None
 
     def __init__(self, robot=None, typespeed=20):
-        """ Create a new robot class.
-
-        :param robot:       Use the given java.awt.Robot() instance for
-                            this instance. If **robot** is None,
-                            create a own instance of the robot class.
-
-        :param typespeed:   The speed to type text in number of keystrokes per second.
-        """
         import java
         from java.awt.event import KeyEvent
 
         self._robot = Proxy(robot) if robot else Robot._robot
         if not self._robot:
             Robot._robot = Proxy(java.awt.Robot())
             self._robot = Robot._robot
@@ -145,29 +145,30 @@
         self._robot.mousePress(btn)
         log.debug(f"sleeping for {1 / self._typespeed}")
         time.sleep(1 / self._typespeed)
         log.debug("mouseup")
         self._robot.mouseRelease(btn)
 
     def selectAll(self):
+        """ Emulate selecting all text in the current context by pressing CTRL-A. """
         from java.awt.event import KeyEvent
         self._typeVKs([KeyEvent.VK_CONTROL, KeyEvent.VK_A])
 
     def type(self, text):
         """ Emulate user typing the given text.
 
-            :param text:    Text to type.
-
             Typing is emulated by generating VK_* events. The type speed
             (delay between each keystroke) is configured in the
             Robot's constructor's `typespeed` argument.
 
-            Limitations:
+            Args:
+                text (string):    Text to type.
 
-            -   Currently, this function assumes that a english keyboard layout
+            Note:
+                Currently, this function assumes that a english keyboard layout
                 is used.
         """
         for char in text:
             if char not in self._KeyCodes:
                 raise Exception("Unknown character to type: '{char}'")
             self._typeVKs(self._KeyCodes[char])
```

### Comparing `pyjt-0.3.1/pyjt/__init__.py` & `pyjt-0.4.0/pyjt/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,12 +39,14 @@
     module.main(args)
 
 def shutdown():
     """ Shuts down pyjt and the JVM. """
     jpype.shutdownJVM()
 
 from .Proxy import Proxy
+from .Robot import Robot
 from .Frame import Frame, FrameFinder
 from .Fixture import Fixture, FillMode
 from .Errors import ElementNotFoundError
 from .ComponentFinder import Locator
 from .Inspector import Inspector
+from .Errors import ElementNotFoundError
```

### Comparing `pyjt-0.3.1/pyjt.egg-info/PKG-INFO` & `pyjt-0.4.0/pyjt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.3.1
+Version: 0.4.0
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjt-0.3.1/tests/test_locator.py` & `pyjt-0.4.0/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.3.1/tests/test_textfield.py` & `pyjt-0.4.0/tests/test_textfield.py`

 * *Files identical despite different names*

