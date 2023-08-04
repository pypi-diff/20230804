# Comparing `tmp/margarine-0.3.1.tar.gz` & `tmp/margarine-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "margarine-0.3.1.tar", last modified: Thu Jan 12 17:08:52 2023, max compression
+gzip compressed data, was "margarine-1.0.0.tar", last modified: Fri Aug  4 12:43:15 2023, max compression
```

## Comparing `margarine-0.3.1.tar` & `margarine-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-01-12 17:08:52.301991 margarine-0.3.1/
--rw-r--r--   0 harry      (501) staff       (20)     1082 2022-09-13 13:30:11.000000 margarine-0.3.1/LICENSE
--rw-r--r--   0 harry      (501) staff       (20)     5595 2023-01-12 17:08:52.301870 margarine-0.3.1/PKG-INFO
--rwxr-xr-x   0 harry      (501) staff       (20)     4864 2022-09-13 15:32:48.000000 margarine-0.3.1/README.rst
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-01-12 17:08:52.300974 margarine-0.3.1/margarine/
--rwxr-xr-x   0 harry      (501) staff       (20)        0 2022-10-11 07:45:31.000000 margarine-0.3.1/margarine/__init__.py
--rwxr-xr-x   0 harry      (501) staff       (20)    10118 2022-10-11 07:45:31.000000 margarine-0.3.1/margarine/kde.py
--rwxr-xr-x   0 harry      (501) staff       (20)    14104 2023-01-12 17:03:50.000000 margarine-0.3.1/margarine/maf.py
--rwxr-xr-x   0 harry      (501) staff       (20)     8073 2022-09-13 15:09:06.000000 margarine-0.3.1/margarine/marginal_stats.py
--rwxr-xr-x   0 harry      (501) staff       (20)     2160 2022-09-13 13:30:11.000000 margarine-0.3.1/margarine/processing.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-01-12 17:08:52.301683 margarine-0.3.1/margarine.egg-info/
--rw-r--r--   0 harry      (501) staff       (20)     5595 2023-01-12 17:08:52.000000 margarine-0.3.1/margarine.egg-info/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)      299 2023-01-12 17:08:52.000000 margarine-0.3.1/margarine.egg-info/SOURCES.txt
--rw-r--r--   0 harry      (501) staff       (20)        1 2023-01-12 17:08:52.000000 margarine-0.3.1/margarine.egg-info/dependency_links.txt
--rw-r--r--   0 harry      (501) staff       (20)       94 2023-01-12 17:08:52.000000 margarine-0.3.1/margarine.egg-info/requires.txt
--rw-r--r--   0 harry      (501) staff       (20)       10 2023-01-12 17:08:52.000000 margarine-0.3.1/margarine.egg-info/top_level.txt
--rw-r--r--   0 harry      (501) staff       (20)       38 2023-01-12 17:08:52.302029 margarine-0.3.1/setup.cfg
--rwxr-xr-x   0 harry      (501) staff       (20)     1280 2023-01-12 17:08:30.000000 margarine-0.3.1/setup.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-08-04 12:43:15.952740 margarine-1.0.0/
+-rw-r--r--   0 harry      (501) staff       (20)     1082 2022-09-13 13:30:11.000000 margarine-1.0.0/LICENSE
+-rw-r--r--   0 harry      (501) staff       (20)     6391 2023-08-04 12:43:15.952625 margarine-1.0.0/PKG-INFO
+-rwxr-xr-x   0 harry      (501) staff       (20)     5660 2023-08-04 12:40:44.000000 margarine-1.0.0/README.rst
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-08-04 12:43:15.951658 margarine-1.0.0/margarine/
+-rwxr-xr-x   0 harry      (501) staff       (20)        0 2022-10-11 07:45:31.000000 margarine-1.0.0/margarine/__init__.py
+-rw-r--r--   0 harry      (501) staff       (20)    17654 2023-08-04 12:40:44.000000 margarine-1.0.0/margarine/clustered.py
+-rwxr-xr-x   0 harry      (501) staff       (20)    12141 2023-08-04 12:40:44.000000 margarine-1.0.0/margarine/kde.py
+-rwxr-xr-x   0 harry      (501) staff       (20)    17329 2023-08-04 12:40:44.000000 margarine-1.0.0/margarine/maf.py
+-rwxr-xr-x   0 harry      (501) staff       (20)     6500 2023-08-04 12:40:44.000000 margarine-1.0.0/margarine/marginal_stats.py
+-rwxr-xr-x   0 harry      (501) staff       (20)     2437 2023-08-04 12:40:44.000000 margarine-1.0.0/margarine/processing.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-08-04 12:43:15.952199 margarine-1.0.0/margarine.egg-info/
+-rw-r--r--   0 harry      (501) staff       (20)     6391 2023-08-04 12:43:15.000000 margarine-1.0.0/margarine.egg-info/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)      365 2023-08-04 12:43:15.000000 margarine-1.0.0/margarine.egg-info/SOURCES.txt
+-rw-r--r--   0 harry      (501) staff       (20)        1 2023-08-04 12:43:15.000000 margarine-1.0.0/margarine.egg-info/dependency_links.txt
+-rw-r--r--   0 harry      (501) staff       (20)       94 2023-08-04 12:43:15.000000 margarine-1.0.0/margarine.egg-info/requires.txt
+-rw-r--r--   0 harry      (501) staff       (20)       10 2023-08-04 12:43:15.000000 margarine-1.0.0/margarine.egg-info/top_level.txt
+-rw-r--r--   0 harry      (501) staff       (20)       38 2023-08-04 12:43:15.952778 margarine-1.0.0/setup.cfg
+-rwxr-xr-x   0 harry      (501) staff       (20)     1280 2023-08-04 12:40:44.000000 margarine-1.0.0/setup.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-08-04 12:43:15.952436 margarine-1.0.0/tests/
+-rw-r--r--   0 harry      (501) staff       (20)     2383 2023-08-04 12:40:44.000000 margarine-1.0.0/tests/test_clusters.py
+-rwxr-xr-x   0 harry      (501) staff       (20)     4938 2023-08-04 12:40:44.000000 margarine-1.0.0/tests/test_stats.py
```

### Comparing `margarine-0.3.1/LICENSE` & `margarine-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `margarine-0.3.1/PKG-INFO` & `margarine-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margarine
-Version: 0.3.1
+Version: 1.0.0
 Summary: margarine: Posterior Sampling and Marginal Bayesian Statistics
 Home-page: https://github.com/htjb/margarine
 Author: Harry T. J. Bevins
 Author-email: htjb2@cam.ac.uk
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -23,15 +23,15 @@
 ================================================================
 
 Introduction
 ------------
 
 :margarine: Marginal Bayesian Statistics
 :Authors: Harry T.J. Bevins
-:Version: 0.3.0
+:Version: 1.0.0
 :Homepage:  https://github.com/htjb/margarine
 :Documentation: https://margarine.readthedocs.io/
 
 .. image:: https://readthedocs.org/projects/margarine/badge/?version=latest
   :target: https://margarine.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
@@ -88,15 +88,17 @@
 --------------------
 
 The software is available on the MIT licence.
 
 If you use the code for academic purposes we request that you cite the following
 `paper <https://ui.adsabs.harvard.edu/abs/2022arXiv220512841B/abstract>`__ and
 the `MaxEnt22 proceedings <https://ui.adsabs.harvard.edu/search/p_=0&q=author%3A%22Bevins%2C%20H.%20T.%20J.%22&sort=date%20desc%2C%20bibcode%20desc>`__
