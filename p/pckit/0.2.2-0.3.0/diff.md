# Comparing `tmp/pckit-0.2.2.tar.gz` & `tmp/pckit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pckit-0.2.2.tar", max compression
+gzip compressed data, was "pckit-0.3.0.tar", max compression
```

## Comparing `pckit-0.2.2.tar` & `pckit-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1066 2022-05-11 07:50:39.121175 pckit-0.2.2/LICENSE
--rw-r--r--   0        0        0     2405 2022-05-11 07:50:39.121175 pckit-0.2.2/README.md
--rw-r--r--   0        0        0      456 2022-05-11 07:50:39.121175 pckit-0.2.2/pckit/__init__.py
--rw-r--r--   0        0        0     1784 2022-05-11 07:50:39.121175 pckit-0.2.2/pckit/_utils.py
--rw-r--r--   0        0        0     5988 2022-05-11 07:50:39.125175 pckit-0.2.2/pckit/models.py
--rw-r--r--   0        0        0     9099 2022-05-11 07:50:39.125175 pckit-0.2.2/pckit/solvers.py
--rw-r--r--   0        0        0      325 2022-05-11 07:50:39.125175 pckit-0.2.2/pckit/task.py
--rw-r--r--   0        0        0     5594 2022-05-11 07:50:39.125175 pckit-0.2.2/pckit/workers.py
--rw-r--r--   0        0        0      617 2022-05-11 07:50:39.125175 pckit-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3166 2022-05-11 07:53:04.285873 pckit-0.2.2/setup.py
--rw-r--r--   0        0        0     3086 2022-05-11 07:53:04.286337 pckit-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-04 11:23:30.757670 pckit-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2287 2023-08-04 11:23:30.757670 pckit-0.3.0/README.md
+-rw-r--r--   0        0        0      441 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/__init__.py
+-rw-r--r--   0        0        0      109 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/_typevars.py
+-rw-r--r--   0        0        0     1866 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/_utils.py
+-rw-r--r--   0        0        0     1492 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/cache.py
+-rw-r--r--   0        0        0     5676 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/models.py
+-rw-r--r--   0        0        0     9465 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/solvers.py
+-rw-r--r--   0        0        0      156 2023-08-04 11:23:30.761670 pckit-0.3.0/pckit/task.py
+-rw-r--r--   0        0        0     5089 2023-08-04 11:23:30.761670 pckit-0.3.0/pckit/workers.py
+-rw-r--r--   0        0        0      617 2023-08-04 11:23:30.761670 pckit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 pckit-0.3.0/PKG-INFO
```

### Comparing `pckit-0.2.2/LICENSE` & `pckit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pckit-0.2.2/README.md` & `pckit-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pckit
+Version: 0.3.0
+Summary: A simple package for parallel computing with Python
+Home-page: https://github.com/djiboshin/pckit
+License: MIT
+Author: djiboshin
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: MPh (>=1.1.5,<2.0.0)
+Requires-Dist: numpy (>=1.25.2,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Project-URL: Repository, https://github.com/djiboshin/pckit
+Description-Content-Type: text/markdown
+
 # pckit
 
 This is a simple package for parallel computing with Python.
 
 ## Usage
 ### Multiprocessing
 If you want to use any solver from the package you have to wrap your functions into a model. 
@@ -9,58 +28,58 @@
 `MyModel` is a subclass of the package `Model`. The method `results` is required.
 
 ```python
 import pckit
 
 
 class MyModel(pckit.Model):
-    def results(self, x):
+    def results(self, x: int) -> int:
         # Solve here problem f(x) = x^2
         return x ** 2
 
 
 if __name__ == '__main__':
     model = MyModel()
-    worker = pckit.SimpleMultiprocessingWorker(model)
+    worker = pckit.MultiprocessingWorker(model)
     with pckit.get_solver(worker, workers_num=2) as solver:
         # Create tasks to solve. You can put args or
         # kwargs for model.results() method in the Task
-        tasks = [pckit.Task(2), pckit.Task(x=3)]
+        tasks = [2, 3]
         results = solver.solve(tasks)
         print(results)
         # >>> [4, 9]
 ```
 
 ### MPI
 You can easily run scripts on the cluster with [mpi4py](https://github.com/mpi4py/mpi4py) implementation on MPI (See [mpi4py installation docs](https://mpi4py.readthedocs.io/en/stable/install.html)).
-Simply change `SimpleMultiprocessingWorker` to `SimpleMPIWorker` in the previous example and start the script with MPI `mpiexec -np 3 python -m mpi4py your_script.py`
+Simply change `MultiprocessingWorker` to `MPIWorker` in the previous example and start the script with MPI `mpiexec -np 3 python -m mpi4py your_script.py`
 
 ```python
-worker = pckit.SimpleMPIWorker(model)
+worker = pckit.MPIWorker(model)
 ```
 Moreover, a multiprocessing solver can be started inside an MPI solver.
 
 ### Single thread
-Single threaded execution is also available with `SimpleWorker`
+Single threaded execution is also available with `Worker`
 
 ```python
-worker = pckit.SimpleWorker(model)
+worker = pckit.Worker(model)
 ```
 
 ### Examples
 [More examples](https://github.com/djiboshin/pckit/tree/main/examples)
 
 ## Features
 ### Cache
 Dict based cache is available by `caching` argument in `get_solver()`.
-`tag` property in `Task` is required and has to be hashable.
+Tasks are required to be hashable.
 
 ```python
 with pckit.get_solver(worker, caching=True) as solver:
-    tasks = [pckit.Task(2, tag='2'), pckit.Task(2, tag='2')]
+    tasks = [2, 2]
 ```
 The second task's solution will be reused from the cache.
 
 ### Custom iterators
 You can send the email or print anything with custom iterator.
 [tqdm](https://pypi.org/project/tqdm/) is also supported.
 ```python
@@ -70,7 +89,8 @@
 ```
 See [example](https://github.com/djiboshin/pckit/blob/main/examples/custom_iterator.py) to create your own iterator.
 
 ### Comsol Models, Solvers, Workers
 Based on [MPh](https://pypi.org/project/MPh/) package.
 
 **TBD**ocumented
+
```

### Comparing `pckit-0.2.2/pckit/models.py` & `pckit-0.3.0/pckit/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,37 @@
 """
 This module contains different Models
 """
-from abc import ABC, abstractmethod
-from typing import Any, AnyStr, Dict
+from abc import ABC, abstractmethod, ABCMeta
+from typing import Any, AnyStr, Dict, Generic, TypeVar, Type, Protocol, Callable
 
 import mph
 import pandas as pd
 import numpy as np
 
 from ._utils import make_unique
+from ._typevars import Task, Result
 
 
-class Model(ABC):
+class Model(Generic[Task, Result]):
     """
     The Model abstract base class.
     """
     @abstractmethod
-    def results(self, *args, **kwargs) -> Any:
+    def results(self, task: Task) -> Result:
         """
         Function to be solved
         """
 
 
-class TestModel(Model):
-    """
-    Simple subclass of Model fot tests
-    """
-    def results(self, x):
-        """Returns squared number
-
-        :param x: any number
-        :return: squared number
-        """
-        if x == 1:
-            return x
-        elif x == 0:
-            return x
-        raise ValueError('Test value error')
-
-
 # TODO SMUTHI Model
 # TODO logging here?
 
 # noinspection PyMissingOrEmptyDocstring
-class ComsolModel(mph.Model, Model):
+class ComsolModel(mph.Model, Model, metaclass=ABCMeta):
     def __init__(self):
         super().__init__(None)
 
     def add_circle(
             self,
             name: str,
             x_i: float,
@@ -130,15 +114,15 @@
 
     @staticmethod
     def global_evaluation(dataset: mph.Node, evaluation: mph.Node) -> pd.DataFrame:
         #  https://github.com/MPh-py/MPh/blob/2b967b77352f9ce7effcd50ad4774bf5eaf731ea/mph/model.py#L425
         evaluation.property('data', dataset)
         java = evaluation.java
         real, imag = java.computeResult()
-        results = np.array(real) + 1j * np.array(imag)
+        results = (np.array(real) + 1j * np.array(imag)) if imag is not None else np.array(real)
         return pd.DataFrame(data=results, columns=make_unique(evaluation.property('descr')))
 
     def clear(self):
         # super().clear()
         super().reset()
 
     def export_image(self, source: mph.Node, filepath: AnyStr, props: Dict = None):
@@ -176,22 +160,18 @@
 
     def getLastComputationTime(self):
         # TODO ADD ANY STUDY SUPPORT
 
         studies = (self / 'studies').children()
         return -1 if not len(studies) else int(studies[-1].java.getLastComputationTime())
 
-    @abstractmethod
-    def results(self, *args: Any, **kwargs: Any) -> Any:
-        pass
-
     def configure(self) -> Any:
         pass
 
-    def pre_build(self, *args: Any, **kwargs: Any):
+    def pre_build(self, task: Task):
         pass
 
-    def pre_solve(self, *args: Any, **kwargs: Any):
+    def pre_solve(self, task: Task):
         pass
 
-    def pre_clear(self, *args: Any, **kwargs: Any):
+    def pre_clear(self, task: Task):
         pass
```

### Comparing `pckit-0.2.2/pckit/solvers.py` & `pckit-0.3.0/pckit/solvers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,44 +2,50 @@
 This module contains different Solvers
 """
 import multiprocessing
 import sys
 from abc import ABC, abstractmethod
 
 from multiprocessing import Queue, JoinableQueue
-from typing import Any, Sequence, Union, List, Iterator, Callable, Iterable
+from typing import Any, Sequence, Union, List, Iterator, Callable, Iterable, Generic
+from ._typevars import Task, Result
 import time
 import logging
 
-from .task import Task
 from .workers import Worker, MultiprocessingWorker, MPIWorker
 from ._utils import tasks_sort
+from .cache import Cache, BaseCache
 
 # TODO(add info to return after .solve())
 # TODO(add additional threads to control workers' errors)
 
 logger = logging.getLogger(__package__ + '.solver')
 
 
 def task_iterator(iterable: Sequence[Task]) -> Iterator[Task]:
     """Returns Iterator from on iterable"""
     return iterable.__iter__()
 
 
-class Solver(ABC):
+class Solver(ABC, Generic[Task, Result]):
     """Base Solver class"""
-    def __init__(self):
-        self.caching = False
-        self.cache = {}
+    def __init__(
+            self,
+            worker: Worker[Task, Result],
+            caching: bool = False
+    ):
+        self.worker = worker
+        self.caching = caching
+        self.cache: BaseCache[Task, Result] = Cache()
         self.total_workers = 0
 
     def solve(self,
               tasks: Sequence[Task],
               iterator: Callable[[Sequence[Task]], Union[Iterator[Task], Iterable[Task]]] = task_iterator
-              ) -> List[Any]:
+              ) -> List[Result]:
         """Solves tasks
 
         :param tasks: tasks to solve
         :param iterator: function which wraps iterable tasks list and return iterator
         :return: list of results
         """
         if self.caching:
@@ -66,15 +72,15 @@
     def _solve(
             self,
             tasks: Sequence[Task],
             to_solve: List[int],
             cached: List[int],
             same: List[int],
             iterator: Callable[[Sequence[Task]], Iterator[Task]]
-    ) -> List[Any]:
+    ) -> List[Result]:
         pass
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
@@ -83,17 +89,21 @@
 class MultiprocessingSolver(Solver):
     """Multiprocessing Solver implementation"""
     def __init__(self,
                  worker: MultiprocessingWorker,
                  workers_num: int = 1,
                  caching: bool = False
                  ):
-        super().__init__()
-        self.caching = caching
+
+        if not isinstance(worker, MultiprocessingWorker):
+            raise TypeError('Worker has to be the object of type MultiprocessingWorker')
+
+        super().__init__(worker=worker, caching=caching)
         self.worker = worker
+
         if workers_num <= 0:
             raise RuntimeError('At least 1 worker is needed')
         self.total_workers = workers_num
 
         self.workers = []
 
         self._jobs = JoinableQueue()
@@ -111,34 +121,34 @@
     def _solve(
             self,
             tasks: Sequence[Task],
             to_solve: List[int],
             cached: List[int],
             same: List[int],
             iterator: Callable[[Sequence[Task]], Iterator[Task]]
-    ) -> List[Any]:
+    ) -> List[Result]:
         results = [None for _ in tasks]
         for i, task in enumerate(tasks):
             if i in to_solve:
-                self._jobs.put((i, task.args, task.kwargs))
+                self._jobs.put((i, task))
             elif i in cached:
-                results[i] = self.cache[task.tag]
+                results[i] = self.cache[task]
             else:
                 results[i] = None
         tasks_to_solve = [task for i, task in enumerate(tasks) if i in to_solve]
         for _ in iterator(tasks_to_solve):
             (i, res) = self._results.get()
             if i == -1:
                 raise RuntimeError(res)
             if self.caching:
-                self.cache[tasks[i].tag] = res
+                self.cache[tasks[i]] = res
             results[i] = res
 
         for i in same:
-            results[i] = self.cache[tasks[i].tag]
+            results[i] = self.cache[tasks[i]]
 
         return results
 
     def _stop(self):
         for worker in self.workers:
             if worker.is_alive():
                 worker.terminate()
@@ -151,53 +161,59 @@
 
 
 class SimpleSolver(Solver):
     """Simplest Solver implementation"""
     def __init__(self, worker: Worker, caching: bool = False):
         if not isinstance(worker, Worker):
             raise TypeError('Worker has to be the object of type Worker')
-        super().__init__()
-        self.caching = caching
-        self.worker = worker
+        super().__init__(worker=worker, caching=caching)
         self.worker.start()
         self.total_workers = 1
 
     def _solve(
             self,
             tasks: Sequence[Task],
             to_solve: List[int],
             cached: List[int],
             same: List[int],
             iterator: Callable[[Sequence[Task]], Iterator[Task]]
-    ) -> List[Any]:
+    ) -> List[Result]:
         results = [None for _ in tasks]
         for i, task in enumerate(iterator(tasks)):
             if i in to_solve:
                 try:
-                    results[i] = self.worker.do_the_job(task.args, task.kwargs)
+                    results[i] = self.worker.do_the_job(task)
+                    print(results[i])
                 except Exception as err:
                     raise RuntimeError from err
                 if self.caching:
-                    self.cache[task.tag] = results[i]
+                    self.cache[task] = results[i]
             elif i in cached or i in same:
-                results[i] = self.cache[task.tag] if task.tag is not None else None
+                results[i] = self.cache[task] if task is not None else None
             else:
                 results[i] = None
         return results
 
 
 class MPISolver(Solver):
     """MPI Solver implementation"""
-    def __init__(self, worker: MPIWorker, caching: bool = False, buffer_size: int = 32768):
+    def __init__(
+            self,
+            worker: MPIWorker,
+            caching: bool = False,
+            buffer_size: int = 32768
+    ):
         from mpi4py import MPI
+
         if not isinstance(worker, MPIWorker):
             raise TypeError('Worker has to be the object of type MPIWorker')
-        super().__init__()
+
+        super().__init__(worker=worker, caching=caching)
         self.worker = worker
-        self.caching = caching
+
         self.buffer_size = buffer_size
         self.comm = MPI.COMM_WORLD
         self._MPI = MPI
         self.rank = self.comm.Get_rank()
         self.total_workers = self.comm.Get_size() - 1
 
         if self.rank != 0:
@@ -221,34 +237,34 @@
     ) -> List[Any]:
         results = [None for _ in tasks]
         requests = []
         tasks_to_solve = []
         for i, task in enumerate(tasks):
             if i in to_solve:
                 dest = len(requests) % self.total_workers + 1
-                req = self.comm.isend((i, task.args, task.kwargs), dest=dest, tag=i)
+                req = self.comm.isend((i, task), dest=dest, tag=i)
                 req.wait()
                 requests.append(self.comm.irecv(self.buffer_size, source=dest))
                 tasks_to_solve.append(task)
             elif i in cached:
-                results[i] = self.cache[task.tag]
+                results[i] = self.cache[task]
         for _ in iterator(tasks_to_solve):
             (k, (i, res)) = self._MPI.Request.waitany(requests)
             if self.caching:
-                self.cache[tasks[i].tag] = res
+                self.cache[tasks[i]] = res
             results[i] = res
 
         for i in same:
-            results[i] = self.cache[tasks[i].tag]
+            results[i] = self.cache[tasks[i]]
 
         return results
 
     def _stop(self):
         for i in range(1, self.comm.Get_size()):
-            req = self.comm.isend((None, None, None), dest=i)
+            req = self.comm.isend((None, None), dest=i)
             req.wait()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._stop()
```

### Comparing `pckit-0.2.2/pckit/workers.py` & `pckit-0.3.0/pckit/workers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 """
 This module contains different Workers
 """
 import multiprocessing
-from abc import ABC, abstractmethod
-from typing import Any, Dict, Tuple
 from multiprocessing import JoinableQueue, Queue
 from pathlib import Path
 import socket
 import logging
 import mph
+from typing import Generic
 
 from .models import ComsolModel, Model
+from ._typevars import Task, Result
 
 logger = logging.getLogger(__package__ + '.worker')
 
 
-class Worker(ABC):
+class Worker(Generic[Task, Result]):
     """
     The Worker abstract base class.
     """
-    @abstractmethod
+    def __init__(
+            self,
+            model: Model[Task, Result]
+    ):
+        self.model = model
+
     def start(self):
-        """Function that stars the worker. Always called on each worker by solver when initializing.
+        """
+        Function that stars the worker.
+        Always called on each worker by solver when initializing.
 
         :return:
         """
 
-    @abstractmethod
-    def do_the_job(self, args: Tuple[Any], kwargs: Dict[str, Any]) -> Any:
-        """calls Model.results() with specified params
+    def do_the_job(self, task):
+        """
+        calls Model.results() with specified params
 
-        :param args: args for Model.results()
-        :param kwargs: kwargs for Model.results()
+        :param task: task for Model.results()
         :return: pass Model.results()
         """
+        return self.model.results(task)
 
 
-class MultiprocessingWorker(Worker, ABC):
+class MultiprocessingWorker(Worker):
     """Class of basic multiprocessing worker."""
     def start_loop(self, jobs: JoinableQueue, results: Queue):
-        """Loop starting will be called by multiprocessing solver.
+        """
+        Loop starting will be called by multiprocessing solver.
 
         :param JoinableQueue jobs: Queue for jobs
         :param Queue results: Queue for results
         """
         logger.info('%s %s Starting',
                     multiprocessing.current_process().name,
                     socket.gethostname())
@@ -51,29 +59,29 @@
         self._loop(jobs, results)
 
     def _loop(self, jobs: JoinableQueue, results: Queue):
         logger.info('%s %s Entering the loop',
                     multiprocessing.current_process().name,
                     socket.gethostname())
         while True:
-            (i, args, kwargs) = jobs.get()
+            (i, task) = jobs.get()
             logger.debug('%s %s Starting doing the job %i',
                          multiprocessing.current_process().name,
                          socket.gethostname(),
                          i)
             try:
-                res = self.do_the_job(args, kwargs)
+                res = self.do_the_job(task)
                 results.put((i, res))
                 jobs.task_done()
             except Exception as err:
                 results.put((-1, err))
                 raise err
 
 
-class MPIWorker(Worker, ABC):
+class MPIWorker(Worker):
     """Class of basic MPI worker"""
     def start_loop(self, comm):
         """Loop start will be called by MPI solver.
 
         :param comm: Intracomm, COMM_WORLD commonly
         """
         import mpi4py
@@ -87,56 +95,41 @@
 
     def _loop(self, comm):
         logger.info('Rang %i %s Entering the loop',
                     comm.Get_rank(),
                     socket.gethostname())
         while True:
             req = comm.irecv(source=0)
-            (i, args, kwargs) = req.wait()
-            if i is None and args is None and kwargs is None:
+            (i, task) = req.wait()
+            if i is None and task is None:
                 return
             logger.debug('Rang %i %s Starting doing the job %i',
                          comm.Get_rank(),
                          socket.gethostname(),
                          i)
-            res = self.do_the_job(args, kwargs)
+            res = self.do_the_job(task)
             req = comm.isend((i, res), dest=0)
             req.wait()
 
 
-class SimpleWorker(Worker):
-    """Simplest implementation of worker"""
-    def __init__(self, model: Model):
-        self.model = model
-
-    def start(self):
-        """Start of worker"""
-
-    def do_the_job(self, args: Tuple[Any], kwargs: Dict[str, Any]) -> Any:
-        """Get model results"""
-        return self.model.results(*args, **kwargs)
-
-
-class SimpleMultiprocessingWorker(SimpleWorker, MultiprocessingWorker):
-    """Simplest multiprocessing worker"""
-
-
-class SimpleMPIWorker(SimpleWorker, MPIWorker):
-    """Simplest MPI worker"""
-
-
 # noinspection PyMissingOrEmptyDocstring
 class ComsolWorker(Worker):
-    def __init__(self, model: ComsolModel, filepath: str or Path,
-                 mph_options: dict = None,
-                 client_args=None,
-                 client_kwargs=None):
+    def __init__(
+            self,
+            model: ComsolModel,
+            filepath: str or Path,
+            mph_options: dict = None,
+            client_args=None,
+            client_kwargs=None
+    ):
         if not isinstance(model, ComsolModel):
             raise TypeError('Model has to be an object of ComsolModel class')
 
+        super(ComsolWorker, self).__init__(model=model)
+
         self.client = None
         self.model = model
 
         self._mph_options = {} if mph_options is None else mph_options
         self._client_args = [] if client_args is None else client_args
         self._client_kwargs = {} if client_kwargs is None else client_kwargs
         self._filepath = filepath
@@ -145,22 +138,22 @@
         for option in self._mph_options:
             mph.option(option, self._mph_options[option])
         logger.debug(f'Opening COMSOL model {self._filepath}')
         self.client = mph.start(*self._client_args, **self._client_kwargs)  # type: mph.client
         self.model.java = self.client.load(self._filepath).java
         self.model.configure()
 
-    def do_the_job(self, args, kwargs) -> Any:
-        self.model.pre_build(*args, **kwargs)
+    def do_the_job(self, task: Task) -> Result:
+        self.model.pre_build(task)
         self.model.build()
-        self.model.pre_solve(*args, **kwargs)
+        self.model.pre_solve(task)
         self.model.mesh()
         self.model.solve()
-        results = self.model.results(*args, **kwargs)
-        self.model.pre_clear(*args, **kwargs)
+        results = self.model.results(task)
+        self.model.pre_clear(task)
         self.model.clear()
         return results
 
 
 # noinspection PyMissingOrEmptyDocstring
 class ComsolMultiprocessingWorker(ComsolWorker, MultiprocessingWorker):
     def start(self):
```

### Comparing `pckit-0.2.2/pyproject.toml` & `pckit-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "pckit"
-version = "0.2.2"
+version = "0.3.0"
 description = "A simple package for parallel computing with Python"
 authors = ["djiboshin"]
 readme = "README.md"
 homepage = "https://github.com/djiboshin/pckit"
 repository = "https://github.com/djiboshin/pckit"
 license = "MIT"
 
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-numpy = "^1.22.3"
-pandas = "^1.4.2"
+python = "^3.9"
+numpy = "^1.25.2"
+pandas = "^2.0.3"
 MPh = "^1.1.5"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.4.0"
 pylint = "^2.13.8"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.1.0"
 tqdm = "^4.64.0"
 mpi4py = "^3.1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pckit-0.2.2/PKG-INFO` & `pckit-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pckit
-Version: 0.2.2
-Summary: A simple package for parallel computing with Python
-Home-page: https://github.com/djiboshin/pckit
-License: MIT
-Author: djiboshin
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: MPh (>=1.1.5,<2.0.0)
-Requires-Dist: numpy (>=1.22.3,<2.0.0)
-Requires-Dist: pandas (>=1.4.2,<2.0.0)
-Project-URL: Repository, https://github.com/djiboshin/pckit
-Description-Content-Type: text/markdown
-
 # pckit
 
 This is a simple package for parallel computing with Python.
 
 ## Usage
 ### Multiprocessing
 If you want to use any solver from the package you have to wrap your functions into a model. 
@@ -28,58 +9,58 @@
 `MyModel` is a subclass of the package `Model`. The method `results` is required.
 
 ```python
 import pckit
 
 
 class MyModel(pckit.Model):
-    def results(self, x):
+    def results(self, x: int) -> int:
         # Solve here problem f(x) = x^2
         return x ** 2
 
 
 if __name__ == '__main__':
     model = MyModel()
-    worker = pckit.SimpleMultiprocessingWorker(model)
+    worker = pckit.MultiprocessingWorker(model)
     with pckit.get_solver(worker, workers_num=2) as solver:
         # Create tasks to solve. You can put args or
         # kwargs for model.results() method in the Task
-        tasks = [pckit.Task(2), pckit.Task(x=3)]
+        tasks = [2, 3]
         results = solver.solve(tasks)
         print(results)
         # >>> [4, 9]
 ```
 
 ### MPI
 You can easily run scripts on the cluster with [mpi4py](https://github.com/mpi4py/mpi4py) implementation on MPI (See [mpi4py installation docs](https://mpi4py.readthedocs.io/en/stable/install.html)).
-Simply change `SimpleMultiprocessingWorker` to `SimpleMPIWorker` in the previous example and start the script with MPI `mpiexec -np 3 python -m mpi4py your_script.py`
+Simply change `MultiprocessingWorker` to `MPIWorker` in the previous example and start the script with MPI `mpiexec -np 3 python -m mpi4py your_script.py`
 
 ```python
-worker = pckit.SimpleMPIWorker(model)
+worker = pckit.MPIWorker(model)
 ```
 Moreover, a multiprocessing solver can be started inside an MPI solver.
 
 ### Single thread
-Single threaded execution is also available with `SimpleWorker`
+Single threaded execution is also available with `Worker`
 
 ```python
-worker = pckit.SimpleWorker(model)
+worker = pckit.Worker(model)
 ```
 
 ### Examples
 [More examples](https://github.com/djiboshin/pckit/tree/main/examples)
 
 ## Features
 ### Cache
 Dict based cache is available by `caching` argument in `get_solver()`.
-`tag` property in `Task` is required and has to be hashable.
+Tasks are required to be hashable.
 
 ```python
 with pckit.get_solver(worker, caching=True) as solver:
-    tasks = [pckit.Task(2, tag='2'), pckit.Task(2, tag='2')]
+    tasks = [2, 2]
 ```
 The second task's solution will be reused from the cache.
 
 ### Custom iterators
 You can send the email or print anything with custom iterator.
 [tqdm](https://pypi.org/project/tqdm/) is also supported.
 ```python
@@ -89,8 +70,7 @@
 ```
 See [example](https://github.com/djiboshin/pckit/blob/main/examples/custom_iterator.py) to create your own iterator.
 
 ### Comsol Models, Solvers, Workers
 Based on [MPh](https://pypi.org/project/MPh/) package.
 
 **TBD**ocumented
-
```

