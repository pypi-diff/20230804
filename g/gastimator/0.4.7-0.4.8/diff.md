# Comparing `tmp/gastimator-0.4.7.tar.gz` & `tmp/gastimator-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gastimator-0.4.7.tar", last modified: Tue Apr 11 11:04:37 2023, max compression
+gzip compressed data, was "gastimator-0.4.8.tar", last modified: Fri Aug  4 11:08:22 2023, max compression
```

## Comparing `gastimator-0.4.7.tar` & `gastimator-0.4.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-11 11:04:37.006528 gastimator-0.4.7/
--rw-r--r--   0 tdavis     (501) staff       (20)    35149 2020-08-19 16:59:58.000000 gastimator-0.4.7/LICENSE
--rw-r--r--   0 tdavis     (501) staff       (20)     1853 2023-04-11 11:04:37.006342 gastimator-0.4.7/PKG-INFO
--rw-r--r--   0 tdavis     (501) staff       (20)     1308 2022-02-14 17:26:04.000000 gastimator-0.4.7/README.md
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-11 11:04:37.003936 gastimator-0.4.7/gastimator/
--rwxr-xr-x   0 tdavis     (501) staff       (20)      120 2020-08-19 16:59:58.000000 gastimator-0.4.7/gastimator/__init__.py
--rw-r--r--   0 tdavis     (501) staff       (20)    19149 2023-04-11 10:46:06.000000 gastimator-0.4.7/gastimator/corner_plot.py
--rwxr-xr-x   0 tdavis     (501) staff       (20)    16794 2023-02-24 13:47:39.000000 gastimator-0.4.7/gastimator/gastimator.py
--rwxr-xr-x   0 tdavis     (501) staff       (20)      422 2022-06-01 11:02:19.000000 gastimator-0.4.7/gastimator/priors.py
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-11 11:04:37.004927 gastimator-0.4.7/gastimator.egg-info/
--rw-r--r--   0 tdavis     (501) staff       (20)     1853 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/PKG-INFO
--rw-r--r--   0 tdavis     (501) staff       (20)      404 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/SOURCES.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/dependency_links.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2020-08-19 17:27:19.000000 gastimator-0.4.7/gastimator.egg-info/not-zip-safe
--rw-r--r--   0 tdavis     (501) staff       (20)       45 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/requires.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       11 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/top_level.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-04-11 11:04:37.006576 gastimator-0.4.7/setup.cfg
--rw-r--r--   0 tdavis     (501) staff       (20)      962 2023-04-11 10:46:42.000000 gastimator-0.4.7/setup.py
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-11 11:04:37.005846 gastimator-0.4.7/test/
--rw-r--r--   0 tdavis     (501) staff       (20)     1108 2023-02-21 10:50:31.000000 gastimator-0.4.7/test/test_gastimator.py
--rw-r--r--   0 tdavis     (501) staff       (20)     1256 2022-08-30 09:40:28.000000 gastimator-0.4.7/test/test_gastimator_prior.py
--rw-r--r--   0 tdavis     (501) staff       (20)     3693 2023-02-13 18:18:51.000000 gastimator-0.4.7/test/test_gastimator_ul.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-08-04 11:08:22.669144 gastimator-0.4.8/
+-rw-r--r--   0 tdavis     (501) staff       (20)    35149 2020-08-19 16:59:58.000000 gastimator-0.4.8/LICENSE
+-rw-r--r--   0 tdavis     (501) staff       (20)     1853 2023-08-04 11:08:22.668967 gastimator-0.4.8/PKG-INFO
+-rw-r--r--   0 tdavis     (501) staff       (20)     1308 2022-02-14 17:26:04.000000 gastimator-0.4.8/README.md
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-08-04 11:08:22.666726 gastimator-0.4.8/gastimator/
+-rwxr-xr-x   0 tdavis     (501) staff       (20)      120 2020-08-19 16:59:58.000000 gastimator-0.4.8/gastimator/__init__.py
+-rw-r--r--   0 tdavis     (501) staff       (20)    19149 2023-04-11 10:46:06.000000 gastimator-0.4.8/gastimator/corner_plot.py
+-rwxr-xr-x   0 tdavis     (501) staff       (20)    16732 2023-08-04 11:06:20.000000 gastimator-0.4.8/gastimator/gastimator.py
+-rwxr-xr-x   0 tdavis     (501) staff       (20)      422 2022-06-01 11:02:19.000000 gastimator-0.4.8/gastimator/priors.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-08-04 11:08:22.667718 gastimator-0.4.8/gastimator.egg-info/
+-rw-r--r--   0 tdavis     (501) staff       (20)     1853 2023-08-04 11:08:22.000000 gastimator-0.4.8/gastimator.egg-info/PKG-INFO
+-rw-r--r--   0 tdavis     (501) staff       (20)      404 2023-08-04 11:08:22.000000 gastimator-0.4.8/gastimator.egg-info/SOURCES.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-08-04 11:08:22.000000 gastimator-0.4.8/gastimator.egg-info/dependency_links.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2020-08-19 17:27:19.000000 gastimator-0.4.8/gastimator.egg-info/not-zip-safe
+-rw-r--r--   0 tdavis     (501) staff       (20)       44 2023-08-04 11:08:22.000000 gastimator-0.4.8/gastimator.egg-info/requires.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       11 2023-08-04 11:08:22.000000 gastimator-0.4.8/gastimator.egg-info/top_level.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-08-04 11:08:22.669192 gastimator-0.4.8/setup.cfg
+-rw-r--r--   0 tdavis     (501) staff       (20)      961 2023-08-04 11:06:14.000000 gastimator-0.4.8/setup.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-08-04 11:08:22.668532 gastimator-0.4.8/test/
+-rw-r--r--   0 tdavis     (501) staff       (20)     1131 2023-08-04 11:06:18.000000 gastimator-0.4.8/test/test_gastimator.py
+-rw-r--r--   0 tdavis     (501) staff       (20)     1256 2022-08-30 09:40:28.000000 gastimator-0.4.8/test/test_gastimator_prior.py
+-rw-r--r--   0 tdavis     (501) staff       (20)     3693 2023-02-13 18:18:51.000000 gastimator-0.4.8/test/test_gastimator_ul.py
```

### Comparing `gastimator-0.4.7/LICENSE` & `gastimator-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.7/PKG-INFO` & `gastimator-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gastimator
-Version: 0.4.7
+Version: 0.4.8
 Summary: Implementation of a Python MCMC gibbs-sampler with adaptive stepping
 Home-page: https://github.com/TimothyADavis/GAStimator
 Author: Timothy A. Davis
 Author-email: DavisT@cardiff.ac.uk
 License: GNU GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gastimator-0.4.7/README.md` & `gastimator-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.7/gastimator/corner_plot.py` & `gastimator-0.4.8/gastimator/corner_plot.py`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.7/gastimator/gastimator.py` & `gastimator-0.4.8/gastimator/gastimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,14 @@
         #try:
         par= Parallel(n_jobs= self.nprocesses, verbose=verboselev)
         results=par(delayed(unwrap_self)(i) for i in zip([self]*nchains, [self.guesses]*nchains,[int(float(niters))]*nchains,[numatonce]*nchains,[knob]*nchains, [plot]*nchains, [False]*nchains,np.arange(nchains)))
         #except:
         #    par= Parallel(n_jobs= self.nprocesses, verbose=verboselev, prefer="threads")
         #    results=par(delayed(unwrap_self)(i) for i in zip([self]*nchains, [self.guesses]*nchains,[int(float(niters))]*nchains,[numatonce]*nchains,[knob]*nchains, [plot]*nchains, [False]*nchains,np.arange(nchains)))
         results=np.array(results,dtype=object)
-        par._terminate_backend()
         get_reusable_executor().shutdown(wait=True)
         ##
         #debug line #results=unwrap_self((self, self.guesses,int(float(niters)),numatonce,knob, False, False,0))
 
         bestchain=np.argmax(np.max(np.stack(results[:,1]),axis=1))
         bestvalinbestchain=np.argmax(results[bestchain,1])
     
@@ -397,15 +396,14 @@
     #try:
     par= Parallel(n_jobs= self.nprocesses, verbose=verboselev)
     results=par(delayed(unwrap_self)(i) for i in zip([self]*self.nprocesses, [verybestvalues]*self.nprocesses,[int(float(niters)/float(self.nprocesses))]*self.nprocesses,[numatonce]*self.nprocesses,[verybestknob]*self.nprocesses, [False]*self.nprocesses, [True]*self.nprocesses,np.arange(self.nprocesses)))
     # except:
     #     par= Parallel(n_jobs= self.nprocesses, verbose=verboselev,prefer="threads")
     #     results=par(delayed(unwrap_self)(i) for i in zip([self]*self.nprocesses, [verybestvalues]*self.nprocesses,[int(float(niters)/float(self.nprocesses))]*self.nprocesses,[numatonce]*self.nprocesses,[verybestknob]*self.nprocesses, [False]*self.nprocesses, [True]*self.nprocesses,np.arange(self.nprocesses)))
     results=np.array(results,dtype=object)
-    par._terminate_backend()
     get_reusable_executor().shutdown(wait=True)
     
     outputvalue= np.concatenate(results[:,0],axis=1)
     outputll= np.concatenate(results[:,1])
     
     if outputll.size < 1: 
         print('WARNING: No accepted models. Perhaps you need to increase the number of steps?')
```