-for which you can use the following bibtex
+If you use the clustering implementation please cite the following
+`prepring <https://arxiv.org/abs/2305.02930>`__.
+You can use the following bibtex
 
 .. code:: bibtex
 
     @ARTICLE{2022arXiv220512841B,
          author = {{Bevins}, Harry T.~J. and {Handley}, William J. and {Lemos}, Pablo and {Sims}, Peter H. and {de Lera Acedo}, Eloy and {Fialkov}, Anastasia and {Alsing}, Justin},
           title = "{Removing the fat from your posterior samples with margarine}",
         journal = {arXiv e-prints},
@@ -128,14 +130,36 @@
   archivePrefix = {arXiv},
        eprint = {2207.11457},
   primaryClass = {astro-ph.CO},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2022arXiv220711457B},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
   }
 
+and
+
+.. code:: bibtex
+
+  @ARTICLE{2023arXiv230502930B,
+        author = {{Bevins}, Harry and {Handley}, Will},
+          title = "{Piecewise Normalizing Flows}",
+        journal = {arXiv e-prints},
+      keywords = {Statistics - Machine Learning, Computer Science - Machine Learning},
+          year = 2023,
+          month = may,
+            eid = {arXiv:2305.02930},
+          pages = {arXiv:2305.02930},
+            doi = {10.48550/arXiv.2305.02930},
+  archivePrefix = {arXiv},
+        eprint = {2305.02930},
+  primaryClass = {stat.ML},
+        adsurl = {https://ui.adsabs.harvard.edu/abs/2023arXiv230502930B},
+        adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+  }
+
+
 Requirements
 ------------
 
 The code requires the following packages to run:
 
 - `numpy <https://pypi.org/project/numpy/>`__
 - `tensorflow <https://pypi.org/project/tensorflow/>`__
```

### Comparing `margarine-0.3.1/README.rst` & `margarine-1.0.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ================================================================
 
 Introduction
 ------------
 
 :margarine: Marginal Bayesian Statistics
 :Authors: Harry T.J. Bevins
-:Version: 0.3.0
+:Version: 1.0.0
 :Homepage:  https://github.com/htjb/margarine
 :Documentation: https://margarine.readthedocs.io/
 
 .. image:: https://readthedocs.org/projects/margarine/badge/?version=latest
   :target: https://margarine.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
@@ -68,15 +68,17 @@
 --------------------
 
 The software is available on the MIT licence.
 
 If you use the code for academic purposes we request that you cite the following
 `paper <https://ui.adsabs.harvard.edu/abs/2022arXiv220512841B/abstract>`__ and
 the `MaxEnt22 proceedings <https://ui.adsabs.harvard.edu/search/p_=0&q=author%3A%22Bevins%2C%20H.%20T.%20J.%22&sort=date%20desc%2C%20bibcode%20desc>`__
-for which you can use the following bibtex
+If you use the clustering implementation please cite the following
+`prepring <https://arxiv.org/abs/2305.02930>`__.
+You can use the following bibtex
 
 .. code:: bibtex
 
     @ARTICLE{2022arXiv220512841B,
          author = {{Bevins}, Harry T.~J. and {Handley}, William J. and {Lemos}, Pablo and {Sims}, Peter H. and {de Lera Acedo}, Eloy and {Fialkov}, Anastasia and {Alsing}, Justin},
           title = "{Removing the fat from your posterior samples with margarine}",
         journal = {arXiv e-prints},
@@ -108,14 +110,36 @@
   archivePrefix = {arXiv},
        eprint = {2207.11457},
   primaryClass = {astro-ph.CO},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2022arXiv220711457B},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
   }
 
+and
+
+.. code:: bibtex
+
+  @ARTICLE{2023arXiv230502930B,
+        author = {{Bevins}, Harry and {Handley}, Will},
+          title = "{Piecewise Normalizing Flows}",
+        journal = {arXiv e-prints},
+      keywords = {Statistics - Machine Learning, Computer Science - Machine Learning},
+          year = 2023,
+          month = may,
+            eid = {arXiv:2305.02930},
+          pages = {arXiv:2305.02930},
+            doi = {10.48550/arXiv.2305.02930},
+  archivePrefix = {arXiv},
+        eprint = {2305.02930},
+  primaryClass = {stat.ML},
+        adsurl = {https://ui.adsabs.harvard.edu/abs/2023arXiv230502930B},
+        adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+  }
+
+
 Requirements
 ------------
 
 The code requires the following packages to run:
 
 - `numpy <https://pypi.org/project/numpy/>`__
 - `tensorflow <https://pypi.org/project/tensorflow/>`__
```

### Comparing `margarine-0.3.1/margarine/kde.py` & `margarine-1.0.0/margarine/kde.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 import numpy as np
 from scipy.stats import gaussian_kde, norm
 from margarine.processing import _forward_transform, _inverse_transform
 from scipy.optimize import root_scalar
+import tensorflow as tf
 import pickle
 import warnings
 from tensorflow_probability import bijectors as tfb
 import margarine
+import anesthetic
 
 
 class KDE(object):
 
     r"""
     This class is used to generate a KDE given a weighted set of samples,
     generate samples from that KDE, transform samples on the
     hypercube into samples on the KDE and save and load the KDE model.
 
     **Parameters:**
 
-        theta: **numpy array**
+        theta: **numpy array or anesthetic.samples**
             | The samples from the probability distribution that we require the
-                bijector to learn.
-
-        weights: **numpy array**
-            | The weights associated with the samples above.
+                MAF to learn. This can either be a numpy array or an anesthetic
+                NestedSamples or MCMCSamples object.
 
     **kwargs:**
 
+        weights: **numpy array / default=np.ones(len(theta))**
+            | The weights associated with the samples above. If an anesthetic
+                NestedSamples or MCMCSamples object is passed the code
+                draws the weights from this.
+
         bw_method: **str, scalar or callable**
             | The bandwidth for the KDE.
-            
+
         theta_max: **numpy array**
             | The true upper limits of the priors used to generate the samples
                 that we want the MAF to learn.
-        
+
         theta_min: **numpy array**
             | As above but the true lower limits of the priors.
 
+        parameters: **list of strings**
+            | A list of the relevant parameters to train on. Only needed
+                if theta is an anestehetic samples object. If not provided,
+                all parameters will be used.
     **Attributes:**
 
     A list of some key attributes accessible to the user.
 
         kde: **Instance of scipy.stats.gaussian_kde**
             | Once the class has been initalised with a set of samples and
                 their corresponding weights we can generate the kde using
@@ -60,47 +69,69 @@
                 class). Once the KDE is generated it can be accessed via
                 `KDE_class.kde`. Initialisation of the class and generation
                 of the KDE are kept seperate to allow models to be saved and
                 loaded effectively.
 
         theta_max: **numpy array**
             | The true upper limits of the priors used to generate the samples
-                that we want the MAF to learn. If theta_max is not supplied as a
-                kwarg, then this is is an approximate estimate (for more info see
-                the ... paper).
+                that we want the MAF to learn. If theta_max is not
+                supplied as a kwarg, then this is is an approximate
+                estimate.
 
         theta_min: **numpy array**
-            | As above but for the true lower limits of the priors. If theta_max is
-                not supplied as a kwarg, then this is is an approximate estimate.
+            | As above but for the true lower limits of the priors.
+                If theta_max is not supplied as a kwarg, then this
+                is an approximate estimate.
 
     """
 
-    def __init__(self, theta, weights, **kwargs):
+    def __init__(self, theta, **kwargs):
+
+        self.parameters = kwargs.pop('parameters', None)
+
+        if isinstance(theta, 
+                      (anesthetic.samples.NestedSamples, 
+                       anesthetic.samples.MCMCSamples)):
+            weights = theta.get_weights()
+            if self.parameters:
+                theta = theta[self.parameters].values
+            else:
+                if isinstance(theta, anesthetic.samples.NestedSamples):
+                    self.parameters = theta.columns[:-3].values
+                    theta = theta[theta.columns[:-3]].values
+                else:
+                    self.parameters = theta.columns[:-1].values
+                    theta = theta[theta.columns[:-1]].values
+        else:
+            weights = kwargs.pop('weights', np.ones(len(theta)))
 
         self.theta = theta
         self.sample_weights = weights
 
         self.n = (np.sum(weights)**2)/(np.sum(weights**2))
         theta_max = np.max(theta, axis=0)
         theta_min = np.min(theta, axis=0)
         a = ((self.n-2)*theta_max-theta_min)/(self.n-3)
         b = ((self.n-2)*theta_min-theta_max)/(self.n-3)
         self.theta_min = kwargs.pop('theta_min', b)
         self.theta_max = kwargs.pop('theta_max', a)
-        
+
         self.bw_method = kwargs.pop('bw_method', 'silverman')
 
     def generate_kde(self):
 
         r"""
         Function noramlises the input data into a standard normal parameter
         space and then generates a weighted KDE.
         """
+        theta = tf.convert_to_tensor(self.theta, dtype=tf.float32)
+        theta_min = tf.convert_to_tensor(self.theta_min, dtype=tf.float32)
+        theta_max = tf.convert_to_tensor(self.theta_max, dtype=tf.float32)
 
-        phi = _forward_transform(self.theta, self.theta_min, self.theta_max)
+        phi = _forward_transform(theta, theta_min, theta_max).numpy()
         mask = np.isfinite(phi).all(axis=-1)
         phi = phi[mask, :]
         weights_phi = self.sample_weights[mask]
         weights_phi /= weights_phi.sum()
 
         self.kde = gaussian_kde(
             phi.T, weights=self.sample_weights, bw_method=self.bw_method)
@@ -140,15 +171,18 @@
                 m = mu[:, i] + steps[i] @ (y[:i] - mu[:, :i]).T
                 y[i] = root_scalar(
                     lambda f:
                     (norm().cdf((f-m)/s[i])*self.kde.weights).sum()-x[i],
                     bracket=(mu[:, i].min()*2, mu[:, i].max()*2),
                     method='bisect').root
             transformed_samples.append(
-                _inverse_transform(y, self.theta_min, self.theta_max))
+                _inverse_transform(
+                    tf.convert_to_tensor(y, dtype=tf.float32),
+                    tf.convert_to_tensor(self.theta_min, dtype=tf.float32),
+                    tf.convert_to_tensor(self.theta_max, dtype=tf.float32)))
         transformed_samples = np.array(transformed_samples)
         return transformed_samples
 
     def sample(self, length=1000):
 
         r"""
 
@@ -162,15 +196,18 @@
 
             length: **int / default=1000**
                 | This should be an integer and is used to determine how many
                     samples are generated when calling the bijector.
 
         """
         x = self.kde.resample(length).T
