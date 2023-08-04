# Comparing `tmp/sinol-make-1.3.1.tar.gz` & `tmp/sinol-make-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-1.3.1.tar", last modified: Sat Jul 22 14:36:50 2023, max compression
+gzip compressed data, was "sinol-make-1.4.0.tar", last modified: Fri Aug  4 21:38:22 2023, max compression
```

## Comparing `sinol-make-1.3.1.tar` & `sinol-make-1.4.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-22 14:36:38.000000 sinol-make-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-22 14:36:50.028787 sinol-make-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-22 14:36:38.000000 sinol-make-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-22 14:36:38.000000 sinol-make-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 14:36:50.028787 sinol-make-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.024787 sinol-make-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.024787 sinol-make-1.3.1/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.024787 sinol-make-1.3.1/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/commands/inwer/
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/inwer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/inwer/inwer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/inwer/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    46165 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/package_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/structs/compiler_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.024787 sinol-make-1.3.1/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-22 14:36:38.000000 sinol-make-1.3.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-04 21:38:09.000000 sinol-make-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 21:38:22.438460 sinol-make-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-04 21:38:09.000000 sinol-make-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-04 21:38:09.000000 sinol-make-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:38:22.438460 sinol-make-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.434460 sinol-make-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.434460 sinol-make-1.4.0/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.434460 sinol-make-1.4.0/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/commands/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/gen/gen_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/gen/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/inwer/inwer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/inwer/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    46043 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-08-04 21:38:09.000000 sinol-make-1.4.0/tests/test_util.py
```

### Comparing `sinol-make-1.3.1/LICENSE` & `sinol-make-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/PKG-INFO` & `sinol-make-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.3.1
+Version: 1.4.0
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sinol-make-1.3.1/README.md` & `sinol-make-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/pyproject.toml` & `sinol-make-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/src/sinol_make/__init__.py` & `sinol-make-1.4.0/src/sinol_make/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argcomplete
 import argparse
 import sys
 
 from sinol_make import util
 
-__version__ = "1.3.1"
+__version__ = "1.4.0"
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
     parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
```

### Comparing `sinol-make-1.3.1/src/sinol_make/commands/inwer/__init__.py` & `sinol-make-1.4.0/src/sinol_make/commands/inwer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,15 @@
         parser.add_argument('-c', '--cpus', type=int,
                             help=f'number of cpus to use, by default {mp.cpu_count()} (all available)')
         add_compilation_arguments(parser)
 
     def compile_inwer(self, args: argparse.Namespace):
         self.inwer_executable, compile_log_path = inwer_util.compile_inwer(self.inwer, args, args.weak_compilation_flags)
         if self.inwer_executable is None:
