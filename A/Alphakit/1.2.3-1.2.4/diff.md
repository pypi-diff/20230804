# Comparing `tmp/Alphakit-1.2.3.tar.gz` & `tmp/Alphakit-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Alphakit-1.2.3.tar", last modified: Fri Jul 14 07:03:55 2023, max compression
+gzip compressed data, was "dist/Alphakit-1.2.4.tar", last modified: Wed Jul 19 02:29:58 2023, max compression
```

## Comparing `Alphakit-1.2.3.tar` & `Alphakit-1.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:03:55.000000 Alphakit-1.2.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:03:55.000000 Alphakit-1.2.3/Alphakit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-14 07:03:54.000000 Alphakit-1.2.3/Alphakit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-07-14 07:03:55.000000 Alphakit-1.2.3/Alphakit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 07:03:54.000000 Alphakit-1.2.3/Alphakit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-14 07:03:54.000000 Alphakit-1.2.3/Alphakit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-14 07:03:54.000000 Alphakit-1.2.3/Alphakit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-14 06:11:10.000000 Alphakit-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-14 06:11:10.000000 Alphakit-1.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-14 07:03:55.000000 Alphakit-1.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-14 06:11:10.000000 Alphakit-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:03:55.000000 Alphakit-1.2.3/alphakit/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-14 07:03:20.000000 Alphakit-1.2.3/alphakit/__init__.py
--rw-r--r--   0 root         (0) root         (0)   123259 2023-07-14 06:14:41.000000 Alphakit-1.2.3/alphakit/const.c
--rw-r--r--   0 root         (0) root         (0)      701 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/const.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:03:55.000000 Alphakit-1.2.3/alphakit/data/
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)   780357 2023-07-14 06:14:41.000000 Alphakit-1.2.3/alphakit/data/calculator.c
--rw-r--r--   0 root         (0) root         (0)     7937 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/data/calculator.pyx
--rw-r--r--   0 root         (0) root         (0)   167556 2023-07-14 06:14:41.000000 Alphakit-1.2.3/alphakit/data/processing.c
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/data/processing.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:03:55.000000 Alphakit-1.2.3/alphakit/factor/
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/factor/__init__.py
--rw-r--r--   0 root         (0) root         (0)   292909 2023-07-14 06:14:41.000000 Alphakit-1.2.3/alphakit/factor/analysis.c
--rw-r--r--   0 root         (0) root         (0)     3799 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/factor/analysis.pyx
--rw-r--r--   0 root         (0) root         (0)   366743 2023-07-14 06:14:41.000000 Alphakit-1.2.3/alphakit/factor/metrics.c
--rw-r--r--   0 root         (0) root         (0)     4267 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/factor/metrics.pyx
--rw-r--r--   0 root         (0) root         (0)   304805 2023-07-14 06:14:41.000000 Alphakit-1.2.3/alphakit/factor/processing.c
--rw-r--r--   0 root         (0) root         (0)     4718 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/factor/processing.pyx
--rw-r--r--   0 root         (0) root         (0)   205219 2023-07-14 07:03:54.000000 Alphakit-1.2.3/alphakit/factor/transform.c
--rw-r--r--   0 root         (0) root         (0)     1509 2023-07-14 06:54:48.000000 Alphakit-1.2.3/alphakit/factor/transform.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:03:55.000000 Alphakit-1.2.3/alphakit/portfolio/
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/portfolio/__init__.py
--rw-r--r--   0 root         (0) root         (0)   152583 2023-07-14 06:14:41.000000 Alphakit-1.2.3/alphakit/portfolio/combine.c
--rw-r--r--   0 root         (0) root         (0)      480 2023-07-14 06:11:10.000000 Alphakit-1.2.3/alphakit/portfolio/combine.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:03:55.000000 Alphakit-1.2.3/requirements/
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-14 06:11:10.000000 Alphakit-1.2.3/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 07:03:55.000000 Alphakit-1.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3332 2023-07-14 06:11:10.000000 Alphakit-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:29:58.000000 Alphakit-1.2.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:29:58.000000 Alphakit-1.2.4/Alphakit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-19 02:29:58.000000 Alphakit-1.2.4/Alphakit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-19 02:29:58.000000 Alphakit-1.2.4/Alphakit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:29:58.000000 Alphakit-1.2.4/Alphakit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-19 02:29:58.000000 Alphakit-1.2.4/Alphakit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-19 02:29:58.000000 Alphakit-1.2.4/Alphakit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-14 06:11:10.000000 Alphakit-1.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-14 06:11:10.000000 Alphakit-1.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-19 02:29:58.000000 Alphakit-1.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-14 06:11:10.000000 Alphakit-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:29:58.000000 Alphakit-1.2.4/alphakit/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 02:29:18.000000 Alphakit-1.2.4/alphakit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   123259 2023-07-14 06:14:41.000000 Alphakit-1.2.4/alphakit/const.c
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-14 06:11:10.000000 Alphakit-1.2.4/alphakit/const.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:29:58.000000 Alphakit-1.2.4/alphakit/data/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-14 06:11:10.000000 Alphakit-1.2.4/alphakit/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   780357 2023-07-14 06:14:41.000000 Alphakit-1.2.4/alphakit/data/calculator.c
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-07-14 06:11:10.000000 Alphakit-1.2.4/alphakit/data/calculator.pyx
+-rw-r--r--   0 root         (0) root         (0)   167556 2023-07-14 06:14:41.000000 Alphakit-1.2.4/alphakit/data/processing.c
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-14 06:11:10.000000 Alphakit-1.2.4/alphakit/data/processing.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:29:58.000000 Alphakit-1.2.4/alphakit/factor/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-14 06:11:10.000000 Alphakit-1.2.4/alphakit/factor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   292909 2023-07-19 02:27:44.000000 Alphakit-1.2.4/alphakit/factor/analysis.c
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-07-19 02:27:21.000000 Alphakit-1.2.4/alphakit/factor/analysis.pyx
+-rw-r--r--   0 root         (0) root         (0)   371085 2023-07-19 02:27:44.000000 Alphakit-1.2.4/alphakit/factor/metrics.c
+-rw-r--r--   0 root         (0) root         (0)     4313 2023-07-19 02:22:36.000000 Alphakit-1.2.4/alphakit/factor/metrics.pyx
+-rw-r--r--   0 root         (0) root         (0)   309922 2023-07-19 02:27:44.000000 Alphakit-1.2.4/alphakit/factor/processing.c
+-rw-r--r--   0 root         (0) root         (0)     5120 2023-07-19 02:22:36.000000 Alphakit-1.2.4/alphakit/factor/processing.pyx
+-rw-r--r--   0 root         (0) root         (0)   205213 2023-07-19 02:27:44.000000 Alphakit-1.2.4/alphakit/factor/transform.c
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-07-19 02:22:36.000000 Alphakit-1.2.4/alphakit/factor/transform.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:29:58.000000 Alphakit-1.2.4/alphakit/portfolio/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-14 06:11:10.000000 Alphakit-1.2.4/alphakit/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   152583 2023-07-14 06:14:41.000000 Alphakit-1.2.4/alphakit/portfolio/combine.c
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-14 06:11:10.000000 Alphakit-1.2.4/alphakit/portfolio/combine.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:29:58.000000 Alphakit-1.2.4/requirements/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-14 06:11:10.000000 Alphakit-1.2.4/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 02:29:58.000000 Alphakit-1.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-07-19 02:22:31.000000 Alphakit-1.2.4/setup.py
```

### Comparing `Alphakit-1.2.3/Alphakit.egg-info/SOURCES.txt` & `Alphakit-1.2.4/Alphakit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/LICENSE` & `Alphakit-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/alphakit/const.c` & `Alphakit-1.2.4/alphakit/const.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/alphakit/const.pyx` & `Alphakit-1.2.4/alphakit/const.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/alphakit/data/calculator.c` & `Alphakit-1.2.4/alphakit/data/calculator.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/alphakit/data/calculator.pyx` & `Alphakit-1.2.4/alphakit/data/calculator.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/alphakit/data/processing.c` & `Alphakit-1.2.4/alphakit/data/processing.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/alphakit/data/processing.pyx` & `Alphakit-1.2.4/alphakit/data/processing.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/alphakit/factor/analysis.c` & `Alphakit-1.2.4/alphakit/factor/analysis.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/alphakit/factor/analysis.pyx` & `Alphakit-1.2.4/alphakit/factor/analysis.pyx`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -90,8 +90,8 @@
                           outpnl,
                           turnover,
                           ic_series,
                           usecol=['TOP', 'BOT', 'TMB'])
     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip,
                                    checkna)
     factor_plot(dummy, invar, gret, outpnl, savepath)
-    return disp, outpnl, pnlstat, gret_stat
+    return disp, outpnl, pnlstat, gret_stat
```

### Comparing `Alphakit-1.2.3/alphakit/factor/metrics.c` & `Alphakit-1.2.4/alphakit/factor/metrics.c`

 * *Files 0% similar despite different names*

