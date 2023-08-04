# Comparing `tmp/teneva_opti-0.3.3.tar.gz` & `tmp/teneva_opti-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_opti-0.3.3.tar", last modified: Wed Aug  2 19:32:13 2023, max compression
+gzip compressed data, was "teneva_opti-0.3.4.tar", last modified: Fri Aug  4 14:23:27 2023, max compression
```

## Comparing `teneva_opti-0.3.3.tar` & `teneva_opti-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.059709 teneva_opti-0.3.3/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.3/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.3/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-02 19:32:13.059913 teneva_opti-0.3.3/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1923 2023-08-02 19:32:03.000000 teneva_opti-0.3.3/README.md
--rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-02 16:02:49.000000 teneva_opti-0.3.3/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      137 2023-08-02 19:19:40.000000 teneva_opti-0.3.3/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-02 19:32:13.060403 teneva_opti-0.3.3/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.3/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.051117 teneva_opti-0.3.3/teneva_opti/
--rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-02 19:31:58.000000 teneva_opti-0.3.3/teneva_opti/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.053841 teneva_opti-0.3.3/teneva_opti/func/
--rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.3/teneva_opti/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     6277 2023-08-02 19:31:20.000000 teneva_opti-0.3.3/teneva_opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      113 2023-07-31 13:44:41.000000 teneva_opti-0.3.3/teneva_opti/opti_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     2442 2023-08-02 19:03:37.000000 teneva_opti-0.3.3/teneva_opti/opti_manager.py
--rw-r--r--   0 andrei     (501) staff       (20)     1043 2023-08-02 15:52:07.000000 teneva_opti-0.3.3/teneva_opti/opti_tens.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.059063 teneva_opti-0.3.3/teneva_opti/tens/
--rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.3/teneva_opti/tens/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)     2090 2023-08-02 14:22:10.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1289 2023-08-02 14:22:01.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.3/teneva_opti/utils.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.053425 teneva_opti-0.3.3/teneva_opti.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      740 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)      137 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.819507 teneva_opti-0.3.4/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.4/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.4/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-04 14:23:27.819646 teneva_opti-0.3.4/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1923 2023-08-04 14:22:51.000000 teneva_opti-0.3.4/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-04 12:11:01.000000 teneva_opti-0.3.4/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      137 2023-08-04 11:56:04.000000 teneva_opti-0.3.4/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-04 14:23:27.820145 teneva_opti-0.3.4/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.4/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.812004 teneva_opti-0.3.4/teneva_opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-04 14:22:30.000000 teneva_opti-0.3.4/teneva_opti/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7856 2023-08-04 14:18:29.000000 teneva_opti-0.3.4/teneva_opti/bm_view.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.814038 teneva_opti-0.3.4/teneva_opti/func/
+-rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.4/teneva_opti/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6795 2023-08-04 13:52:05.000000 teneva_opti-0.3.4/teneva_opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      171 2023-08-04 11:59:34.000000 teneva_opti-0.3.4/teneva_opti/opti_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6992 2023-08-04 13:39:55.000000 teneva_opti-0.3.4/teneva_opti/opti_manager.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2357 2023-08-04 13:41:01.000000 teneva_opti-0.3.4/teneva_opti/opti_tens.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.819229 teneva_opti-0.3.4/teneva_opti/tens/
+-rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.4/teneva_opti/tens/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2393 2023-08-04 13:57:19.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1586 2023-08-04 13:43:52.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.4/teneva_opti/utils.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.813697 teneva_opti-0.3.4/teneva_opti.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      763 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      137 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/top_level.txt
```

### Comparing `teneva_opti-0.3.3/LICENSE.txt` & `teneva_opti-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.3/PKG-INFO` & `teneva_opti-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_opti
-Version: 0.3.3
+Version: 0.3.4
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
@@ -30,15 +30,15 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.3.3".
+> Current version "0.3.4".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
 We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
```

### Comparing `teneva_opti-0.3.3/README.md` & `teneva_opti-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.3.3".
+> Current version "0.3.4".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
 We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
```

### Comparing `teneva_opti-0.3.3/demo.py` & `teneva_opti-0.3.4/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.3/setup.py` & `teneva_opti-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.3/teneva_opti/opti.py` & `teneva_opti-0.3.4/teneva_opti/opti.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self.log = Log(self.fpath('log') if log_file else None, log, log_info)
         self.bm.set_log(self.log, prefix=self.name,
             cond=('max' if self.is_max else 'min'),
             with_max=self.is_max, with_min=not self.is_max)
 
         self.is_fail = False
 
+        self.init()
         self.set_opts()
 
     @property
     def d(self):
         return self.bm.d
 
     @property
@@ -51,22 +52,32 @@
         return self.bm.i_max if self.is_max else self.bm.i_min
 
     @property
     def identity(self):
         return ['seed', 'm']
 
     @property
+    def is_func(self):
+        """Check if the optimizer is continuous."""
+        return not self.is_tens
+
+    @property
     def is_max(self):
         return self.bm.is_opti_max
 
     @property
     def is_n_equal(self):
         return self.bm.is_n_equal
 
     @property
+    def is_tens(self):
+        """Check if the optimizer is discrete."""
+        return not self.is_func
+
+    @property
     def n(self):
         return self.bm.n
 
     @property
     def n0(self):
         return self.bm.n0
 
@@ -92,14 +103,16 @@
         conf = {}
         conf['d'] = self.d
         conf['n'] = self.bm.list_convert(self.n, 'int')
         conf['m'] = self.m
         conf['seed'] = self.seed
         conf['name'] = self.name
         conf['machine'] = self.machine