-        return _inverse_transform(x, self.theta_min, self.theta_max)
+        return _inverse_transform(
+            tf.convert_to_tensor(x, dtype='float32'),
+            tf.convert_to_tensor(self.theta_min, dtype=tf.float32),
+            tf.convert_to_tensor(self.theta_max, dtype=tf.float32))
 
     def log_prob(self, params):
 
         """
         Function to caluclate the log-probability for a given KDE and
         set of parameters.
 
@@ -186,18 +223,20 @@
                     probability.
 
         """
         mins = self.theta_min.astype(np.float32)
         maxs = self.theta_max.astype(np.float32)
 
         transformed_x = _forward_transform(
-            params, mins, maxs)
+            tf.convert_to_tensor(params, dtype=tf.float32),
+            tf.convert_to_tensor(mins, dtype=tf.float32),
+            tf.convert_to_tensor(maxs, dtype=tf.float32)).numpy()
 
         transform_chain = tfb.Chain([
-            tfb.Invert(tfb.NormalCDF()), 
+            tfb.Invert(tfb.NormalCDF()),
             tfb.Scale(1/(maxs - mins)), tfb.Shift(-mins)])
 
         def norm_jac(y):
             return transform_chain.inverse_log_det_jacobian(
                 y, event_ndims=0).numpy()
 
         correction = norm_jac(transformed_x)
@@ -237,16 +276,17 @@
                     experiments/data sets. In this case samples and prior
                     samples should be reweighted prior to any training.
 
         """
 
         if prior is None:
             warnings.warn('Assuming prior is uniform!')
-            prior_logprob = np.prod([1/(self.theta_max[i] - self.theta_min[i])
-                                    for i in range(len(self.theta_min))])
+            prior_logprob = np.log(np.prod(
+                                   [1/(self.theta_max[i] - self.theta_min[i])
+                                    for i in range(len(self.theta_min))]))
         else:
             self.prior = margarine.kde.KDE(prior, prior_weights)
             self.prior.generate_kde()
             prior_logprob_func = self.prior.log_prob
             prior_logprob = prior_logprob_func(params)
 
         posterior_logprob = self.log_prob(params)
@@ -274,27 +314,27 @@
 
         r"""
 
         This function can be used to load a saved KDE. For example
 
         .. code:: python
 
-            from bayesstats.kde import KDE
+            from margarine.kde import KDE
 
             file = 'path/to/pickled/bijector.pkl'
             KDE_class = KDE.load(file)
 
         **Parameters:**
 
             filename: **string**
                 | Path to the saved KDE.
 
         """
 
         with open(filename, 'rb') as f:
             theta, sample_weights, kde = pickle.load(f)
 
-        kde_class = cls(theta, sample_weights)
+        kde_class = cls(theta, weights=sample_weights)
         kde_class.kde = kde
         kde_class(np.random.uniform(0, 1, size=(2, theta.shape[-1])))
 
         return kde_class
```

### Comparing `margarine-0.3.1/margarine/maf.py` & `margarine-1.0.0/margarine/clustered.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+from scipy.special import logsumexp
+from sklearn.cluster import KMeans
+from tensorflow import keras
+from margarine.maf import MAF
+import anesthetic
 import numpy as np
 import tensorflow as tf
-from tensorflow_probability import (bijectors as tfb, distributions as tfd)
-from margarine.processing import _forward_transform, _inverse_transform
-import pickle
 import warnings
-import margarine
+import pickle
 
 
-class MAF(object):
+class clusterMAF():
 
     r"""
 
-    This class is used to train, load and call instances of a bijector
-    built from a series of autoregressive neural networks.
+    This class is used to train, load and call a piecewise normalising flow
+    built from a set of masked autoregressive flows. The class
+    is essentially a wrapper around the MAF class with some additional
+    clustering functionality. This class has all the same
+    functionality as the MAF class and can be used in the same way.
 
     **Parameters:**
 
-        theta: **numpy array**
+        theta: **numpy array or anesthetic.samples**
             | The samples from the probability distribution that we require the
-                MAF to learn.
-
-        weights: **numpy array**
-            | The weights associated with the samples above.
+                MAF to learn. This can either be a numpy array or an anesthetic
+                NestedSamples or MCMCSamples object.
 
     **kwargs:**
 