```diff
@@ -1445,15 +1445,14 @@
 static const char __pyx_k_Series[] = "Series";
 static const char __pyx_k_astype[] = "astype";
 static const char __pyx_k_calmar[] = "calmar";
 static const char __pyx_k_concat[] = "concat";
 static const char __pyx_k_cumsum[] = "cumsum";
 static const char __pyx_k_er_fnd[] = "er_fnd";
 static const char __pyx_k_factor[] = "factor";
-static const char __pyx_k_gnline[] = "gnline";
 static const char __pyx_k_icmean[] = "icmean";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_median[] = "median";
 static const char __pyx_k_method[] = "method";
 static const char __pyx_k_nanmax[] = "nanmax";
 static const char __pyx_k_nanmin[] = "nanmin";
 static const char __pyx_k_nanstd[] = "nanstd";
@@ -1531,15 +1530,14 @@
 static PyObject *__pyx_n_s_factor_group;
 static PyObject *__pyx_n_s_factor_group_locals_lambda;
 static PyObject *__pyx_n_s_factor_pnl;
 static PyObject *__pyx_n_s_factor_stat;
 static PyObject *__pyx_n_s_file;
 static PyObject *__pyx_n_s_fill_value;
 static PyObject *__pyx_n_s_freq;
-static PyObject *__pyx_n_s_gnline;
 static PyObject *__pyx_n_s_gret;
 static PyObject *__pyx_n_s_gret_stat;
 static PyObject *__pyx_n_s_group;
 static PyObject *__pyx_n_s_group_keys;
 static PyObject *__pyx_n_s_groupby;
 static PyObject *__pyx_n_s_hold;
 static PyObject *__pyx_n_s_ic;
@@ -3766,20 +3764,20 @@
   __pyx_r = __pyx_pf_8alphakit_6factor_7metrics_6factor_group(__pyx_self, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_group, __pyx_v_hold, __pyx_v_skip, __pyx_v_checkna);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "alphakit/factor/metrics.pyx":94
- *     megedata.index.names = ['tradingday', 'ticker']
- *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
- *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))             # <<<<<<<<<<<<<<
- *     if not nanframe.empty:
- *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
+/* "alphakit/factor/metrics.pyx":99
+ *                   ['er_fnd'].mean().unstack() + 1)
+ *     gret.columns = pd.Series(
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))             # <<<<<<<<<<<<<<
+ *     if checkna and not nanframe.empty:
+ *         gret['GN'] = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8alphakit_6factor_7metrics_12factor_group_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
 static PyMethodDef __pyx_mdef_8alphakit_6factor_7metrics_12factor_group_lambda = {"lambda", (PyCFunction)__pyx_pw_8alphakit_6factor_7metrics_12factor_group_lambda, METH_O, 0};
 static PyObject *__pyx_pw_8alphakit_6factor_7metrics_12factor_group_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x) {
   PyObject *__pyx_r = 0;
@@ -3798,20 +3796,20 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_x, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_x, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_n_s_G, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_n_s_G, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
@@ -3837,29 +3835,29 @@
 static PyObject *__pyx_pf_8alphakit_6factor_7metrics_6factor_group(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_group, PyObject *__pyx_v_hold, PyObject *__pyx_v_skip, PyObject *__pyx_v_checkna) {
   PyObject *__pyx_v_ret_f1d_skip = NULL;
   PyObject *__pyx_v_ret_mkt_fnd = NULL;
   PyObject *__pyx_v_er_fnd = NULL;
   PyObject *__pyx_v_megedata = NULL;
   PyObject *__pyx_v_nanframe = NULL;
   PyObject *__pyx_v_gret = NULL;
-  PyObject *__pyx_v_gnline = NULL;
   PyObject *__pyx_v_gret_stat = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
+  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("factor_group", 0);
   __Pyx_INCREF(__pyx_v_invar);
   __Pyx_INCREF(__pyx_v_ret_f1d);
 
@@ -4038,29 +4036,29 @@
   __pyx_v_er_fnd = __pyx_t_5;
   __pyx_t_5 = 0;
 
   /* "alphakit/factor/metrics.pyx":82
  *     er_fnd = ret_f1d_skip.sub(ret_mkt_fnd, axis='rows')
  *     #
  *     megedata = np.exp(             # <<<<<<<<<<<<<<
- *         np.log(er_fnd + 1).rolling(hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
- *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
+ *         np.log(er_fnd + 1).rolling(
+ *             hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_exp); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "alphakit/factor/metrics.pyx":83
  *     #
  *     megedata = np.exp(
- *         np.log(er_fnd + 1).rolling(hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1             # <<<<<<<<<<<<<<
+ *         np.log(er_fnd + 1).rolling(             # <<<<<<<<<<<<<<
+ *             hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
  *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
- *     megedata.columns = ['er_fnd', 'factor', 'dummy']
  */
   __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = __Pyx_PyInt_AddObjC(__pyx_v_er_fnd, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
@@ -4080,51 +4078,75 @@
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_rolling); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "alphakit/factor/metrics.pyx":84
+ *     megedata = np.exp(
+ *         np.log(er_fnd + 1).rolling(
+ *             hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1             # <<<<<<<<<<<<<<
+ *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
+ *     megedata.columns = ['er_fnd', 'factor', 'dummy']
+ */
   __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_hold);
   __Pyx_GIVEREF(__pyx_v_hold);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_hold);
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_min_periods, __pyx_int_1) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_min_periods, __pyx_int_1) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
+
+  /* "alphakit/factor/metrics.pyx":83
+ *     #
+ *     megedata = np.exp(
+ *         np.log(er_fnd + 1).rolling(             # <<<<<<<<<<<<<<
+ *             hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
+ *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
+ */
   __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_sum); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
+
+  /* "alphakit/factor/metrics.pyx":84
+ *     megedata = np.exp(
+ *         np.log(er_fnd + 1).rolling(
+ *             hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1             # <<<<<<<<<<<<<<
+ *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
+ *     megedata.columns = ['er_fnd', 'factor', 'dummy']
+ */
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_sum); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_shift); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_shift); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_hold, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_hold, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_10 = PyNumber_Negative(__pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_10 = PyNumber_Negative(__pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -4132,36 +4154,36 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_6, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_10);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_v_hold); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_v_hold); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -4172,361 +4194,452 @@
   }
   __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_1, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_megedata = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "alphakit/factor/metrics.pyx":84
- *     megedata = np.exp(
- *         np.log(er_fnd + 1).rolling(hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
+  /* "alphakit/factor/metrics.pyx":85
+ *         np.log(er_fnd + 1).rolling(
+ *             hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
  *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)             # <<<<<<<<<<<<<<
  *     megedata.columns = ['er_fnd', 'factor', 'dummy']
  *     megedata = megedata.loc[megedata.dummy == 1]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_concat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_concat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dummy, __pyx_n_s_stack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dummy, __pyx_n_s_stack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_8 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_megedata);
   __Pyx_GIVEREF(__pyx_v_megedata);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_megedata);
   __Pyx_GIVEREF(__pyx_t_4);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_8);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_t_8);
   __pyx_t_4 = 0;
   __pyx_t_8 = 0;
-  __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_megedata, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "alphakit/factor/metrics.pyx":85
- *         np.log(er_fnd + 1).rolling(hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
+  /* "alphakit/factor/metrics.pyx":86
+ *             hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
  *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
  *     megedata.columns = ['er_fnd', 'factor', 'dummy']             # <<<<<<<<<<<<<<
  *     megedata = megedata.loc[megedata.dummy == 1]
- *     nanframe = megedata.loc[megedata.factor.isna()]
+ *     nanframe = megedata.loc[(megedata.factor.isna())
  */
-  __pyx_t_4 = PyList_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_er_fnd);
   __Pyx_GIVEREF(__pyx_n_s_er_fnd);
   PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_er_fnd);
   __Pyx_INCREF(__pyx_n_s_factor);
   __Pyx_GIVEREF(__pyx_n_s_factor);
   PyList_SET_ITEM(__pyx_t_4, 1, __pyx_n_s_factor);
   __Pyx_INCREF(__pyx_n_s_dummy);
   __Pyx_GIVEREF(__pyx_n_s_dummy);
   PyList_SET_ITEM(__pyx_t_4, 2, __pyx_n_s_dummy);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_megedata, __pyx_n_s_columns, __pyx_t_4) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_megedata, __pyx_n_s_columns, __pyx_t_4) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "alphakit/factor/metrics.pyx":86
+  /* "alphakit/factor/metrics.pyx":87
  *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
  *     megedata.columns = ['er_fnd', 'factor', 'dummy']
  *     megedata = megedata.loc[megedata.dummy == 1]             # <<<<<<<<<<<<<<
- *     nanframe = megedata.loc[megedata.factor.isna()]
- *     megedata = megedata.loc[~megedata.factor.isna()]
+ *     nanframe = megedata.loc[(megedata.factor.isna())
+ *                             & (~megedata.er_fnd.isna())]
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_dummy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_dummy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF_SET(__pyx_v_megedata, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/metrics.pyx":87
+  /* "alphakit/factor/metrics.pyx":88
  *     megedata.columns = ['er_fnd', 'factor', 'dummy']
  *     megedata = megedata.loc[megedata.dummy == 1]
- *     nanframe = megedata.loc[megedata.factor.isna()]             # <<<<<<<<<<<<<<
+ *     nanframe = megedata.loc[(megedata.factor.isna())             # <<<<<<<<<<<<<<
+ *                             & (~megedata.er_fnd.isna())]
  *     megedata = megedata.loc[~megedata.factor.isna()]
- *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_isna); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_isna); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
+
+  /* "alphakit/factor/metrics.pyx":89
+ *     megedata = megedata.loc[megedata.dummy == 1]
+ *     nanframe = megedata.loc[(megedata.factor.isna())
+ *                             & (~megedata.er_fnd.isna())]             # <<<<<<<<<<<<<<
+ *     megedata = megedata.loc[~megedata.factor.isna()]
+ *     megedata["quantile"] = megedata["factor"].groupby(
+ */
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_isna); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyNumber_Invert(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyNumber_And(__pyx_t_8, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_v_nanframe = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "alphakit/factor/metrics.pyx":88
+ *     megedata.columns = ['er_fnd', 'factor', 'dummy']
  *     megedata = megedata.loc[megedata.dummy == 1]
- *     nanframe = megedata.loc[megedata.factor.isna()]
+ *     nanframe = megedata.loc[(megedata.factor.isna())             # <<<<<<<<<<<<<<
+ *                             & (~megedata.er_fnd.isna())]
+ *     megedata = megedata.loc[~megedata.factor.isna()]
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_v_nanframe = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "alphakit/factor/metrics.pyx":90
+ *     nanframe = megedata.loc[(megedata.factor.isna())
+ *                             & (~megedata.er_fnd.isna())]
  *     megedata = megedata.loc[~megedata.factor.isna()]             # <<<<<<<<<<<<<<
- *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
- *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
+ *     megedata["quantile"] = megedata["factor"].groupby(
+ *         level=0, group_keys=False).rank(pct=True)
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_isna); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_isna); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_1)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
-  __pyx_t_8 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
+  __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = PyNumber_Invert(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Invert(__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_DECREF_SET(__pyx_v_megedata, __pyx_t_5);
+  __pyx_t_5 = 0;
+
+  /* "alphakit/factor/metrics.pyx":91
+ *                             & (~megedata.er_fnd.isna())]
+ *     megedata = megedata.loc[~megedata.factor.isna()]
+ *     megedata["quantile"] = megedata["factor"].groupby(             # <<<<<<<<<<<<<<
+ *         level=0, group_keys=False).rank(pct=True)
+ *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
+ */
+  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_groupby); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF_SET(__pyx_v_megedata, __pyx_t_8);
-  __pyx_t_8 = 0;
 
-  /* "alphakit/factor/metrics.pyx":89
- *     nanframe = megedata.loc[megedata.factor.isna()]
+  /* "alphakit/factor/metrics.pyx":92
  *     megedata = megedata.loc[~megedata.factor.isna()]
- *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)             # <<<<<<<<<<<<<<
+ *     megedata["quantile"] = megedata["factor"].groupby(
+ *         level=0, group_keys=False).rank(pct=True)             # <<<<<<<<<<<<<<
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
  */
-  __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_groupby); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_group_keys, Py_False) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_group_keys, Py_False) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+
+  /* "alphakit/factor/metrics.pyx":91
+ *                             & (~megedata.er_fnd.isna())]
+ *     megedata = megedata.loc[~megedata.factor.isna()]
+ *     megedata["quantile"] = megedata["factor"].groupby(             # <<<<<<<<<<<<<<
+ *         level=0, group_keys=False).rank(pct=True)
+ *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
+ */
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_rank); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+
+  /* "alphakit/factor/metrics.pyx":92
+ *     megedata = megedata.loc[~megedata.factor.isna()]
+ *     megedata["quantile"] = megedata["factor"].groupby(
+ *         level=0, group_keys=False).rank(pct=True)             # <<<<<<<<<<<<<<
+ *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
+ *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
+ */
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_rank); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_pct, Py_True) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_pct, Py_True) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_megedata, __pyx_n_s_quantile, __pyx_t_4) < 0)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "alphakit/factor/metrics.pyx":90
+  /* "alphakit/factor/metrics.pyx":91
+ *                             & (~megedata.er_fnd.isna())]
  *     megedata = megedata.loc[~megedata.factor.isna()]
- *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
+ *     megedata["quantile"] = megedata["factor"].groupby(             # <<<<<<<<<<<<<<
+ *         level=0, group_keys=False).rank(pct=True)
+ *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
+ */
+  if (unlikely(PyObject_SetItem(__pyx_v_megedata, __pyx_n_s_quantile, __pyx_t_8) < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+
+  /* "alphakit/factor/metrics.pyx":93
+ *     megedata["quantile"] = megedata["factor"].groupby(
+ *         level=0, group_keys=False).rank(pct=True)
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1             # <<<<<<<<<<<<<<
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
  *     megedata.index.names = ['tradingday', 'ticker']
  */
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_quantile); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_quantile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = PyNumber_Multiply(__pyx_t_3, __pyx_v_group); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_8 = PyNumber_Multiply(__pyx_t_5, __pyx_v_group); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_astype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_8);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_8, __pyx_n_s_int) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_int);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_megedata, __pyx_n_s_quantile, __pyx_t_5) < 0)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_8 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_n_s_int) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_int);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_8, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(PyObject_SetItem(__pyx_v_megedata, __pyx_n_s_quantile, __pyx_t_3) < 0)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "alphakit/factor/metrics.pyx":91
- *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
+  /* "alphakit/factor/metrics.pyx":94
+ *         level=0, group_keys=False).rank(pct=True)
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group             # <<<<<<<<<<<<<<
  *     megedata.index.names = ['tradingday', 'ticker']
- *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
+ *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_quantile); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_PyInt_AddObjC(__pyx_v_group, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_quantile); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_t_4, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_v_group, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_8, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_quantile);
   __Pyx_GIVEREF(__pyx_n_s_quantile);
-  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_n_s_quantile);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_quantile);
   __pyx_t_1 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_t_5, __pyx_t_8, __pyx_v_group) < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_t_5, __pyx_v_group) < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "alphakit/factor/metrics.pyx":92
+  /* "alphakit/factor/metrics.pyx":95
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
  *     megedata.index.names = ['tradingday', 'ticker']             # <<<<<<<<<<<<<<
- *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
- *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+ *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])
+ *                   ['er_fnd'].mean().unstack() + 1)
  */
-  __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_tradingday);
   __Pyx_GIVEREF(__pyx_n_s_tradingday);
-  PyList_SET_ITEM(__pyx_t_8, 0, __pyx_n_s_tradingday);
+  PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_tradingday);
   __Pyx_INCREF(__pyx_n_s_ticker);
   __Pyx_GIVEREF(__pyx_n_s_ticker);
-  PyList_SET_ITEM(__pyx_t_8, 1, __pyx_n_s_ticker);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_names, __pyx_t_8) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_ticker);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_3, __pyx_n_s_names, __pyx_t_5) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "alphakit/factor/metrics.pyx":93
+  /* "alphakit/factor/metrics.pyx":96
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
  *     megedata.index.names = ['tradingday', 'ticker']
- *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)             # <<<<<<<<<<<<<<
- *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
- *     if not nanframe.empty:
+ *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])             # <<<<<<<<<<<<<<
+ *                   ['er_fnd'].mean().unstack() + 1)
+ *     gret.columns = pd.Series(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "alphakit/factor/metrics.pyx":97
+ *     megedata.index.names = ['tradingday', 'ticker']
+ *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])
+ *                   ['er_fnd'].mean().unstack() + 1)             # <<<<<<<<<<<<<<
+ *     gret.columns = pd.Series(
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+ */
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_10 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_groupby); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
+
+  /* "alphakit/factor/metrics.pyx":96
+ *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
+ *     megedata.index.names = ['tradingday', 'ticker']
+ *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])             # <<<<<<<<<<<<<<
+ *                   ['er_fnd'].mean().unstack() + 1)
+ *     gret.columns = pd.Series(
+ */
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_groupby); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = PyList_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_10 = PyList_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_INCREF(__pyx_n_s_tradingday);
   __Pyx_GIVEREF(__pyx_n_s_tradingday);
   PyList_SET_ITEM(__pyx_t_10, 0, __pyx_n_s_tradingday);
   __Pyx_INCREF(__pyx_n_s_quantile);
   __Pyx_GIVEREF(__pyx_n_s_quantile);
   PyList_SET_ITEM(__pyx_t_10, 1, __pyx_n_s_quantile);
@@ -4536,294 +4649,279 @@
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_10);
+  __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_10);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
+
+  /* "alphakit/factor/metrics.pyx":97
+ *     megedata.index.names = ['tradingday', 'ticker']
+ *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])
+ *                   ['er_fnd'].mean().unstack() + 1)             # <<<<<<<<<<<<<<
+ *     gret.columns = pd.Series(
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+ */
+  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_mean); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __pyx_t_8 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_unstack); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_8, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_unstack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
+  __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
+    }
+  }
+  __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_gret = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __pyx_v_gret = __pyx_t_3;
+  __pyx_t_3 = 0;
 
-  /* "alphakit/factor/metrics.pyx":94
- *     megedata.index.names = ['tradingday', 'ticker']
- *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
- *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))             # <<<<<<<<<<<<<<
- *     if not nanframe.empty:
- *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
+  /* "alphakit/factor/metrics.pyx":98
+ *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])
+ *                   ['er_fnd'].mean().unstack() + 1)
+ *     gret.columns = pd.Series(             # <<<<<<<<<<<<<<
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+ *     if checkna and not nanframe.empty:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Series); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Series); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8alphakit_6factor_7metrics_12factor_group_lambda, 0, __pyx_n_s_factor_group_locals_lambda, NULL, __pyx_n_s_alphakit_factor_metrics, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+
+  /* "alphakit/factor/metrics.pyx":99
+ *                   ['er_fnd'].mean().unstack() + 1)
+ *     gret.columns = pd.Series(
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))             # <<<<<<<<<<<<<<
+ *     if checkna and not nanframe.empty:
+ *         gret['GN'] = nanframe.groupby(axis=0, level=0).er_fnd.mean()
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8alphakit_6factor_7metrics_12factor_group_lambda, 0, __pyx_n_s_factor_group_locals_lambda, NULL, __pyx_n_s_alphakit_factor_metrics, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_shape); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_8, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_5, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
-  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_int_0);
-  __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
-  __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_int_0);
+  __Pyx_GIVEREF(__pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_8);
+  __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_8);
   __pyx_t_1 = 0;
-  __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_8);
+  __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+
+  /* "alphakit/factor/metrics.pyx":98
+ *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])
+ *                   ['er_fnd'].mean().unstack() + 1)
+ *     gret.columns = pd.Series(             # <<<<<<<<<<<<<<
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+ *     if checkna and not nanframe.empty:
+ */
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_gret, __pyx_n_s_columns, __pyx_t_3) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_gret, __pyx_n_s_columns, __pyx_t_5) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "alphakit/factor/metrics.pyx":95
- *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
- *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
- *     if not nanframe.empty:             # <<<<<<<<<<<<<<
- *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
- *     else:
+  /* "alphakit/factor/metrics.pyx":100
+ *     gret.columns = pd.Series(
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+ *     if checkna and not nanframe.empty:             # <<<<<<<<<<<<<<
+ *         gret['GN'] = nanframe.groupby(axis=0, level=0).er_fnd.mean()
+ *     gret_stat = gret.mean()
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_nanframe, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_11 = ((!__pyx_t_2) != 0);
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_checkna); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 100, __pyx_L1_error)
   if (__pyx_t_11) {
+  } else {
+    __pyx_t_2 = __pyx_t_11;
+    goto __pyx_L5_bool_binop_done;
+  }
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_nanframe, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_12 = ((!__pyx_t_11) != 0);
+  __pyx_t_2 = __pyx_t_12;
+  __pyx_L5_bool_binop_done:;
+  if (__pyx_t_2) {
 
-    /* "alphakit/factor/metrics.pyx":96
- *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
- *     if not nanframe.empty:
- *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()             # <<<<<<<<<<<<<<
- *     else:
- *         gnline = np.nan
+    /* "alphakit/factor/metrics.pyx":101
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+ *     if checkna and not nanframe.empty:
+ *         gret['GN'] = nanframe.groupby(axis=0, level=0).er_fnd.mean()             # <<<<<<<<<<<<<<
+ *     gret_stat = gret.mean()
+ *     return gret, gret_stat
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_nanframe, __pyx_n_s_groupby); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_nanframe, __pyx_n_s_groupby); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_mean); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_mean); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
-    __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_v_gnline = __pyx_t_5;
-    __pyx_t_5 = 0;
-
-    /* "alphakit/factor/metrics.pyx":95
- *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
- *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
- *     if not nanframe.empty:             # <<<<<<<<<<<<<<
- *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
- *     else:
- */
-    goto __pyx_L4;
-  }
-
-  /* "alphakit/factor/metrics.pyx":98
- *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
- *     else:
- *         gnline = np.nan             # <<<<<<<<<<<<<<
- *     if checkna:
- *         gret['GN'] = gnline
- */
-  /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nan); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 98, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_v_gnline = __pyx_t_8;
-    __pyx_t_8 = 0;
-  }
-  __pyx_L4:;
-
-  /* "alphakit/factor/metrics.pyx":99
- *     else:
- *         gnline = np.nan
- *     if checkna:             # <<<<<<<<<<<<<<
- *         gret['GN'] = gnline
- *     gret_stat = gret.mean()
- */
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_checkna); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
-  if (__pyx_t_11) {
+    if (unlikely(PyObject_SetItem(__pyx_v_gret, __pyx_n_s_GN, __pyx_t_3) < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "alphakit/factor/metrics.pyx":100
- *         gnline = np.nan
- *     if checkna:
- *         gret['GN'] = gnline             # <<<<<<<<<<<<<<
- *     gret_stat = gret.mean()
- *     return gret, gret_stat
- */
-    if (unlikely(PyObject_SetItem(__pyx_v_gret, __pyx_n_s_GN, __pyx_v_gnline) < 0)) __PYX_ERR(0, 100, __pyx_L1_error)
-
-    /* "alphakit/factor/metrics.pyx":99
- *     else:
- *         gnline = np.nan
- *     if checkna:             # <<<<<<<<<<<<<<
- *         gret['GN'] = gnline
+ *     gret.columns = pd.Series(
+ *         map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+ *     if checkna and not nanframe.empty:             # <<<<<<<<<<<<<<
+ *         gret['GN'] = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  *     gret_stat = gret.mean()
  */
   }
 
-  /* "alphakit/factor/metrics.pyx":101
- *     if checkna:
- *         gret['GN'] = gnline
+  /* "alphakit/factor/metrics.pyx":102
+ *     if checkna and not nanframe.empty:
+ *         gret['GN'] = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  *     gret_stat = gret.mean()             # <<<<<<<<<<<<<<
  *     return gret, gret_stat
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_mean); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_mean); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = NULL;
+  __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_4)) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_gret_stat = __pyx_t_8;
-  __pyx_t_8 = 0;
+  __pyx_v_gret_stat = __pyx_t_3;
+  __pyx_t_3 = 0;
 
-  /* "alphakit/factor/metrics.pyx":102
- *         gret['GN'] = gnline
+  /* "alphakit/factor/metrics.pyx":103
+ *         gret['GN'] = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  *     gret_stat = gret.mean()
  *     return gret, gret_stat             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 102, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_gret);
   __Pyx_GIVEREF(__pyx_v_gret);
-  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_gret);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_gret);
   __Pyx_INCREF(__pyx_v_gret_stat);
   __Pyx_GIVEREF(__pyx_v_gret_stat);
-  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_gret_stat);
-  __pyx_r = __pyx_t_8;
-  __pyx_t_8 = 0;
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_gret_stat);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "alphakit/factor/metrics.pyx":71
  * 
  * 
  * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):             # <<<<<<<<<<<<<<
  *     if skip < 0:
@@ -4846,15 +4944,14 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ret_f1d_skip);
   __Pyx_XDECREF(__pyx_v_ret_mkt_fnd);
   __Pyx_XDECREF(__pyx_v_er_fnd);
   __Pyx_XDECREF(__pyx_v_megedata);
   __Pyx_XDECREF(__pyx_v_nanframe);
   __Pyx_XDECREF(__pyx_v_gret);
-  __Pyx_XDECREF(__pyx_v_gnline);
   __Pyx_XDECREF(__pyx_v_gret_stat);
   __Pyx_XDECREF(__pyx_v_invar);
   __Pyx_XDECREF(__pyx_v_ret_f1d);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -4934,15 +5031,14 @@
   {&__pyx_n_s_factor_group, __pyx_k_factor_group, sizeof(__pyx_k_factor_group), 0, 0, 1, 1},
   {&__pyx_n_s_factor_group_locals_lambda, __pyx_k_factor_group_locals_lambda, sizeof(__pyx_k_factor_group_locals_lambda), 0, 0, 1, 1},
   {&__pyx_n_s_factor_pnl, __pyx_k_factor_pnl, sizeof(__pyx_k_factor_pnl), 0, 0, 1, 1},
   {&__pyx_n_s_factor_stat, __pyx_k_factor_stat, sizeof(__pyx_k_factor_stat), 0, 0, 1, 1},
   {&__pyx_n_s_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 0, 1, 1},
   {&__pyx_n_s_fill_value, __pyx_k_fill_value, sizeof(__pyx_k_fill_value), 0, 0, 1, 1},
   {&__pyx_n_s_freq, __pyx_k_freq, sizeof(__pyx_k_freq), 0, 0, 1, 1},
-  {&__pyx_n_s_gnline, __pyx_k_gnline, sizeof(__pyx_k_gnline), 0, 0, 1, 1},
   {&__pyx_n_s_gret, __pyx_k_gret, sizeof(__pyx_k_gret), 0, 0, 1, 1},
   {&__pyx_n_s_gret_stat, __pyx_k_gret_stat, sizeof(__pyx_k_gret_stat), 0, 0, 1, 1},
   {&__pyx_n_s_group, __pyx_k_group, sizeof(__pyx_k_group), 0, 0, 1, 1},
   {&__pyx_n_s_group_keys, __pyx_k_group_keys, sizeof(__pyx_k_group_keys), 0, 0, 1, 1},
   {&__pyx_n_s_groupby, __pyx_k_groupby, sizeof(__pyx_k_groupby), 0, 0, 1, 1},
   {&__pyx_n_s_hold, __pyx_k_hold, sizeof(__pyx_k_hold), 0, 0, 1, 1},
   {&__pyx_n_s_ic, __pyx_k_ic, sizeof(__pyx_k_ic), 0, 0, 1, 1},
@@ -5025,16 +5121,16 @@
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {&__pyx_n_s_weight, __pyx_k_weight, sizeof(__pyx_k_weight), 0, 0, 1, 1},
   {&__pyx_n_s_win, __pyx_k_win, sizeof(__pyx_k_win), 0, 0, 1, 1},
   {&__pyx_n_s_zeror, __pyx_k_zeror, sizeof(__pyx_k_zeror), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 99, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -5079,18 +5175,18 @@
   /* "alphakit/factor/metrics.pyx":71
  * 
  * 
  * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):             # <<<<<<<<<<<<<<
  *     if skip < 0:
  *         print('skip must >=0')
  */
-  __pyx_tuple__7 = PyTuple_Pack(15, __pyx_n_s_dummy, __pyx_n_s_invar, __pyx_n_s_ret_f1d, __pyx_n_s_group, __pyx_n_s_hold, __pyx_n_s_skip, __pyx_n_s_checkna, __pyx_n_s_ret_f1d_skip, __pyx_n_s_ret_mkt_fnd, __pyx_n_s_er_fnd, __pyx_n_s_megedata, __pyx_n_s_nanframe, __pyx_n_s_gret, __pyx_n_s_gnline, __pyx_n_s_gret_stat); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(14, __pyx_n_s_dummy, __pyx_n_s_invar, __pyx_n_s_ret_f1d, __pyx_n_s_group, __pyx_n_s_hold, __pyx_n_s_skip, __pyx_n_s_checkna, __pyx_n_s_ret_f1d_skip, __pyx_n_s_ret_mkt_fnd, __pyx_n_s_er_fnd, __pyx_n_s_megedata, __pyx_n_s_nanframe, __pyx_n_s_gret, __pyx_n_s_gret_stat); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(7, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_metrics_pyx, __pyx_n_s_factor_group, 71, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(7, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_metrics_pyx, __pyx_n_s_factor_group, 71, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
```