### Comparing `gastimator-0.4.7/gastimator.egg-info/PKG-INFO` & `gastimator-0.4.8/gastimator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gastimator
-Version: 0.4.7
+Version: 0.4.8
 Summary: Implementation of a Python MCMC gibbs-sampler with adaptive stepping
 Home-page: https://github.com/TimothyADavis/GAStimator
 Author: Timothy A. Davis
 Author-email: DavisT@cardiff.ac.uk
 License: GNU GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gastimator-0.4.7/setup.py` & `gastimator-0.4.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
  
 setup(name='gastimator',
-       version='0.4.7',
+       version='0.4.8',
        description='Implementation of a Python MCMC gibbs-sampler with adaptive stepping',
        url='https://github.com/TimothyADavis/GAStimator',
        author='Timothy A. Davis',
        author_email='DavisT@cardiff.ac.uk',
        long_description=long_description,
        long_description_content_type="text/markdown",
        license='GNU GPLv3',
        packages=['gastimator'],
        install_requires=[
            'numpy',
            'matplotlib',
            'tqdm',
            'plotbin',
-           'joblib>=0.16.0',
+           'joblib>=1.3.1',
        ],
        classifiers=[
          'Development Status :: 3 - Alpha',
          'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
          'Programming Language :: Python :: 3',
          'Operating System :: OS Independent',
        ],
```

### Comparing `gastimator-0.4.7/test/test_gastimator.py` & `gastimator-0.4.8/test/test_gastimator.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,10 +25,13 @@
 mcmc.fixed=np.array([False, False]) #if you would like to fix a variable then you can set its value to True here.
 mcmc.precision=np.array([1.,1.]) #here we assume we can get the intercept and gradient within ±1.0 - very conservative
 mcmc.prior_func=(None,None)
 nsamples=1000000
 
 #mcmc.input_checks()
 #print(mcmc.prior_func)
-#mcmc.nprocesses=1
+mcmc.nprocesses=1
 outputvalue, outputll= mcmc.run(data,1e-3,nsamples,nchains=3,plot=False)    
-print("Time taken:",time.time()-t)
+print("Time taken:",time.time()-t)
+
+
+#joblib '1.1.1' works
```

### Comparing `gastimator-0.4.7/test/test_gastimator_prior.py` & `gastimator-0.4.8/test/test_gastimator_prior.py`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.7/test/test_gastimator_ul.py` & `gastimator-0.4.8/test/test_gastimator_ul.py`

 * *Files identical despite different names*