+        weights: **numpy array / default=np.ones(len(theta))**
+            | The weights associated with the samples above. If an anesthetic
+                NestedSamples or MCMCSamples object is passed the code
+                draws the weights from this.
+
         number_networks: **int / default = 6**
             | The bijector is built by chaining a series of
                 autoregressive neural
                 networks together and this parameter is used to determine
                 how many networks there are in the chain.
 
         learning_rate: **float / default = 1e-3**
@@ -38,365 +46,418 @@
 
         hidden_layers: **list / default = [50, 50]**
             | The number of layers and number of nodes in each hidden layer for
                 each neural network. The default is two hidden layers with
                 50 nodes each and each network in the chain has the same hidden
                 layer structure.
 
-        theta_max: **numpy array**
-            | The true upper limits of the priors used to generate the samples
-                that we want the MAF to learn.
-
-        theta_min: **numpy array**
-            | As above but the true lower limits of the priors.
-
-
-    **Attributes:**
-
-    A list of some key attributes accessible to the user.
-
-        maf: **Instance of tfd.TransformedDistribution**
-            | By loading a trained instance of this class and accessing the
-                ``maf`` (masked autoregressive flow) attribute, which is an
-                instance of
-                ``tensorflow_probability.distributions.TransformedDistribution``,
-                the used can sample the trained MAF. e.g.
-
-                .. code:: python
-
-                    from ...maf import MAF
-
-                    file = '/trained_maf.pkl'
-                    bij = MAF.load(file)
-
-                    samples = bij.maf.sample(1000)
+        cluster_labels: **list / default = None**
+            | If clustering has been performed externally to margarine you can
+                provide a list of labels for the samples theta. The labels
+                should be integers from 0 to k corresponding to the cluster
+                that each sample is in.
+
+        cluster_number: **int / default = None**
+            | If clustering has been performed externally to margarine you
+                need to provide the number of clusters, k, alongside the
+                cluster labels.
+
+        parameters: **list of strings**
+            | A list of the relevant parameters to train on. Only needed
+                if theta is an anestehetic samples object. If not provided,
+                all parameters will be used.
 
-                It can also be used to calculate log probabilities via
-
-                .. code:: python
-
-                    log_prob = bij.log_prob(samples)
-
-                For more information on the attributes associated with
-                ``tensorflow_probability.distributions.TransformedDistribution``
-                see the tensorflow documentation.
-
-        theta_max: **numpy array**
-            | The true upper limits of the priors used to generate the samples
-                that we want the MAF to learn. If theta_max is not supplied as a
-                kwarg, then this is is an approximate estimate (for more info see
-                the ... paper).
-
-        theta_min: **numpy array**
-            | As above but for the true lower limits of the priors. If theta_max is
-                not supplied as a kwarg, then this is is an approximate estimate.
+    """
 
-        loss_history: **list**
-            | This list contains the value of the loss function at each epoch
-                during training.
+    def __init__(self, theta, **kwargs):
 
-    """
+        self.number_networks = kwargs.pop('number_networks', 6)
+        self.learning_rate = kwargs.pop('learning_rate', 1e-3)
+        self.hidden_layers = kwargs.pop('hidden_layers', [50, 50])
+        self.cluster_labels = kwargs.pop('cluster_labels', None)
+        self.cluster_number = kwargs.pop('cluster_number', None)
+        self.parameters = kwargs.pop('parameters', None)
+
+        if isinstance(theta, 
+                      (anesthetic.samples.NestedSamples, 
+                       anesthetic.samples.MCMCSamples)):
+            weights = theta.get_weights()
+            if self.parameters:
+                theta = theta[self.parameters].values
+            else:
+                if isinstance(theta, anesthetic.samples.NestedSamples):
+                    self.parameters = theta.columns[:-3].values
+                    theta = theta[theta.columns[:-3]].values
+                else:
+                    self.parameters = theta.columns[:-1].values
+                    theta = theta[theta.columns[:-1]].values
+        else:
+            weights = kwargs.pop('weights', np.ones(len(theta)))
 
-    def __init__(self, theta, weights, **kwargs):
-        self.n = (np.sum(weights)**2)/(np.sum(weights**2))
+        self.theta = theta
         self.sample_weights = weights
 
-        theta_max = np.max(theta, axis=0)
-        theta_min = np.min(theta, axis=0)
+        # needed for marginal stats
+        self.n = np.sum(self.sample_weights)**2 / \
+            np.sum(self.sample_weights**2)
+        theta_max = np.max(self.theta, axis=0)
+        theta_min = np.min(self.theta, axis=0)
         a = ((self.n-2)*theta_max-theta_min)/(self.n-3)
         b = ((self.n-2)*theta_min-theta_max)/(self.n-3)
-        self.theta_min = kwargs.pop('theta_min', b)
-        self.theta_max = kwargs.pop('theta_max', a)
-
-        self.theta = theta
-
-        self.number_networks = kwargs.pop('number_networks', 6)
-        self.learning_rate = kwargs.pop('learning_rate', 1e-3)
-        self.hidden_layers = kwargs.pop('hidden_layers', [50, 50])
+        self.theta_min = b
+        self.theta_max = a
 
         if type(self.number_networks) is not int:
             raise TypeError("'number_networks' must be an integer.")
-        if type(self.learning_rate) not in [int, float]:
-            raise TypeError("'learning_rate', must be a float.")
+        if not isinstance(self.learning_rate,
+                          (int, float,
+                           keras.optimizers.schedules.LearningRateSchedule)):
+            raise TypeError("'learning_rate', " +
+                            "must be an integer, float or keras scheduler.")
         if type(self.hidden_layers) is not list:
             raise TypeError("'hidden_layers' must be a list of integers.")
         else:
             for i in range(len(self.hidden_layers)):
                 if type(self.hidden_layers[i]) is not int:
                     raise TypeError(
                         "One or more valus in 'hidden_layers'" +
                         "is not an integer.")
 