### Comparing `Alphakit-1.2.3/alphakit/factor/metrics.pyx` & `Alphakit-1.2.4/alphakit/factor/metrics.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -76,27 +76,28 @@
     ret_f1d = ret_f1d * dummy
     ret_f1d_skip = ret_f1d.shift(-skip)
     ret_f1d_skip = np.exp(ret_f1d_skip) - 1
     ret_mkt_fnd = (ret_f1d_skip * dummy).mean(axis=1)
     er_fnd = ret_f1d_skip.sub(ret_mkt_fnd, axis='rows')
     # 分层画图
     megedata = np.exp(
-        np.log(er_fnd + 1).rolling(hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
+        np.log(er_fnd + 1).rolling(
+            hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
     megedata.columns = ['er_fnd', 'factor', 'dummy']
     megedata = megedata.loc[megedata.dummy == 1]
-    nanframe = megedata.loc[megedata.factor.isna()]
+    nanframe = megedata.loc[(megedata.factor.isna())
+                            & (~megedata.er_fnd.isna())]
     megedata = megedata.loc[~megedata.factor.isna()]
-    megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
+    megedata["quantile"] = megedata["factor"].groupby(
+        level=0, group_keys=False).rank(pct=True)
     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
     megedata.index.names = ['tradingday', 'ticker']
-    gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
-    gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
-    if not nanframe.empty:
-        gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
-    else:
-        gnline = np.nan
-    if checkna:
-        gret['GN'] = gnline
+    gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])
+                  ['er_fnd'].mean().unstack() + 1)
+    gret.columns = pd.Series(
+        map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
+    if checkna and not nanframe.empty:
+        gret['GN'] = nanframe.groupby(axis=0, level=0).er_fnd.mean()
     gret_stat = gret.mean()
     return gret, gret_stat
```

### Comparing `Alphakit-1.2.3/alphakit/factor/processing.c` & `Alphakit-1.2.4/alphakit/factor/processing.c`

 * *Files 1% similar despite different names*

```diff
@@ -3047,16 +3047,16 @@
   return __pyx_r;
 }
 
 /* "alphakit/factor/processing.pyx":69
  * 
  * #
  * def indLineNeu(invar, ind):             # <<<<<<<<<<<<<<
- *     tradingday = invar.index
- *     ticker = invar.columns
+ *     invar.index.name = 'tradingday'
+ *     invar.columns.name = 'ticker'
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8alphakit_6factor_10processing_7indLineNeu(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_8alphakit_6factor_10processing_6indLineNeu[] = "indLineNeu(invar, ind)";
 static PyMethodDef __pyx_mdef_8alphakit_6factor_10processing_7indLineNeu = {"indLineNeu", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8alphakit_6factor_10processing_7indLineNeu, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8alphakit_6factor_10processing_6indLineNeu};
 static PyObject *__pyx_pw_8alphakit_6factor_10processing_7indLineNeu(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -3140,133 +3140,181 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("indLineNeu", 0);
 
   /* "alphakit/factor/processing.pyx":70
  * #
  * def indLineNeu(invar, ind):
+ *     invar.index.name = 'tradingday'             # <<<<<<<<<<<<<<
+ *     invar.columns.name = 'ticker'
+ *     ind.index.name = 'tradingday'
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_name, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "alphakit/factor/processing.pyx":71
+ * def indLineNeu(invar, ind):
+ *     invar.index.name = 'tradingday'
+ *     invar.columns.name = 'ticker'             # <<<<<<<<<<<<<<
+ *     ind.index.name = 'tradingday'
+ *     ind.columns.name = 'ticker'
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_name, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "alphakit/factor/processing.pyx":72
+ *     invar.index.name = 'tradingday'
+ *     invar.columns.name = 'ticker'
+ *     ind.index.name = 'tradingday'             # <<<<<<<<<<<<<<
+ *     ind.columns.name = 'ticker'
+ *     tradingday = invar.index
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_ind, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_name, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "alphakit/factor/processing.pyx":73
+ *     invar.columns.name = 'ticker'
+ *     ind.index.name = 'tradingday'
+ *     ind.columns.name = 'ticker'             # <<<<<<<<<<<<<<
+ *     tradingday = invar.index
+ *     ticker = invar.columns
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_ind, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_name, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "alphakit/factor/processing.pyx":74
+ *     ind.index.name = 'tradingday'
+ *     ind.columns.name = 'ticker'
  *     tradingday = invar.index             # <<<<<<<<<<<<<<
  *     ticker = invar.columns
  *     data = pd.concat([invar.unstack(), ind.unstack()], axis=1)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_tradingday = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":71
- * def indLineNeu(invar, ind):
+  /* "alphakit/factor/processing.pyx":75
+ *     ind.columns.name = 'ticker'
  *     tradingday = invar.index
  *     ticker = invar.columns             # <<<<<<<<<<<<<<
  *     data = pd.concat([invar.unstack(), ind.unstack()], axis=1)
  *     data.columns = ['factor', 'ind']
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ticker = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":72
+  /* "alphakit/factor/processing.pyx":76
  *     tradingday = invar.index
  *     ticker = invar.columns
  *     data = pd.concat([invar.unstack(), ind.unstack()], axis=1)             # <<<<<<<<<<<<<<
  *     data.columns = ['factor', 'ind']
  *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_concat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_concat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_unstack); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_unstack); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ind, __pyx_n_s_unstack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ind, __pyx_n_s_unstack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":73
+  /* "alphakit/factor/processing.pyx":77
  *     ticker = invar.columns
  *     data = pd.concat([invar.unstack(), ind.unstack()], axis=1)
  *     data.columns = ['factor', 'ind']             # <<<<<<<<<<<<<<
  *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
- *     indmean = data.reset_index().drop('factor', axis=1).merge(ind_mean, on=['tradingday', 'ind'], how='left').drop(
+ *     indmean = data.reset_index().drop('factor',
  */
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_factor);
   __Pyx_GIVEREF(__pyx_n_s_factor);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_factor);
   __Pyx_INCREF(__pyx_n_s_ind);
   __Pyx_GIVEREF(__pyx_n_s_ind);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_ind);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_columns, __pyx_t_1) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_columns, __pyx_t_1) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":74
