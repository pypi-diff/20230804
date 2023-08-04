# Comparing `tmp/logfunc-1.4.1.tar.gz` & `tmp/logfunc-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-1.4.1.tar", last modified: Fri Jun 30 15:02:21 2023, max compression
+gzip compressed data, was "logfunc-1.5.0.tar", last modified: Fri Aug  4 00:57:09 2023, max compression
```

## Comparing `logfunc-1.4.1.tar` & `logfunc-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 15:02:21.476024 logfunc-1.4.1/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.4.1/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     4191 2023-06-30 15:02:21.475919 logfunc-1.4.1/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     3226 2023-06-30 07:40:13.000000 logfunc-1.4.1/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 15:02:21.475247 logfunc-1.4.1/logfunc/
--rw-r--r--   0 work       (501) staff       (20)     5659 2023-06-30 14:51:50.000000 logfunc-1.4.1/logfunc/__init__.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 15:02:21.475758 logfunc-1.4.1/logfunc.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     4191 2023-06-30 15:02:21.000000 logfunc-1.4.1/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      170 2023-06-30 15:02:21.000000 logfunc-1.4.1/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-06-30 15:02:21.000000 logfunc-1.4.1/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-06-30 15:02:21.000000 logfunc-1.4.1/logfunc.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-06-30 15:02:21.476057 logfunc-1.4.1/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)     1219 2023-06-30 15:01:49.000000 logfunc-1.4.1/setup.py
+drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-04 00:57:09.509585 logfunc-1.5.0/
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     1068 2023-06-24 05:08:03.000000 logfunc-1.5.0/LICENSE
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     4281 2023-08-04 00:57:09.509585 logfunc-1.5.0/PKG-INFO
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     3417 2023-08-04 00:55:39.000000 logfunc-1.5.0/README.md
+drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-04 00:57:09.509585 logfunc-1.5.0/logfunc/
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     6116 2023-08-04 00:54:29.000000 logfunc-1.5.0/logfunc/__init__.py
+drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-04 00:57:09.509585 logfunc-1.5.0/logfunc.egg-info/
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     4281 2023-08-04 00:57:09.000000 logfunc-1.5.0/logfunc.egg-info/PKG-INFO
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)      170 2023-08-04 00:57:09.000000 logfunc-1.5.0/logfunc.egg-info/SOURCES.txt
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)        1 2023-08-04 00:57:09.000000 logfunc-1.5.0/logfunc.egg-info/dependency_links.txt
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)        8 2023-08-04 00:57:09.000000 logfunc-1.5.0/logfunc.egg-info/top_level.txt
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)       38 2023-08-04 00:57:09.509585 logfunc-1.5.0/setup.cfg
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     1121 2023-08-04 00:56:44.000000 logfunc-1.5.0/setup.py
```

### Comparing `logfunc-1.4.1/LICENSE` & `logfunc-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-1.4.1/PKG-INFO` & `logfunc-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.4.1
+Version: 1.5.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logf
 
-`@logf()` is a decorator designed to enable effortless and automatic logging of your Python functions' execution, requiring zero configuration for basic usage. Formerly a part of the myfuncs pip package, it is now a standalone pip package. This repository is dedicated to its continued development and maintenance.
+`@logf()` is a decorator designed to enable effortless logging of your Python functions' execution, requiring zero configuration for basic usage. Formerly a part of the myfuncs pip package, it is now a standalone pip package. This repository is dedicated to its continued development and maintenance.
 
 ## Usage
 
 This is a brief guide on how to use the `logfunc` module.
 
 ### Installation
 
@@ -49,29 +47,37 @@
 
 The `logf` function is a decorator that you can apply to any function you want to log:
 
 ```python
 from logfunc import logf
 
 @logf()
-def my_function(a, b):
-    return a + b
+def my_function(a, b='b'):
+    return str(a) + str(b) + 'c'
 ```
 
 In the example above, `logf()` is used to wrap `my_function`. When `my_function` is called, it logs the function name, arguments, return value, and execution time.
 
+```
+>>> my_function('a')
+my_function() | ('a',) {}
+my_function() 0.00051s | abc
+'abc'
+```
+
 ### Customize Logging
 
-The `logf` function allows you to customize your logging:
+The `logf` decorator allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
 - `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `log_exec_time` parameter.
 - You can include the execution time, args, and return value in a single message with the `single_msg` parameter.
+- `use_print` print() log messages rather than logging them
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
 @logf(level='INFO', log_args=False, log_return=True,
@@ -87,14 +93,15 @@
 The `logf` function supports overriding some default/passed parameters with environment variables:
 
 | Env Var          | Example Values       |
 |------------------|-------------|
 | LOGF_LEVEL       | DEBUG INFO WARNING ERROR CRITICAL 10 20 30 40 50|
 | LOGF_MAX_STR_LEN | 10 50 10000000 None NONE none |
 | LOGF_SINGLE_MSG  | True False
+| LOGF_USE_PRINT   | True False
 
 
 ## Testing
 
 This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
 
 To run the tests, navigate to the directory where the `logfunc` package is installed and run:
```