-        self.mades = [tfb.AutoregressiveNetwork(params=2,
-                      hidden_units=self.hidden_layers, activation='tanh',
-                      input_order='random')
-                      for _ in range(self.number_networks)]
-
-        self.bij = tfb.Chain([
-            tfb.MaskedAutoregressiveFlow(made) for made in self.mades])
-
-        self.base = tfd.Blockwise(
-            [tfd.Normal(loc=0, scale=1)
-             for _ in range(len(theta_min))])
-        self.maf = tfd.TransformedDistribution(self.base, bijector=self.bij)
-
-        self.optimizer = tf.keras.optimizers.Adam(
-            learning_rate=self.learning_rate)
-
-    def _train_step(self, x, w, loss_type, prior_phi=None, prior_weights=None):
-
-        r"""
-        This function is used to calculate the loss value at each epoch and
-        adjust the weights and biases of the neural networks via the
-        optimizer algorithm.
-        """
-
-        with tf.GradientTape() as tape:
-            if loss_type == 'sum':
-                    loss = -tf.reduce_sum(w*self.maf.log_prob(x))
-            elif loss_type == 'mean':
-                    loss = -tf.reduce_mean(w*self.maf.log_prob(x))
-            gradients = tape.gradient(loss, self.maf.trainable_variables)
-            self.optimizer.apply_gradients(
-                zip(gradients,
-                    self.maf.trainable_variables))
-            return loss
+        mask = np.isfinite(theta).all(axis=-1)
+        self.theta = self.theta[mask]
+        self.sample_weights = self.sample_weights[mask]
+
+        if self.cluster_number is not None:
+            if self.cluster_labels is None:
+                raise ValueError("'cluster_labels' should be provided if " +
+                                 "'cluster_number' is specified.")
+        else:
+            if self.cluster_labels is not None:
+                raise ValueError("'cluster_number' should be provided if " +
+                                 "'cluster_labels' is specified.")
+
+        if self.cluster_number is not None:
+            if self.cluster_number % 1 != 0:
+                raise TypeError("'cluster_number' must be a whole number.")
+        if self.cluster_labels is not None:
+            if not isinstance(self.cluster_labels, (np.ndarray, list)):
+                raise TypeError("'cluster_labels' must be an array " +
+                                "or a list.")
+
+        if self.cluster_number is None:
+            # this code currently performs the clustering with
+            # kmeans but we could have anything here.
+            from sklearn.metrics import silhouette_score
+            ks = np.arange(2, 21)
+            losses = []
+            for k in ks:
+                kmeans = KMeans(k, random_state=0)
+                labels = kmeans.fit(self.theta).predict(self.theta)
+                losses.append(-silhouette_score(self.theta, labels))
+            losses = np.array(losses)
+            minimum_index = np.argmin(losses)
+            self.cluster_number = ks[minimum_index]
+
+            kmeans = KMeans(self.cluster_number, random_state=0)
+            self.cluster_labels = kmeans.fit(self.theta).predict(self.theta)
+
+        if self.cluster_number == 20:
+            warnings.warn("The number of clusters is 20. " +
+                          "This is the maximum " +
+                          "number of clusters that can be used. If you " +
+                          "require more clusters, please specify the " +
+                          "'cluster_number' kwarg. " +
+                          "margarine will continue " +
+                          "with 20 clusters.")
+
+        if np.array(list(self.cluster_labels)).dtype == 'float':
+            # convert cluster labels to integers
+            self.cluster_labels = self.cluster_labels.astype(int)
+        # count the number of times a cluster label appears in cluster_labels
+        self.cluster_count = np.bincount(self.cluster_labels)
+        # While loop to make sure clusters are not too small
+        while self.cluster_count.min() < 100:
+            warnings.warn("One or more clusters are too small " +
+                          "(n_cluster < 100). " +
+                          "Reducing the number of clusters by 1.")
+            minimum_index -= 1
+            self.cluster_number = ks[minimum_index]
+            kmeans = KMeans(self.cluster_number, random_state=0)
+            self.cluster_labels = kmeans.fit(self.theta).predict(self.theta)
+            self.cluster_count = np.bincount(self.cluster_labels)
+            if self.cluster_number == 2:
+                # break if two clusters
+                warnings.warn("The number of clusters is 2. This is the " +
+                              "minimum number of clusters that can be used. " +
+                              "Some clusters may be too small and the " +
+                              "train/test split may fail." +
+                              "Try running without clusting. ")
+                break
+
+        split_theta = []
+        split_sample_weights = []
+        for i in range(self.cluster_number):
+            split_theta.append(self.theta[self.cluster_labels == i])
+            split_sample_weights.append(
+                self.sample_weights[self.cluster_labels == i])
+
+        self.split_theta = split_theta
+        self.split_sample_weights = split_sample_weights
+
+        self.flow = []
+        for i in range(len(split_theta)):
+            self.flow.append(MAF(split_theta[i], 
+                                 weights=split_sample_weights[i],
+                                 number_networks=self.number_networks,
+                                 learning_rate=self.learning_rate,
+                                 hidden_layers=self.hidden_layers))
 
     def train(self, epochs=100, early_stop=False, loss_type='sum'):
-        r"""
 
-        This function is called to train the MAF once it has been
-        initialised. For example
+        r"""
+        This function is called to train the clusterMAF once it has been
+        initialised. It calls the `train()` function for each flow.
 
         .. code:: python
 
-            from ...maf import MAF
+            from margarine.clustered import clusterMAF
 
-            bij = MAF(theta, weights)
+            bij = clusterMAF(theta, weights=weights)
             bij.train()
 
         **Kwargs:**
 
             epochs: **int / default = 100**
                 | The number of iterations to train the neural networks for.
 
             early_stop: **boolean / default = False**
                 | Determines whether or not to implement an early stopping
                     algorithm or
                     train for the set number of epochs. If set to True then the
-                    algorithm will stop training when the
-                    fractional difference
-                    between the current loss
-                    and the average loss value over the
-                    preceeding 10 epochs is < 1e-6.
-
-        """
-        if type(epochs) is not int:
-            raise TypeError("'epochs' is not an integer.")
-        if type(early_stop) is not bool:
-            raise TypeError("'early_stop' must be a boolean.")
-
-        phi = _forward_transform(self.theta, self.theta_min, self.theta_max)
-
-        mask = np.isfinite(phi).all(axis=-1)
-        phi = phi[mask, :]
-        weights_phi = self.sample_weights[mask]
-        weights_phi /= weights_phi.sum()
-
-        phi = phi.astype('float32')
-        self.phi = phi.copy()
-        weights_phi = weights_phi.astype('float32')
-
-        self.loss_history = []
-        for i in range(epochs):
-            loss = self._train_step(phi, weights_phi, loss_type).numpy()
-            self.loss_history.append(loss)
-            if early_stop:
-                if len(self.loss_history) > 10:
-                    delta = (
-                        self.loss_history[-1] -
-                        np.mean(self.loss_history[-11:-1])) \
-                        / np.mean(self.loss_history[-11:-1])
-                    if np.abs(delta) < 1e-6:
-                        print('Early Stopped:' +
-                              ' (Loss[-1] - Mean(Loss[-11:-1]))' +
-                              '/Mean(Loss[-11:-1]) < 1e-6')
-                        break
-
-    def __call__(self, u):
-
-        r"""
-
-        This function is used when calling the MAF class to transform
-        samples from the unit hypercube to samples on the MAF.
-
-        **Parameters:**
-
-            u: **numpy array**
-                | Samples on the uniform hypercube.
-
-        """
-
-        x = _forward_transform(u)
-        x = self.bij(x.astype(np.float32)).numpy()
-        x = _inverse_transform(x, self.theta_min, self.theta_max)
-        mask = np.isfinite(x).all(axis=-1)
-        return x[mask, ...]
-
-    def sample(self, length=1000):
-
-        r"""
-
-        This function is used to generate samples on the MAF via the
-        MAF __call__ function.
-
-        **Kwargs:**
-
-            length: **int / default=1000**
-                | This should be an integer and is used to determine how many
-                    samples are generated when calling the MAF.
+                    algorithm will stop training when test loss has not
+                    improved for 2% of the requested epochs. At this point
+                    margarine will roll back to the best model and return this
+                    to the user.
+
+            loss_type: **string / default = 'sum'**
+                | Determines whether to use the sum or mean of the weighted
+                    log probabilities to calculate the loss function.
 
         """
-        if type(length) is not int:
-            raise TypeError("'length' must be an integer.")
 
-        u = np.random.uniform(0, 1, size=(length, self.theta.shape[-1]))
-        return self(u)
+        for i in range(len(self.flow)):
+            self.flow[i].train(epochs=epochs, early_stop=early_stop,
+                               loss_type=loss_type)
 
     def log_prob(self, params):
 
         """
-        Function to caluclate the log-probability for a given MAF and
+        Function to caluclate the log-probability for a given clusterMAF and
         set of parameters.
 
-        While the density estimator has its own built in log probability
+        While each density estimator has its own built in log probability
         function, a correction has to be applied for the transformation of