+  /* "alphakit/factor/processing.pyx":78
  *     data = pd.concat([invar.unstack(), ind.unstack()], axis=1)
  *     data.columns = ['factor', 'ind']
  *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()             # <<<<<<<<<<<<<<
- *     indmean = data.reset_index().drop('factor', axis=1).merge(ind_mean, on=['tradingday', 'ind'], how='left').drop(
- *         'ind', axis=1)
+ *     indmean = data.reset_index().drop('factor',
+ *                                       axis=1).merge(ind_mean,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_groupby); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_groupby); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_tradingday);
   __Pyx_GIVEREF(__pyx_n_s_tradingday);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_tradingday);
   __Pyx_INCREF(__pyx_n_s_ind);
   __Pyx_GIVEREF(__pyx_n_s_ind);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_ind);
@@ -3279,206 +3327,254 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mean); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mean); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ind_mean = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":75
+  /* "alphakit/factor/processing.pyx":79
  *     data.columns = ['factor', 'ind']
  *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
- *     indmean = data.reset_index().drop('factor', axis=1).merge(ind_mean, on=['tradingday', 'ind'], how='left').drop(             # <<<<<<<<<<<<<<
- *         'ind', axis=1)
- *     dmean = indmean.pivot_table(index='tradingday', columns='ticker', values='factor')
+ *     indmean = data.reset_index().drop('factor',             # <<<<<<<<<<<<<<
+ *                                       axis=1).merge(ind_mean,
+ *                                                     on=['tradingday', 'ind'],
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_drop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_drop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+
+  /* "alphakit/factor/processing.pyx":80
+ *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
+ *     indmean = data.reset_index().drop('factor',
+ *                                       axis=1).merge(ind_mean,             # <<<<<<<<<<<<<<
+ *                                                     on=['tradingday', 'ind'],
+ *                                                     how='left').drop('ind',
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple_, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
+
+  /* "alphakit/factor/processing.pyx":79
+ *     data.columns = ['factor', 'ind']
+ *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
+ *     indmean = data.reset_index().drop('factor',             # <<<<<<<<<<<<<<
+ *                                       axis=1).merge(ind_mean,
+ *                                                     on=['tradingday', 'ind'],
+ */
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple_, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_merge); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+
+  /* "alphakit/factor/processing.pyx":80
+ *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
+ *     indmean = data.reset_index().drop('factor',
+ *                                       axis=1).merge(ind_mean,             # <<<<<<<<<<<<<<
+ *                                                     on=['tradingday', 'ind'],
+ *                                                     how='left').drop('ind',
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_merge); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_ind_mean);
   __Pyx_GIVEREF(__pyx_v_ind_mean);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_ind_mean);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+
+  /* "alphakit/factor/processing.pyx":81
+ *     indmean = data.reset_index().drop('factor',
+ *                                       axis=1).merge(ind_mean,
+ *                                                     on=['tradingday', 'ind'],             # <<<<<<<<<<<<<<
+ *                                                     how='left').drop('ind',
+ *                                                                      axis=1)
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_tradingday);
   __Pyx_GIVEREF(__pyx_n_s_tradingday);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_tradingday);
   __Pyx_INCREF(__pyx_n_s_ind);
   __Pyx_GIVEREF(__pyx_n_s_ind);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_ind);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_on, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_on, __pyx_t_3) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_how, __pyx_n_s_left) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_how, __pyx_n_s_left) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+
+  /* "alphakit/factor/processing.pyx":80
+ *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
+ *     indmean = data.reset_index().drop('factor',
+ *                                       axis=1).merge(ind_mean,             # <<<<<<<<<<<<<<
+ *                                                     on=['tradingday', 'ind'],
+ *                                                     how='left').drop('ind',
+ */
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_drop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+
+  /* "alphakit/factor/processing.pyx":82
+ *                                       axis=1).merge(ind_mean,
+ *                                                     on=['tradingday', 'ind'],
+ *                                                     how='left').drop('ind',             # <<<<<<<<<<<<<<
+ *                                                                      axis=1)
+ *     dmean = indmean.pivot_table(index='tradingday',
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_drop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "alphakit/factor/processing.pyx":76
- *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
- *     indmean = data.reset_index().drop('factor', axis=1).merge(ind_mean, on=['tradingday', 'ind'], how='left').drop(
- *         'ind', axis=1)             # <<<<<<<<<<<<<<
- *     dmean = indmean.pivot_table(index='tradingday', columns='ticker', values='factor')
- *     dmean = dmean.reindex(index=tradingday, columns=ticker)
+  /* "alphakit/factor/processing.pyx":83
+ *                                                     on=['tradingday', 'ind'],
+ *                                                     how='left').drop('ind',
+ *                                                                      axis=1)             # <<<<<<<<<<<<<<
+ *     dmean = indmean.pivot_table(index='tradingday',
+ *                                 columns='ticker',
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
 
-  /* "alphakit/factor/processing.pyx":75
- *     data.columns = ['factor', 'ind']
- *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
- *     indmean = data.reset_index().drop('factor', axis=1).merge(ind_mean, on=['tradingday', 'ind'], how='left').drop(             # <<<<<<<<<<<<<<
- *         'ind', axis=1)
- *     dmean = indmean.pivot_table(index='tradingday', columns='ticker', values='factor')
+  /* "alphakit/factor/processing.pyx":82
+ *                                       axis=1).merge(ind_mean,
+ *                                                     on=['tradingday', 'ind'],
+ *                                                     how='left').drop('ind',             # <<<<<<<<<<<<<<
+ *                                                                      axis=1)
+ *     dmean = indmean.pivot_table(index='tradingday',
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_indmean = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "alphakit/factor/processing.pyx":77
- *     indmean = data.reset_index().drop('factor', axis=1).merge(ind_mean, on=['tradingday', 'ind'], how='left').drop(
- *         'ind', axis=1)
- *     dmean = indmean.pivot_table(index='tradingday', columns='ticker', values='factor')             # <<<<<<<<<<<<<<
- *     dmean = dmean.reindex(index=tradingday, columns=ticker)
- *     return invar - dmean
+  /* "alphakit/factor/processing.pyx":84
+ *                                                     how='left').drop('ind',
+ *                                                                      axis=1)
+ *     dmean = indmean.pivot_table(index='tradingday',             # <<<<<<<<<<<<<<
+ *                                 columns='ticker',
+ *                                 values='factor')
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_indmean, __pyx_n_s_pivot_table); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_indmean, __pyx_n_s_pivot_table); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_values, __pyx_n_s_factor) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_values, __pyx_n_s_factor) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_dmean = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "alphakit/factor/processing.pyx":78
- *         'ind', axis=1)
- *     dmean = indmean.pivot_table(index='tradingday', columns='ticker', values='factor')
+  /* "alphakit/factor/processing.pyx":87
+ *                                 columns='ticker',
+ *                                 values='factor')
  *     dmean = dmean.reindex(index=tradingday, columns=ticker)             # <<<<<<<<<<<<<<
  *     return invar - dmean
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_dmean, __pyx_n_s_reindex); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_dmean, __pyx_n_s_reindex); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_v_tradingday) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_v_ticker) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_v_tradingday) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_v_ticker) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_dmean, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "alphakit/factor/processing.pyx":79
- *     dmean = indmean.pivot_table(index='tradingday', columns='ticker', values='factor')
+  /* "alphakit/factor/processing.pyx":88
+ *                                 values='factor')
  *     dmean = dmean.reindex(index=tradingday, columns=ticker)
  *     return invar - dmean             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = PyNumber_Subtract(__pyx_v_invar, __pyx_v_dmean); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_v_invar, __pyx_v_dmean); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
   /* "alphakit/factor/processing.pyx":69
  * 
  * #
  * def indLineNeu(invar, ind):             # <<<<<<<<<<<<<<
- *     tradingday = invar.index
- *     ticker = invar.columns
+ *     invar.index.name = 'tradingday'
+ *     invar.columns.name = 'ticker'
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -3495,15 +3591,15 @@
   __Pyx_XDECREF(__pyx_v_indmean);
   __Pyx_XDECREF(__pyx_v_dmean);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "alphakit/factor/processing.pyx":83
+/* "alphakit/factor/processing.pyx":92
  * 
  * # riskfactor: ['tradingday','ticker,'riskfactor1','riskfactor2']
  * def alphaOpNeu(invar, riskfactor):             # <<<<<<<<<<<<<<
  *     tradingday = invar.index
  *     ticker = invar.columns
  */
 
