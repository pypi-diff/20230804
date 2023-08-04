# Comparing `tmp/parallelism-0.0.3.tar.gz` & `tmp/parallelism-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallelism-0.0.3.tar", last modified: Sat Jul 29 17:58:06 2023, max compression
+gzip compressed data, was "parallelism-0.1.0.tar", last modified: Fri Aug  4 11:50:36 2023, max compression
```

## Comparing `parallelism-0.0.3.tar` & `parallelism-0.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.321160 parallelism-0.0.3/
--rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.0.3/.gitignore
--rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.0.3/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      674 2023-07-29 17:58:06.321160 parallelism-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.177020 parallelism-0.0.3/docs/
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.192642 parallelism-0.0.3/docs/api_reference/
--rw-rw-rw-   0        0        0      249 2023-07-29 11:22:19.000000 parallelism-0.0.3/docs/api_reference/scheduled_task.rst
--rw-rw-rw-   0        0        0      249 2023-07-29 11:22:19.000000 parallelism-0.0.3/docs/api_reference/task_scheduler.rst
--rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.0.3/docs/conf.py
--rw-rw-rw-   0        0        0      986 2023-07-29 11:22:19.000000 parallelism-0.0.3/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.210966 parallelism-0.0.3/parallelism/
--rw-rw-rw-   0        0        0      296 2023-07-29 17:56:59.000000 parallelism-0.0.3/parallelism/__init__.py
--rw-rw-rw-   0        0        0     7123 2023-07-29 17:13:19.000000 parallelism-0.0.3/parallelism/api_reference.py
--rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.0.3/parallelism/config.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.257831 parallelism-0.0.3/parallelism/core/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.0.3/parallelism/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.273483 parallelism-0.0.3/parallelism/core/exceptions/
--rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.0.3/parallelism/core/exceptions/__init__.py
--rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.0.3/parallelism/core/exceptions/dependency_error.py
--rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.0.3/parallelism/core/exceptions/worker_error.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.289074 parallelism-0.0.3/parallelism/core/executors/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.0.3/parallelism/core/executors/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.0.3/parallelism/core/executors/process_executor.py
--rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.0.3/parallelism/core/executors/thread_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.321160 parallelism-0.0.3/parallelism/core/handlers/
--rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.0.3/parallelism/core/handlers/__init__.py
--rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.0.3/parallelism/core/handlers/dependency_handler.py
--rw-rw-rw-   0        0        0      340 2023-07-18 13:08:21.000000 parallelism-0.0.3/parallelism/core/handlers/error_handler.py
--rw-rw-rw-   0        0        0     6888 2023-07-28 11:34:19.000000 parallelism-0.0.3/parallelism/core/handlers/function_handler.py
--rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.0.3/parallelism/core/handlers/parameters_handler.py
--rw-rw-rw-   0        0        0     2718 2023-07-29 17:54:53.000000 parallelism-0.0.3/parallelism/core/handlers/shared_memory_handler.py
--rw-rw-rw-   0        0        0     1388 2023-07-21 22:43:02.000000 parallelism-0.0.3/parallelism/core/return_value.py
--rw-rw-rw-   0        0        0     3247 2023-07-29 17:19:03.000000 parallelism-0.0.3/parallelism/core/scheduled_task.py
--rw-rw-rw-   0        0        0      399 2023-07-25 21:47:04.000000 parallelism-0.0.3/parallelism/core/scheduler_result.py
--rw-rw-rw-   0        0        0     7102 2023-07-29 17:27:16.000000 parallelism-0.0.3/parallelism/core/task_scheduler.py
--rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.0.3/parallelism/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.242210 parallelism-0.0.3/parallelism.egg-info/
--rw-rw-rw-   0        0        0      674 2023-07-29 17:58:05.000000 parallelism-0.0.3/parallelism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1109 2023-07-29 17:58:06.000000 parallelism-0.0.3/parallelism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 17:58:05.000000 parallelism-0.0.3/parallelism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-29 17:58:05.000000 parallelism-0.0.3/parallelism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 17:58:06.321160 parallelism-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.365749 parallelism-0.1.0/
+-rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.1.0/.gitignore
+-rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.1.0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      674 2023-08-04 11:50:36.365749 parallelism-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.218892 parallelism-0.1.0/docs/
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.218892 parallelism-0.1.0/docs/api_reference/
+-rw-rw-rw-   0        0        0     5083 2023-08-04 11:42:22.000000 parallelism-0.1.0/docs/api_reference/scheduled_task.rst
+-rw-rw-rw-   0        0        0     2945 2023-08-04 11:46:52.000000 parallelism-0.1.0/docs/api_reference/task_scheduler.rst
+-rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.1.0/docs/conf.py
+-rw-rw-rw-   0        0        0      986 2023-08-04 09:49:41.000000 parallelism-0.1.0/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.250131 parallelism-0.1.0/parallelism/
+-rw-rw-rw-   0        0        0      296 2023-08-04 11:48:06.000000 parallelism-0.1.0/parallelism/__init__.py
+-rw-rw-rw-   0        0        0     7143 2023-08-04 09:28:23.000000 parallelism-0.1.0/parallelism/api_reference.py
+-rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.1.0/parallelism/config.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.281373 parallelism-0.1.0/parallelism/core/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.1.0/parallelism/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.296994 parallelism-0.1.0/parallelism/core/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.1.0/parallelism/core/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.1.0/parallelism/core/exceptions/dependency_error.py
+-rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.1.0/parallelism/core/exceptions/worker_error.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.328238 parallelism-0.1.0/parallelism/core/executors/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.1.0/parallelism/core/executors/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.1.0/parallelism/core/executors/process_executor.py
+-rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.1.0/parallelism/core/executors/thread_executor.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.365749 parallelism-0.1.0/parallelism/core/handlers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.1.0/parallelism/core/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.1.0/parallelism/core/handlers/dependency_handler.py
+-rw-rw-rw-   0        0        0     6993 2023-08-04 11:46:52.000000 parallelism-0.1.0/parallelism/core/handlers/function_handler.py
+-rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.1.0/parallelism/core/handlers/parameters_handler.py
+-rw-rw-rw-   0        0        0     3754 2023-08-04 11:46:52.000000 parallelism-0.1.0/parallelism/core/handlers/shared_memory_handler.py
+-rw-rw-rw-   0        0        0      344 2023-08-04 11:42:19.000000 parallelism-0.1.0/parallelism/core/raise_exception.py
+-rw-rw-rw-   0        0        0     1275 2023-08-02 21:46:54.000000 parallelism-0.1.0/parallelism/core/return_value.py
+-rw-rw-rw-   0        0        0     3182 2023-08-02 21:46:54.000000 parallelism-0.1.0/parallelism/core/scheduled_task.py
+-rw-rw-rw-   0        0        0      474 2023-08-04 11:46:52.000000 parallelism-0.1.0/parallelism/core/scheduler_result.py
+-rw-rw-rw-   0        0        0     7203 2023-08-04 11:48:06.000000 parallelism-0.1.0/parallelism/core/task_scheduler.py
+-rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.1.0/parallelism/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.265756 parallelism-0.1.0/parallelism.egg-info/
+-rw-rw-rw-   0        0        0      674 2023-08-04 11:50:36.000000 parallelism-0.1.0/parallelism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2023-08-04 11:50:36.000000 parallelism-0.1.0/parallelism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:50:36.000000 parallelism-0.1.0/parallelism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 11:50:36.000000 parallelism-0.1.0/parallelism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 11:50:36.365749 parallelism-0.1.0/setup.cfg
```

### Comparing `parallelism-0.0.3/.gitignore` & `parallelism-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.3/LICENSE` & `parallelism-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.3/PKG-INFO` & `parallelism-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.0.3
+Version: 0.1.0
 Summary: Empowering workflows with parallelism
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
 Keywords: parallelism,parallel,task,scheduler