-        variables that is used to improve accuracy when learning. The
-        correction is implemented here.
+        variables that is used to improve accuracy when learning and we
+        have to sum probabilities over the series of flows. The
+        correction and the sum are implemented here.
 
         **Parameters:**
 
             params: **numpy array**
                 | The set of samples for which to calculate the log
                     probability.
 
         """
-        mins = self.theta_min.astype(np.float32)
-        maxs = self.theta_max.astype(np.float32)
 
-        transformed_x = _forward_transform(params, mins, maxs)
-
-        transform_chain = tfb.Chain([
-            tfb.Invert(tfb.NormalCDF()),
-            tfb.Scale(1/(maxs - mins)), tfb.Shift(-mins)])
-
-        def norm_jac(y):
-            return transform_chain.inverse_log_det_jacobian(
-                y, event_ndims=0).numpy()
-
-        correction = norm_jac(transformed_x)
-        logprob = (self.maf.log_prob(transformed_x).numpy() -
-                   np.sum(correction, axis=-1)).astype(np.float64)
+        # currently working with numpy not tensorflow
+        # nan repalacement with 0 difficult in tensorflow
+        logprob = []
+        for flow in self.flow:
+            probs = flow.log_prob(params).numpy()
+            for j in range(len(probs)):
+                if np.isnan(probs[j]):
+                    probs[j] = np.log(1e-300)
+            logprob.append(probs)
+        logprob = np.array(logprob)
+        print(logprob.shape)
+        logprob = logsumexp(logprob, axis=0)
 
         return logprob
 
-    def log_like(self, params, logevidence, prior=None, prior_weights=None):
+    def log_like(self, params, logevidence, prior_de=None):
 
         r"""
         This function should return the log-likelihood for a given set of
         parameters.
 
         It requires the logevidence from the original nested sampling run
         in order to do this and in the case that the prior is non-uniform
-        prior samples should be provided.
+        a trained prior density estimator should be provided.
 
         **Parameters:**
 
             params: **numpy array**
                 | The set of samples for which to calculate the log
                     probability.
 
             logevidence: **float**
                 | Should be the log-evidence from the full nested sampling
                     run with nuisance parameters.
 
-            prior: **numpy array/default=None**
-                | An array of prior samples corresponding to the prior. Default
-                    assumption is that the prior is uniform which is
-                    required if you want to combine likelihoods from different
-                    experiments/data sets. In this case samples and prior
-                    samples should be reweighted prior to any training.
+            prior_de: **margarine.maf.MAF / default=None**
+                | If the prior is non-uniform then a trained prior density
+                    estimator should be provided. Otherwise the prior
+                    is assumed to be uniform and the prior probability
+                    is calculated analytically from the minimum and maximum
+                    values of the parameters.
 
         """
 
-        if prior is None:
+        if prior_de is None:
             warnings.warn('Assuming prior is uniform!')
-            prior_logprob = np.prod([1/(self.theta_max[i] - self.theta_min[i])
-                                    for i in range(len(self.theta_min))])
+
+            n = (np.sum(self.sample_weights)**2) / \
+                (np.sum(self.sample_weights**2))
+
+            theta_max = np.max(self.theta, axis=0)
+            theta_min = np.min(self.theta, axis=0)
+            a = ((n-2)*theta_max-theta_min)/(n-3)
+            b = ((n-2)*theta_min-theta_max)/(n-3)
+            prior_logprob = np.log(
+                np.prod([1/(a - b)
+                         for i in range(len(b))]))
         else:
-            self.prior = margarine.maf.MAF(prior, prior_weights)
-            self.prior.train()
-            prior_logprob_func = self.prior.log_prob
-            prior_logprob = prior_logprob_func(params)
+            prior_logprob = prior_de.log_prob(params).numpy()
 
         posterior_logprob = self.log_prob(params)
 
-        loglike = posterior_logprob + logevidence - prior_logprob
+        loglike = posterior_logprob + prior_logprob - logevidence
 
         return loglike
 
+    @tf.function(jit_compile=True)
+    def __call__(self, u):
+
+        r"""
+
+        This function is used when calling the clusterMAF class to transform
+        samples from the unit hypercube to samples on the clusterMAF.
+
+        **Parameters:**
+
+            u: **numpy array**
+                | Samples on the uniform hypercube.
+
+        """
+
+        len_thetas = [len(self.split_theta[i])
+                      for i in range(len(self.split_theta))]
+        probabilities = [len_thetas[i]/np.sum(len_thetas)
+                         for i in range(len(self.split_theta))]
+        options = np.arange(0, self.cluster_number)
+        choice = np.random.choice(options,
+                                  p=probabilities, size=len(u))
+
+        totals = [len(choice[choice == options[i]])
+                  for i in range(len(options))]
+        totals = np.hstack([0, np.cumsum(totals)])
+
+        values = []
+        for i in range(len(options)):
+            x = self.flow[i](u[totals[i]:totals[i+1]])
+            values.append(x)
+
+        x = tf.concat(values, axis=0)
+        return x
+
+    def sample(self, length=1000):
+
+        r"""
+
+        This function is used to generate samples on the clusterMAF via the
+        clusterMAF __call__ function.
+
+        **Kwargs:**
+
+            length: **int / default=1000**
+                | This should be an integer and is used to determine how many
+                    samples are generated when calling the clusterMAF.
+
+        """
+
+        u = np.random.uniform(size=(length, self.theta.shape[-1]))
+        return self(u)
+
     def save(self, filename):
+
         r"""
 
-        This function can be used to save an instance of a trained MAF as
+        This function can be used to save an instance of
+        a trained clusterMAF as
         a pickled class so that it can be loaded and used in differnt scripts.
 
         **Parameters:**
 
             filename: **string**
                 | Path in which to save the pickled MAF.
 
         """
-        nn_weights = [made.get_weights() for made in self.mades]
+
+        nn_weights = {}
+        for i in range(self.cluster_number):
+            made = self.flow[i].mades
+            w = [m.get_weights() for m in made]
+            nn_weights[i] = w
+
         with open(filename, 'wb') as f:
             pickle.dump([self.theta,
-                         nn_weights,
-                         self.sample_weights,
-                         self.number_networks,
-                         self.hidden_layers,
-                         self.learning_rate], f)
+                        nn_weights,
+                        self.sample_weights,
+                        self.number_networks,
+                        self.hidden_layers,
+                        self.learning_rate,
+                        self.cluster_number,
+                        self.cluster_labels], f)
 
     @classmethod
     def load(cls, filename):
+
         r"""
 
         This function can be used to load a saved MAF. For example
 
         .. code:: python
 
-            from ...maf import MAF
+            from margarine.clustered import clusterMAF
 
             file = 'path/to/pickled/MAF.pkl'