@@ -3539,32 +3635,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_invar)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_riskfactor)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("alphaOpNeu", 1, 2, 2, 1); __PYX_ERR(0, 83, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("alphaOpNeu", 1, 2, 2, 1); __PYX_ERR(0, 92, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "alphaOpNeu") < 0)) __PYX_ERR(0, 83, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "alphaOpNeu") < 0)) __PYX_ERR(0, 92, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_invar = values[0];
     __pyx_v_riskfactor = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("alphaOpNeu", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 83, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("alphaOpNeu", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 92, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("alphakit.factor.processing.alphaOpNeu", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8alphakit_6factor_10processing_8alphaOpNeu(__pyx_self, __pyx_v_invar, __pyx_v_riskfactor);
 
@@ -3592,517 +3688,517 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("alphaOpNeu", 0);
   __Pyx_INCREF(__pyx_v_invar);
 
-  /* "alphakit/factor/processing.pyx":84
+  /* "alphakit/factor/processing.pyx":93
  * # riskfactor: ['tradingday','ticker,'riskfactor1','riskfactor2']
  * def alphaOpNeu(invar, riskfactor):
  *     tradingday = invar.index             # <<<<<<<<<<<<<<
  *     ticker = invar.columns
  *     invar = invar.copy()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_tradingday = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":85
+  /* "alphakit/factor/processing.pyx":94
  * def alphaOpNeu(invar, riskfactor):
  *     tradingday = invar.index
  *     ticker = invar.columns             # <<<<<<<<<<<<<<
  *     invar = invar.copy()
  *     invar.index.name = 'tradingday'
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ticker = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":86
+  /* "alphakit/factor/processing.pyx":95
  *     tradingday = invar.index
  *     ticker = invar.columns
  *     invar = invar.copy()             # <<<<<<<<<<<<<<
  *     invar.index.name = 'tradingday'
  *     invar.columns.name = 'ticker'
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF_SET(__pyx_v_invar, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":87
+  /* "alphakit/factor/processing.pyx":96
  *     ticker = invar.columns
  *     invar = invar.copy()
  *     invar.index.name = 'tradingday'             # <<<<<<<<<<<<<<
  *     invar.columns.name = 'ticker'
  *     tvar = invar.unstack()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_name, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_name, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":88
+  /* "alphakit/factor/processing.pyx":97
  *     invar = invar.copy()
  *     invar.index.name = 'tradingday'
  *     invar.columns.name = 'ticker'             # <<<<<<<<<<<<<<
  *     tvar = invar.unstack()
  *     tvar.name = 'testvar'
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_name, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_name, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":89
+  /* "alphakit/factor/processing.pyx":98
  *     invar.index.name = 'tradingday'
  *     invar.columns.name = 'ticker'
  *     tvar = invar.unstack()             # <<<<<<<<<<<<<<
  *     tvar.name = 'testvar'
  *     risk_col = riskfactor.columns
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_unstack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_unstack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_tvar = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":90
+  /* "alphakit/factor/processing.pyx":99
  *     invar.columns.name = 'ticker'
  *     tvar = invar.unstack()
  *     tvar.name = 'testvar'             # <<<<<<<<<<<<<<
  *     risk_col = riskfactor.columns
  *     dfall = pd.concat([tvar, riskfactor], axis=1)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_tvar, __pyx_n_s_name, __pyx_n_s_testvar) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_tvar, __pyx_n_s_name, __pyx_n_s_testvar) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
 
-  /* "alphakit/factor/processing.pyx":91
+  /* "alphakit/factor/processing.pyx":100
  *     tvar = invar.unstack()
  *     tvar.name = 'testvar'
  *     risk_col = riskfactor.columns             # <<<<<<<<<<<<<<
  *     dfall = pd.concat([tvar, riskfactor], axis=1)
  *     dfall[risk_col] = dfall[risk_col].astype('float64')
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_riskfactor, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_riskfactor, __pyx_n_s_columns); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_risk_col = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/processing.pyx":92
+  /* "alphakit/factor/processing.pyx":101
  *     tvar.name = 'testvar'
  *     risk_col = riskfactor.columns
  *     dfall = pd.concat([tvar, riskfactor], axis=1)             # <<<<<<<<<<<<<<
  *     dfall[risk_col] = dfall[risk_col].astype('float64')
  *     dfall['testvar'] = dfall['testvar'].astype('float64')
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_concat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_concat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_tvar);
   __Pyx_GIVEREF(__pyx_v_tvar);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_tvar);
   __Pyx_INCREF(__pyx_v_riskfactor);
   __Pyx_GIVEREF(__pyx_v_riskfactor);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_v_riskfactor);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_dfall = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "alphakit/factor/processing.pyx":93
+  /* "alphakit/factor/processing.pyx":102
  *     risk_col = riskfactor.columns
  *     dfall = pd.concat([tvar, riskfactor], axis=1)
  *     dfall[risk_col] = dfall[risk_col].astype('float64')             # <<<<<<<<<<<<<<
  *     dfall['testvar'] = dfall['testvar'].astype('float64')
  *     dfall.reset_index(inplace=True)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_dfall, __pyx_v_risk_col); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_dfall, __pyx_v_risk_col); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_n_s_float64) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_float64);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_dfall, __pyx_v_risk_col, __pyx_t_4) < 0)) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_dfall, __pyx_v_risk_col, __pyx_t_4) < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "alphakit/factor/processing.pyx":94
+  /* "alphakit/factor/processing.pyx":103
  *     dfall = pd.concat([tvar, riskfactor], axis=1)
  *     dfall[risk_col] = dfall[risk_col].astype('float64')
  *     dfall['testvar'] = dfall['testvar'].astype('float64')             # <<<<<<<<<<<<<<
  *     dfall.reset_index(inplace=True)
  *     dfall.drop_duplicates(['tradingday', 'ticker'], inplace=True)
  */
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dfall, __pyx_n_s_testvar); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dfall, __pyx_n_s_testvar); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_n_s_float64) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_n_s_float64);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_dfall, __pyx_n_s_testvar, __pyx_t_4) < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_dfall, __pyx_n_s_testvar, __pyx_t_4) < 0)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "alphakit/factor/processing.pyx":95
+  /* "alphakit/factor/processing.pyx":104
  *     dfall[risk_col] = dfall[risk_col].astype('float64')
  *     dfall['testvar'] = dfall['testvar'].astype('float64')
  *     dfall.reset_index(inplace=True)             # <<<<<<<<<<<<<<
  *     dfall.drop_duplicates(['tradingday', 'ticker'], inplace=True)
  *     dfall.dropna(inplace=True)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_dfall, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_dfall, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "alphakit/factor/processing.pyx":96
+  /* "alphakit/factor/processing.pyx":105
  *     dfall['testvar'] = dfall['testvar'].astype('float64')
  *     dfall.reset_index(inplace=True)
  *     dfall.drop_duplicates(['tradingday', 'ticker'], inplace=True)             # <<<<<<<<<<<<<<
  *     dfall.dropna(inplace=True)
  *     dfall.reset_index(inplace=True, drop=True)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dfall, __pyx_n_s_drop_duplicates); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dfall, __pyx_n_s_drop_duplicates); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_tradingday);
   __Pyx_GIVEREF(__pyx_n_s_tradingday);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_tradingday);
   __Pyx_INCREF(__pyx_n_s_ticker);
   __Pyx_GIVEREF(__pyx_n_s_ticker);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_ticker);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "alphakit/factor/processing.pyx":97
+  /* "alphakit/factor/processing.pyx":106
  *     dfall.reset_index(inplace=True)
  *     dfall.drop_duplicates(['tradingday', 'ticker'], inplace=True)
  *     dfall.dropna(inplace=True)             # <<<<<<<<<<<<<<
  *     dfall.reset_index(inplace=True, drop=True)
  *     dfall['tradingday'] = dfall['tradingday'].astype('datetime64[ns]')
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_dfall, __pyx_n_s_dropna); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_dfall, __pyx_n_s_dropna); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "alphakit/factor/processing.pyx":98
+  /* "alphakit/factor/processing.pyx":107
  *     dfall.drop_duplicates(['tradingday', 'ticker'], inplace=True)
  *     dfall.dropna(inplace=True)
  *     dfall.reset_index(inplace=True, drop=True)             # <<<<<<<<<<<<<<
  *     dfall['tradingday'] = dfall['tradingday'].astype('datetime64[ns]')
  *     retdbeta = neutralize(dfall[risk_col].values, dfall['testvar'].values, groups=dfall['tradingday'].values)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_dfall, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_dfall, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_drop, Py_True) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_drop, Py_True) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "alphakit/factor/processing.pyx":99
+  /* "alphakit/factor/processing.pyx":108
  *     dfall.dropna(inplace=True)
  *     dfall.reset_index(inplace=True, drop=True)
  *     dfall['tradingday'] = dfall['tradingday'].astype('datetime64[ns]')             # <<<<<<<<<<<<<<
  *     retdbeta = neutralize(dfall[risk_col].values, dfall['testvar'].values, groups=dfall['tradingday'].values)
  *     ret_dbeta = dfall[['tradingday', 'ticker']].copy()
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dfall, __pyx_n_s_tradingday); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dfall, __pyx_n_s_tradingday); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_1, __pyx_kp_s_datetime64_ns) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_datetime64_ns);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_dfall, __pyx_n_s_tradingday, __pyx_t_2) < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_dfall, __pyx_n_s_tradingday, __pyx_t_2) < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "alphakit/factor/processing.pyx":100
+  /* "alphakit/factor/processing.pyx":109
  *     dfall.reset_index(inplace=True, drop=True)
  *     dfall['tradingday'] = dfall['tradingday'].astype('datetime64[ns]')
  *     retdbeta = neutralize(dfall[risk_col].values, dfall['testvar'].values, groups=dfall['tradingday'].values)             # <<<<<<<<<<<<<<
  *     ret_dbeta = dfall[['tradingday', 'ticker']].copy()
  *     ret_dbeta['adjfactor'] = retdbeta
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_neutralize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_neutralize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_dfall, __pyx_v_risk_col); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_dfall, __pyx_v_risk_col); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dfall, __pyx_n_s_testvar); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dfall, __pyx_n_s_testvar); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dfall, __pyx_n_s_tradingday); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dfall, __pyx_n_s_tradingday); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_values); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_values); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_groups, __pyx_t_5) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_groups, __pyx_t_5) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_retdbeta = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "alphakit/factor/processing.pyx":101
+  /* "alphakit/factor/processing.pyx":110
  *     dfall['tradingday'] = dfall['tradingday'].astype('datetime64[ns]')
  *     retdbeta = neutralize(dfall[risk_col].values, dfall['testvar'].values, groups=dfall['tradingday'].values)
  *     ret_dbeta = dfall[['tradingday', 'ticker']].copy()             # <<<<<<<<<<<<<<
  *     ret_dbeta['adjfactor'] = retdbeta
  *     adjdata = ret_dbeta.pivot_table(index='tradingday', columns='ticker', values='adjfactor')
  */
