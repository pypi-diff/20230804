# Comparing `tmp/pyjt-0.3.0.tar.gz` & `tmp/pyjt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.3.0.tar", last modified: Thu Aug  3 08:07:33 2023, max compression
+gzip compressed data, was "pyjt-0.3.1.tar", last modified: Thu Aug  3 16:42:28 2023, max compression
```

## Comparing `pyjt-0.3.0.tar` & `pyjt-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:33.600980 pyjt-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 08:06:43.000000 pyjt-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-03 08:07:33.600980 pyjt-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 08:06:43.000000 pyjt-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:33.596980 pyjt-0.3.0/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:33.600980 pyjt-0.3.0/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:07:33.600980 pyjt-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:33.600980 pyjt-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 08:06:43.000000 pyjt-0.3.0/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-03 08:06:43.000000 pyjt-0.3.0/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-03 08:06:43.000000 pyjt-0.3.0/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:42:28.684167 pyjt-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 16:41:47.000000 pyjt-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-03 16:42:28.684167 pyjt-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-03 16:41:47.000000 pyjt-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:42:28.684167 pyjt-0.3.1/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:42:28.684167 pyjt-0.3.1/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 16:42:28.000000 pyjt-0.3.1/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-03 16:41:47.000000 pyjt-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:42:28.684167 pyjt-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:42:28.684167 pyjt-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 16:41:47.000000 pyjt-0.3.1/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 16:41:47.000000 pyjt-0.3.1/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-03 16:41:47.000000 pyjt-0.3.1/tests/test_textfield.py
```

### Comparing `pyjt-0.3.0/LICENSE` & `pyjt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.3.0/PKG-INFO` & `pyjt-0.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.3.0
+Version: 0.3.1
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
+Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
+Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,14 +27,16 @@
 This library makes use of **jpype** as the interface to the java
 virtual machine. It basicaly consists of helper functions to
 control the application from a test automation perspective.
 
 ## Quickstart
 
     import pyjt
+
+    pyjt.start()
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
     pyjt.start(classpath="myapp/")
     pyjt.run("HelloWorld")
@@ -45,7 +49,10 @@
 
     # Locate and fill text to an text field
     frame.locate(JTextField, name="textfield1").fill("John Smith")
 
     # Close the frame (application)
     frame.close()
 