-            bij = MAF.load(file)
+            bij = clusterMAF.load(file)
 
         **Parameters:**
 
             filename: **string**
                 | Path to the saved MAF.
 
         """
 
         with open(filename, 'rb') as f:
+            data = pickle.load(f)
             theta, nn_weights, \
                 sample_weights, \
                 number_networks, \
                 hidden_layers, \
-                learning_rate = pickle.load(f)
-
-        bijector = cls(
-            theta, sample_weights, number_networks=number_networks,
-            learning_rate=learning_rate, hidden_layers=hidden_layers)
-        bijector(np.random.uniform(0, 1, size=(len(theta), theta.shape[-1])))
-        for made, nn_weights in zip(bijector.mades, nn_weights):
-            made.set_weights(nn_weights)
+                learning_rate, \
+                cluster_number, \
+                labels = data
+
+        maf = cls(theta, weights=sample_weights,
+                  number_networks=number_networks,
+                  hidden_layers=hidden_layers,
+                  learning_rate=learning_rate,
+                  cluster_number=cluster_number,
+                  cluster_labels=labels)
+        maf(np.random.uniform(size=(1, theta.shape[-1])))
+        for j in range(len(maf.flow)):
+            for made, nnw in zip(maf.flow[j].mades, nn_weights[j]):
+                made.set_weights(nnw)
 
-        return bijector
+        return maf
```

### Comparing `margarine-0.3.1/margarine/marginal_stats.py` & `margarine-1.0.0/margarine/marginal_stats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import tensorflow as tf
 import numpy as np
-from margarine.processing import _forward_transform
 from tensorflow_probability import distributions as tfd
-import margarine
-import warnings
 import pandas as pd
 from margarine.maf import MAF
 
 
 class calculate(object):
 
     r"""
@@ -15,166 +11,146 @@
     This class, once initalised with a trained MAF or KDE and samples,
     can be used to calculate marginal KL divergences and
     bayesian dimensionalities.
 
     **Paramesters:**
 
         de: **instance of MAF class or KDE class**
-            | This should be a loaded and trained instance of a MAF or KDE.
-                Bijectors can be loaded like so
+            | This should be a loaded and trained instance of a MAF, clusterMAF
+                or KDE.Bijectors can be loaded like so
 
                 .. code:: python
 
                     from margarine.maf import MAF
                     from margarine.kde import KDE
+                    from margarine.clustered import clusterMAF
 
                     file = '/trained_maf.pkl'
                     maf = MAF.load(file)
 
                     file = '/trained_kde.pkl'
                     kde = KDE.load(file)
 
+                    file = '/trained_clustered_maf.pkl'
+                    clustered_maf = clusterMAF.load(file)
+
         samples: **numpy array**
             | This should be the output of the bijector when called to generate
                 a set of samples from the replicated probability
                 distribution. e.g. after loading a trained MAF we would pass
 
                 .. code:: python
 
                     u = np.random.uniform(0, 1, size=(10000, 5))
                     prior_limits = np.array([[0]*5, [1]*5])
                     samples = maf(u, prior_limits)
 
     **Kwargs:**
 