-  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_tradingday);
   __Pyx_GIVEREF(__pyx_n_s_tradingday);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_tradingday);
   __Pyx_INCREF(__pyx_n_s_ticker);
   __Pyx_GIVEREF(__pyx_n_s_ticker);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_ticker);
-  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_dfall, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_dfall, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_copy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_copy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_ret_dbeta = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "alphakit/factor/processing.pyx":102
+  /* "alphakit/factor/processing.pyx":111
  *     retdbeta = neutralize(dfall[risk_col].values, dfall['testvar'].values, groups=dfall['tradingday'].values)
  *     ret_dbeta = dfall[['tradingday', 'ticker']].copy()
  *     ret_dbeta['adjfactor'] = retdbeta             # <<<<<<<<<<<<<<
  *     adjdata = ret_dbeta.pivot_table(index='tradingday', columns='ticker', values='adjfactor')
  *     redata = adjdata.reindex(index=tradingday, columns=ticker)
  */
-  if (unlikely(PyObject_SetItem(__pyx_v_ret_dbeta, __pyx_n_s_adjfactor, __pyx_v_retdbeta) < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_ret_dbeta, __pyx_n_s_adjfactor, __pyx_v_retdbeta) < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
 
-  /* "alphakit/factor/processing.pyx":103
+  /* "alphakit/factor/processing.pyx":112
  *     ret_dbeta = dfall[['tradingday', 'ticker']].copy()
  *     ret_dbeta['adjfactor'] = retdbeta
  *     adjdata = ret_dbeta.pivot_table(index='tradingday', columns='ticker', values='adjfactor')             # <<<<<<<<<<<<<<
  *     redata = adjdata.reindex(index=tradingday, columns=ticker)
  *     redata.index.name = 'tradingday'
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ret_dbeta, __pyx_n_s_pivot_table); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ret_dbeta, __pyx_n_s_pivot_table); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_values, __pyx_n_s_adjfactor) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_values, __pyx_n_s_adjfactor) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_adjdata = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "alphakit/factor/processing.pyx":104
+  /* "alphakit/factor/processing.pyx":113
  *     ret_dbeta['adjfactor'] = retdbeta
  *     adjdata = ret_dbeta.pivot_table(index='tradingday', columns='ticker', values='adjfactor')
  *     redata = adjdata.reindex(index=tradingday, columns=ticker)             # <<<<<<<<<<<<<<
  *     redata.index.name = 'tradingday'
  *     redata.columns.name = 'ticker'
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_adjdata, __pyx_n_s_reindex); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_adjdata, __pyx_n_s_reindex); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_v_tradingday) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_v_ticker) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_v_tradingday) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_v_ticker) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_redata = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "alphakit/factor/processing.pyx":105
+  /* "alphakit/factor/processing.pyx":114
  *     adjdata = ret_dbeta.pivot_table(index='tradingday', columns='ticker', values='adjfactor')
  *     redata = adjdata.reindex(index=tradingday, columns=ticker)
  *     redata.index.name = 'tradingday'             # <<<<<<<<<<<<<<
  *     redata.columns.name = 'ticker'
  *     return redata
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_redata, __pyx_n_s_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_redata, __pyx_n_s_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_name, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_name, __pyx_n_s_tradingday) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "alphakit/factor/processing.pyx":106
+  /* "alphakit/factor/processing.pyx":115
  *     redata = adjdata.reindex(index=tradingday, columns=ticker)
  *     redata.index.name = 'tradingday'
  *     redata.columns.name = 'ticker'             # <<<<<<<<<<<<<<
  *     return redata
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_redata, __pyx_n_s_columns); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_redata, __pyx_n_s_columns); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_name, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_name, __pyx_n_s_ticker) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "alphakit/factor/processing.pyx":107
+  /* "alphakit/factor/processing.pyx":116
  *     redata.index.name = 'tradingday'
  *     redata.columns.name = 'ticker'
  *     return redata             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_redata);
   __pyx_r = __pyx_v_redata;
   goto __pyx_L0;
 
-  /* "alphakit/factor/processing.pyx":83
+  /* "alphakit/factor/processing.pyx":92
  * 
  * # riskfactor: ['tradingday','ticker,'riskfactor1','riskfactor2']
  * def alphaOpNeu(invar, riskfactor):             # <<<<<<<<<<<<<<
  *     tradingday = invar.index
  *     ticker = invar.columns
  */
 
@@ -4288,25 +4384,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "alphakit/factor/processing.pyx":75
+  /* "alphakit/factor/processing.pyx":79
  *     data.columns = ['factor', 'ind']
  *     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
- *     indmean = data.reset_index().drop('factor', axis=1).merge(ind_mean, on=['tradingday', 'ind'], how='left').drop(             # <<<<<<<<<<<<<<
- *         'ind', axis=1)
- *     dmean = indmean.pivot_table(index='tradingday', columns='ticker', values='factor')
+ *     indmean = data.reset_index().drop('factor',             # <<<<<<<<<<<<<<
+ *                                       axis=1).merge(ind_mean,
+ *                                                     on=['tradingday', 'ind'],
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_n_s_factor); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_n_s_factor); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_ind); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 75, __pyx_L1_error)
+
+  /* "alphakit/factor/processing.pyx":82
+ *                                       axis=1).merge(ind_mean,
+ *                                                     on=['tradingday', 'ind'],
+ *                                                     how='left').drop('ind',             # <<<<<<<<<<<<<<
+ *                                                                      axis=1)
+ *     dmean = indmean.pivot_table(index='tradingday',
+ */
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_ind); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "alphakit/factor/processing.pyx":7
  * 
  * 
  * def standardize(raw_data):             # <<<<<<<<<<<<<<