+## Further documentation
+
+Check the [documentation on rtfd.io](https://pyjt.readthedocs.io/en/latest/)
```

### Comparing `pyjt-0.3.0/README.md` & `pyjt-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 This library makes use of **jpype** as the interface to the java
 virtual machine. It basicaly consists of helper functions to
 control the application from a test automation perspective.
 
 ## Quickstart
 
     import pyjt
+
+    pyjt.start()
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
     pyjt.start(classpath="myapp/")
     pyjt.run("HelloWorld")
@@ -31,7 +33,10 @@
 
     # Locate and fill text to an text field
     frame.locate(JTextField, name="textfield1").fill("John Smith")
 
     # Close the frame (application)
     frame.close()
 
+## Further documentation
+
+Check the [documentation on rtfd.io](https://pyjt.readthedocs.io/en/latest/)
```

### Comparing `pyjt-0.3.0/pyjt/Fixture.py` & `pyjt-0.3.1/pyjt/Fixture.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,56 +6,72 @@
 
 log = logging.getLogger(__name__)
 
 FillMode = Enum('FillMode', ['TYPE', 'SET', 'PASTE'])
 
 
 class Fixture:
+    """ Wrapper class to control a specific UI element.
+    """
     def __init__(self, control):
         self._control = control
         self.robot = Robot()
 
     def locate(self, locator=None, **kwargs):
+        """ Search a control as a sub-element of the control
+            managed by this fixture.
+
+            Parameters
+            ----------
+
+            locator:    Locator
+                A locator object to find the sub-control
+            **kwargs:
+                Additional search parameters.
+        """
         log.debug(f"frame.find({locator}, {kwargs})")
         locator = locator if locator else Locator(**kwargs)
         control = ComponentFinder.findIn(self._control.getComponents, locator)
         if not control:
             raise ElementNotFoundError(f"Control({kwargs}) not found!")
         return Fixture(control)
 
     def find(self, role, **kwargs):
         kwargs['role'] = role
         return self.locate(**kwargs)
 
     def click(self):
+        """ Move the mouse over this control and execute a click. """
         log.debug(f"click({self._control})")
         self.robot.move(self._control)
         log.debug(f"executing click({self._control})")
         self.robot.click()
 
     def fill(self, text, mode=FillMode.TYPE, clear=True):
         """ Fill this control with the given **text**.
 
-            :param text:    Text to fill this control with.
-            :param mode:    Chosse the mode to fill the control with the
-                            given text. See the table below.
-            :param clear:   If set to true, select all text in the given control
-                            before typing.
-
-            ## Fill Modes
-
-            -   FillMode.TYPE
-                -   Fill the control by emulating keystrokes.
-                -   Only supports US keyboard layout at this time.
-            -   FillMode.SET
-                -   Just set the text of the  component using the component.setText() function.
-                -   The existing text is always overwritten ignoring the **clear** argument
-            -   FillMode.PASTE
-                -   Fill the control by pasting the text from the clipboard
-                -   **Not implemented yet**
+            Args:
+                text:   Text to fill this control with.
+                mode:   FillMode - Choose the mode to fill the control with the given text.
+                        See the table below.
+                clear:  If set to True, select all text in the given control
+                        before typing.
+
+            FillMode:
+
+                FillMode.TYPE:
+                  - Fill the control by emulating keystrokes.
+                  - Only supports US keyboard layout at this time.
+                FillMode.SET:
+                  -   Just set the text of the  component using the component.setText() function.
+                  -   The existing text is always overwritten ignoring the **clear** argument
+                FillMode.PASTE:
+                  - Fill the control by pasting the text from the clipboard
+                  - **Not implemented yet**
+
         """
         if mode == FillMode.TYPE:
             self.click()
             if clear:
                 self.robot.selectAll()
             self.robot.type(text)
         if mode == FillMode.SET:
```

### Comparing `pyjt-0.3.0/pyjt/Inspector.py` & `pyjt-0.3.1/pyjt/Inspector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+""" Inspect UI components """
 import logging
 
 log = logging.getLogger(__name__)
 
 
 class Inspector:
+    """ Helper class for inspecting the component tree of a specific component.
+    """
     @staticmethod
     def inspect(component):
         """ Inspects the component tree of a component and returns a dictionary
             with test-relevant data.
         """
         result = {}
         result['name'] = str(component.getName())
```

### Comparing `pyjt-0.3.0/pyjt/Proxy.py` & `pyjt-0.3.1/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.3.0/pyjt/Robot.py` & `pyjt-0.3.1/pyjt/Robot.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.3.0/pyjt/__init__.py` & `pyjt-0.3.1/pyjt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.3.0/pyjt.egg-info/PKG-INFO` & `pyjt-0.3.1/pyjt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.3.0
+Version: 0.3.1
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
+Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
+Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,14 +27,16 @@
 This library makes use of **jpype** as the interface to the java
 virtual machine. It basicaly consists of helper functions to
 control the application from a test automation perspective.
 
 ## Quickstart
 
     import pyjt
+
+    pyjt.start()
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
     pyjt.start(classpath="myapp/")
     pyjt.run("HelloWorld")
@@ -45,7 +49,10 @@
 
     # Locate and fill text to an text field
     frame.locate(JTextField, name="textfield1").fill("John Smith")
 
     # Close the frame (application)
     frame.close()
 
+## Further documentation
+
+Check the [documentation on rtfd.io](https://pyjt.readthedocs.io/en/latest/)
```

### Comparing `pyjt-0.3.0/pyproject.toml` & `pyjt-0.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.3.0"
+version = "0.3.1"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 
@@ -24,7 +24,9 @@
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
 "Homepage" = "https://github.com/realtimeprojects/pyjt"
 "Bug Tracker" = "https://github.com/realtimeprojects/pyjt/issues"
+"Documentation" = "https://pyjt.readthedocs.io/en/latest/"
+"Releases" = "https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md"
```

### Comparing `pyjt-0.3.0/tests/test_locator.py` & `pyjt-0.3.1/tests/test_locator.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,7 +23,11 @@
     tf4 = helloworld.locate(loc)
     logging.warning(tf3)
     assert tf4 is not None
     tf = tf4.find(javax.swing.JTextField)
     assert tf.getText() == "textfield4"
     tf.fill("john@smith.com")
     assert tf.getText() == "john@smith.com"
+
+    loc = Locator(role=java.awt.Container).has(role=javax.swing.JLabel, text="Email:").has(text="john@smith.com")
+    match = helloworld.locate(loc)
+    assert match is not None
```

### Comparing `pyjt-0.3.0/tests/test_textfield.py` & `pyjt-0.3.1/tests/test_textfield.py`

 * *Files identical despite different names*