### Comparing `logfunc-1.4.1/README.md` & `logfunc-1.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # logf
 
-`@logf()` is a decorator designed to enable effortless and automatic logging of your Python functions' execution, requiring zero configuration for basic usage. Formerly a part of the myfuncs pip package, it is now a standalone pip package. This repository is dedicated to its continued development and maintenance.
+`@logf()` is a decorator designed to enable effortless logging of your Python functions' execution, requiring zero configuration for basic usage. Formerly a part of the myfuncs pip package, it is now a standalone pip package. This repository is dedicated to its continued development and maintenance.
 
 ## Usage
 
 This is a brief guide on how to use the `logfunc` module.
 
 ### Installation
 
@@ -26,29 +26,37 @@
 
 The `logf` function is a decorator that you can apply to any function you want to log:
 
 ```python
 from logfunc import logf
 
 @logf()
-def my_function(a, b):
-    return a + b
+def my_function(a, b='b'):
+    return str(a) + str(b) + 'c'
 ```
 
 In the example above, `logf()` is used to wrap `my_function`. When `my_function` is called, it logs the function name, arguments, return value, and execution time.
 
+```
+>>> my_function('a')
+my_function() | ('a',) {}
+my_function() 0.00051s | abc
+'abc'
+```
+
 ### Customize Logging
 
-The `logf` function allows you to customize your logging:
+The `logf` decorator allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
 - `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `log_exec_time` parameter.
 - You can include the execution time, args, and return value in a single message with the `single_msg` parameter.
+- `use_print` print() log messages rather than logging them
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
 @logf(level='INFO', log_args=False, log_return=True,
@@ -64,20 +72,21 @@
 The `logf` function supports overriding some default/passed parameters with environment variables:
 
 | Env Var          | Example Values       |
 |------------------|-------------|
 | LOGF_LEVEL       | DEBUG INFO WARNING ERROR CRITICAL 10 20 30 40 50|
 | LOGF_MAX_STR_LEN | 10 50 10000000 None NONE none |
 | LOGF_SINGLE_MSG  | True False
+| LOGF_USE_PRINT   | True False
 
 
 ## Testing
 
 This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
 
 To run the tests, navigate to the directory where the `logfunc` package is installed and run:
 
 ```sh
 python tests.py
 ```
 
-The test suite includes tests for the default behavior of the `logf` decorator as well as its behavior when custom parameters are passed. The tests check whether the function name, arguments, return value, and execution time are correctly logged, and whether the `max_str_len` parameter correctly truncates the logged strings.
+The test suite includes tests for the default behavior of the `logf` decorator as well as its behavior when custom parameters are passed. The tests check whether the function name, arguments, return value, and execution time are correctly logged, and whether the `max_str_len` parameter correctly truncates the logged strings.
```

### Comparing `logfunc-1.4.1/logfunc/__init__.py` & `logfunc-1.5.0/logfunc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,21 @@
                 curval = val
     elif evar == 'LOGF_MAX_STR_LEN': # int/none
         try:
             curval = int(val)
         except ValueError:
             if str(val).upper() == 'NONE':
                 curval = None
-    elif evar == 'LOGF_SINGLE_MSG':
+    elif evar in ['LOGF_SINGLE_MSG', 'LOGF_USE_PRINT']:
         val = str(val).upper()
         if val == 'TRUE':
             curval = True
         elif val == 'FALSE':
             curval = False
-
+    print('@@evar', evar, val, curval)
     return curval
 
 
 def trunc_str(string: str, max_length: Optional[int] = TRUNC_STR_LEN) -> str:
     """
     Truncates a string if its length exceeds the specified maximum length.
     If the string is truncated, it appends '...' to indicate the truncation. If
@@ -78,48 +78,52 @@
 def logf(
     level: Optional[Union[int, str]] = logging.DEBUG,
     log_args: bool = True,
     log_return: bool = True,
     max_str_len: Optional[int] = TRUNC_STR_LEN,
     log_exec_time: bool = True,
     single_msg: bool = False,
+    use_print: bool = False,
     **kwargs
 ) -> Callable[..., Callable[..., Any]]:
     """
     A decorator that logs the execution time, function name, arguments, keyword arguments,
     and return value of a function using a specified log level.
 
     Args:
         level (Union[int, str]): The log level to use for logging. Defaults to logging.DEBUG.
         log_args (bool): Should the function arguments be logged? Defaults to True.
         log_return (bool): Should function return be logged? Defaults to True.
         max_str_len (Optional[int]): Maximum length of the logged arguments and return values. Defaults to 1000.
         log_exec_time (bool): Should the function execution time be measured? Defaults to True.
         single_msg (bool): Should both enter and exit log messages be combined into a single message? Default False
