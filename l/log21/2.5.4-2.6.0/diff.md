# Comparing `tmp/log21-2.5.4.tar.gz` & `tmp/log21-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.5.4.tar", last modified: Wed Jul 12 15:56:22 2023, max compression
+gzip compressed data, was "log21-2.6.0.tar", last modified: Fri Aug  4 08:40:19 2023, max compression
```

## Comparing `log21-2.5.4.tar` & `log21-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-12 15:56:05.000000 log21-2.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-12 15:56:22.150226 log21-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-12 15:56:05.000000 log21-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-12 15:56:05.000000 log21-2.5.4/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-12 15:56:05.000000 log21-2.5.4/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-07-12 15:56:05.000000 log21-2.5.4/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-07-12 15:56:05.000000 log21-2.5.4/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-12 15:56:05.000000 log21-2.5.4/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-07-12 15:56:05.000000 log21-2.5.4/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-12 15:56:05.000000 log21-2.5.4/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-12 15:56:05.000000 log21-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:56:22.150226 log21-2.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.659241 log21-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-04 08:40:09.000000 log21-2.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-08-04 08:40:19.659241 log21-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-08-04 08:40:09.000000 log21-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-04 08:40:09.000000 log21-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:40:19.659241 log21-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.655241 log21-2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.659241 log21-2.6.0/src/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Argumentify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.659241 log21-2.6.0/src/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.659241 log21-2.6.0/src/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/top_level.txt
```

### Comparing `log21-2.5.4/LICENSE.txt` & `log21-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/PKG-INFO` & `log21-2.6.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: log21
-Version: 2.5.4
-Summary: A simple logging package that helps you log colorized messages in Windows console.
-Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
-License: Apache License 2.0
-Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
-Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
-Project-URL: Source, https://github.com/MPCodeWriter21/log21
-Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/log21)
 ![forks](https://img.shields.io/github/forks/MPCodeWriter21/log21)
 ![repo size](https://img.shields.io/github/repo-size/MPCodeWriter21/log21)
@@ -40,17 +18,20 @@
   modifications. It can also decolorize the output if you want to log into a file.
 + Pretty printing : Have you ever wanted to colorize the output of the pprint module? log21's pretty printer can do
   that.
 + Tree printing : You can pass a dict or list to log21.tree_print function and it will print it in a tree-like
   structure. It's also colorized XD.
 + ProgressBar : log21's progress bar can be used to show progress of a process in a beautiful way.
 + LoggingWindow : Helps you to log messages and debug your code in a window other than the console.
-+ CrashReporter : log21's crash reporter can be used to report crashes in different ways. You can use it to log crashes
-  to console or files or use it to receive crash reports of your program through email. And you can also define your own
-  crash reporter functions and use them instead!
++ CrashReporter : log21's crash reporter can be used to report crashes in different
+  ways. You can use it to log crashes to console or files or use it to receive crash
+  reports of your program through email. And you can also define your own crash
+  reporter functions and use them instead!
++ Argumentify : You can use the argumentify feature to decrease the number of lines you
+  need to write to parse command-line arguments. It's colored by the way!
 + Any idea? Feel free to [open an issue](https://github.com/MPCodeWriter21/log21/issues) or submit a pull request.
 
 ![issues](https://img.shields.io/github/issues/MPCodeWriter21/log21)
 ![contributors](https://img.shields.io/github/contributors/MPCodeWriter21/log21)
 
 Installation
 ------------
@@ -58,44 +39,45 @@
 Well, this is a python package so the first thing you need is python.
 
 If you don't have python installed, please visit [Python.org](https://python.org) and install the latest version of
 python.
 
 Then you can install log21 using pip module:
 
-```shell
+```bash
 python -m pip install log21 -U
 ```
 
 Or you can clone [the repository](https://github.com/MPCodeWriter21/log21) and run:
 
-```shell
-python setup.py install
+```bash
+pip install .
+```
+
+Or let the pip get it using git:
+```bash
+pip install git+https://github.com/MPCodeWriter21/log21
 ```
 
 Changes
 -------
 
-### 2.5.4
-
-Added constant colors directly to the Colors module. Now you can do this:
-```python
-from log21 import print
-from log21.colors import GREEN, WHITE, RED
+### 2.6.0
 
-print(GREEN + 'This' + WHITE + ' is' + RED + ' Red')
-```
+Added the `Argumentify` module. Check the examples.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
 
-```python3
+### Basic Logging
+
+```python
 import log21
 
 log21.print(log21.get_color('#FF0000') + 'This' + log21.get_color((0, 255, 0)) + ' is' + log21.get_color('Blue') +
             ' Blue' + log21.get_colors('BackgroundWhite', 'Black') + ' 8)')
 
 logger = log21.get_logger('My Logger', level_names={21: 'SpecialInfo', log21.WARNING: ' ! ', log21.ERROR: '!!!'})
 logger.info('You are reading the README.md file...')
@@ -111,15 +93,17 @@
 logger.error(log21.get_colors('LightRed') + "I'm still here ;1")
 ```
 
 ![Basic Logging](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-1.png)
 
 ----------------
 
-```python3
+### Argument Parsing (See Also: [Argumentify](https://github.com/MPCodeWriter21/log21#argumentify))
+
+```python
 import log21
 from log21 import ColorizingArgumentParser, get_logger, get_colors as gc
 
 parser = ColorizingArgumentParser(description="This is a simple example of a ColorizingArgumentParser.",
                                   colors={'help': 'LightCyan'})
 parser.add_argument('test1', action='store', help='Test 1')
 parser.add_argument('test2', action='store', help='Test 2')
@@ -157,15 +141,17 @@
 
 ![Valid example 2](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-2.4.png)
 
 ![Valid example 3](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-2.5.png)
 
 ------------------
 
-```python3
+### Pretty-Printing and Tree-Printing
+
+```python
 import json
 import log21
 
 data = json.load(open('json.json', 'r'))
 
 # Prints data using python's built-in print function
 print(data)
@@ -180,15 +166,17 @@
 ![Python print](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-3.1.png)
 ![log21 pretty print](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-3.2.png)
 ![log21 tree print 1](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-3.3.1.png)
 ![log21 tree print 1](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-3.3.2.png)
 
 ------------------
 
-```python3
+### Logging Window
+
+```python
 import log21
 
 window = log21.get_logging_window('My Logging Window', width=80)
 window.font = ('Courier New', 9)
 
 # Basic logging
 window.info('This is a basic logging message.')
@@ -221,15 +209,17 @@
 
 ```
 
 ![The LoggingWindow](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-4.png)
 
 ------------------
 
-```python3
+### ProgressBar
+
+```python
 # Example 1
 import log21, time
 
 # Define a very simple log21 progress bar
 progress_bar = log21.ProgressBar()
 
 # And here is a simple loop that will print the progress bar
@@ -259,14 +249,207 @@
     time.sleep(random.uniform(0.05, 0.21))
 
 ```
 
 ![ProgressBar - Example 1](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-5.1.gif)
 ![ProgressBar - Example 2](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-5.2.gif)
 
+------------------
+
+### Argumentify (Check out [the manual way](https://github.com/MPCodeWriter21/log21#argument-parsing))
+
+```python
+# Common Section
+import log21
+
+
+class ReversedText:
+    def __init__(self, text: str):
+        self._text = text[::-1]
+
+    def __str__(self):
+        return self._text
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__}(text='{self._text}') at {hex(id(self))}>"
+
+
+# Old way
+def main():
+    """Here is my main function"""
+    parser = log21.ColorizingArgumentParser()
+    parser.add_argument('--positional-arg', '-p', action='store', type=int,
+                        required=True, help="This argument is positional!")
+    parser.add_argument('--optional-arg', '-o', action='store', type=ReversedText,
+                        help="Whatever you pass here will be REVERSED!")
+    parser.add_argument('--arg-with-default', '-a', action='store', default=21,
+                        help="The default value is 21")
+    parser.add_argument('--additional-arg', '-A', action='store',
+                        help="This one is extra.")
+    parser.add_argument('--verbose', '-v', action='store_true',
+                        help="Increase verbosity")
+    args = parser.parse_args()
+
+    if args.verbose:
+        log21.basic_config(level='DEBUG')
+
+    log21.info(f"positional_arg = {args.positional_arg}")
+    log21.info(f"optional_arg = {args.optional_arg}")
+    log21.debug(f"arg_with_default = {args.arg_with_default}")
+    log21.debug(f"additional_arg = {args.additional_arg}")
+
+
+if __name__ == '__main__':
+    main()
+
+
+# New way
+def main(positional_arg: int, /, optional_arg: ReversedText, arg_with_default: int = 21,
+         additional_arg=None, verbose: bool = False):
+    """Some description
+
+    :param positional_arg: This argument is positional!
+    :param optional_arg: Whatever you pass here will be REVERSED!
+    :param arg_with_default: The default value is 21
+    :param additional_arg: This one is extra.
+    :param verbose: Increase verbosity
+    """
+    if verbose:
+        log21.basic_config(level='DEBUG')
+
+    log21.info(f"{positional_arg = }")
+    log21.info(f"{optional_arg = !s}")
+    log21.debug(f"{arg_with_default = }")
+    log21.debug(f"{additional_arg = !s}")
+
+
+if __name__ == '__main__':
+    log21.argumentify(main)
+```
+
+![Old-Way](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-6.1.png)
+![New-Way](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-6.2.png)
+
+Example with multiple functions as entry-point:
+
+```python
+import ast
+import operator
+from functools import reduce
+
+import log21
+
+# `safe_eval` Based on https://stackoverflow.com/a/9558001/1113207
+# Supported Operators
+operators = {
+    ast.Add: operator.add,
+    ast.Sub: operator.sub,
+    ast.Mult: operator.mul,
+    ast.Div: operator.truediv,
+    ast.FloorDiv: operator.floordiv,
+    ast.Pow: operator.pow,
+    ast.BitXor: operator.xor,
+    ast.USub: operator.neg
+}
+
+
+def safe_eval(expr: str):
+    """Safely evaluate a mathematical expression.
+
+    >>> eval_expr('2^6')
+    4
+    >>> eval_expr('2**6')
+    64
+    >>> eval_expr('1 + 2*3**(4^5) / (6 + -7)')
+    -5.0
+
+    :param expr: expression to evaluate
+    :raises SyntaxError: on invalid expression
+    :return: result of the evaluation
+    """
+    try:
+        return _eval(ast.parse(expr, mode='eval').body)
+    except (TypeError, KeyError, SyntaxError):
+        log21.error(f'Invalid expression: {expr}')
+        raise
+
+
+def _eval(node: ast.AST):
+    """Internal implementation of `safe_eval`.
+
+    :param node: AST node to evaluate
+    :raises TypeError: on invalid node
+    :raises KeyError: on invalid operator
+    :raises ZeroDivisionError: on division by zero
+    :raises ValueError: on invalid literal
+    :raises SyntaxError: on invalid syntax
+    :return: result of the evaluation
+    """
+    if isinstance(node, ast.Num):  # <number>
+        return node.n
+    if isinstance(node, ast.BinOp):  # <left> <operator> <right>
+        return operators[type(node.op)](_eval(node.left), _eval(node.right))
+    if isinstance(node, ast.UnaryOp):  # <operator> <operand> e.g., -1
+        return operators[type(node.op)](_eval(node.operand))
+    raise TypeError(node)
+
+
+# Example code
+def addition(*numbers: float):
+    """Addition of numbers.
+
+    Args:
+        numbers (float): numbers to add
+    """
+    if len(numbers) < 2:
+        log21.error('At least two numbers are required! Use `-n`.')
+        return
+    log21.info(f'Result: {sum(numbers)}')
+
+
+def multiplication(*numbers: float):
+    """Multiplication of numbers.
+
+    Args:
+        numbers (float): numbers to multiply
+    """
+    if len(numbers) < 2:
+        log21.error('At least two numbers are required! Use `-n`.')
+        return
+    log21.info(f'Result: {reduce(lambda x, y: x * y, numbers)}')
+
+
+def calc(*inputs: str, verbose: bool = False):
+    """Calculate numbers.
+
+    :param inputs: numbers and operators
+    """
+    expression = ' '.join(inputs)
+
+    if len(expression) < 3:
+        log21.error('At least two numbers and one operator are required! Use `-i`.')
+        return
+
+    if verbose:
+        log21.basic_config(level='DEBUG')
+
+    log21.debug(f'Expression: {expression}')
+    try:
+        log21.info(f'Result: {safe_eval(expression)}')
+    except (TypeError, KeyError, SyntaxError):
+        pass
+
+
+if __name__ == "__main__":
+    log21.argumentify({'add': addition, 'mul': multiplication, 'calc': calc})
+```
+
+![multi-entry](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-6.3.png)
+
+
 About
 -----
 Author: CodeWriter21 (Mehrad Pooryoussof)
 
 GitHub: [MPCodeWriter21](https://github.com/MPCodeWriter21)
 
 Telegram Channel: [@CodeWriter21](https://t.me/CodeWriter21)
```

### Comparing `log21-2.5.4/log21/Argparse.py` & `log21-2.6.0/src/log21/Argparse.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/Colors.py` & `log21-2.6.0/src/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/CrashReporter/Formatters.py` & `log21-2.6.0/src/log21/CrashReporter/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/CrashReporter/Reporters.py` & `log21-2.6.0/src/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/FileHandler.py` & `log21-2.6.0/src/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/Formatters.py` & `log21-2.6.0/src/log21/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/Logger.py` & `log21-2.6.0/src/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/LoggingWindow.py` & `log21-2.6.0/src/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/Manager.py` & `log21-2.6.0/src/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/PPrint.py` & `log21-2.6.0/src/log21/PPrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/ProgressBar.py` & `log21-2.6.0/src/log21/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/StreamHandler.py` & `log21-2.6.0/src/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/TreePrint.py` & `log21-2.6.0/src/log21/TreePrint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # log21.TreePrint.py
 # CodeWriter21
 
 from __future__ import annotations
 
-from typing import Union as _Union, Mapping as _Mapping, Sequence as _Sequence, Optional as _Optional, List as _List
+from typing import (
+    List as _List, Union as _Union, Mapping as _Mapping, Optional as _Optional, Sequence
+    as _Sequence
+)
 
 from log21.Colors import get_colors as _gc
 
 
 class TreePrint:
+
     class Node:
-        def __init__(self, value: _Union[str, int], children: _Optional[_List[TreePrint.Node]] = None, indent: int = 4,
-                     colors: _Optional[_Mapping[str, str]] = None, mode: str='-'):
+
+        def __init__(
+            self,
+            value: _Union[str, int],
+            children: _Optional[_List[TreePrint.Node]] = None,
+            indent: int = 4,
+            colors: _Optional[_Mapping[str, str]] = None,
+            mode: str = '-'
+        ):
             self.value = str(value)
             if children:
                 self._children = children
             else:
                 self._children = []
             self.indent = indent
             self.colors = {
@@ -78,15 +89,16 @@
                         prefix_ += prefix[j]
 
                 if i + 1 == len(self._children):
                     prefix_ += chars[6]  # └ OR ╚
                 else:
                     prefix_ += chars[5]  # ├ OR ╠
                 prefix_ += chars[0] * (self.indent - 1)  # ─ OR ═
-                prefix_ = prefix_[:len(prefix)] + _gc(self.colors['branches']) + prefix_[len(prefix):]
+                prefix_ = prefix_[:len(prefix)] + _gc(self.colors['branches']
+                                                      ) + prefix_[len(prefix):]
                 text += child.__str__(level=level + 1, prefix=prefix_, mode=mode)
 
             return text
 
         def has_child(self):
             return len(self._children) > 0
 
@@ -103,67 +115,109 @@
             if value:
                 for child in self._children:
                     if child.value == value:
                         return child
             if index:
                 return self._children[index]
 
-        @staticmethod
-        def add_to(node: TreePrint.Node, data: _Union[_Mapping, _Sequence, str, int], indent: int = 4,
-                   colors: _Optional[_Mapping[str, str]] = None, mode='-'):
+        def add_to(
+            self: TreePrint.Node,
+            data: _Union[_Mapping, _Sequence, str, int],
+            indent: int = 4,
+            colors: _Optional[_Mapping[str, str]] = None,
+            mode='-'
+        ):
             if isinstance(data, _Mapping):
                 if len(data) == 1:
-                    child = TreePrint.Node(list(data.keys())[0], indent=indent, colors=colors, mode=mode)
-                    TreePrint.Node.add_to(child, list(data.values())[0], indent=indent, colors=colors, mode=mode)
-                    node.add_child(child)
+                    child = TreePrint.Node(
+                        list(data.keys())[0], indent=indent, colors=colors, mode=mode
+                    )
+                    child.add_to(
+                        list(data.values())[0], indent=indent, colors=colors, mode=mode
+                    )
+                    self.add_child(child)
                 else:
                     for key, value in data.items():
-                        child = TreePrint.Node(key, indent=indent, colors=colors, mode=mode)
-                        TreePrint.Node.add_to(child, value, indent=indent, colors=colors, mode=mode)
-                        node.add_child(child)
-            elif isinstance(data, _Sequence):
-                for value in data:
-                    if isinstance(value, _Mapping):
-                        for key, dict_value in value.items():
-                            child = TreePrint.Node(key, indent=indent, colors=colors, mode=mode)
-                            TreePrint.Node.add_to(child, dict_value, indent=indent, colors=colors, mode=mode)
-                            node.add_child(child)
-                    elif isinstance(value, _Sequence):
-                        child = TreePrint.Node('>', indent=indent, colors=colors, mode=mode)
-                        TreePrint.Node.add_to(child, value, indent=indent, colors=colors, mode=mode)
-                        node.add_child(child)
-                    else:
-                        child = TreePrint.Node(str(value), indent=indent, colors=colors, mode=mode)
-                        node.add_child(child)
+                        child = TreePrint.Node(
+                            key, indent=indent, colors=colors, mode=mode
+                        )
+                        child.add_to(value, indent=indent, colors=colors, mode=mode)
+                        self.add_child(child)
+            elif isinstance(data, _Sequence) and not isinstance(data, str):
+                if len(data) == 1:
+                    self.add_child(
+                        TreePrint.Node(
+                            data[0], indent=indent, colors=colors, mode=mode
+                        )
+                    )
+                else:
+                    for value in data:
+                        if isinstance(value, _Mapping):
+                            for key, dict_value in value.items():
+                                child = TreePrint.Node(
+                                    key, indent=indent, colors=colors, mode=mode
+                                )
+                                child.add_to(
+                                    dict_value, indent=indent, colors=colors, mode=mode
+                                )
+                                self.add_child(child)
+                        elif isinstance(value, _Sequence):
+                            child = TreePrint.Node(
+                                '>', indent=indent, colors=colors, mode=mode
+                            )
+                            child.add_to(value, indent=indent, colors=colors, mode=mode)
+                            self.add_child(child)
+                        else:
+                            child = TreePrint.Node(
+                                str(value), indent=indent, colors=colors, mode=mode
+                            )
+                            self.add_child(child)
             else:
-                child = TreePrint.Node(str(data), indent=indent, colors=colors, mode=mode)
-                node.add_child(child)
-
-    def __init__(self, data: _Union[_Mapping, _Sequence, str, int], indent: int = 4, 
-                 colors: _Optional[_Mapping[str, str]] = None, mode='-'):
+                child = TreePrint.Node(
+                    str(data), indent=indent, colors=colors, mode=mode
+                )
+                self.add_child(child)
+
+    def __init__(
+        self,
+        data: _Union[_Mapping, _Sequence, str, int],
+        indent: int = 4,
+        colors: _Optional[_Mapping[str, str]] = None,
+        mode='-'
+    ):
         self.indent = indent
         self.mode = mode
         if isinstance(data, _Mapping):
             if len(data) == 1:
-                self.root = self.Node(list(data.keys())[0], indent=indent, colors=colors)
+                self.root = self.Node(
+                    list(data.keys())[0], indent=indent, colors=colors
+                )
                 self.add_to_root(list(data.values()), colors=colors)
             else:
                 self.root = self.Node('root', indent=indent, colors=colors)
                 self.add_to_root(data, colors=colors)
         elif isinstance(data, _Sequence):
             self.root = self.Node('root', indent=indent, colors=colors)
             self.add_to_root(data, colors=colors)
         else:
             self.root = self.Node(str(data), indent=indent, colors=colors)
 
-    def add_to_root(self, data: _Union[_Mapping, _Sequence, str, int], colors: _Optional[_Mapping[str, str]] = None):
-        self.Node.add_to(self.root, data, indent=self.indent, colors=colors, mode=self.mode)
+    def add_to_root(
+        self,
+        data: _Union[_Mapping, _Sequence, str, int],
+        colors: _Optional[_Mapping[str, str]] = None
+    ):
+        self.root.add_to(data, indent=self.indent, colors=colors, mode=self.mode)
 
     def __str__(self, mode=None):
         if not mode:
             mode = self.mode
         return self.root.__str__(mode=mode)
 
 
-def tree_format(data: _Union[_Mapping, _Sequence, str, int], indent: int = 4, mode='-',
-                colors: _Optional[_Mapping[str, str]] = None):
+def tree_format(
+    data: _Union[_Mapping, _Sequence, str, int],
+    indent: int = 4,
+    mode='-',
+    colors: _Optional[_Mapping[str, str]] = None
+):
     return str(TreePrint(data, indent=indent, colors=colors, mode=mode))
```

### Comparing `log21-2.5.4/log21/__init__.py` & `log21-2.6.0/src/log21/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,116 @@
 # log21.__init__.py
 # CodeWriter21
 
 import io as _io
 import os as _os
 import logging as _logging
+from typing import (Type as _Type, Tuple as _Tuple, Union as _Union,
+                    Mapping as _Mapping, Optional as _Optional)
 
-from typing import Union as _Union, Mapping as _Mapping, Type as _Type, Tuple as _Tuple, Optional as _Optional
-
-import log21.CrashReporter as CrashReporter
-
-from log21.Levels import INPUT, CRITICAL, FATAL, ERROR, WARNING, WARN, INFO, DEBUG, NOTSET
+from log21 import CrashReporter
+from log21.Colors import (Colors, get_color, get_colors, ansi_escape, closest_color,
+                          get_color_name)
+from log21.Levels import (INFO, WARN, DEBUG, ERROR, FATAL, INPUT, NOTSET, WARNING,
+                          CRITICAL)
 from log21.Logger import Logger
-from log21.Manager import Manager
-from log21.ProgressBar import ProgressBar
 from log21.PPrint import PrettyPrinter, pformat
-from log21.TreePrint import TreePrint, tree_format
+from log21.Manager import Manager
 from log21.Argparse import ColorizingArgumentParser
+from log21.TreePrint import TreePrint, tree_format
+from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
+from log21.Argumentify import argumentify
 from log21.FileHandler import DecolorizingFileHandler
+from log21.ProgressBar import ProgressBar
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
-from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
-from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
-from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
+from log21.StreamHandler import StreamHandler, ColorizingStreamHandler
 
-__version__ = "2.5.4"
+__version__ = "2.6.0"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
-__all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
-           'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
-           'INFO', 'DEBUG', 'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
-           'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
-           'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
-           'critical', 'fatal', 'exception', 'log', 'basic_config', 'basicConfig', 'ProgressBar', 'progress_bar',
-           'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter', 'console_reporter',
-           'file_reporter']
+__all__ = [
+    'ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter',
+    'DecolorizingFormatter', 'get_logger', 'Logger', 'Colors', 'get_color',
+    'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN', 'INFO', 'DEBUG',
+    'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter',
+    'pformat', 'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager',
+    'get_color_name', 'closest_color', 'ansi_escape', '__version__', '__author__',
+    '__github__', 'debug', 'info', 'warning', 'warn', 'error', 'critical', 'fatal',
+    'exception', 'log', 'basic_config', 'basicConfig', 'ProgressBar', 'progress_bar',
+    'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter',
+    'console_reporter', 'file_reporter', 'argumentify'
+]
 
 _manager = Manager()
 _logging.setLoggerClass(Logger)
 
 
-def _prepare_formatter(fmt: _Optional[str] = None, style: str = '%', datefmt: str = "%H:%M:%S",
-                       show_level: bool = True, show_time: bool = True, colorize_time_and_level: bool = True,
-                       level_names: _Optional[_Mapping[int, str]] = None,
-                       level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
-                       formatter_class: _Type[_logging.Formatter] = ColorizingFormatter):
+def _prepare_formatter(
+    fmt: _Optional[str] = None,
+    style: str = '%',
+    datefmt: str = "%H:%M:%S",
+    show_level: bool = True,
+    show_time: bool = True,
+    colorize_time_and_level: bool = True,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
+    formatter_class: _Type[_logging.Formatter] = ColorizingFormatter
+):
     # Prepares a formatting if the fmt was None
     if not fmt:
         style = '%'
         fmt = "%(message)s"
         if show_level:
             fmt = "[%(levelname)s] " + fmt
         if show_time:
             fmt = "[%(asctime)s] " + fmt
         fmt = '\r' + fmt
 
     if level_colors and not issubclass(formatter_class, ColorizingFormatter):
-        warning('`formatter_class` should be a subclass of ColorizingFormatter when used with level_colors.')
-        warning(f'Using `{formatter_class.__name__}` might lead to unexpected behaviour!')
+        warning(
+            '`formatter_class` should be a subclass of ColorizingFormatter when used with level_colors.'
+        )
+        warning(
+            f'Using `{formatter_class.__name__}` might lead to unexpected behaviour!'
+        )
 
     # Defines the formatter
     if level_colors:
-        formatter = formatter_class(fmt, datefmt, style=style, level_colors=level_colors)
+        formatter = formatter_class(
+            fmt, datefmt, style=style, level_colors=level_colors
+        )
     else:
         formatter = formatter_class(fmt, datefmt, style=style)
-    
+
     if isinstance(formatter, Formatters._Formatter) and level_names:
         formatter.level_names = level_names
     if not colorize_time_and_level and isinstance(formatter, ColorizingFormatter):
         for key in formatter.level_colors:
             formatter.level_colors[key] = tuple()
         formatter.time_color = tuple()
 
     return formatter
 
 
-def get_logger(name: str = '', level: _Union[int, str] = NOTSET, show_time: bool = True,
-               show_level: bool = True, colorize_time_and_level: bool = True, fmt: _Optional[str] = None,
-               datefmt: str = "%H:%M:%S", style: str = '%', handle_carriage_return: bool = True,
-               handle_new_line: bool = True, override=False, level_names: _Optional[_Mapping[int, str]] = None,
-               level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
-               file: _Optional[_Union[_os.PathLike, str]] = None) -> _Union[Logger, _logging.Logger]:
+def get_logger(
+    name: str = '',
+    level: _Union[int, str] = NOTSET,
+    show_time: bool = True,
+    show_level: bool = True,
+    colorize_time_and_level: bool = True,
+    fmt: _Optional[str] = None,
+    datefmt: str = "%H:%M:%S",
+    style: str = '%',
+    handle_carriage_return: bool = True,
+    handle_new_line: bool = True,
+    override=False,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
+    file: _Optional[_Union[_os.PathLike, str]] = None
+) -> _Union[Logger, _logging.Logger]:
     """
     Returns a logging.Logger with colorizing support.
     >>>
     >>> import log21
     >>>
     >>> l = log21.get_logger()
     >>> l.warning('Pretty basic, huh?')
@@ -144,41 +172,64 @@
     if not isinstance(name, str):
         raise TypeError('A logger name must be a string')
     logger = None
     if name:
         logger = _manager.getLogger(name)
     if (not logger) or override:
         logger = Logger(name, level)
-        formatter = _prepare_formatter(fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
-                                       level_names, level_colors)
+        formatter = _prepare_formatter(
+            fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
+            level_names, level_colors
+        )
 
         # Defines the handler
-        handler = ColorizingStreamHandler(handle_carriage_return=handle_carriage_return,
-                                          handle_new_line=handle_new_line)
+        handler = ColorizingStreamHandler(
+            handle_carriage_return=handle_carriage_return,
+            handle_new_line=handle_new_line
+        )
         handler.setFormatter(formatter)
         logger.addHandler(handler)
         _manager.addLogger(name, logger)
 
         if file:
             file_handler = FileHandler.FileHandler(file)
-            file_formatter = _prepare_formatter(fmt, style, datefmt, show_level, show_time, False, level_names,
-                                                formatter_class=Formatters.DecolorizingFormatter)
+            file_formatter = _prepare_formatter(
+                fmt,
+                style,
+                datefmt,
+                show_level,
+                show_time,
+                False,
+                level_names,
+                formatter_class=Formatters.DecolorizingFormatter
+            )
             file_handler.setFormatter(file_formatter)
             logger.addHandler(file_handler)
 
     return logger
 
 
-def get_logging_window(name: str = '', level: _Union[int, str] = NOTSET, show_time: bool = True,
-                       show_level: bool = True, colorize_time_and_level: bool = True, fmt: _Optional[str] = None,
-                       datefmt: str = "%H:%M:%S", style: str = '%', handle_carriage_return: bool = True,
-                       handle_new_line: bool = True, override=False, level_names: _Optional[_Mapping[int, str]] = None,
-                       width: int = 80, height: int = 20, allow_shell: bool = False) -> LoggingWindow:
-    """
-    Returns a logging window.
+def get_logging_window(
+    name: str = '',
+    level: _Union[int, str] = NOTSET,
+    show_time: bool = True,
+    show_level: bool = True,
+    colorize_time_and_level: bool = True,
+    fmt: _Optional[str] = None,
+    datefmt: str = "%H:%M:%S",
+    style: str = '%',
+    handle_carriage_return: bool = True,
+    handle_new_line: bool = True,
+    override=False,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    width: int = 80,
+    height: int = 20,
+    allow_shell: bool = False
+) -> LoggingWindow:
+    """Returns a logging window.
 
     >>> # Let's see how it works
     >>> # Imports log21 and time modules
     >>> import log21, time
     >>> # Creates a new LoggingWindow object
     >>> window = log21.get_logging_window('Test Window')
     >>> # Now use it without any additional steps to add handlers and formatters!
@@ -228,20 +279,28 @@
     """
     if not isinstance(name, str):
         raise TypeError('A logger name must be a string')
     logging_window = None
     if name:
         logging_window = _manager.getLogger(name)
     if (not logging_window) or override:
-        logging_window = LoggingWindow(name, level=level, width=width, height=height, allow_shell=allow_shell)
-        formatter = _prepare_formatter(fmt, style, datefmt, show_level, show_time, colorize_time_and_level, level_names)
+        logging_window = LoggingWindow(
+            name, level=level, width=width, height=height, allow_shell=allow_shell
+        )
+        formatter = _prepare_formatter(
+            fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
+            level_names
+        )
 
         # Defines the handler
-        handler = LoggingWindowHandler(logging_window, handle_carriage_return=handle_carriage_return,
-                                       handle_new_line=handle_new_line)
+        handler = LoggingWindowHandler(
+            logging_window,
+            handle_carriage_return=handle_carriage_return,
+            handle_new_line=handle_new_line
+        )
         handler.setFormatter(formatter)
         logging_window.addHandler(handler)
         _manager.addLogger(name, logging_window)
     return logging_window
 
 
 getLogger = get_logger
@@ -258,39 +317,82 @@
 
 
 def getpass(*msg, args: tuple = (), end='', **kwargs):
     logger = get_logger('log21.getpass', level=DEBUG, show_time=False, show_level=False)
     return logger.getpass(*msg, args=args, end=end, **kwargs)
 
 
-def pprint(obj, indent=1, width=80, depth=None, signs_colors: _Optional[_Mapping[str, str]] = None, *, sort_dicts=True,
-           underscore_numbers=False, compact=False, end='\033[0m\n', **kwargs):
+def pprint(
+    obj,
+    indent=1,
+    width=80,
+    depth=None,
+    signs_colors: _Optional[_Mapping[str, str]] = None,
+    *,
+    sort_dicts=True,
+    underscore_numbers=False,
+    compact=False,
+    end='\033[0m\n',
+    **kwargs
+):
     logger = get_logger('log21.pprint', level=DEBUG, show_time=False, show_level=False)
-    logger.print(pformat(obj=obj, indent=indent, width=width, depth=depth, signs_colors=signs_colors, compact=compact,
-                         sort_dicts=sort_dicts, underscore_numbers=underscore_numbers), end=end, **kwargs)
+    logger.print(
+        pformat(
+            obj=obj,
+            indent=indent,
+            width=width,
+            depth=depth,
+            signs_colors=signs_colors,
+            compact=compact,
+            sort_dicts=sort_dicts,
+            underscore_numbers=underscore_numbers
+        ),
+        end=end,
+        **kwargs
+    )
 
 
 pretty_print = pprint
 
 
-def tree_print(obj, indent: int = 4, mode='-', colors: _Mapping[str, str] = None, end='\033[0m\n', **kwargs):
-    logger = get_logger('log21.tree_print', level=DEBUG, show_time=False, show_level=False)
-    logger.print(tree_format(obj, indent=indent, mode=mode, colors=colors), end=end, **kwargs)
+def tree_print(
+    obj,
+    indent: int = 4,
+    mode='-',
+    colors: _Mapping[str, str] = None,
+    end='\033[0m\n',
+    **kwargs
+):
+    logger = get_logger(
+        'log21.tree_print', level=DEBUG, show_time=False, show_level=False
+    )
+    logger.print(
+        tree_format(obj, indent=indent, mode=mode, colors=colors), end=end, **kwargs
+    )
 
 
 tprint = tree_print
 
 root = Logger('root-logger', INFO)
 
 
-def basic_config(force: bool = False, encoding: str = None, errors: _Optional[str] = 'backslashreplace', handlers=None,
-                 stream=None, filename=None, filemode: str = 'a', date_format: str = "%H:%M:%S", style: str = '%',
-                 format_: str = None, level: _Union[int, str] = None):
-    """
-    Do basic configuration for the logging system.
+def basic_config(
+    force: bool = False,
+    encoding: str = None,
+    errors: _Optional[str] = 'backslashreplace',
+    handlers=None,
+    stream=None,
+    filename=None,
+    filemode: str = 'a',
+    date_format: str = "%H:%M:%S",
+    style: str = '%',
+    format_: str = None,
+    level: _Union[int, str] = None
+):
+    """Do basic configuration for the logging system.
 
     This function does nothing if the root logger already has handlers
     configured, unless the keyword argument *force* is set to ``True``.
     It is a convenience method intended for use by simple scripts
     to do one-shot configuration of the logging package.
 
     The default behaviour is to create a ColorizingStreamHandler which writes to
@@ -339,34 +441,42 @@
     if force:
         for handler in root.handlers[:]:
             root.removeHandler(handler)
             handler.close()
     if len(root.handlers) == 0:
         if handlers is None:
             if stream and filename:
-                raise ValueError("'stream' and 'filename' should not be specified together")
+                raise ValueError(
+                    "'stream' and 'filename' should not be specified together"
+                )
         else:
             if stream or filename:
-                raise ValueError("'stream' or 'filename' should not be specified together with 'handlers'")
+                raise ValueError(
+                    "'stream' or 'filename' should not be specified together with 'handlers'"
+                )
         if handlers is None:
             if filename:
                 if 'b' in filemode:
                     errors = None
                 else:
                     encoding = _io.text_encoding(encoding)
-                handler = DecolorizingFileHandler(filename, filemode, encoding=encoding, errors=errors)
+                handler = DecolorizingFileHandler(
+                    filename, filemode, encoding=encoding, errors=errors
+                )
             else:
                 handler = ColorizingStreamHandler(stream=stream)
             handlers = [handler]
         if style not in '%{$':
             raise ValueError('Style must be one of: %, {, $')
         if not format_:
-            format_ = {'%': '[%(asctime)s] [%(levelname)s] %(message)s',
-                       '{': '[{asctime}] [{levelname}] {message}',
-                       '$': '[${asctime}] [${levelname}] ${message}'}[style]
+            format_ = {
+                '%': '[%(asctime)s] [%(levelname)s] %(message)s',
+                '{': '[{asctime}] [{levelname}] {message}',
+                '$': '[${asctime}] [${levelname}] ${message}'
+            }[style]
         else:
             format_ = format_
         formatter = ColorizingFormatter(format_, date_format, style=style)
         for handler in handlers:
             if handler.formatter is None:
                 handler.setFormatter(formatter)
             root.addHandler(handler)
@@ -374,99 +484,111 @@
             root.setLevel(level)
 
 
 basicConfig = basic_config
 
 
 def critical(*msg, args=(), **kwargs):
-    """
-    Log a message with severity 'CRITICAL' on the root logger. If the logger has no handlers, call basicConfig() to add
-    a console handler with a pre-defined format.
+    """Log a message with severity 'CRITICAL' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console
+    handler with a pre-defined format.
     """
     if len(root.handlers) == 0:
         basic_config()
     root.critical(*msg, args=args, **kwargs)
 
 
 def fatal(*msg, args=(), **kwargs):
-    """
-    Don't use this function, use critical() instead.
-    """
+    """Don't use this function, use critical() instead."""
     critical(*msg, args=args, **kwargs)
 
 
 def error(*msg, args=(), **kwargs):
-    """
-    Log a message with severity 'ERROR' on the root logger. If the logger has no handlers, call basicConfig() to add a
-    console handler with a pre-defined format.
+    """Log a message with severity 'ERROR' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console
+    handler with a pre-defined format.
     """
     if len(root.handlers) == 0:
         basic_config()
     root.error(*msg, args=args, **kwargs)
 
 
 def exception(*msg, args=(), exc_info=True, **kwargs):
-    """
-    Log a message with severity 'ERROR' on the root logger, with exception information. If the logger has no handlers,
-    basicConfig() is called to add a console handler with a pre-defined format.
+    """Log a message with severity 'ERROR' on the root logger, with exception
+    information.
+
+    If the logger has no handlers, basicConfig() is called to add a
+    console handler with a pre-defined format.
     """
     error(*msg, args=args, exc_info=exc_info, **kwargs)
 
 
 def warning(*msg, args=(), **kwargs):
-    """
-    Log a message with severity 'WARNING' on the root logger. If the logger has no handlers, call basicConfig() to add
-    a console handler with a pre-defined format.
+    """Log a message with severity 'WARNING' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console
+    handler with a pre-defined format.
     """
     if len(root.handlers) == 0:
         basic_config()
     root.warning(*msg, args=args, **kwargs)
 
 
 def warn(*msg, args=(), **kwargs):
     warning(*msg, args=args, **kwargs)
 
 
 def info(*msg, args=(), **kwargs):
-    """
-    Log a message with severity 'INFO' on the root logger. If the logger has no handlers, call basicConfig() to add a
-    console handler with a pre-defined format.
+    """Log a message with severity 'INFO' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console
+    handler with a pre-defined format.
     """
     if len(root.handlers) == 0:
         basic_config()
     root.info(*msg, args=args, **kwargs)
 
 
 def debug(*msg, args=(), **kwargs):
-    """
-    Log a message with severity 'DEBUG' on the root logger. If the logger has no handlers, call basicConfig() to add a
-    console handler with a pre-defined format.
+    """Log a message with severity 'DEBUG' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console
+    handler with a pre-defined format.
     """
     if len(root.handlers) == 0:
         basic_config()
     root.debug(*msg, args=args, **kwargs)
 
 
 def log(level, *msg, args=(), **kwargs):
-    """
-    Log 'msg % args' with the integer severity 'level' on the root logger. If the logger has no handlers, call
-    basicConfig() to add a console handler with a pre-defined format.
+    """Log 'msg % args' with the integer severity 'level' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console
+    handler with a pre-defined format.
     """
     if len(root.handlers) == 0:
         basic_config()
     root.log(level, *msg, args=args, **kwargs)
 
 
-def progress_bar(progress: float, total: float, width: _Optional[int] = None, prefix: str = '|', suffix: str = '|',
-                 show_percentage: bool = True):
-    """
-    Print a progress bar to the console.
-    """
-
-    bar = ProgressBar(width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage)
+def progress_bar(
+    progress: float,
+    total: float,
+    width: _Optional[int] = None,
+    prefix: str = '|',
+    suffix: str = '|',
+    show_percentage: bool = True
+):
+    """Print a progress bar to the console."""
+
+    bar = ProgressBar(
+        width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage
+    )
 
     print(bar.get_bar(progress, total))
 
 
 console_reporter = CrashReporter.ConsoleReporter()
 
 file_reporter = CrashReporter.FileReporter(file='crash_report.log')
```

### Comparing `log21-2.5.4/pyproject.toml` & `log21-2.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,19 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Unix",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X"
 ]
 dependencies = [
-  "webcolors"
+  "webcolors",
+  "docstring-parser"
 ]
-version = "2.5.4"
+version = "2.6.0"
+
+[tool.setuptools.packages.find]
+where = ["src"]
 
 [project.urls]
 Homepage = "https://github.com/MPCodeWriter21/log21"
 Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
 Source = "https://github.com/MPCodeWriter21/log21"
```