@@ -4342,33 +4446,33 @@
   __Pyx_GIVEREF(__pyx_tuple__7);
   __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_processing_pyx, __pyx_n_s_indfill_median, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 49, __pyx_L1_error)
 
   /* "alphakit/factor/processing.pyx":69
  * 
  * #
  * def indLineNeu(invar, ind):             # <<<<<<<<<<<<<<
- *     tradingday = invar.index
- *     ticker = invar.columns
+ *     invar.index.name = 'tradingday'
+ *     invar.columns.name = 'ticker'
  */
   __pyx_tuple__9 = PyTuple_Pack(8, __pyx_n_s_invar, __pyx_n_s_ind, __pyx_n_s_tradingday, __pyx_n_s_ticker, __pyx_n_s_data, __pyx_n_s_ind_mean, __pyx_n_s_indmean, __pyx_n_s_dmean); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
   __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_processing_pyx, __pyx_n_s_indLineNeu, 69, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 69, __pyx_L1_error)
 
-  /* "alphakit/factor/processing.pyx":83
+  /* "alphakit/factor/processing.pyx":92
  * 
  * # riskfactor: ['tradingday','ticker,'riskfactor1','riskfactor2']
  * def alphaOpNeu(invar, riskfactor):             # <<<<<<<<<<<<<<
  *     tradingday = invar.index
  *     ticker = invar.columns
  */