-            print(util.error('Compilation failed.'))
-            compile.print_compile_log(compile_log_path)
-            exit(1)
+            util.exit_with_error('Compilation failed.', lambda: compile.print_compile_log(compile_log_path))
         else:
             print(util.info('Compilation successful.'))
 
     @staticmethod
     def verify_test(execution: InwerExecution) -> VerificationResult:
         """
         Verifies a test and returns the result of inwer on this test.
```

### Comparing `sinol-make-1.3.1/src/sinol_make/commands/inwer/inwer_util.py` & `sinol-make-1.4.0/src/sinol_make/commands/inwer/inwer_util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/src/sinol_make/commands/inwer/structs.py` & `sinol-make-1.4.0/src/sinol_make/commands/inwer/structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/src/sinol_make/commands/run/__init__.py` & `sinol-make-1.4.0/src/sinol_make/commands/run/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,18 +362,16 @@
             if len(checker_output) >= 3:
                 try:
                     points = int(checker_output[2].strip())
                 except ValueError:
                     pass
 
             return True, points
-        elif checker_output[0].strip() == "WRONG":
-            return False, 0
         else:
-            raise CheckerOutputException("Checker output is invalid.")
+            return False, 0
 
 
     def check_output(self, name, input_file, output_file_path, output, answer_file_path):
         """
         Checks if the output file is correct.
         Returns a tuple (is correct, number of points).
         """
```

### Comparing `sinol-make-1.3.1/src/sinol_make/commands/run/structs.py` & `sinol-make-1.4.0/src/sinol_make/commands/run/structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/src/sinol_make/helpers/compile.py` & `sinol-make-1.4.0/src/sinol_make/helpers/compile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Tuple
+import os
+import sys
+import stat
+import subprocess
 
 import sinol_make.helpers.compiler as compiler
 from sinol_make.interfaces.Errors import CompilationError
 from sinol_make.structs.compiler_structs import Compilers
-import os, subprocess, sys
+
 
 def compile(program, output, compilers: Compilers = None, compile_log = None, weak_compilation_flags = False):
     """
     Compile a program
     compilers - A Compilers object with compilers to use. If None, default compilers will be used.
     """
     gcc_compilation_flags = '-Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'
@@ -28,15 +32,16 @@
     elif ext == '.py':
         if sys.platform == 'win32' or sys.platform == 'cygwin':
             # TODO: Make this work on Windows
             pass
         else:
             open(output, 'w').write('#!/usr/bin/python3\n')
             open(output, 'a').write(open(program, 'r').read())
-            subprocess.call(['chmod', '+x', output])
+            st = os.stat(output)
+            os.chmod(output, st.st_mode | stat.S_IEXEC)
         arguments = [compilers.python_interpreter_path, '-m', 'py_compile', program]
     elif ext == '.java':
         raise NotImplementedError('Java compilation is not implemented')
     else:
         raise CompilationError('Unknown file extension: ' + ext)
 
     process = subprocess.Popen(arguments, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
```

### Comparing `sinol-make-1.3.1/src/sinol_make/helpers/compiler.py` & `sinol-make-1.4.0/src/sinol_make/helpers/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,26 @@
 
     if not check_if_installed('javac'):
         return None
     else:
         return 'javac'
 
 
+def get_default_compilers():
+    """
+    Get the default compilers
+    """
+    return argparse.Namespace(
+        c_compiler_path=get_c_compiler_path(),
+        cpp_compiler_path=get_cpp_compiler_path(),
+        python_interpreter_path=get_python_interpreter_path(),
+        java_compiler_path=get_java_compiler_path()
+    )
+
+
 def verify_compilers(args: argparse.Namespace, solutions: list[str]) -> Compilers:
     for solution in solutions:
         ext = os.path.splitext(solution)[1]
         compiler = ""
         tried = ""
         flag = ""
         if ext == '.c' and args.c_compiler_path is None:
```

### Comparing `sinol-make-1.3.1/src/sinol_make/helpers/package_util.py` & `sinol-make-1.4.0/src/sinol_make/helpers/package_util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/src/sinol_make/helpers/parsers.py` & `sinol-make-1.4.0/src/sinol_make/helpers/parsers.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/src/sinol_make/helpers/printer.py` & `sinol-make-1.4.0/src/sinol_make/helpers/printer.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/src/sinol_make/structs/compiler_structs.py` & `sinol-make-1.4.0/src/sinol_make/structs/compiler_structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.1/src/sinol_make/util.py` & `sinol-make-1.4.0/src/sinol_make/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -259,22 +259,33 @@
         terminal_height = os.get_terminal_size().lines
     except OSError:
         has_terminal = False
         terminal_width = 80
         terminal_height = 30
     return has_terminal, terminal_width, terminal_height
 
+
+def fix_file_endings(file):
+    with open(file, "rb") as f:
+        content = f.read()
+    with open(file, "wb") as f:
+        f.write(content.replace(b"\r\n", b"\n"))
+
+
 def color_red(text): return "\033[91m{}\033[00m".format(text)
 def color_green(text): return "\033[92m{}\033[00m".format(text)
 def color_yellow(text): return "\033[93m{}\033[00m".format(text)
 def bold(text): return "\033[01m{}\033[00m".format(text)
 
 def info(text):
     return bold(color_green(text))
 def warning(text):
     return bold(color_yellow(text))
 def error(text):
     return bold(color_red(text))
 
-def exit_with_error(text):
+
+def exit_with_error(text, func=None):
     print(error(text))
+    if func is not None:
+        func()
     exit(1)
```

### Comparing `sinol-make-1.3.1/src/sinol_make.egg-info/PKG-INFO` & `sinol-make-1.4.0/src/sinol_make.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.3.1
+Version: 1.4.0
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sinol-make-1.3.1/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.4.0/src/sinol_make.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 src/sinol_make/util.py
 src/sinol_make.egg-info/PKG-INFO
 src/sinol_make.egg-info/SOURCES.txt
 src/sinol_make.egg-info/dependency_links.txt
 src/sinol_make.egg-info/entry_points.txt
 src/sinol_make.egg-info/requires.txt
 src/sinol_make.egg-info/top_level.txt
+src/sinol_make/commands/gen/__init__.py
+src/sinol_make/commands/gen/gen_util.py
+src/sinol_make/commands/gen/structs.py
 src/sinol_make/commands/inwer/__init__.py
 src/sinol_make/commands/inwer/inwer_util.py
 src/sinol_make/commands/inwer/structs.py
 src/sinol_make/commands/run/__init__.py
 src/sinol_make/commands/run/structs.py
 src/sinol_make/helpers/__init__.py
 src/sinol_make/helpers/compile.py
```

### Comparing `sinol-make-1.3.1/tests/test_util.py` & `sinol-make-1.4.0/tests/test_util.py`

 * *Files identical despite different names*

