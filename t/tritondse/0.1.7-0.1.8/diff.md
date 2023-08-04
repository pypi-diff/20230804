# Comparing `tmp/tritondse-0.1.7.tar.gz` & `tmp/tritondse-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritondse-0.1.7.tar", last modified: Sat Jul 29 12:32:53 2023, max compression
+gzip compressed data, was "tritondse-0.1.8.tar", last modified: Fri Aug  4 21:30:40 2023, max compression
```

## Comparing `tritondse-0.1.7.tar` & `tritondse-0.1.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.871581 tritondse-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 12:32:50.000000 tritondse-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-29 12:32:53.871581 tritondse-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-29 12:32:50.000000 tritondse-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:32:53.871581 tritondse-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 12:32:50.000000 tritondse-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.867581 tritondse-0.1.7/tritondse/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    36167 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29299 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/heap_allocator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.871581 tritondse-0.1.7/tritondse/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/cle_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/quokkaprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.871581 tritondse-0.1.7/tritondse/probes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/probes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/probes/basic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    52218 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/process_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/qbdi_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    75406 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/sanitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/seeds_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    36666 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/symbolic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/symbolic_explorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/thread_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/worklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.871581 tritondse-0.1.7/tritondse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 21:30:37.000000 tritondse-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-04 21:30:40.095861 tritondse-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-08-04 21:30:37.000000 tritondse-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:30:40.095861 tritondse-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-04 21:30:37.000000 tritondse-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/tritondse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36167 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29299 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/heap_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/tritondse/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/cle_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/quokkaprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/tritondse/probes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/probes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/probes/basic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52429 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/process_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/qbdi_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75406 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/sanitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/seeds_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/symbolic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/symbolic_explorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/thread_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/worklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/tritondse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/top_level.txt
```

### Comparing `tritondse-0.1.7/LICENSE` & `tritondse-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/PKG-INFO` & `tritondse-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.7 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.8 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.7/README.md` & `tritondse-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/setup.py` & `tritondse-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md") as f:
     README = f.read()
 
 
 setup(
     name="tritondse",
-    version="0.1.7",
+    version="0.1.8",
     description="A library of Dynamic Symbolic Exploration based the Triton library",
     packages=find_packages(),
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/quarkslab/tritondse",
     project_urls={
         "Documentation": "https://quarkslab.github.io/tritondse/",
```

### Comparing `tritondse-0.1.7/tritondse/__init__.py` & `tritondse-0.1.8/tritondse/__init__.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/arch.py` & `tritondse-0.1.8/tritondse/arch.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/callbacks.py` & `tritondse-0.1.8/tritondse/callbacks.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/config.py` & `tritondse-0.1.8/tritondse/config.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/coverage.py` & `tritondse-0.1.8/tritondse/coverage.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/exception.py` & `tritondse-0.1.8/tritondse/exception.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/heap_allocator.py` & `tritondse-0.1.8/tritondse/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/loaders/cle_loader.py` & `tritondse-0.1.8/tritondse/loaders/cle_loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/loaders/loader.py` & `tritondse-0.1.8/tritondse/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/loaders/program.py` & `tritondse-0.1.8/tritondse/loaders/program.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/loaders/quokkaprogram.py` & `tritondse-0.1.8/tritondse/loaders/quokkaprogram.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/logging.py` & `tritondse-0.1.8/tritondse/logging.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/memory.py` & `tritondse-0.1.8/tritondse/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,20 +149,21 @@
         """
         Context manager enabling manipulating temporarily the memory
         without considering the memory permissions.
         E.g: It enables writing data in a memory mapped in RX
         :param disable_callbacks: Whether to disable memory callbacks that could have been set
         :return:
         """
+        previous = self._segment_enabled
         self.disable_segmentation()
         cbs = self._mem_cbs_enabled
         self._mem_cbs_enabled = not disable_callbacks
         yield self
         self._mem_cbs_enabled = cbs
-        self.enable_segmentation()
+        self.set_segmentation(previous)
 
     def callbacks_enabled(self) -> bool:
         """
         Return whether memory callbacks are enabled.
 
         :return: True if callbacks are enabled
         """
```

### Comparing `tritondse-0.1.7/tritondse/probes/basic_trace.py` & `tritondse-0.1.8/tritondse/probes/basic_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/process_state.py` & `tritondse-0.1.8/tritondse/process_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -499,38 +499,41 @@
 
     def is_syscall(self) -> bool:
         """
         Check whether the current instrution fetched is a syscall or not.
         """
         return bool(self.current_instruction.getType() in self._archinfo.syscall_inst)
 
-    def fetch_instruction(self, address: Addr = None, set_as_current: bool = True) -> Instruction:
+    def fetch_instruction(self, address: Addr = None, set_as_current: bool = True, disable_callbacks: bool = True) -> Instruction:
         """
         Fetch the instruction at the given address. If no address
         is specified the current program counter one is used.
 
         :raise MemoryAccessViolation: If the instruction cannot be fetched in the memory.
 
         :param address: address where to get the instruction from
         :param set_as_current: set as the current instruction in the process state
+        :param disable_callbacks: whether memory callbacks should be disabled to fetch memory bytes
         :return: instruction disassembled
         """
         if address is None:
             address = self.cpu.program_counter
-        with self.memory.without_segmentation(disable_callbacks=True):
+        with self.memory.without_segmentation(disable_callbacks=disable_callbacks):
             data = self.memory.read(address, 16)
         i = Instruction(address, data)
         i.setThreadId(self.current_thread.tid)
         self.tt_ctx.disassembly(i)  # This needs to be done before using i.getSize()
                                     # otherwise, i.getSize() will always be 16
-        map = self.memory.get_map(address, i.getSize())
-        if map is None:
-            raise MemoryAccessViolation(address, Perm.X, memory_not_mapped=True)
-        if Perm.X not in map.perm:  # Note: in this model we can execute code in non-readable pages
-            raise MemoryAccessViolation(address, Perm.X, map_perm=map.perm, perm_error=True)
+
+        if self.memory.segmentation_enabled:
+            map = self.memory.get_map(address, i.getSize())
+            if map is None:
+                raise MemoryAccessViolation(address, Perm.X, memory_not_mapped=True)
+            if Perm.X not in map.perm:  # Note: in this model we can execute code in non-readable pages
+                raise MemoryAccessViolation(address, Perm.X, map_perm=map.perm, perm_error=True)
         if set_as_current:
             self.__current_inst = i
         return i
 
     def process_instruction(self, instruction: Instruction) -> bool:
         """
         Process the given triton instruction on this process state.
```

### Comparing `tritondse-0.1.7/tritondse/qbdi_trace.py` & `tritondse-0.1.8/tritondse/qbdi_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/routines.py` & `tritondse-0.1.8/tritondse/routines.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/sanitizers.py` & `tritondse-0.1.8/tritondse/sanitizers.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/seed.py` & `tritondse-0.1.8/tritondse/seed.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,26 @@
         :param status: status of the seed if any, otherwise :py:obj:`SeedStatus.NEW`
         :type status: SeedStatus
 
         :returns: fresh seed instance
         :rtype: Seed
         """
         raw = Path(path).read_bytes()
-        return Seed.from_bytes(raw, status)
+
+        seed = Seed.from_bytes(raw, status)
+
+        # Parse filename to extract back metadata if any
+        name = Path(path).name
+        if name.endswith(".tritondse.cov"):
+            name = name.replace(".tritondse.cov", "")
+        metas = name.split("_")
+        if len(metas) >= 4:
+            seed.meta_fname = metas[3:]
+
+        return seed
 
     # Utility function for composite seeds
     def is_file_defined(self, name: str) -> bool:
         if self.is_composite():
             return name in self.content.files
         else:
             return False
```

### Comparing `tritondse-0.1.7/tritondse/seeds_manager.py` & `tritondse-0.1.8/tritondse/seeds_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,18 @@
 
                 typ, p_prefix, branch, covitem, ith = path_generator.send(status)
 
                 # Create edge in case of conditional branch, for all the other the edge shall be already set
                 edge = (branch['srcAddr'], branch['dstAddr']) if typ == SymExType.CONDITIONAL_JMP else covitem
 
                 # Call on_branch_solving, if one replies False does not solve the branch
-                cb_result = all(cb(execution, execution.pstate, edge, typ) for cb in self.cbm.get_on_solving_callback())
+                if self.cbm is not None:
+                    cb_result = all(cb(execution, execution.pstate, edge, typ) for cb in self.cbm.get_on_solving_callback())
+                else:
+                    cb_result = True
 
                 # Add path_prefix in path predicate (regardless on whether we solve the item or not)
                 path_predicate.extend(x.getTakenPredicate() for x in p_prefix)
 
                 # Skip processing the current path in case the result of the
                 # callbacks return False.
                 if not cb_result:
```

### Comparing `tritondse-0.1.7/tritondse/symbolic_executor.py` & `tritondse-0.1.8/tritondse/symbolic_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,36 +252,50 @@
             return
         if lea_ast.isSymbolized():
             s = "write" if bool(args) else "read"
             pc = self.pstate.cpu.program_counter
             logger.debug(f"symbolic {s} at 0x{pc:x}: target: 0x{tgt_addr:x} [{lea_ast}]")
             self.pstate.push_constraint(lea_ast == tgt_addr, f"sym-{s}:{self.trace_offset}:{pc}")
 
-    def __emulate(self):
+    def emulate(self):
         while not self.pstate.stop and self.pstate.threads:
+            if not self.step():
+                break
+        if not self.seed.is_status_set():  # Set a status if it has not already been done
+            self.seed.status = SeedStatus.OK_DONE
+        return
+
+
+    def step(self) -> bool:
+        """
+        Perform a single instruction step. Returns whether the emulation can
+        continue or we have to stop.
+        """
+        try:
             # Schedule thread if it's time
             self.__schedule_thread()
 
             if not self.pstate.current_thread.is_running():
                 logger.warning(f"After scheduling current thread is not running (probably in a deadlock state)")
-                break  # Were not able to find a suitable thread thus exit emulation
+                return False  # Were not able to find a suitable thread thus exit emulation
 
             # Fetch program counter (of the thread selected), at this point the current thread should be running!
             self.current_pc = self.pstate.cpu.program_counter  # should normally be already set but still.
 
             if self.current_pc == self._run_to_target:  # Hit the location we wanted to reach
-                break
+                return False
 
             if self.current_pc == 0:
                 logger.error(f"PC=0, is it normal ? (stop)")
-                break
+                return False
 
-            if not self.pstate.memory.has_ever_been_written(self.current_pc, CPUSIZE.BYTE):
-                logger.error(f"Instruction not mapped: 0x{self.current_pc:x}")
-                break
+            if self.pstate.memory.segmentation_enabled:
+                if not self.pstate.memory.has_ever_been_written(self.current_pc, CPUSIZE.BYTE):
+                    logger.error(f"Instruction not mapped: 0x{self.current_pc:x}")
+                    return False
 
             instruction = self.pstate.fetch_instruction()
             opcode = instruction.getOpcode()
             mnemonic = instruction.getType()
 
             try:
                 # Trigger pre-address callback
@@ -300,15 +314,15 @@
                     cb(self, self.pstate, mnemonic)
 
                 # Trigger pre-instruction callback
                 pre_insts, post_insts = self.cbm.get_instruction_callbacks()
                 for cb in pre_insts:
                     cb(self, self.pstate, instruction)
             except SkipInstructionException as _:
-                continue
+                return True
 
             if self.pstate.is_syscall():
                 logger.warning(f"execute syscall instruction {self.pstate.read_register(self.pstate._syscall_register)}")
 
             # Process
             prev_pc = self.current_pc
             self._in_processing = True
@@ -317,15 +331,15 @@
                     logger.info(f"hit {str(instruction)} instruction stop.")
                 else:
                     logger.error('Instruction not supported: %s' % (str(instruction)))
 
                 if self.config.skip_unsupported_instruction:
                     self.pstate.cpu.program_counter += instruction.getSize() # try to jump over the instruction
                 else:
-                    break  # stop emulation
+                    return False  # stop emulation
             self._in_processing = False
             # increment trace offset
             self.trace_offset += 1
 
             # update previous program counters
             self.previous_pc = prev_pc
             self.current_pc = self.pstate.cpu.program_counter  # current_pc becomes new instruction pointer
@@ -378,25 +392,36 @@
 
             # Simulate routines
             try:
                 self._routines_handler(instruction)
             except AllocatorException as e:
                 logger.info(f'An exception has been raised: {e}')
                 self.seed.status = SeedStatus.CRASH
-                return
+                return False
 
             # Check timeout of the execution
             if self.config.execution_timeout and (time.time() - self.start_time) >= self.config.execution_timeout:
                 logger.info('Timeout of an execution reached')
                 self.seed.status = SeedStatus.HANG
-                return
+                return False
+            return True
+        except AbortExecutionException as e:
+            return False
+        except MemoryAccessViolation as e:
+            logger.warning(f"Memory violation: {str(e)}")
+
+            # Call all the callbacks on the memory violations
+            for cb in self.callback_manager.get_memory_violation_callbacks():
+                cb(self, self.pstate, e)
+
+            # Assign the seed the status of crash
+            if not self.seed.is_status_set():
+                self.seed.status = SeedStatus.CRASH
+            return False
 
-        if not self.seed.is_status_set():  # Set a status if it has not already been done
-            self.seed.status = SeedStatus.OK_DONE
-        return
 
     def __handle_external_return(self, routine_name: str, ret_val: Optional[Union[int, Expression]]) -> None:
         """ Symbolize or concretize return values of external functions """
         if ret_val is not None:
             reg = self.pstate.return_register
             if isinstance(ret_val, int): # Write its concrete value
                 self.pstate.write_register(reg, ret_val)
@@ -526,30 +551,18 @@
         Function to call to stop the whole exploration of
         the program. It raises an exception which is caught by SymbolicExplorator.
 
         :raise StopExplorationException: to stop the exploration
         """
         raise StopExplorationException("Stop exploration")
 
-    def run(self, stop_at: Addr = None) -> None:
-        """
-        Execute the program.
-
-        If the :py:attr:`tritondse.Config.execution_timeout` is not set
-        the execution might hang forever if the program does.
-
-        :param stop_at: Address where to stop (if necessary)
-        :return: None
-        """
-        if stop_at:
-            self._run_to_target = stop_at
-
+    def emulation_init(self) -> bool:
         if self.pstate is None:
             logger.error(f"ProcessState is None (have you called \"load\"?")
-            return
+            return False
 
         self.start_time = time.time()
 
         # Configure memory segmentation using configuration
         self.pstate.memory.set_segmentation(self.config.memory_segmentation)
         if self.config.memory_segmentation:
             self.cbm.register_memory_read_callback(self._mem_accesses_callback)
@@ -571,30 +584,41 @@
         pre_cb, post_cb = self.cbm.get_execution_callbacks()
         # Iterate through all pre exec callbacks
         for cb in pre_cb:
             cb(self, self.pstate)
 
         # Call it here to make sure in case of "load_process" the use has properly instanciated the architecture
         self._configure_pstate()
+        return True
 
-        try:
-            self.__emulate()
-        except AbortExecutionException as e:
-            pass
-        except MemoryAccessViolation as e:
-            logger.warning(f"Memory violation: {str(e)}")
+    def run(self, stop_at: Addr = None) -> None:
+        """
+        Execute the program.
 
-            # Call all the callbacks on the memory violations
-            for cb in self.callback_manager.get_memory_violation_callbacks():
-                cb(self, self.pstate, e)
+        If the :py:attr:`tritondse.Config.execution_timeout` is not set
+        the execution might hang forever if the program does.
 
-            # Assign the seed the status of crash
-            if not self.seed.is_status_set():
-                self.seed.status = SeedStatus.CRASH
+        :param stop_at: Address where to stop (if necessary)
+        :return: None
+        """
+        if stop_at:
+            self._run_to_target = stop_at
+
+        # Call init steps
+        if not self.emulation_init():
+            return
+
+        # Run until reaching a stopping condition
+        self.emulate()
+
+        # Call termination steps
+        self.emulation_deinit()
 
+    def emulation_deinit(self):
+        _, post_cb = self.cbm.get_execution_callbacks()
         # Iterate through post exec callbacks
         for cb in post_cb:
             cb(self, self.pstate)
 
         self.end_time = time.time()
 
         # IMPORTANT The next call is necessary otherwise there is a memory
```

### Comparing `tritondse-0.1.7/tritondse/symbolic_explorator.py` & `tritondse-0.1.8/tritondse/symbolic_explorator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/thread_context.py` & `tritondse-0.1.8/tritondse/thread_context.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/trace.py` & `tritondse-0.1.8/tritondse/trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/types.py` & `tritondse-0.1.8/tritondse/types.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/worklist.py` & `tritondse-0.1.8/tritondse/worklist.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse/workspace.py` & `tritondse-0.1.8/tritondse/workspace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.7/tritondse.egg-info/PKG-INFO` & `tritondse-0.1.8/tritondse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.7 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.8 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.7/tritondse.egg-info/SOURCES.txt` & `tritondse-0.1.8/tritondse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