-  __pyx_tuple__11 = PyTuple_Pack(11, __pyx_n_s_invar, __pyx_n_s_riskfactor, __pyx_n_s_tradingday, __pyx_n_s_ticker, __pyx_n_s_tvar, __pyx_n_s_risk_col, __pyx_n_s_dfall, __pyx_n_s_retdbeta, __pyx_n_s_ret_dbeta, __pyx_n_s_adjdata, __pyx_n_s_redata); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(11, __pyx_n_s_invar, __pyx_n_s_riskfactor, __pyx_n_s_tradingday, __pyx_n_s_ticker, __pyx_n_s_tvar, __pyx_n_s_risk_col, __pyx_n_s_dfall, __pyx_n_s_retdbeta, __pyx_n_s_ret_dbeta, __pyx_n_s_adjdata, __pyx_n_s_redata); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_processing_pyx, __pyx_n_s_alphaOpNeu, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_processing_pyx, __pyx_n_s_alphaOpNeu, 92, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -4730,32 +4834,32 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_indfill_median, __pyx_t_2) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "alphakit/factor/processing.pyx":69
  * 
  * #
  * def indLineNeu(invar, ind):             # <<<<<<<<<<<<<<
- *     tradingday = invar.index
- *     ticker = invar.columns
+ *     invar.index.name = 'tradingday'
+ *     invar.columns.name = 'ticker'
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8alphakit_6factor_10processing_7indLineNeu, NULL, __pyx_n_s_alphakit_factor_processing); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_indLineNeu, __pyx_t_2) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "alphakit/factor/processing.pyx":83
+  /* "alphakit/factor/processing.pyx":92
  * 
  * # riskfactor: ['tradingday','ticker,'riskfactor1','riskfactor2']
  * def alphaOpNeu(invar, riskfactor):             # <<<<<<<<<<<<<<
  *     tradingday = invar.index
  *     ticker = invar.columns
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8alphakit_6factor_10processing_9alphaOpNeu, NULL, __pyx_n_s_alphakit_factor_processing); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8alphakit_6factor_10processing_9alphaOpNeu, NULL, __pyx_n_s_alphakit_factor_processing); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_alphaOpNeu, __pyx_t_2) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_alphaOpNeu, __pyx_t_2) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "alphakit/factor/processing.pyx":1
  * # -*- coding: utf-8 -*-             # <<<<<<<<<<<<<<
  * import pandas as pd
  * import numpy as np
  */
```

### Comparing `Alphakit-1.2.3/alphakit/factor/processing.pyx` & `Alphakit-1.2.4/alphakit/factor/processing.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -63,22 +63,31 @@
     rdata.index.name = 'tradingday'
     rdata.columns.name = 'ticker'
     return rdata
 
 
 # 行业线性中性化
 def indLineNeu(invar, ind):
+    invar.index.name = 'tradingday'
+    invar.columns.name = 'ticker'
+    ind.index.name = 'tradingday'
+    ind.columns.name = 'ticker'
     tradingday = invar.index
     ticker = invar.columns
     data = pd.concat([invar.unstack(), ind.unstack()], axis=1)
     data.columns = ['factor', 'ind']
     ind_mean = data.groupby(['tradingday', 'ind']).mean().reset_index()
-    indmean = data.reset_index().drop('factor', axis=1).merge(ind_mean, on=['tradingday', 'ind'], how='left').drop(
-        'ind', axis=1)
-    dmean = indmean.pivot_table(index='tradingday', columns='ticker', values='factor')
+    indmean = data.reset_index().drop('factor',
+                                      axis=1).merge(ind_mean,
+                                                    on=['tradingday', 'ind'],
+                                                    how='left').drop('ind',
+                                                                     axis=1)
+    dmean = indmean.pivot_table(index='tradingday',
+                                columns='ticker',
+                                values='factor')
     dmean = dmean.reindex(index=tradingday, columns=ticker)
     return invar - dmean
 
 
 # riskfactor: ['tradingday','ticker,'riskfactor1','riskfactor2']
 def alphaOpNeu(invar, riskfactor):
     tradingday = invar.index
```

### Comparing `Alphakit-1.2.3/alphakit/factor/transform.c` & `Alphakit-1.2.4/alphakit/factor/transform.c`

 * *Files 0% similar despite different names*

```diff
@@ -2258,15 +2258,15 @@
   __Pyx_RefNannySetupContext("factor_score_sig", 0);
 
   /* "alphakit/factor/transform.pyx":34
  * 
  * def factor_score_sig(invar):
  *     invar_rank = invar.rank(axis=1, method='max')             # <<<<<<<<<<<<<<
  *     count = invar_rank.count(axis=1)
- *     invar_rank = (invar_rank - 3. / 8. ).div(count + 1. / 4., axis='rows')
+ *     invar_rank = (invar_rank - 3. / 8.).div(count + 1. / 4., axis='rows')
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_rank); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_method, __pyx_n_s_max) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
@@ -2277,15 +2277,15 @@
   __pyx_v_invar_rank = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "alphakit/factor/transform.pyx":35
  * def factor_score_sig(invar):
  *     invar_rank = invar.rank(axis=1, method='max')
  *     count = invar_rank.count(axis=1)             # <<<<<<<<<<<<<<
- *     invar_rank = (invar_rank - 3. / 8. ).div(count + 1. / 4., axis='rows')
+ *     invar_rank = (invar_rank - 3. / 8.).div(count + 1. / 4., axis='rows')
  *     invar_score = pd.DataFrame(norm.ppf(invar_rank),
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar_rank, __pyx_n_s_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
@@ -2295,15 +2295,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_count = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "alphakit/factor/transform.pyx":36
  *     invar_rank = invar.rank(axis=1, method='max')
  *     count = invar_rank.count(axis=1)
- *     invar_rank = (invar_rank - 3. / 8. ).div(count + 1. / 4., axis='rows')             # <<<<<<<<<<<<<<
+ *     invar_rank = (invar_rank - 3. / 8.).div(count + 1. / 4., axis='rows')             # <<<<<<<<<<<<<<
  *     invar_score = pd.DataFrame(norm.ppf(invar_rank),
  *                                index=invar.index,
  */
   __pyx_t_1 = PyFloat_FromDouble((3. / 8.)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyNumber_Subtract(__pyx_v_invar_rank, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -2330,15 +2330,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_invar_rank, __pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "alphakit/factor/transform.pyx":37
  *     count = invar_rank.count(axis=1)
- *     invar_rank = (invar_rank - 3. / 8. ).div(count + 1. / 4., axis='rows')
+ *     invar_rank = (invar_rank - 3. / 8.).div(count + 1. / 4., axis='rows')
  *     invar_score = pd.DataFrame(norm.ppf(invar_rank),             # <<<<<<<<<<<<<<
  *                                index=invar.index,
  *                                columns=invar.columns)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
@@ -2367,15 +2367,15 @@
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "alphakit/factor/transform.pyx":38
- *     invar_rank = (invar_rank - 3. / 8. ).div(count + 1. / 4., axis='rows')
+ *     invar_rank = (invar_rank - 3. / 8.).div(count + 1. / 4., axis='rows')
  *     invar_score = pd.DataFrame(norm.ppf(invar_rank),
  *                                index=invar.index,             # <<<<<<<<<<<<<<
  *                                columns=invar.columns)
  *     return invar_score
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
@@ -2393,15 +2393,15 @@
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_columns); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_columns, __pyx_t_2) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "alphakit/factor/transform.pyx":37
  *     count = invar_rank.count(axis=1)
- *     invar_rank = (invar_rank - 3. / 8. ).div(count + 1. / 4., axis='rows')
+ *     invar_rank = (invar_rank - 3. / 8.).div(count + 1. / 4., axis='rows')
  *     invar_score = pd.DataFrame(norm.ppf(invar_rank),             # <<<<<<<<<<<<<<
  *                                index=invar.index,
  *                                columns=invar.columns)
  */
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
```

### Comparing `Alphakit-1.2.3/alphakit/factor/transform.pyx` & `Alphakit-1.2.4/alphakit/factor/transform.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -29,12 +29,12 @@
         invar_score[invar_bak < 0] = -invar_score[invar_bak < 0]
     return invar_score
 
 
 def factor_score_sig(invar):
     invar_rank = invar.rank(axis=1, method='max')
     count = invar_rank.count(axis=1)
-    invar_rank = (invar_rank - 3. / 8. ).div(count + 1. / 4., axis='rows')
+    invar_rank = (invar_rank - 3. / 8.).div(count + 1. / 4., axis='rows')
     invar_score = pd.DataFrame(norm.ppf(invar_rank),
                                index=invar.index,
                                columns=invar.columns)
     return invar_score
```

### Comparing `Alphakit-1.2.3/alphakit/portfolio/combine.c` & `Alphakit-1.2.4/alphakit/portfolio/combine.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.3/setup.py` & `Alphakit-1.2.4/setup.py`

 * *Files identical despite different names*