+        conf['is_func'] = self.is_func
+        conf['is_tens'] = self.is_tens
         conf['opti'] = self.__class__.__name__
         conf['bm'] = self.bm.get_config()
         return conf
 
     def get_history(self):
         """Return a dict with optimization results."""
         hist = {}
@@ -146,23 +159,30 @@
         v = self.m
         text += f'{v}\n'
 
         text += 'Optimizer                                : '
         v = self.__class__.__name__
         text += f'{v}\n'
 
+        text += 'Optimization task                        : '
+        v = 'maximize' if self.is_max else 'minimize'
+        text += f'{v}\n'
+
         if footer:
             text += '-' * 41 + '|             '
             text += '>               Options'
             text += '\n'
             text += footer
 
         text += '#' * 78 + '\n'
         return text
 
+    def init(self):
+        return
+
     def load(self, fpath=None):
         """Load configuration and optimization result from npz file."""
         fpath = path(fpath or self.fpath('data'), 'npz')
         data = np.load(fpath, allow_pickle=True).get('data').item()
         return data
 
     def run(self, with_err=True):
```

### Comparing `teneva_opti-0.3.3/teneva_opti/tens/opti_tens_optimatt.py` & `teneva_opti-0.3.4/teneva_opti/tens/opti_tens_optimatt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.3/teneva_opti/tens/opti_tens_protes.py` & `teneva_opti-0.3.4/teneva_opti/tens/opti_tens_protes.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     def get_config(self):
         conf = super().get_config()
         conf['k'] = self.k
         conf['k_top'] = self.k_top
         conf['k_gd'] = self.k_gd
         conf['lr'] = self.lr
         conf['r'] = self.r
+        conf['quan'] = self.quan
+        conf['with_quan'] = self.with_quan
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'k (batch size)                           : '
         v = self.k
@@ -51,25 +53,31 @@
         v = self.lr
         text += f'{v}\n'
 
         text += 'r (TT-rank of the inner prob tensor)     : '
         v = self.r
         text += f'{v}\n'
 
+        if self.with_quan:
+            text += 'quan (use quantization of tensor modes)  : '
+            v = 'YES' if self.with_quan else 'no'
+            text += f'{v}\n'
+
         return super().info(text + footer)
 
-    def set_opts(self, k=100, k_top=10, k_gd=1, lr=5.E-2, r=5):
+    def set_opts(self, k=100, k_top=10, k_gd=1, lr=5.E-2, r=5, quan=True):
         self.k = k
         self.k_top = k_top
         self.k_gd = k_gd
         self.lr = lr
         self.r = r
+        self.quan = quan
 
     def _optimize(self):
         if self.is_n_equal:
-            protes(self.target, self.d, self.n0, 1.E+99,
+            protes(self.target, self.d_inner, self.n0_inner, 1.E+99,
                 k=self.k, k_top=self.k_top, k_gd=self.k_gd, lr=self.lr,
                 r=self.r, seed=self.seed, is_max=self.is_max)
         else:
-            protes_general(self.target, self.n, 1.E+99,
+            protes_general(self.target, self.n_inner, 1.E+99,
                 k=self.k, k_top=self.k_top, k_gd=self.k_gd, lr=self.lr,
                 r=self.r, seed=self.seed, is_max=self.is_max)
```

### Comparing `teneva_opti-0.3.3/teneva_opti/tens/opti_tens_ttopt.py` & `teneva_opti-0.3.4/teneva_opti/tens/opti_tens_ttopt.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,31 +17,39 @@
     def __init__(self, *args, **kwargs):
         super().__init__('ttopt', DESC, *args, **kwargs)
 
     def get_config(self):
         conf = super().get_config()
         conf['rank'] = self.rank
         conf['fs_opt'] = self.fs_opt
+        conf['quan'] = self.quan
+        conf['with_quan'] = self.with_quan
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'rank (TT-rank)                           : '
         v = self.rank
         text += f'{v}\n'
 
         text += 'fs_opt (transformation option)           : '
         v = self.fs_opt
         text += f'{v}\n'
 
+        if self.with_quan:
+            text += 'quan (use quantization of tensor modes)  : '
+            v = 'YES' if self.with_quan else 'no'
+            text += f'{v}\n'
+
         return super().info(text + footer)
 
-    def set_opts(self, rank=4, fs_opt=1.):
+    def set_opts(self, rank=4, fs_opt=1., quan=True):
         self.rank = rank
         self.fs_opt = fs_opt
+        self.quan = quan
 
     def _optimize(self):
-        tto = TTOpt(f=self.target, d=self.d, n=self.n,
+        tto = TTOpt(f=self.target, d=self.d_inner, n=self.n_inner,
             evals=1.E+99, is_func=False, is_vect=True)
         tto.optimize(rank=self.rank, seed=self.seed,
             fs_opt=self.fs_opt, is_max=self.is_max)
```

### Comparing `teneva_opti-0.3.3/teneva_opti/utils.py` & `teneva_opti-0.3.4/teneva_opti/utils.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.3/teneva_opti.egg-info/PKG-INFO` & `teneva_opti-0.3.4/teneva_opti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-opti
-Version: 0.3.3
+Version: 0.3.4
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
@@ -30,15 +30,15 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.3.3".
+> Current version "0.3.4".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
 We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
```

### Comparing `teneva_opti-0.3.3/teneva_opti.egg-info/SOURCES.txt` & `teneva_opti-0.3.4/teneva_opti.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 demo.py
 requirements.txt
 setup.cfg
 setup.py
 teneva_opti/__init__.py
+teneva_opti/bm_view.py
 teneva_opti/opti.py
 teneva_opti/opti_func.py
 teneva_opti/opti_manager.py
 teneva_opti/opti_tens.py
 teneva_opti/utils.py
 teneva_opti.egg-info/PKG-INFO
 teneva_opti.egg-info/SOURCES.txt
```