```

### Comparing `parallelism-0.0.3/docs/index.rst` & `parallelism-0.1.0/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 ::
 
     pip install parallelism
 
 API Reference
 -------------
 
-- `scheduled_task <https://parallelism.readthedocs.io/en/latest/api_reference/scheduled_task.html>`_
-- `task_scheduler <https://parallelism.readthedocs.io/en/latest/api_reference/task_scheduler.html>`_
+- `Scheduled Task <https://parallelism.readthedocs.io/en/latest/api_reference/scheduled_task.html>`_
+- `Task Scheduler <https://parallelism.readthedocs.io/en/latest/api_reference/task_scheduler.html>`_
 
 .. Hidden TOCs
 
 .. toctree::
     :hidden:
     :caption: API Reference
     :maxdepth: 0
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 parallelism ========== Empowering workflows with parallelism Information ------
 ----- - Package: |package| - Documentation: |documentation| - Source Code:
 |source-code| .. |package| raw:: html Python_Package_Index_(PyPI) ..
 |documentation| raw:: html Read_the_Docs .. |source-code| raw:: html GitHub
 Installation ------------ :: pip install parallelism API Reference ------------
-- - `scheduled_task
+- - `Scheduled Task
 parallelism.readthedocs.io/en/latest/api_reference/scheduled_task.html>`_ -
-`task_scheduler
+`Task Scheduler
 parallelism.readthedocs.io/en/latest/api_reference/task_scheduler.html>`_ ..
 Hidden TOCs .. toctree:: :hidden: :caption: API Reference :maxdepth: 0 :glob:
 api_reference/*
```

### Comparing `parallelism-0.0.3/parallelism/api_reference.py` & `parallelism-0.1.0/parallelism/api_reference.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     continual: bool = False,
 ) -> ScheduledTask:
     """
     Schedule a task to be executed at the right moment in the task scheduler
 
     Parameters
     ----------
-    executor : multiprocessing.Process or threading.Thread
+    executor : type of `multiprocessing.Process` or `threading.Thread`
         | The execution unit of a task
     name : str
         | A unique identifier representing a task
     target : callable
         | A function to be invoked by a task scheduler
     args : tuple, optional
         | Positional arguments that are related to the target
@@ -133,23 +133,23 @@
     """
     Schedule multiple tasks for execution
 
     Parameters
     ----------
     tasks : tuple of ScheduledTask
         | Tasks that need to be performed
-    processes : int, optional
+    processes : int, default `os.cpu_count()`
         | The number of processes assigned to perform the tasks
-    threads : int, optional
+    threads : int, default `os.cpu_count()`
         | The number of threads assigned to perform the tasks
     """
     if processes is None:
-        processes = processes or cpu_count() or 1
+        processes = cpu_count() or 1
     if threads is None:
-        threads = threads or cpu_count() or 1
+        threads = cpu_count() or 1
     if not isinstance(tasks, tuple):
         pattern = 'The {!r} parameter should be of type {!r}'
         raise TypeError(pattern.format('tasks', 'tuple'))
     if not all(isinstance(item, ScheduledTask) for item in tasks):
         pattern = 'The {!r} parameter should only contain {!r}'
         raise TypeError(pattern.format('tasks', 'ScheduledTask'))
     if not len({task.name for task in tasks}) == len(tasks):
```

### Comparing `parallelism-0.0.3/parallelism/core/executors/process_executor.py` & `parallelism-0.1.0/parallelism/core/executors/process_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.3/parallelism/core/executors/thread_executor.py` & `parallelism-0.1.0/parallelism/core/executors/thread_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.3/parallelism/core/handlers/dependency_handler.py` & `parallelism-0.1.0/parallelism/core/handlers/dependency_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.3/parallelism/core/handlers/function_handler.py` & `parallelism-0.1.0/parallelism/core/handlers/function_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
+from datetime import datetime
 from decimal import Decimal
 from time import time
 from traceback import format_exc
 from typing import TYPE_CHECKING
 
 from parallelism.config import DECIMAL_PRECISION, DECIMAL_ROUNDING_MODE
 from parallelism.core.exceptions.dependency_error import DependencyError
 from parallelism.core.exceptions.worker_error import WorkerError
-from parallelism.core.handlers.error_handler import ErrorHandler
+from parallelism.core.raise_exception import RaiseException
 from parallelism.logger import get_logger
 
 if TYPE_CHECKING:
     from multiprocessing.managers import DictProxy
     from typing import Any, Callable, Dict, Optional
 
 __all__ = ('FunctionHandler',)
@@ -27,44 +28,45 @@
         target: Callable[..., Any],
         proxy: DictProxy,
         blocker: Optional[Dict[str, Any]],
     ) -> None:
         self.name = name
         self.target = target
         self.proxy = proxy
+        self.proxy['execution_time'] = datetime.now()
         self.proxy['elapsed_time'] = None
-        self.proxy['error_handler'] = None
+        self.proxy['raise_exception'] = None
         self.proxy['return_value'] = None
         self.proxy['finish'] = False
         self.proxy['complete'] = False
         if blocker:
             self.log_current_state(blocker)
 
     def __call__(self, *args: Any, **kwargs: Any) -> None:
         start = time()
         try:
             self.proxy['return_value'] = self.target(*args, **kwargs)
             self.proxy['complete'] = True
         except Exception as exception:
-            self.proxy['error_handler'] = ErrorHandler(exception, format_exc())
+            self.proxy['raise_exception'] = RaiseException(exception, format_exc())
         finally:
             end = time()
             self.proxy['finish'] = True
             self.proxy['elapsed_time'] = end - start
             self.log_current_state()
 
     def log_current_state(
         self,
         blocker: Optional[Dict[str, Any]] = None,
     ) -> None:
         logger = get_logger()
         name = self.name
         elapsed_time = self.proxy.get('elapsed_time')
         elapsed_time = self.beautify_time(seconds=elapsed_time)
-        error_handler = self.proxy.get('error_handler')
+        raise_exception = self.proxy.get('raise_exception')
         if blocker and blocker.get('reason') == 'dependency':
             *left, right = blocker.get('tasks')
             pattern = '{!r} is being canceled, due to '
             if len(left) == 0:
                 pattern += 'task {!r}'
                 message = pattern.format(name, right)
             elif len(left) == 1:
@@ -75,15 +77,15 @@
                 pattern += 'tasks {}, and {!r}'
                 left = ', '.join(map(repr, left))
                 message = pattern.format(name, left, right)
             exception = DependencyError(
                 message='{!r} has been canceled'.format(name),
                 tasks=blocker.get('tasks'),
             )
-            self.proxy['error_handler'] = ErrorHandler(exception)
+            self.proxy['raise_exception'] = RaiseException(exception)
             self.proxy['finish'] = True
             logger.warning(msg=message)
         elif blocker and blocker.get('reason') == 'worker':
             processes = blocker.get('processes')
             threads = blocker.get('threads')
             pattern = '{!r} is being canceled, due to '
             if processes > 1 and threads > 1:
@@ -114,20 +116,20 @@
                 pattern += 'lack of workers'
                 message = pattern.format(name)
             exception = WorkerError(
                 message='{!r} has been canceled'.format(name),
                 processes=processes,
                 threads=threads,
             )
-            self.proxy['error_handler'] = ErrorHandler(exception)
+            self.proxy['raise_exception'] = RaiseException(exception)
             self.proxy['finish'] = True
             logger.warning(msg=message)
-        elif isinstance(error_handler, ErrorHandler):
+        elif isinstance(raise_exception, RaiseException):
             pattern = '{!r} ran approximately {} - {!r}'
-            message = pattern.format(name, elapsed_time, error_handler)
+            message = pattern.format(name, elapsed_time, raise_exception)
             logger.error(msg=message)
         else:
             pattern = '{!r} ran approximately {}'
             message = pattern.format(name, elapsed_time)
             logger.info(msg=message)
 
     @staticmethod
```

### Comparing `parallelism-0.0.3/parallelism/core/handlers/parameters_handler.py` & `parallelism-0.1.0/parallelism/core/handlers/parameters_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.3/parallelism/core/return_value.py` & `parallelism-0.1.0/parallelism/core/return_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 
 __all__ = ('ReturnValue',)
 
 
 class ReturnValue:
     __slots__ = ('task', 'transformations')
 
-    # def __init__(self, name: str) -> None:
-    #     self.name = name
-    #     self.transformations = []
-
     def __init__(self, task: ScheduledTask) -> None:
         self.task = task
         self.transformations = []
 
     def __call__(self, *args: Any, **kwargs: Any) -> ReturnValue:
         transformations = getattr(self, ':transformations')
         transformations.append(('__call__', (args, kwargs)))
```

### Comparing `parallelism-0.0.3/parallelism/core/scheduled_task.py` & `parallelism-0.1.0/parallelism/core/scheduled_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     @property
     def amount_of_dependencies(self) -> int:
         return len(self.dependencies)
 
     @property
     def depends_on_dependencies(self) -> Tuple[ScheduledTask, ...]:
         return tuple(task for task in self.dependencies)
-        # return tuple(task.name for task in self.dependencies)
 
     @property
     def depends_on_parameters(self) -> Tuple[ScheduledTask, ...]:
         tasks = {}
         for parameter in list(self.args) + list(self.kwargs.values()):
             if isinstance(parameter, ReturnValue):
                 task = getattr(parameter, ':task')
```

### Comparing `parallelism-0.0.3/parallelism/core/task_scheduler.py` & `parallelism-0.1.0/parallelism/core/task_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,19 @@
                 task = self.initialize(task)
                 self.tasks[index] = task
                 task.executor.start()
                 break
         for index, task in enumerate(self.tasks):
             self.shared_memory_handler.free(index, task)
         self.manager.shutdown()
+        self.shared_memory_handler.sort()
         return SchedulerResult(
+            self.shared_memory_handler.execution_time,
             self.shared_memory_handler.elapsed_time,
-            self.shared_memory_handler.error_handler,
+            self.shared_memory_handler.raise_exception,
             self.shared_memory_handler.return_value,
         )
 
     def initialize(
         self,
         task: ScheduledTask,
         blocked: Literal['dependency', 'worker'] = None,
```

### Comparing `parallelism-0.0.3/parallelism.egg-info/PKG-INFO` & `parallelism-0.1.0/parallelism.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.0.3
+Version: 0.1.0
 Summary: Empowering workflows with parallelism
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
 Keywords: parallelism,parallel,task,scheduler
```

### Comparing `parallelism-0.0.3/parallelism.egg-info/SOURCES.txt` & `parallelism-0.1.0/parallelism.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 parallelism/config.py
 parallelism/logger.py
 parallelism.egg-info/PKG-INFO
 parallelism.egg-info/SOURCES.txt
 parallelism.egg-info/dependency_links.txt
 parallelism.egg-info/top_level.txt
 parallelism/core/__init__.py
+parallelism/core/raise_exception.py
 parallelism/core/return_value.py
 parallelism/core/scheduled_task.py
 parallelism/core/scheduler_result.py
 parallelism/core/task_scheduler.py
 parallelism/core/exceptions/__init__.py
 parallelism/core/exceptions/dependency_error.py
 parallelism/core/exceptions/worker_error.py
 parallelism/core/executors/__init__.py
 parallelism/core/executors/process_executor.py
 parallelism/core/executors/thread_executor.py
 parallelism/core/handlers/__init__.py
 parallelism/core/handlers/dependency_handler.py
-parallelism/core/handlers/error_handler.py
 parallelism/core/handlers/function_handler.py
 parallelism/core/handlers/parameters_handler.py
 parallelism/core/handlers/shared_memory_handler.py
```

### Comparing `parallelism-0.0.3/pyproject.toml` & `parallelism-0.1.0/pyproject.toml`

 * *Files identical despite different names*