+        use_print (bool): Should the log messages be printed instead of logged? Default False
 
     Returns:
         Callable[..., Callable[..., Any]]: The executed decorated function.
     """
     level = get_evar('LOGF_LEVEL', level)
     max_str_len = get_evar('LOGF_MAX_STR_LEN', max_str_len)
     single_msg = get_evar('LOGF_SINGLE_MSG', single_msg)
+    use_print = get_evar('LOGF_USE_PRINT', use_print)
 
     if isinstance(level, str):
         level_int = logging.getLevelName(level.upper())
     else:
         level_int = int(level)
 
     # for backwards compatability, override log_exec_time using
     # the measure_time kwarg if present
     if 'measure_time' in kwargs:
         log_exec_time = kwargs['measure_time']
 
     def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
         @wraps(func)
         def wrapper(*args, **kwargs) -> Any:
+            print('@@useprint', use_print)
             # Start the timer if required and execute the function.
             start_time = time.time() if log_exec_time else None
 
             fname = '{}()'.format(func.__name__) # shorthand reference
 
             # Log function arguments if required argstr used later if single msg
             # otherwise, only the function name is logged on entry
@@ -130,15 +134,18 @@
                     trunc_str(str(kwargs), max_str_len)
                 )
                 logmsg_enter = '{} | {}'.format(fname, argstr)
 
 
             # if single_msg=True log both enter/exit in one message later
             if not single_msg:
-                logger.log(level_int, logmsg_enter)
+                if use_print:
+                    print(logmsg_enter)
+                else:
+                    logger.log(level_int, logmsg_enter)
 
             # Execute the function
             result = func(*args, **kwargs)
 
             # include execution time if log_exec_time=True
             if log_exec_time:
                 exec_time = time.time() - start_time
@@ -152,12 +159,15 @@
 
             # if log_return=True include returned obj str in logmsg
             if log_return:
                 logmsg_exit = '{} | {}'.format(
                     logmsg_exit, trunc_str(str(result), max_str_len))
 
             # Log the return value and execution time if required
-            logger.log(level_int, logmsg_exit)
+            if use_print:
+                print(logmsg_exit)
+            else:
+                logger.log(level_int, logmsg_exit)
 
             return result
         return wrapper
     return decorator
```

### Comparing `logfunc-1.4.1/logfunc.egg-info/PKG-INFO` & `logfunc-1.5.0/logfunc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.4.1
+Version: 1.5.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logf
 
-`@logf()` is a decorator designed to enable effortless and automatic logging of your Python functions' execution, requiring zero configuration for basic usage. Formerly a part of the myfuncs pip package, it is now a standalone pip package. This repository is dedicated to its continued development and maintenance.
+`@logf()` is a decorator designed to enable effortless logging of your Python functions' execution, requiring zero configuration for basic usage. Formerly a part of the myfuncs pip package, it is now a standalone pip package. This repository is dedicated to its continued development and maintenance.
 
 ## Usage
 
 This is a brief guide on how to use the `logfunc` module.
 
 ### Installation
 
@@ -49,29 +47,37 @@
 
 The `logf` function is a decorator that you can apply to any function you want to log:
 
 ```python
 from logfunc import logf
 
 @logf()
-def my_function(a, b):
-    return a + b
+def my_function(a, b='b'):
+    return str(a) + str(b) + 'c'
 ```
 
 In the example above, `logf()` is used to wrap `my_function`. When `my_function` is called, it logs the function name, arguments, return value, and execution time.
 
+```
+>>> my_function('a')
+my_function() | ('a',) {}
+my_function() 0.00051s | abc
+'abc'
+```
+
 ### Customize Logging
 
-The `logf` function allows you to customize your logging:
+The `logf` decorator allows you to customize your logging:
 
 - You can set the log level with the `level` parameter.
 - Use `log_args` and `log_return` parameters to choose whether to log the arguments and the return value of the function.
 - `max_str_len` parameter allows you to set the maximum length of the logged arguments and return values. If `None` is passed, the entire args/kwargs/result are logged as their full-length strings.
 - You can choose whether to measure and log the function execution time with the `log_exec_time` parameter.
 - You can include the execution time, args, and return value in a single message with the `single_msg` parameter.
+- `use_print` print() log messages rather than logging them
 
 Here is an example:
 
 ```python
 from logfunc import logf
 
 @logf(level='INFO', log_args=False, log_return=True,
@@ -87,14 +93,15 @@
 The `logf` function supports overriding some default/passed parameters with environment variables:
 
 | Env Var          | Example Values       |
 |------------------|-------------|
 | LOGF_LEVEL       | DEBUG INFO WARNING ERROR CRITICAL 10 20 30 40 50|
 | LOGF_MAX_STR_LEN | 10 50 10000000 None NONE none |
 | LOGF_SINGLE_MSG  | True False
+| LOGF_USE_PRINT   | True False
 
 
 ## Testing
 
 This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
 
 To run the tests, navigate to the directory where the `logfunc` package is installed and run:
```

### Comparing `logfunc-1.4.1/setup.py` & `logfunc-1.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='logfunc',
-    version='1.4.1',
+    version='1.5.0',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -17,16 +17,14 @@
     license='MIT',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
```

