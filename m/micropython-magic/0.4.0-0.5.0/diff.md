# Comparing `tmp/micropython_magic-0.4.0.tar.gz` & `tmp/micropython_magic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_magic-0.4.0.tar", max compression
+gzip compressed data, was "micropython_magic-0.5.0.tar", max compression
```

## Comparing `micropython_magic-0.4.0.tar` & `micropython_magic-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1090 2023-04-13 20:20:40.063549 micropython_magic-0.4.0/LICENSE
--rw-r--r--   0        0        0     1492 2023-07-06 14:02:07.913898 micropython_magic-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6364 2023-06-29 18:39:42.591892 micropython_magic-0.4.0/readme.md
--rw-r--r--   0        0        0      877 2023-07-06 14:02:07.933922 micropython_magic-0.4.0/src/micropython_magic/__init__.py
--rw-r--r--   0        0        0     5497 2023-07-06 12:34:39.272049 micropython_magic-0.4.0/src/micropython_magic/interactive.py
--rw-r--r--   0        0        0      773 2023-06-29 18:39:42.638770 micropython_magic-0.4.0/src/micropython_magic/magic_transformer.py
--rw-r--r--   0        0        0    26107 2023-06-29 18:51:41.327067 micropython_magic-0.4.0/src/micropython_magic/memoryinfo.py
--rw-r--r--   0        0        0     5093 2023-07-06 10:21:54.314700 micropython_magic-0.4.0/src/micropython_magic/mpr.py
--rw-r--r--   0        0        0    12264 2023-07-06 12:54:55.520197 micropython_magic-0.4.0/src/micropython_magic/octarine.py
--rw-r--r--   0        0        0      488 2023-06-07 09:44:35.636682 micropython_magic-0.4.0/src/micropython_magic/param_fixup.py
--rw-r--r--   0        0        0     4105 2023-07-06 11:01:06.908674 micropython_magic-0.4.0/src/micropython_magic/scripts/fw_info.py
--rw-r--r--   0        0        0     2928 2023-06-29 18:39:42.645270 micropython_magic-0.4.0/src/micropython_magic/test_magics.py
--rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 micropython_magic-0.4.0/setup.py
--rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 micropython_magic-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-13 20:20:40.063549 micropython_magic-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1534 2023-08-04 14:50:20.250102 micropython_magic-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6364 2023-06-29 18:39:42.591892 micropython_magic-0.5.0/readme.md
+-rw-r--r--   0        0        0      878 2023-08-04 14:39:44.079916 micropython_magic-0.5.0/src/micropython_magic/__init__.py
+-rw-r--r--   0        0        0     2880 2023-08-04 14:38:30.887241 micropython_magic-0.5.0/src/micropython_magic/exp_magics.py
+-rw-r--r--   0        0        0     5497 2023-07-06 12:34:39.272049 micropython_magic-0.5.0/src/micropython_magic/interactive.py
+-rw-r--r--   0        0        0      773 2023-06-29 18:39:42.638770 micropython_magic-0.5.0/src/micropython_magic/magic_transformer.py
+-rw-r--r--   0        0        0    26107 2023-06-29 18:51:41.327067 micropython_magic-0.5.0/src/micropython_magic/memoryinfo.py
+-rw-r--r--   0        0        0     5093 2023-07-06 10:21:54.314700 micropython_magic-0.5.0/src/micropython_magic/mpr.py
+-rw-r--r--   0        0        0    12768 2023-07-06 18:54:37.874377 micropython_magic-0.5.0/src/micropython_magic/octarine.py
+-rw-r--r--   0        0        0      488 2023-06-07 09:44:35.636682 micropython_magic-0.5.0/src/micropython_magic/param_fixup.py
+-rw-r--r--   0        0        0     4105 2023-07-06 11:01:06.908674 micropython_magic-0.5.0/src/micropython_magic/scripts/fw_info.py
+-rw-r--r--   0        0        0     6972 1970-01-01 00:00:00.000000 micropython_magic-0.5.0/PKG-INFO
```

### Comparing `micropython_magic-0.4.0/LICENSE` & `micropython_magic-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.4.0/pyproject.toml` & `micropython_magic-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-magic"
-version = "0.4.0"
+version = "0.5.0"
 description = "MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs"
 keywords = [
     "MicroPython",
     "stubs",
     "Jupyter",
     "notebooks",
     "Jupyter Labs",
@@ -17,14 +17,16 @@
 packages = [{ include = "micropython_magic", from = "src" }]
 include = []
 exclude = ["**/tests/**", "**/*-test", "**/samples.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 mpremote = "1.20.0"
+loguru = "^0.7.0"
+matplotlib = "^3.7.2"
 
 [tool.poetry.extras]
 widgets = ["bqplot", "numpy"]
 
 [tool.poetry.group.dev]
 optional = true
 [tool.poetry.group.dev.dependencies]
```

### Comparing `micropython_magic-0.4.0/readme.md` & `micropython_magic-0.5.0/readme.md`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.4.0/src/micropython_magic/__init__.py` & `micropython_magic-0.5.0/src/micropython_magic/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 
 from IPython.core.interactiveshell import InteractiveShell
 from loguru import logger as log
 
 from .magic_transformer import comment_magic_transformer
 from .octarine import MpyMagics
-from .test_magics import TestMagics
+
+# from .exp_magics import ExpMagics
 
 
 def load_ipython_extension(ipython: InteractiveShell):
     # register the input transformer to allow %%cell_magics in comments
     ipython.input_transformers_cleanup.append(comment_magic_transformer)
     # register the magics
     ipython.register_magics(MpyMagics)
-    # ipython.register_magics(TestMagics)
+    # ipython.register_magics(ExpMagics)
 
 
 def unload_ipython_extension(ipython: InteractiveShell):
     # unregister the magics, allows to unload / reload the extension
     # ipython.magics_manager.magics["cell"].pop("mpy", None)
     # TODO
     pass
```

### Comparing `micropython_magic-0.4.0/src/micropython_magic/interactive.py` & `micropython_magic-0.5.0/src/micropython_magic/interactive.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.4.0/src/micropython_magic/magic_transformer.py` & `micropython_magic-0.5.0/src/micropython_magic/magic_transformer.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.4.0/src/micropython_magic/memoryinfo.py` & `micropython_magic-0.5.0/src/micropython_magic/memoryinfo.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.4.0/src/micropython_magic/mpr.py` & `micropython_magic-0.5.0/src/micropython_magic/mpr.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.4.0/src/micropython_magic/octarine.py` & `micropython_magic-0.5.0/src/micropython_magic/octarine.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pkg_resources
 from colorama import Style
 from IPython.core.error import UsageError
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.core.magic import Magics, cell_magic, line_magic, magics_class, output_can_be_silenced
 from IPython.core.magic_arguments import argument, argument_group, magic_arguments, parse_argstring
 from IPython.utils.text import LSString, SList
-from loguru import logger as log
+from loguru import logger as log  # type: ignore
 
 from micropython_magic.interactive import TIMEOUT
 from micropython_magic.param_fixup import get_code
 
 from .mpr import DONT_KNOW, JSON_END, JSON_START, MPRemote2
 
 # https://ipython.readthedocs.io/en/stable/config/custommagics.html
@@ -71,23 +71,34 @@
         return "\n".join(output.list)
     elif isinstance(output, LSString):
         return output
     else:
         return str(output)
 
 
+from traitlets import All
+from traitlets import Float as Float_
+from traitlets import HasTraits
+from traitlets import Integer as Integer_
+from traitlets import Unicode, default, observe, validate
+from traitlets.config.configurable import Configurable
+
+
 @magics_class
 class MpyMagics(Magics):
     """A class to define the magic functions for Micropython."""
 
+    # The default timeout
+    timeout = Float_(TIMEOUT).tag(config=True)
+
     def __init__(self, shell: InteractiveShell):
         # first call the parent constructor
         super(MpyMagics, self).__init__(shell)
         self.shell: InteractiveShell
-        self._MCUs: List[MPRemote2] = [MPRemote2(shell)]
+        self._MCUs: list[MPRemote2] = [MPRemote2(shell)]
         # self.port: str = "auto"  # by default connect to the first device
         # self.resume = True  # by default resume the device to maintain state
 
     @property
     def port(self) -> None:
         return None
 
@@ -104,26 +115,29 @@
     @cell_magic("micropython")
     @cell_magic("mpy")
     @magic_arguments("%micropython")  # add additional % to display two %% in help
     @argument_group("Code execution")
     @argument("--writefile", "--save", "-wf", type=str, help="MCU [path/]filename to write to", metavar="PATH/FILE.PY")
     @argument("--readfile", "--load", "-rf", type=str, help="MCU [path/]filename to read from", metavar="PATH/FILE.PY")
     @argument("--new", action="store_true", help="new cell is added after the current cell instead of replacing it")
-    @argument("--timeout", default=TIMEOUT, help="maximum timeout for the cell to run")
+    @argument("--timeout", default=-1, help="maximum timeout for the cell to run")
     # #
     @argument_group("Devices")
     @argument("--select", nargs="+", help="serial port to connect to", metavar="PORT")
     @argument("--reset", "--soft-reset", action="store_true", help="Reset device (before running cell).")
     @argument("--hard-reset", action="store_true", help="reset device.")
     def micropython(self, line: str, cell: str = ""):
         """
         Run Micropython code on an attached device using mpremote.
         """
         args = parse_argstring(self.micropython, line or "")
 
+        if args.timeout == -1:
+            args.timeout = self.timeout
+
         if args.select:
             if len(args.select) > 1:
                 # allow a list of ports to be specified
                 log.warning(f"{args.select=} not yet implemented")
                 return
             else:
                 self.select(args.select[0])
@@ -168,15 +182,15 @@
 
     @line_magic("micropython")
     @line_magic("mpy")
     @magic_arguments("mpy")
     @argument_group("Code execution")
     @argument("statement", nargs="*", help="Micropython code to run.", metavar="STATEMENT(S)")
     @argument("--eval", "-e", nargs="*", help="Expression to evaluate", metavar="EXPRESSION")
-    @argument("--timeout", default=TIMEOUT, help="maximum timeout for the cell to run")
+    @argument("--timeout", default=-1, help="maximum timeout for the cell to run")
     @argument("--stream", action="store_true", help="stream each line of output as it is received")
     @argument_group("Devices")
     @argument("--list", "--devs", "-l", action="store_true", help="List available devices.")
     @argument("--select", "-s", nargs="+", help="serial port to connect to", metavar="PORT")
     @argument("--reset", "--soft-reset", action="store_true", help="reset device.")
     @argument("--hard-reset", action="store_true", help="reset device.")
     @argument("--info", action="store_true", help="get boardinfo from device")
@@ -184,14 +198,17 @@
     def mpy_line(self, line: str):
         """
         Run Micropython code on an attached device using mpremote.
 
         - can be silenced with a trailing semicolon when used as a line magic
         """
         args = parse_argstring(self.mpy_line, line or "")
+        if args.timeout == -1:
+            args.timeout = self.timeout
+
         # try to fixup the expression after shell and argparse mangled it
         if args.statement and len(args.statement) >= 1:
             args.statement = get_code(line, args.statement[0])
         if args.eval and len(args.eval) >= 1:
             args.eval = get_code(line, args.eval[0])
         if isinstance(args.eval, list):
             args.eval = " ".join(args.eval)
@@ -215,15 +232,15 @@
         # processing
         if args.list:
             return self.list_devices()
         elif args.info:
             #  load datafile  from installed package
             script_path = pkg_resources.resource_filename("micropython_magic", "scripts/fw_info.py")
             cmd = ["run", script_path]
-            if out := self.MCU.run_cmd(" ".join(cmd), stream_out=False, timeout=TIMEOUT):
+            if out := self.MCU.run_cmd(" ".join(cmd), stream_out=False, timeout=int(self.timeout)):
                 if not out[0].startswith("{"):
                     return out
                 r = eval(out[0])
                 r["serial_port"] = self.MCU.port
                 return r
         elif args.eval:
             return self.eval(args.eval)
```

### Comparing `micropython_magic-0.4.0/src/micropython_magic/scripts/fw_info.py` & `micropython_magic-0.5.0/src/micropython_magic/scripts/fw_info.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.4.0/src/micropython_magic/test_magics.py` & `micropython_magic-0.5.0/src/micropython_magic/exp_magics.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,20 @@
 from IPython.core.error import UsageError
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.core.magic import Magics, cell_magic, line_magic, magics_class, needs_local_scope, output_can_be_silenced
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from IPython.display import display
 from IPython.utils.text import LSString, SList
 from loguru import logger as log
-from mpremote import pyboard, pyboardextended
 
 from micropython_magic.octarine import MpyMagics, PrettyOutput
 
 
 @magics_class
-class TestMagics(MpyMagics):
+class ExpMagics(MpyMagics):
     # @cell_magic("cool")
     # def magic_cool(self, line, cell):
     #     """\
     #     A really cool magic command.
     #     """
     #     print(f"Magically cool ! {cell=}")
```

### Comparing `micropython_magic-0.4.0/setup.py` & `micropython_magic-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,210 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: micropython-magic
+Version: 0.5.0
+Summary: MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs
+License: MIT
+Keywords: MicroPython,stubs,Jupyter,notebooks,Jupyter Labs,vscode
+Author: Jos Verlinde
+Author-email: jos_verlinde@hotmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: widgets
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
+Requires-Dist: mpremote (==1.20.0)
+Description-Content-Type: text/markdown
+
+# micropython-magic
+
+These magic methods allow MicroPython to be used from within any Jupyter Notebook or JupyterLab (formerly IPython Notebook)
+The magics make use of the [mpremote tool](https://github.com/micropython/micropython/blob/master/tools/mpremote/README.md) to enable communication with the MCUs 
+
+
+It allows 
+ * Mixing of Host and MCU Code ( and languages if you wish)
+ * Creating graphs of the data captured by MCU sensors 
+ * create re-uasable sequences ( download/compile firmware - flash firmware - uploade code - run expiriment - same outcome) 
+ * create and execute tests that require orchestration across multiple MCUs and hosts 
+ * Rapid Prototyping 
+ * Capturing the results and outputs in a consistent way
+ * Mixing documentation with code  
+
+
+## Samples 
+
+<table>
+
+<tr>
+<td>
+Plot cpu temperature  
+
+<img src="docs/cpu_plot.gif" width="300" />
+</td>
+<td>
+Visualize the memory map of the MCU
+
+<img src="docs/memory_map.gif" width="300" />
+</td>
+</tr>
+
+<tr>
+<td>
+</td>
+<td>
+Memory allocation of the MCU over time
+
+<img src="docs/memory_map_sequence.gif" width="300" />
+</td>
+</tr>
+</table>
+
+For the source please refer to the samples folder
+## Installation
+- create and activate a venv `python3 -m venv .venv`
+ - [ ] `pip install -U "micropython-magic"`
+
+- or install directly into your notbook environment/kernel using the '%pip' magic by running
+  - [ ] `%pip install -U "micropython-magic"`
+
+Recommended : install stubs for your MCU of choice
+- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs` (or your port of choise)
+
+## Usage
+
+**1) Create a notebook**
+- install your desired notebook environment:
+  - [VScode and the **Juypyter extension**](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) ,
+  - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook) 
+  - [JupyterLab ](https://jupyter.org/install)
+
+- create a new notebook 
+
+**2) Load the magic**
+```python
+%load_ext micropython_magic
+```
+This can also be configured once to always load automatically ( see below)
+
+
+**3) add a cell with some code to run on the MCU**
+```python
+# %%micropython  
+from machine import Pin
+led = Pin(25, Pin.OUT)
+led.value(1)
+```
+The `%%micropython` cell magic will instruct Jupyter to run the code on the connected MCU
+
+**4) enable code highlighting for MicroPython**
+```python
+%pip install micropython-esp32-stubs==1.20.0.*
+# installs the stubs for MicroPython syntax checking (one time install per environment) 
+```
+
+```python
+# %%micropython  
+from machine import Pin
+led = Pin(25, Pin.OUT)
+led.value(1)
+```
+This allows for syntax highlighting and code completion of MicroPython code.
+Tested in VSCode with
+- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) extension
+- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension
+
+
+## Advanced 
+List the connected devices 
+```python
+%mpy --list
+```
+
+## Automatically load the magic on startup
+
+In order to automatically load the magic on startup, you can add the following to your `ipython_config.py` file:
+
+- create a ipython profile 
+  - `ipython profile create`
+  - add the following to the configuration file (`.../.ipython/profile_default/ipython_config.py`)
+
+    ```python
+    c = get_config()  #noqa
+
+    c.InteractiveShellApp.extensions = [
+        'micropython_magic'
+    ]
+    ```
+
+# initial 
+
+ - [x] run a code cell on a MCU 
+ - [ ] mpremote primitives
+   - [x] list connected boards and loop through them 
+   - [x] switch the active MCU
+   - [x] avoid resetting MCU between cells ( use `resume`)
+   - [x] soft-reset a MCU
+   - [/] hard-reset a MCU
+       - only works on non-rp2040 devices 
+       - report / fix hardware reset  issue on rp2040 `machine.reset()` ?
+   - all mpremote commands are possible using `!mpremote`
+   - [ ] mip install 
+   - [ ] direct - copy file / files to / from 
+   - [ ] mount folder 
+   - [ ] ls and other file operations 
+   - [ ] recursive delete wipe files from MCU - as a built-in magic ? / wait for / create PR for mpremote update ?
+   - [ ] cellmagic to copy cell content to specific files on the MCS 
+       - [ ] %%micropython --writefile main.py
+       - [ ] %%micropython --readfile boot.py
+- [ ] Notebook essentials
+   - [x] load magics from `%pip install micropython-magic`
+   - [x] get the output from the MCU into a python variable `local = %eval remote`
+         - eval is not quite the same as mpremote
+         - retain type through json ?
+         - [?] can this be done with repr(insted) of json ?
+   - [x] plot data from a MCU
+            - [x] using bqplot ( > pyplot > vscode-Jupyter) 
+            - [/] add documentation / sample
+-   
+   - [ ] copy/echo MCU global vars to local vars ( sync_from / sync_to)?
+   - [ ] get a data series onto the notebook and plot the outcome 
+       - [x] loop one by one and update plot
+       - [ ] get larger series 
+   - [ ] loop and update plot 
+         https://ipywidgets.readthedocs.io/en/7.x/examples/Widget%20Asynchronous.html#Updating-a-widget-in-the-background
+   - [ ] long running via mqtt / async / folder mount ?
+ - [ ] is there a way to avoid needing to set %%micropython on all cells ?
+       this could be done via an input_transformer - but keeping the state between cells may be quuite hard / confusing
+ - [ ] %timeit / %%timeit for micropython code to avoid measuring the mpremote startup overhead 
+
+Samples
+   - [x] Install
+   - [x] basic board control
+   - [x] blink
+   - [x] list connected boards and loop through them 
+   - [~] read sensor and build series ( file / list / plot)
+   - [ ] flash a mcu with new firmware ( sample per port )
+   - [ ] mip install 
+   - [ ] upload a repo / folder to a MCU
+
+## development
+## Testing 
+
+- using Pytest
+- using testbook for testing notebooks
+  - located in the `./tests/` folder
+  - tests are paired with notebooks that contain the cells and magic commands to be tested
+  - tests have not been mocked - and therefore require a connected MCU to run ( rp2040 )
+
+- TODO: add tests for (remote) kernels 
+  - [x] Local (on windows)
+  - [ ] on windows 
+  - [ ] on linux
+  - [ ] jupyter notebook
+  - [ ] jupyter labs 
 
-package_dir = \
-{'': 'src'}
 
-packages = \
-['micropython_magic', 'micropython_magic.scripts']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['mpremote==1.20.0']
-
-setup_kwargs = {
-    'name': 'micropython-magic',
-    'version': '0.4.0',
-    'description': 'MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs',
-    'long_description': '# micropython-magic\n\nThese magic methods allow MicroPython to be used from within any Jupyter Notebook or JupyterLab (formerly IPython Notebook)\nThe magics make use of the [mpremote tool](https://github.com/micropython/micropython/blob/master/tools/mpremote/README.md) to enable communication with the MCUs \n\n\nIt allows \n * Mixing of Host and MCU Code ( and languages if you wish)\n * Creating graphs of the data captured by MCU sensors \n * create re-uasable sequences ( download/compile firmware - flash firmware - uploade code - run expiriment - same outcome) \n * create and execute tests that require orchestration across multiple MCUs and hosts \n * Rapid Prototyping \n * Capturing the results and outputs in a consistent way\n * Mixing documentation with code  \n\n\n## Samples \n\n<table>\n\n<tr>\n<td>\nPlot cpu temperature  \n\n<img src="docs/cpu_plot.gif" width="300" />\n</td>\n<td>\nVisualize the memory map of the MCU\n\n<img src="docs/memory_map.gif" width="300" />\n</td>\n</tr>\n\n<tr>\n<td>\n</td>\n<td>\nMemory allocation of the MCU over time\n\n<img src="docs/memory_map_sequence.gif" width="300" />\n</td>\n</tr>\n</table>\n\nFor the source please refer to the samples folder\n## Installation\n- create and activate a venv `python3 -m venv .venv`\n - [ ] `pip install -U "micropython-magic"`\n\n- or install directly into your notbook environment/kernel using the \'%pip\' magic by running\n  - [ ] `%pip install -U "micropython-magic"`\n\nRecommended : install stubs for your MCU of choice\n- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs` (or your port of choise)\n\n## Usage\n\n**1) Create a notebook**\n- install your desired notebook environment:\n  - [VScode and the **Juypyter extension**](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) ,\n  - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook) \n  - [JupyterLab ](https://jupyter.org/install)\n\n- create a new notebook \n\n**2) Load the magic**\n```python\n%load_ext micropython_magic\n```\nThis can also be configured once to always load automatically ( see below)\n\n\n**3) add a cell with some code to run on the MCU**\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThe `%%micropython` cell magic will instruct Jupyter to run the code on the connected MCU\n\n**4) enable code highlighting for MicroPython**\n```python\n%pip install micropython-esp32-stubs==1.20.0.*\n# installs the stubs for MicroPython syntax checking (one time install per environment) \n```\n\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThis allows for syntax highlighting and code completion of MicroPython code.\nTested in VSCode with\n- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) extension\n- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension\n\n\n## Advanced \nList the connected devices \n```python\n%mpy --list\n```\n\n## Automatically load the magic on startup\n\nIn order to automatically load the magic on startup, you can add the following to your `ipython_config.py` file:\n\n- create a ipython profile \n  - `ipython profile create`\n  - add the following to the configuration file (`.../.ipython/profile_default/ipython_config.py`)\n\n    ```python\n    c = get_config()  #noqa\n\n    c.InteractiveShellApp.extensions = [\n        \'micropython_magic\'\n    ]\n    ```\n\n# initial \n\n - [x] run a code cell on a MCU \n - [ ] mpremote primitives\n   - [x] list connected boards and loop through them \n   - [x] switch the active MCU\n   - [x] avoid resetting MCU between cells ( use `resume`)\n   - [x] soft-reset a MCU\n   - [/] hard-reset a MCU\n       - only works on non-rp2040 devices \n       - report / fix hardware reset  issue on rp2040 `machine.reset()` ?\n   - all mpremote commands are possible using `!mpremote`\n   - [ ] mip install \n   - [ ] direct - copy file / files to / from \n   - [ ] mount folder \n   - [ ] ls and other file operations \n   - [ ] recursive delete wipe files from MCU - as a built-in magic ? / wait for / create PR for mpremote update ?\n   - [ ] cellmagic to copy cell content to specific files on the MCS \n       - [ ] %%micropython --writefile main.py\n       - [ ] %%micropython --readfile boot.py\n- [ ] Notebook essentials\n   - [x] load magics from `%pip install micropython-magic`\n   - [x] get the output from the MCU into a python variable `local = %eval remote`\n         - eval is not quite the same as mpremote\n         - retain type through json ?\n         - [?] can this be done with repr(insted) of json ?\n   - [x] plot data from a MCU\n            - [x] using bqplot ( > pyplot > vscode-Jupyter) \n            - [/] add documentation / sample\n-   \n   - [ ] copy/echo MCU global vars to local vars ( sync_from / sync_to)?\n   - [ ] get a data series onto the notebook and plot the outcome \n       - [x] loop one by one and update plot\n       - [ ] get larger series \n   - [ ] loop and update plot \n         https://ipywidgets.readthedocs.io/en/7.x/examples/Widget%20Asynchronous.html#Updating-a-widget-in-the-background\n   - [ ] long running via mqtt / async / folder mount ?\n - [ ] is there a way to avoid needing to set %%micropython on all cells ?\n       this could be done via an input_transformer - but keeping the state between cells may be quuite hard / confusing\n - [ ] %timeit / %%timeit for micropython code to avoid measuring the mpremote startup overhead \n\nSamples\n   - [x] Install\n   - [x] basic board control\n   - [x] blink\n   - [x] list connected boards and loop through them \n   - [~] read sensor and build series ( file / list / plot)\n   - [ ] flash a mcu with new firmware ( sample per port )\n   - [ ] mip install \n   - [ ] upload a repo / folder to a MCU\n\n## development\n## Testing \n\n- using Pytest\n- using testbook for testing notebooks\n  - located in the `./tests/` folder\n  - tests are paired with notebooks that contain the cells and magic commands to be tested\n  - tests have not been mocked - and therefore require a connected MCU to run ( rp2040 )\n\n- TODO: add tests for (remote) kernels \n  - [x] Local (on windows)\n  - [ ] on windows \n  - [ ] on linux\n  - [ ] jupyter notebook\n  - [ ] jupyter labs \n\n',
-    'author': 'Jos Verlinde',
-    'author_email': 'jos_verlinde@hotmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