-        prior_samples: **numpy array / default=None**
-            | Can be provided if the prior is non-uniform and will be
-                used to generate a prior density estimator to calcualte
-                prior log-probabilities. If not provided the prior is
-                assumed to be uniform.
-
-        prior_weights: **numpy array / default=None**
-            | Weights associated with the above prior samples.
+        prior_de: **instance of MAF class, clusterMAF class or KDE class**
+            | This should be a loaded and trained instance of a MAF, clusterMAF
+                or KDE for the prior.
+                If not provided, a uniform prior will be used.
 
     """
 
     def __init__(self, de, **kwargs):
 
         self.de = de
+
         self.theta = self.de.theta
         self.theta_weights = self.de.sample_weights
+        self.theta_min = self.de.theta_min
+        self.theta_max = self.de.theta_max
+
+        if isinstance(self.de, MAF):
+            self.theta_weights = self.theta_weights.numpy()
+            self.theta_min = self.theta_min.numpy()
+            self.theta_max = self.theta_max.numpy()
+
         self.samples = self.de.sample(len(self.theta))
 
         self.prior_de = kwargs.pop('prior_de', None)
-        self.prior_samples = kwargs.pop('prior_samples', None)
-        self.prior_weights = kwargs.pop('prior_weights', None)
-
-        if self.prior_samples is None:
-            warnings.warn('If prior samples are not provided the prior is ' +
-                'assumed to be uniform and the posterior samples are ' +
-                'are assumed to be from the same uniform space.')
-        else:
-            if self.prior_weights is None:
-                warnings.warn('No prior weights have been provided. ' +
-                    'Assuming there are none.')
 
     def statistics(self):
 
+        """
+        Calculate marginal bayesian KL divergence and dimensionality with
+        approximate errors.
+        """
+
         def mask_arr(arr):
             return arr[np.isfinite(arr)], np.isfinite(arr)
 
-        min = self.de.theta_min
-        max = self.de.theta_max
+        logprob = self.de.log_prob(self.samples)
+        theta_logprob = self.de.log_prob(self.theta)
 
-        if isinstance(self.de, margarine.kde.KDE):
-            logprob_func = self.de.log_prob
-            logprob = logprob_func(self.samples)
-            theta_logprob = logprob_func(self.theta)
-        elif isinstance(self.de, margarine.maf.MAF):
-            logprob_func = self.de.log_prob
-            logprob = logprob_func(self.samples)
-            theta_logprob = logprob_func(self.theta)
+        if isinstance(self.de, MAF):
+            logprob = logprob.numpy()
+            theta_logprob = theta_logprob.numpy()
 
         args = np.argsort(theta_logprob)
         self.theta_weights = self.theta_weights[args]
         theta_logprob = theta_logprob[args]
 
         deargs = np.argsort(logprob)
         logprob = logprob[deargs]
         wde = [np.sum(self.theta_weights)/len(logprob)]*len(logprob)
         logprob = np.interp(
             np.cumsum(self.theta_weights), np.cumsum(wde), logprob)
 
         mid_point = np.log((np.exp(logprob) + np.exp(theta_logprob))/2)
 
-        if self.prior_samples is None:
+        if self.prior_de is None:
             self.base = tfd.Blockwise(
-                [tfd.Uniform(self.de.theta_min[i], self.de.theta_max[i])
-                for i in range(self.samples.shape[-1])])
+                [tfd.Uniform(self.theta_min[i], self.theta_max[i])
+                 for i in range(self.samples.shape[-1])])
             prior = self.base.sample(len(self.theta)).numpy()
 
             theta_base_logprob = self.base.log_prob(self.theta).numpy()
-
             base_logprob = self.base.log_prob(prior).numpy()
-            prior_wde = [np.sum(self.theta_weights)/len(base_logprob)]*len(base_logprob)
+
+            prior_wde = [np.sum(self.theta_weights)/len(base_logprob)] * \
+                len(base_logprob)
 
             base_logprob = base_logprob[deargs]
             base_logprob = np.interp(
-                np.cumsum(self.theta_weights), np.cumsum(prior_wde), base_logprob)
+                np.cumsum(self.theta_weights), np.cumsum(prior_wde),
+                base_logprob)
 
             theta_base_logprob = theta_base_logprob[args]
         elif self.prior_de is not None:
-            if isinstance(self.prior_de, margarine.kde.KDE):
-                self.base = self.prior_de.copy()
-                base_logprob_func = self.base.log_prob
-                de_prior_samples = self.base.sample(len(self.theta))
-                theta_base_logprob = base_logprob_func(self.prior_samples)
-                base_logprob = base_logprob_func(self.theta)
-            elif isinstance(self.prior_de, margarine.maf.MAF):
-                self.base = self.prior_de.copy()
-                base_logprob_func = self.base.log_prob
-                de_prior_samples = self.base.sample(len(self.theta))
-                theta_base_logprob = base_logprob_func(self.prior_samples)
-                base_logprob = base_logprob_func(self.theta)
-        else:
-            if isinstance(self.de, margarine.kde.KDE):
-                self.base = margarine.kde.KDE(
-                    self.prior_samples, self.prior_weights)
-                self.base.generate_kde()
-                base_logprob_func = self.base.log_prob
-                de_prior_samples = self.base.sample(len(self.theta))
-                theta_base_logprob = base_logprob_func(self.prior_samples)
-                base_logprob = base_logprob_func(de_prior_samples)
-            elif isinstance(self.de, margarine.maf.MAF):
-                self.base = MAF(
-                    self.prior_samples, self.prior_weights)
-                self.base.train(epochs=250)
-                base_logprob_func = self.base.log_prob
-                de_prior_samples = self.base.sample(len(self.theta))
-                theta_base_logprob = base_logprob_func(self.prior_samples)
-                base_logprob = base_logprob_func(de_prior_samples)
+            self.base = self.prior_de.copy()
+            de_prior_samples = self.base.sample(len(self.theta))
+            theta_base_logprob = self.base.log_prob(de_prior_samples)
+            base_logprob = self.base.log_prob(self.theta)
+
+            if isinstance(self.prior_de, MAF):
+                theta_base_logprob = theta_base_logprob.numpy()
+                base_logprob = base_logprob.numpy()
 
             base_logprob = base_logprob[deargs]
             base_logprob = np.interp(
                 np.cumsum(self.theta_weights), np.cumsum(wde), base_logprob)
 
             base_args = np.argsort(theta_base_logprob)
             theta_base_logprob = theta_base_logprob[base_args]
-            prior_weights = np.cumsum(self.prior_weights[base_args])
+            prior_weights = np.cumsum(self.prior_de.sample_weights[base_args])
 
-            prior_weights = (np.cumsum(self.theta_weights).max()-
-                np.cumsum(self.theta_weights).min())*(prior_weights -
-                prior_weights.min())/ \
-                (prior_weights.max() - prior_weights.min()) + \
+            prior_weights = (np.cumsum(self.theta_weights).max() -
+                             np.cumsum(self.theta_weights).min()) * \
+                            (prior_weights - prior_weights.min()) / \
+                            (prior_weights.max() - prior_weights.min()) + \
                 np.cumsum(self.theta_weights).min()
 
             theta_base_logprob = np.interp(np.cumsum(self.theta_weights),
-                prior_weights, theta_base_logprob)
+                                           prior_weights, theta_base_logprob)
 
-        midbasepoint = np.log((np.exp(base_logprob) + np.exp(theta_base_logprob))/2)
+        midbasepoint = np.log((np.exp(base_logprob) +
+                               np.exp(theta_base_logprob))/2)
 
         mid_logL, mask = mask_arr(mid_point - midbasepoint)
         midkl = np.average(mid_logL, weights=self.theta_weights[mask])
         midbd = 2*np.cov(mid_logL, aweights=self.theta_weights[mask])
         de_logL, mask = mask_arr(logprob - base_logprob)
         dekl = np.average(de_logL, weights=self.theta_weights[mask])
         debd = 2*np.cov(de_logL, aweights=self.theta_weights[mask])
@@ -182,15 +158,15 @@
         thetakl = np.average(theta_logL, weights=self.theta_weights[mask])
         thetabd = 2*np.cov(theta_logL, aweights=self.theta_weights[mask])
 
         kl_array = np.sort([midkl, dekl, thetakl])
         bd_array = np.sort([midbd, debd, thetabd])
 
         results_dict = {'Statistic': ['KL Divergence', 'BMD'],
-            'Value': [kl_array[1], bd_array[1]],
-            'Lower Bound': [kl_array[0], bd_array[0]],
-            'Upper Bound': [kl_array[2], bd_array[2]]}
+                        'Value': [kl_array[1], bd_array[1]],
+                        'Lower Bound': [kl_array[0], bd_array[0]],
+                        'Upper Bound': [kl_array[2], bd_array[2]]}
 
         results = pd.DataFrame(results_dict)
         results.set_index('Statistic', inplace=True)
 
         return results
```

### Comparing `margarine-0.3.1/margarine.egg-info/PKG-INFO` & `margarine-1.0.0/margarine.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margarine
-Version: 0.3.1
+Version: 1.0.0
 Summary: margarine: Posterior Sampling and Marginal Bayesian Statistics
 Home-page: https://github.com/htjb/margarine
 Author: Harry T. J. Bevins
 Author-email: htjb2@cam.ac.uk
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -23,15 +23,15 @@
 ================================================================
 
 Introduction
 ------------
 
 :margarine: Marginal Bayesian Statistics
 :Authors: Harry T.J. Bevins
-:Version: 0.3.0
+:Version: 1.0.0
 :Homepage:  https://github.com/htjb/margarine
 :Documentation: https://margarine.readthedocs.io/
 
 .. image:: https://readthedocs.org/projects/margarine/badge/?version=latest
   :target: https://margarine.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
@@ -88,15 +88,17 @@
 --------------------
 
 The software is available on the MIT licence.
 
 If you use the code for academic purposes we request that you cite the following
 `paper <https://ui.adsabs.harvard.edu/abs/2022arXiv220512841B/abstract>`__ and
 the `MaxEnt22 proceedings <https://ui.adsabs.harvard.edu/search/p_=0&q=author%3A%22Bevins%2C%20H.%20T.%20J.%22&sort=date%20desc%2C%20bibcode%20desc>`__
-for which you can use the following bibtex
+If you use the clustering implementation please cite the following
+`prepring <https://arxiv.org/abs/2305.02930>`__.
+You can use the following bibtex
 
 .. code:: bibtex
 
     @ARTICLE{2022arXiv220512841B,
          author = {{Bevins}, Harry T.~J. and {Handley}, William J. and {Lemos}, Pablo and {Sims}, Peter H. and {de Lera Acedo}, Eloy and {Fialkov}, Anastasia and {Alsing}, Justin},
           title = "{Removing the fat from your posterior samples with margarine}",
         journal = {arXiv e-prints},
@@ -128,14 +130,36 @@
   archivePrefix = {arXiv},
        eprint = {2207.11457},
   primaryClass = {astro-ph.CO},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2022arXiv220711457B},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
   }
 
+and
+
+.. code:: bibtex
+
+  @ARTICLE{2023arXiv230502930B,
+        author = {{Bevins}, Harry and {Handley}, Will},
+          title = "{Piecewise Normalizing Flows}",
+        journal = {arXiv e-prints},
+      keywords = {Statistics - Machine Learning, Computer Science - Machine Learning},
+          year = 2023,
+          month = may,
+            eid = {arXiv:2305.02930},
+          pages = {arXiv:2305.02930},
+            doi = {10.48550/arXiv.2305.02930},
+  archivePrefix = {arXiv},
+        eprint = {2305.02930},
+  primaryClass = {stat.ML},
+        adsurl = {https://ui.adsabs.harvard.edu/abs/2023arXiv230502930B},
+        adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+  }
+
+
 Requirements
 ------------
 
 The code requires the following packages to run:
 
 - `numpy <https://pypi.org/project/numpy/>`__
 - `tensorflow <https://pypi.org/project/tensorflow/>`__
```

### Comparing `margarine-0.3.1/setup.py` & `margarine-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         if short:
             return f.readlines()[1].strip()
         else:
             return f.read()
 
 setup(
     name='margarine',
-    version='0.3.1',
+    version='1.0.0',
     description='margarine: Posterior Sampling and Marginal Bayesian Statistics',
     long_description=readme(),
     author='Harry T. J. Bevins',
     author_email='htjb2@cam.ac.uk',
     url='https://github.com/htjb/margarine',
     packages=find_packages(),
     install_requires=['numpy', 'tensorflow', 'tensorflow_probability', 'scipy', 'pandas'],
```

