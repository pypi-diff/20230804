# Comparing `tmp/engression-0.0.1.tar.gz` & `tmp/engression-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engression-0.0.1.tar", last modified: Tue Jul  4 07:09:22 2023, max compression
+gzip compressed data, was "engression-0.1.0.tar", last modified: Fri Aug  4 12:08:46 2023, max compression
```

## Comparing `engression-0.0.1.tar` & `engression-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-04 07:09:22.821675 engression-0.0.1/
--rw-r--r--   0 shenxi   (571559) staff       (20)     2377 2023-07-04 07:09:22.821554 engression-0.0.1/PKG-INFO
--rw-r--r--   0 shenxi   (571559) staff       (20)     2117 2023-07-04 07:06:20.000000 engression-0.0.1/README.md
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-04 07:09:22.820129 engression-0.0.1/engression/
--rw-r--r--   0 shenxi   (571559) staff       (20)      365 2023-07-02 07:57:11.000000 engression-0.0.1/engression/__init__.py
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-04 07:09:22.821290 engression-0.0.1/engression/data/
--rw-r--r--   0 shenxi   (571559) staff       (20)        0 2023-07-01 15:22:34.000000 engression-0.0.1/engression/data/__init__.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     1980 2023-07-01 15:22:34.000000 engression-0.0.1/engression/data/loader.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     2673 2023-07-01 15:22:34.000000 engression-0.0.1/engression/data/simulator.py
--rw-r--r--   0 shenxi   (571559) staff       (20)    17701 2023-07-03 08:33:47.000000 engression-0.0.1/engression/engression.py
--rw-r--r--   0 shenxi   (571559) staff       (20)    12725 2023-07-02 07:57:03.000000 engression-0.0.1/engression/engression_bagged.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     2026 2023-07-02 12:42:28.000000 engression-0.0.1/engression/loss_func.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     6999 2023-07-02 12:36:08.000000 engression-0.0.1/engression/models.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     1910 2023-07-02 13:49:25.000000 engression-0.0.1/engression/utils.py
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-04 07:09:22.820829 engression-0.0.1/engression.egg-info/
--rw-r--r--   0 shenxi   (571559) staff       (20)     2377 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/PKG-INFO
--rw-r--r--   0 shenxi   (571559) staff       (20)      415 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/SOURCES.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)        1 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/dependency_links.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       23 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/requires.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       11 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/top_level.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       38 2023-07-04 07:09:22.821713 engression-0.0.1/setup.cfg
--rw-r--r--   0 shenxi   (571559) staff       (20)      599 2023-07-04 07:09:04.000000 engression-0.0.1/setup.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-04 12:08:46.120067 engression-0.1.0/
+-rw-r--r--   0 shenxi   (571559) staff       (20)     1522 2023-07-06 08:06:16.000000 engression-0.1.0/LICENSE
+-rw-r--r--   0 shenxi   (571559) staff       (20)     3192 2023-08-04 12:08:46.119933 engression-0.1.0/PKG-INFO
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2876 2023-08-04 10:06:11.000000 engression-0.1.0/README.md
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-04 12:08:46.118685 engression-0.1.0/engression/
+-rw-r--r--   0 shenxi   (571559) staff       (20)      363 2023-08-01 07:59:51.000000 engression-0.1.0/engression/__init__.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-04 12:08:46.119778 engression-0.1.0/engression/data/
+-rw-r--r--   0 shenxi   (571559) staff       (20)        0 2023-07-01 15:22:34.000000 engression-0.1.0/engression/data/__init__.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     1980 2023-07-01 15:22:34.000000 engression-0.1.0/engression/data/loader.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2673 2023-07-01 15:22:34.000000 engression-0.1.0/engression/data/simulator.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)    18122 2023-08-04 11:51:17.000000 engression-0.1.0/engression/engression.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)    17650 2023-08-04 12:01:31.000000 engression-0.1.0/engression/engression_bagged.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2354 2023-07-24 19:22:24.000000 engression-0.1.0/engression/loss_func.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     6430 2023-07-24 19:22:41.000000 engression-0.1.0/engression/models.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     1910 2023-07-02 13:49:25.000000 engression-0.1.0/engression/utils.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-04 12:08:46.119431 engression-0.1.0/engression.egg-info/
+-rw-r--r--   0 shenxi   (571559) staff       (20)     3192 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/PKG-INFO
+-rw-r--r--   0 shenxi   (571559) staff       (20)      423 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/SOURCES.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)        1 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/dependency_links.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       23 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/requires.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       11 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/top_level.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       38 2023-08-04 12:08:46.120111 engression-0.1.0/setup.cfg
+-rw-r--r--   0 shenxi   (571559) staff       (20)      633 2023-08-04 12:08:01.000000 engression-0.1.0/setup.py
```

### Comparing `engression-0.0.1/PKG-INFO` & `engression-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-Metadata-Version: 2.1
-Name: engression
-Version: 0.0.1
-Summary: Engression
-Home-page: https://github.com/xwshen51/engression
-Author: Xinwei Shen
-Author-email: xinwei.shen@stat.math.ethz.ch
-License: BSD 3-Clause License
-Description-Content-Type: text/markdown
-
 # Engression
 
-Engression is a nonlinear regression methodology proposed in the paper "[*Engression: Extrapolation for Nonlinear Regression?*](https://arxiv.org/abs/2307.00835)" by Xinwei Shen and Nicolai Meinshausen. 
-This directory contains the Python implementation of engression.
+Engression is a nonlinear regression methodology proposed in the paper "[*Engression: Extrapolation for Nonlinear Regression?*](https://arxiv.org/abs/2307.00835)" by Xinwei Shen and Nicolai Meinshausen. This directory contains the Python implementation of engression.
+
+Consider targets $Y\in\mathbb{R}^k$ and predictors $X\in\mathbb{R}^d$; both variables can be univariate or multivariate. Engression can be used to 
+* estimate the conditional mean $\mathbb{E}[Y|X=x]$ (as in least-squares regression), 
+* estimate the conditional quantiles of $Y$ given $X=x$ (as in quantile regression), and 
+* sample from the fitted conditional distribution of $Y$ given $X=x$ (as a generative model).
+
+The results in the paper show the advantages of engression over existing regression approaches in terms of extrapolation. 
+
 
 ## Installation
 The latest release of the Python package can be installed through pip:
 ```sh
 pip install engression
 ```
 
@@ -26,15 +23,15 @@
 ```
 
 
 ## Usage Example
 
 ### Python
 
-Below is one simple demonstration. See [this tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_simu.ipynb) for more details on simulated data and [this tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_air.ipynb) for a real data example.
+Below is one simple demonstration. See [this tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_simu.ipynb) for more details on simulated data and [this tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_air.ipynb) for a real data example. We demonstrate in [another tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_bag.ipynb) how to fit a bagged engression model, which also helps with hyperparameter tuning.
 ```python
 from engression import engression
 from engression.data.simulator import preanm_simulator
 
 ## Simulate data
 x, y = preanm_simulator("square", n=10000, x_lower=0, x_upper=2, noise_std=1, train=True, device=device)
 x_eval, y_eval_med, y_eval_mean = preanm_simulator("square", n=1000, x_lower=0, x_upper=4, noise_std=1, train=False, device=device)
@@ -52,8 +49,8 @@
 y_pred_mean = engressor.predict(x_eval, target="mean") ## for the conditional mean
 y_pred_med = engressor.predict(x_eval, target="median") ## for the conditional median
 y_pred_quant = engressor.predict(x_eval, target=[0.025, 0.5, 0.975]) ## for the conditional 2.5% and 97.5% quantiles
 ```
 
 
 ## Contact information
-If you meet any problems with the code, please submit an issue or contact [Xinwei Shen](mailto:xinwei.shen@stat.math.ethz.ch).
+If you meet any problems with the code, please submit an issue or contact [Xinwei Shen](mailto:xinwei.shen@stat.math.ethz.ch).
```

### Comparing `engression-0.0.1/engression/data/loader.py` & `engression-0.1.0/engression/data/loader.py`

 * *Files identical despite different names*

### Comparing `engression-0.0.1/engression/data/simulator.py` & `engression-0.1.0/engression/data/simulator.py`

 * *Files identical despite different names*

### Comparing `engression-0.0.1/engression/engression.py` & `engression-0.1.0/engression/engression.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,47 +3,83 @@
 
 from .loss_func import *
 from .models import StoNet
 from .data.loader import make_dataloader
 from .utils import *
 
 
+def engression(x, y, 
+               num_layer=2, hidden_dim=100, noise_dim=100,
+               lr=0.001, num_epoches=500, batch_size=None, 
+               print_every_nepoch=100, print_times_per_epoch=1,
+               device="cpu", standardize=True, verbose=True): 
+    """This function fits an engression model to the data. It allows multivariate predictors and response variables. Variables are per default internally standardized (training with standardized data, while predictions and evaluations are on original scale).
+
+    Args:
+        x (torch.Tensor): training data of predictors.
+        y (torch.Tensor): training data of responses.
+        num_layer (int, optional): number of layers. Defaults to 2.
+        hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
+        noise_dim (int, optional): noise dimension. Defaults to 100.
+        lr (float, optional): learning rate. Defaults to 0.001.
+        num_epoches (int, optional): number of epochs. Defaults to 500.
+        batch_size (int, optional): batch size. Defaults to None.
+        print_every_nepoch (int, optional): print losses every print_every_nepoch number of epochs. Defaults to 100.
+        print_times_per_epoch (int, optional): print losses for print_times_per_epoch times per epoch. Defaults to 1.
+        device (str, torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "gpu", "cuda"].
+        standardize (bool, optional):  whether to standardize data during training. Defaults to True.
+        verbose (bool, optional): whether to print losses and info. Defaults to True.
+
+    Returns:
+        Engressor object: a fitted engression model.
+    """
+    engressor = Engressor(in_dim=x.shape[1], out_dim=y.shape[1], num_layer=num_layer, hidden_dim=hidden_dim, noise_dim=noise_dim, 
+                          lr=lr, num_epoches=num_epoches, batch_size=batch_size, standardize=standardize, device=device)
+    engressor.train(x, y, num_epoches=num_epoches, batch_size=batch_size, 
+                    print_every_nepoch=print_every_nepoch, print_times_per_epoch=print_times_per_epoch, 
+                    standardize=standardize, verbose=verbose)
+    return engressor
+
+
 class Engressor(object):
 
     def __init__(self, 
                  in_dim, out_dim, num_layer=2, hidden_dim=100, noise_dim=100,
-                 lr=0.001, num_epoches=500, batch_size=None, device="cpu", standardize=True): 
-        """Engressor class
+                 lr=0.001, num_epoches=500, batch_size=None, standardize=True, 
+                 device="cpu", check_device=True): 
+        """Engressor class.
 
         Args:
             in_dim (int): input dimension
             out_dim (int): output dimension
             num_layer (int, optional): number of layers. Defaults to 2.
             hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
             noise_dim (int, optional): noise dimension. Defaults to 100.
             lr (float, optional): learning rate. Defaults to 0.001.
             num_epoches (int, optional): number of epoches. Defaults to 500.
             batch_size (int, optional): batch size. Defaults to None, referring to the full batch.
+            standardize (bool, optional): whether to standardize data during training. Defaults to True.
             device (str or torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "gpu", "cuda"].
-            standardize (bool, optional): whether to standardize data for training. Defaults to True.
+            check_device (bool, optional): whether to check the device. Defaults to True.
         """
         super().__init__()
         self.num_layer = num_layer
         self.hidden_dim = hidden_dim
         self.noise_dim = noise_dim
         self.lr = lr
         self.num_epoches = num_epoches
         self.batch_size = batch_size
         if isinstance(device, str):
             if device == "gpu" or device == "cuda":
                 device = torch.device("cuda")
             else:
                 device = torch.device(device)
         self.device = device
-        check_for_gpu(self.device)
+        if check_device:
+            check_for_gpu(self.device)
         self.standardize = standardize
         self.x_mean = None
         self.x_std = None
         self.y_mean = None
         self.y_std = None
         
         self.model = StoNet(in_dim, out_dim, num_layer, hidden_dim, noise_dim).to(self.device)
@@ -68,15 +104,14 @@
               "\t learning rate: {}\n".format(self.lr) +
               "\t standardization: {}\n".format(self.standardize) +
               "\t training mode: {}\n".format(self.model.training) +
               "\t device: {}\n".format(self.device))
         print("Training loss (original scale):\n" +
               "\t energy-loss: {:.2f}, \n\tE(|Y-Yhat|): {:.2f}, \n\tE(|Yhat-Yhat'|): {:.2f}".format(
                   self.tr_loss[0], self.tr_loss[1], self.tr_loss[2]))
-
         
     def _standardize_data_and_record_stats(self, x, y):
         """Standardize the data and record the mean and standard deviation of the training data.
 
         Args:
             x (torch.Tensor): training data of predictors.
             y (torch.Tensor): training data of responses.
@@ -128,41 +163,42 @@
         else:
             if self.standardize:
                 return x * self.x_std + self.x_mean, y * self.y_std + self.y_mean
             else:
                 return x, y
         
     def train(self, x, y, num_epoches=None, batch_size=512, print_every_nepoch=100, print_times_per_epoch=1, standardize=True, verbose=True):
-        """Training function.
+        """Fit the model.
 
         Args:
             x (torch.Tensor): training data of predictors.
             y (torch.Tensor): trainging data of responses.
             num_epoches (int, optional): number of training epochs. Defaults to None.
             batch_size (int, optional): batch size for mini-batch SGD. Defaults to 512.
             print_every_nepoch (int, optional): print losses every print_every_nepoch number of epochs. Defaults to 100.
             print_times_per_epoch (int, optional): print losses for print_times_per_epoch times per epoch. Defaults to 1.
-            standardize (bool, optional): standardize the data. Defaults to True.
+            standardize (bool, optional): whether to standardize the data. Defaults to True.
             verbose (bool, optional): whether to print losses and info. Defaults to True.
         """
         self.train_mode()
         if num_epoches is None:
             num_epoches = self.num_epoches
         if batch_size is None:
             batch_size = self.batch_size
         if standardize:
             self.standardize = standardize
             
         x = vectorize(x)
         y = vectorize(y)
         x = x.to(self.device)
         y = y.to(self.device)
-        if self.standardize and verbose: 
-            print("Data is standardized for training only; the printed training losses are on the standardized scale. \n" +
-                  "However during evaluation, the predictions, evaluation metrics, and plots will be on the original scale.\n")
+        if self.standardize:
+            if verbose:
+                print("Data is standardized for training only; the printed training losses are on the standardized scale. \n" +
+                    "However during evaluation, the predictions, evaluation metrics, and plots will be on the original scale.\n")
             x, y = self._standardize_data_and_record_stats(x, y)
         
         if batch_size >= x.size(0)//2:
             if verbose:
                 print("Batch is larger than half of the sample size. Training based on full-batch gradient descent.")
             self.batch_size = x.size(0)
             for epoch_idx in range(num_epoches):
@@ -207,16 +243,16 @@
                 "\n-- consider training for more epochs or adjusting hyperparameters if there is a mismatch ")
     
     def predict(self, x, target="mean", sample_size=100):
         """Point prediction.
 
         Args:
             x (torch.Tensor): data of predictors.
-            target (str or float or list, optional): single-valued functional to predict. float refers to the quantiles. Defaults to ["mean"].
-            sample_size (int, optional): sample sizes for each x. Defaults to 100.
+            target (str or float or list, optional): a quantity of interest to predict. float refers to the quantiles. Defaults to "mean".
+            sample_size (int, optional): generated sample sizes for each x. Defaults to 100.
 
         Returns:
             torch.Tensor or list of torch.Tensor: point predictions.
         """
         self.eval_mode()  
         x = vectorize(x)
         x = x.to(self.device)
@@ -226,21 +262,21 @@
         return y_pred
     
     def sample(self, x, sample_size=100, expand_dim=True):
         """Sample new response data.
 
         Args:
             x (torch.Tensor): test data of predictors.
-            target (str or float or list, optional): single-valued functional to predict. float refers to the quantiles. Defaults to ["mean"].
-            sample_size (int, optional): sample sizes for each x. Defaults to 100.
+            sample_size (int, optional): generated sample sizes for each x. Defaults to 100.
+            expand_dim (bool, optional): whether to expand the sample dimension. Defaults to True.
 
         Returns:
-            torch.Tensor or list of torch.Tensor: samples.
-                - [:,:,i] gives the i-th sample of all x.
-                - [i,:,:] gives all samples of x_i.
+            torch.Tensor of shape (data_size, response_dim, sample_size).
+                - [:,:,i] consists of the i-th sample of all x.
+                - [i,:,:] consists of all samples of x_i.
         """
         self.eval_mode()
         x = vectorize(x)
         x = x.to(self.device)
         x = self.standardize_data(x)
         y_samples = self.model.sample(x, sample_size, expand_dim=expand_dim)
         y_samples = self.unstandardize_data(y_samples)
@@ -249,15 +285,15 @@
     def eval_loss(self, x, y, loss_type="l2", sample_size=None, verbose=False):
         """Compute the loss for evaluation.
 
         Args:
             x (torch.Tensor): data of predictors.
             y (torch.Tensor): data of responses.
             loss_type (str, optional): loss type. Defaults to "l2". Choices: ["l2", "l1", "energy", "cor"].
-            sample_size (int, optional): sample sizes for each x. Defaults to 100.
+            sample_size (int, optional): generated sample sizes for each x. Defaults to 100.
         
         Returns:
             float: evaluation loss.
         """
         if sample_size is None:
             sample_size = 2 if loss_type == "energy" else 100
         self.eval_mode()
@@ -293,15 +329,15 @@
             x_te (torch.Tensor): test data of predictors
             y_te (torch.Tensor): test data of responses
             x_tr (torch.Tensor): training data of predictors
             y_tr (torch.Tensor): training data of responses
             x_idx (int, optional): index of the predictor to plot (if there are multiple). Defaults to 0.
             y_idx (int, optional): index of the response to plot (if there are multiple). Defaults to 0.
             target (str or float, optional): target quantity. Defaults to "mean". Choice: ["mean", "median", "sample", float].
-            sample_size (int, optional): sample sizes for each x. Defaults to 100.
+            sample_size (int, optional): generated sample sizes for each x. Defaults to 100.
             save_dir (str, optional): directory to save the plot. Defaults to None.
             alpha (float, optional): transparency of the sampled data points. Defaults to 0.8.
             ymin (float, optional): minimum value of y in the plot. Defaults to None.
             ymax (float, optional): maximum value of y in the plot. Defaults to None.
         """
         if x_tr is not None and y_tr is not None:
             # Plot training data as well.
@@ -340,41 +376,7 @@
             plt.ylabel(r"$y_{}$".format(y_idx))
         if save_dir is not None:
             make_folder(save_dir)
             plt.savefig(save_dir, bbox_inches="tight")
             plt.close()
         else:
             plt.show()
-
-
-def engression(x, y, 
-               num_layer=2, hidden_dim=100, noise_dim=100,
-               lr=0.001, num_epoches=500, batch_size=None, 
-               print_every_nepoch=100, print_times_per_epoch=1,
-               device="cpu", standardize=True,
-               verbose=True): 
-    """engression function.
-
-    Args:
-        x (torch.Tensor): training data of predictors.
-        y (torch.Tensor): training data of responses.
-        num_layer (int, optional): number of layers. Defaults to 2.
-        hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
-        noise_dim (int, optional): noise dimension. Defaults to 100.
-        lr (float, optional): learning rate. Defaults to 0.001.
-        num_epoches (int, optional): number of epochs. Defaults to 500.
-        batch_size (int, optional): batch size. Defaults to None.
-        print_every_nepoch (int, optional): print losses every print_every_nepoch number of epochs. Defaults to 100.
-        print_times_per_epoch (int, optional): print losses for print_times_per_epoch times per epoch. Defaults to 1.
-        device (str, torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "gpu", "cuda"].
-        standardize (bool, optional):  whether to standardize data for training. Defaults to True.
-        verbose (bool, optional): whether to print losses and info. Defaults to True.
-
-    Returns:
-        Engressor object: a fitted engression model.
-    """
-    engressor = Engressor(in_dim=x.shape[1], out_dim=y.shape[1], num_layer=num_layer, hidden_dim=hidden_dim, noise_dim=noise_dim, 
-                          lr=lr, num_epoches=num_epoches, batch_size=batch_size, device=device, standardize=standardize)
-    engressor.train(x, y, num_epoches=num_epoches, batch_size=batch_size, 
-                    print_every_nepoch=print_every_nepoch, print_times_per_epoch=print_times_per_epoch, 
-                    standardize=standardize, verbose=verbose)
-    return engressor
```

### Comparing `engression-0.0.1/engression/engression_bagged.py` & `engression-0.1.0/engression/engression_bagged.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,56 @@
-# coming soon.
-
 import torch
 import numpy as np
 import matplotlib.pyplot as plt
 
 from .engression import Engressor
 from .loss_func import *
-from .models import StoNet
-from .data.loader import make_dataloader
 from .utils import *
 
 
+def engression_bagged(x, y, 
+                      num_layer=2, hidden_dim=100, noise_dim=100,
+                      lr=0.001, num_epoches=500, batch_size=None, 
+                      device="cpu", standardize=True,
+                      ensemble_size=10, val_loss_type="energy"):
+    """This function fits a bagged engression model to the data by aggregating multiple engression models fitted on subsamples of the data. It calculates validation losses that helps with hyperparameter tuning.
+
+    Args:
+        x (torch.Tensor): training data of predictors.
+        y (torch.Tensor): training data of responses.
+        num_layer (int, optional): number of layers. Defaults to 2.
+        hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
+        noise_dim (int, optional): noise dimension. Defaults to 100.
+        lr (float, optional): learning rate. Defaults to 0.001.
+        num_epoches (int, optional): number of epochs. Defaults to 500.
+        batch_size (int, optional): batch size. Defaults to None.
+        device (str, torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "gpu", "cuda"].
+        standardize (bool, optional):  whether to standardize data for training. Defaults to True.
+        ensemble_size (int, optional): number of ensemble models. Defaults to 10.
+        val_loss_type (str, optional): loss type for validation. Defaults to "energy". Choices: ["l1", "l2", "energy"].
+
+    Returns:
+        BaggedEngressor object: a fitted bagged engression model.
+    """
+    engressor = BaggedEngressor(in_dim=x.shape[1], out_dim=y.shape[1], 
+                                num_layer=num_layer, hidden_dim=hidden_dim, noise_dim=noise_dim, 
+                                lr=lr, num_epoches=num_epoches, batch_size=batch_size, 
+                                device=device, standardize=standardize, 
+                                ensemble_size=ensemble_size, val_loss_type=val_loss_type)
+    engressor.train(x, y)
+    return engressor
+
+
 class BaggedEngressor(object):
     def __init__(self, 
                  in_dim, out_dim, num_layer=2, hidden_dim=100, noise_dim=100,
-                 lr=0.001, num_epoches=500, batch_size=None, device="cpu", standardize=True,
+                 lr=0.001, num_epoches=500, batch_size=None, 
+                 device="cpu", standardize=True,
                  ensemble_size=10, val_loss_type="energy"): 
-        """Engressor with bagging.
+        """Bagged engressor.
 
         Args:
             in_dim (int): input dimension
             out_dim (int): output dimension
             num_layer (int, optional): number of layers. Defaults to 2.
             hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
             noise_dim (int, optional): noise dimension. Defaults to 100.
@@ -29,64 +59,92 @@
             batch_size (int, optional): batch size. Defaults to None, referring to the full batch.
             device (str or torch.device, optional): device. Defaults to "cpu".
             standardize (bool, optional): whether to standardize data. Defaults to True.
             ensemble_size (int, optional): number of models for ensemble. Defaults to 10.
             val_loss_type (str, optional): loss type for validation. Defaults to "energy". Choices: ["l1", "l2", "energy"].
         """
         super().__init__()
+        self.num_layer = num_layer
+        self.hidden_dim = hidden_dim
+        self.noise_dim = noise_dim
         self.lr = lr
         self.num_epoches = num_epoches
         self.batch_size = batch_size
         self.ensemble_size = ensemble_size
-        self.num_models_for_each_sample = ensemble_size // 2
+        self.num_models_for_each_sample = ensemble_size // 2 
+        # As such, each model has around 50% training data and the remaining 50% as validation data. 
+        
         if isinstance(device, str):
             device = torch.device(device)
         self.device = device
         self.standardize = standardize
         self.x_mean = None
         self.x_std = None
         self.y_mean = None
         self.y_std = None
         self.split_mask = None
         
         # Build ensemble models.
         self.models = []        
-        for _ in range(ensemble_size):
+        for i in range(ensemble_size):
+            check_device = i == 0 
             self.models.append(Engressor(in_dim, out_dim, num_layer, hidden_dim, noise_dim, 
-                                         lr=lr, device=device, standardize=standardize))
+                                         lr=lr, standardize=standardize, device=device, check_device=check_device))
         self.val_loss_type = val_loss_type
+        
+        self.train_losses = [] # training losses of each model
+        self.val_losses = [] # validation losses of each model
+        self.val_loss_final = None # validation loss of aggregated model on the entire training data set
 
     def train_mode(self):
         for i in range(self.ensemble_size):
             self.models[i].train_mode()
         
     def eval_mode(self):
         for i in range(self.ensemble_size):
             self.models[i].eval_mode()
+
+    def summary(self):
+        """Print the model architecture and hyperparameters."""
+        print("Engression model with\n" +
+              "\t number of layers: {}\n".format(self.num_layer) +
+              "\t hidden dimensions: {}\n".format(self.hidden_dim) +
+              "\t noise dimensions: {}\n".format(self.noise_dim) +
+              "\t number of epochs: {}\n".format(self.num_epoches) +
+              "\t batch size: {}\n".format(self.batch_size) +
+              "\t learning rate: {}\n".format(self.lr) +
+              "\t standardization: {}\n".format(self.standardize) +
+              "\t training mode: {}\n".format(self.models[0].model.training) +
+              "\t device: {}\n".format(self.device) + 
+              "\t ensemble size: {}\n".format(self.ensemble_size))
+        print("Validation {} loss: {:.4f}".format(self.val_loss_type, self.val_loss_final))
         
-    def train(self, x, y, num_epoches=None, batch_size=None, standardize=True, val_loss_type="", val_sample_size=100, verbose=True):
-        """_summary_
+    def train(self, x, y, num_epoches=None, batch_size=None, standardize=True, val_loss_type="energy", val_sample_size=100):
+        """Fit multiple models on subsamples of the training data.
 
         Args:
-            x (_type_): _description_
-            y (_type_): _description_
-            num_epoches (_type_, optional): _description_. Defaults to None.
-            batch_size (_type_, optional): _description_. Defaults to None.
-            standardize (bool, optional): _description_. Defaults to True.
-                - Standardization scheme for bagging: 
-                    for each model, all data are standardized using the mean and standard deviation of the training data for this model alone.
-            val_loss_type (str, optional): _description_. Defaults to "".
-            val_sample_size (int, optional): _description_. Defaults to 100.
-            verbose (bool, optional): _description_. Defaults to True.
+            x (torch.Tensor): training data of predictors.
+            y (torch.Tensor): trainging data of responses.
+            num_epoches (int, optional): number of training epochs. Defaults to None.
+            batch_size (int, optional): batch size for mini-batch SGD. Defaults to 512.
+            print_every_nepoch (int, optional): print losses every print_every_nepoch number of epochs. Defaults to 100.
+            print_times_per_epoch (int, optional): print losses for print_times_per_epoch times per epoch. Defaults to 1.
+            standardize (bool, optional): whether to standardize the data. Defaults to True.
+                - standardization scheme for bagging: 
+                    for each model, all data are standardized using the mean and standard deviation of the training data for fitting this model alone.
+            val_loss_type (str, optional): loss type for validation. Defaults to "energy". Choices: ["l1", "l2", "energy"].
+            val_sample_size (int, optional): generated sample size for evaluating the validation loss. Defaults to 100.
         """
         self.train_mode()
         if num_epoches is None:
             num_epoches = self.num_epoches
         if batch_size is None:
             batch_size = self.batch_size
+        if val_loss_type == "":
+            val_loss_type = self.val_loss_type
         if standardize:
             self.standardize = standardize
 
         x = vectorize(x)
         y = vectorize(y)
         x = x.to(self.device)
         y = y.to(self.device)
@@ -94,41 +152,47 @@
         # Mask matrix for splitting training and validation data.
         data_size = x.shape[0]
         rng = np.random.default_rng(21875667591346)
         self.split_mask = torch.from_numpy(rng.multivariate_hypergeometric([1]*self.ensemble_size, self.num_models_for_each_sample, size=data_size))
         
         # Training.
         for i in range(self.ensemble_size):
+            verbose = i == 0
             model = self.models[i]
-            train_idx = self.split_mask[:,i]
+            train_idx = self.split_mask[:,i] == 1
             x_train = x[train_idx]
             y_train = y[train_idx]
             x_val = x[~train_idx]
             y_val = y[~train_idx]
-            model.train(x_train, y_train, num_epoches=num_epoches, batch_size=batch_size, standardize=self.standardize, verbose=False)
+            if verbose:
+                print("Model 1 training details:\n")
+            model.train(x_train, y_train, num_epoches=num_epoches, batch_size=batch_size, standardize=self.standardize, verbose=verbose)
+            if verbose:
+                print("\n")
             val_loss = model.eval_loss(x_val, y_val, loss_type="energy", sample_size=2)
             train_loss = model.eval_loss(x_train, y_train, loss_type="energy", sample_size=2)
-            standardize_str = "(standardized)" if self.standardize else ""
-            print("[Model {}] train_loss{}: {:.4f}, val_loss{}: {:.4f}".format(i + 1, standardize_str, train_loss, standardize_str, val_loss))
+            self.train_losses.append(train_loss)
+            self.val_losses.append(val_loss)
+            print("[Model {}] train_loss: {:.4f}, val_loss: {:.4f}".format(i + 1, train_loss, val_loss))
         
         # Validation.
-        val_loss_final = self.validate_bagged(x, y, loss_type=val_loss_type, sample_size=val_sample_size)
-        print("Final validation {} loss: {:.4f}".format(val_loss_type, val_loss_final))
+        self.val_loss_final = self.validate_bagged(x, y, loss_type=val_loss_type, sample_size=val_sample_size)
+        print("\nValidation {} loss of the bagged engression model: {:.4f}".format(val_loss_type, self.val_loss_final))
     
     def validate_bagged(self, x, y, loss_type="energy", sample_size=100):
-        """Evaluate the bagged model on the validation data.
+        """Validation loss of the bagged model (on training data set). The loss for each data point is computed using the models that are not fitted on this data point. Note that this is a better validation metric than simply averaging the validation losses of each model. 
 
         Args:
             x (torch.Tensor): training data for predictors.
             y (torch.Tensor): training data for responses.
             loss_type (str, optional): type of the loss. Defaults to "energy".
-            sample_size (int, optional): _description_. Defaults to 100.
+            sample_size (int, optional): generated sample size to evaluate the loss. Defaults to 100.
 
         Returns:
-            float: loss of the bagged model on the validation data.
+            float: validation loss of the bagged model.
         """
         self.eval_mode()
         x = vectorize(x)
         y = vectorize(y)
         x = x.to(self.device)
         y = y.to(self.device)
         
@@ -138,41 +202,65 @@
         for i in range(self.ensemble_size):
             model = self.models[i]
             val_idx = self.split_mask[:,i] == 0
             y_samples[val_idx, :, :, i] = model.sample(x[val_idx], sample_size=sample_size_per_model)
         val_idx = (1 - self.split_mask).nonzero(as_tuple=True)
         y_samples = y_samples[val_idx[0], :, :, val_idx[1]]
         y_samples = y_samples.reshape(y.shape[0], self.num_models_for_each_sample, y.shape[1], sample_size_per_model).permute(0, 2, 3, 1)
+        y_samples = y_samples.reshape(y.shape[0], y.shape[1], -1)
         
         # Compute the loss (on the original scale).
         if loss_type == "energy":
+            y_samples = list(torch.split(y_samples, 1, dim=2))
             loss = energy_loss(y, y_samples, verbose=False)
         elif loss_type == "l2":
             y_pred = y_samples.mean(dim=len(y_samples.shape) - 1)
             loss = (y - y_pred).pow(2).mean()
         elif loss_type == "l1":
-            y_pred = y_samples.median(dim=len(y_samples.shape) - 1)
+            y_pred = y_samples.median(dim=len(y_samples.shape) - 1).values
             loss = (y - y_pred).abs().mean()
         return loss.item()
     
     def sample(self, x, sample_size=100):
+        """Sample new response data from all ensemble models. 
+
+        Args:
+            x (torch.Tensor): test data of predictors.
+            sample_size (int, optional): generated sample sizes for each x. Defaults to 100.
+            expand_dim (bool, optional): whether to expand the sample dimension. Defaults to True.
+
+        Returns:
+            torch.Tensor of shape (data_size, response_dim, sample_size).
+                - [:,:,i] consists of the i-th sample of all x.
+                - [i,:,:] consists of all samples of x_i.
+        """
         self.eval_mode()
         x = vectorize(x)
         x = x.to(self.device)
         sample_size_per_model = sample_size // self.ensemble_size
         y_samples = []
         for i in range(self.ensemble_size):
             model = self.models[i]
             if i == self.ensemble_size:
                 sample_size_per_model += sample_size % self.ensemble_size
             y_samples.append(model.sample(x, sample_size=sample_size_per_model))
         y_samples = torch.cat(y_samples, dim=-1)
         return y_samples
     
     def predict(self, x, target="mean", sample_size=100):
+        """Point prediction.
+
+        Args:
+            x (torch.Tensor): data of predictors.
+            target (str or float or list, optional): a quantity of interest to predict. float refers to the quantiles. Defaults to "mean".
+            sample_size (int, optional): generated sample sizes for each x. Defaults to 100.
+
+        Returns:
+            torch.Tensor or list of torch.Tensor: point predictions.
+        """
         self.eval_mode()
         x = vectorize(x)
         x = x.to(self.device)
         y_samples = self.sample(x, sample_size=sample_size)
         if not isinstance(target, list):
             target = [target]
         y_pred = []
@@ -192,34 +280,37 @@
             print("Warning: the estimate for quantiles at {} with a sample size of {} could be inaccurate. Please increase the `sample_size`.".format(extremes, sample_size))
 
         if len(y_pred) == 1:
             return y_pred[0]
         else:
             return y_pred
         
-    def eval_loss(self, x, y, loss_type="energy", sample_size=100):
+    def eval_loss(self, x, y, loss_type="l2", sample_size=100):
         """Evaluate the bagged model.
 
         Args:
-            x (_type_): _description_
-            y (_type_): _description_
-            loss_type (str, optional): _description_. Defaults to "energy".
-            sample_size (int, optional): _description_. Defaults to 100.
+            x (torch.Tensor): data of predictors.
+            y (torch.Tensor): data of responses.
+            loss_type (str, optional): loss type. Defaults to "l2". Choices: ["l2", "l1", "energy", "cor"].
+            sample_size (int, optional): generated sample sizes for each x. Defaults to 100.
 
         Returns:
-            _type_: _description_
+            float: evaluation loss.
         """
         self.eval_mode()
         x = vectorize(x)
         y = vectorize(y)
         x = x.to(self.device)
         y = y.to(self.device)
         if loss_type == "l2":
             y_pred = self.predict(x, target="mean", sample_size=sample_size)
             loss = (y - y_pred).pow(2).mean()
+        elif loss_type == "cor":
+            y_pred = self.predict(x, target="mean", sample_size=sample_size)
+            loss = cor(y, y_pred)
         elif loss_type == "l1":
             y_pred = self.predict(x, target=0.5, sample_size=sample_size)
             loss = (y - y_pred).abs().mean()
         else:
             assert loss_type == "energy"
             y_samples = self.sample(x, sample_size=sample_size, expand_dim=False)
             loss = energy_loss(y, y_samples, verbose=False)
@@ -231,15 +322,15 @@
 
         Args:
             x (torch.Tensor): data of predictors
             y (torch.Tensor): data of responses
             x_idx (int, optional): index of the predictor to plot (if there are multiple). Defaults to 0.
             y_idx (int, optional): index of the response to plot (if there are multiple). Defaults to 0.
             target (str or float, optional): target quantity. Defaults to "mean". Choice: ["mean", "median", "sample", float].
-            sample_size (int, optional): sample size used for estimation. Defaults to 100.
+            sample_size (int, optional): generated sample size used for estimation. Defaults to 100.
             save_dir (str, optional): directory to save the plot. Defaults to None.
             alpha (float, optional): transparency of the sampled data points. Defaults to 0.8.
             ymin (float, optional): minimum value of y in the plot. Defaults to None.
             ymax (float, optional): maximum value of y in the plot. Defaults to None.
         """
         x = vectorize(x)
         y = vectorize(y)
@@ -265,18 +356,7 @@
             plt.ylabel(r"$y_{}$".format(y_idx))
         if save_dir is not None:
             make_folder(save_dir)
             plt.savefig(save_dir, bbox_inches="tight")
             plt.close()
         else:
             plt.show()
-
-
-def engression_bagged(x, y, 
-                       num_layer=2, hidden_dim=100, noise_dim=100,
-                       lr=0.001, num_epoches=500, batch_size=None, device="cpu",
-                       nfolds=10, loss_type="energy"):
-    engressor = BaggedEngressor(in_dim=x.shape[1], out_dim=y.shape[1], num_layer=num_layer, hidden_dim=hidden_dim, noise_dim=noise_dim, 
-                            lr=lr, num_epoches=num_epoches, batch_size=batch_size, device=device, nfolds=nfolds)
-    engressor.train(x, y)
-    print("Average validation {} loss: {:.4f}".format(loss_type, np.mean(engressor.val_losses)))
-    return engressor
```

### Comparing `engression-0.0.1/engression/loss_func.py` & `engression-0.1.0/engression/loss_func.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import torch
 from .utils import vectorize
 
 def energy_loss(x_true, x_est, beta=1, verbose=False):
     """Loss function based on the energy score.
 
     Args:
-        x_true (torch.Tensor): iid samples from the true distribution.
-        x_est (list of torch.Tensor): a list of iid samples from the estimated distribution. ## todo: not a list!!!
+        x_true (torch.Tensor): iid samples from the true distribution of shape (data_size, data_dim)
+        x_est (list of torch.Tensor): 
+            - a list of length sample_size, where each element is a tensor of shape (data_size, data_dim) that contains one sample for each data point from the estimated distribution, or 
+            - a tensor of shape (data_size*sample_size, response_dim) such that x_est[data_size*(i-1):data_size*i,:] contains one sample for each data point, for i = 1, ..., sample_size.
         beta (float): power parameter in the energy score.
         verbose (bool): whether to return two terms of the loss.
 
     Returns:
         loss (torch.Tensor): energy loss.
     """
     x_true = vectorize(x_true).unsqueeze(1)
```

### Comparing `engression-0.0.1/engression/models.py` & `engression-0.1.0/engression/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,36 +65,14 @@
         Returns:
             torch.Tensor or list of torch.Tensor: point predictions
                 - [:,:,i] gives the i-th sample of all x.
                 - [i,:,:] gives all samples of x_i.
             
         Here we do not call `sample` but directly call `forward`.
         """
-        # eval_size = x.size(0)
-        # # Sampling
-        # with torch.no_grad():
-        #     x_rep = torch.repeat_interleave(x, (sample_size * torch.ones(eval_size, device=x.device)).long(), dim=0)
-        #     y_pred = self.forward(x=x_rep).detach()
-        #     y_pred = list(torch.split(y_pred, sample_size))
-            
-        # if not isinstance(target, list):
-        #     target = [target]
-        # results = []
-        # extremes = []
-        # for t in target:
-        #     if t == "mean":
-        #         results.append(torch.cat([y_pred[i].mean().unsqueeze(0) for i in range(eval_size)], dim=0).unsqueeze(1))
-        #     else:
-        #         if t == "median":
-        #             t = 0.5
-        #         assert isinstance(t, float)
-        #         results.append(torch.cat([y_pred[i].quantile(t).unsqueeze(0) for i in range(eval_size)], dim=0).unsqueeze(1))
-        #         if min(t, 1-t) * sample_size < 10:
-        #             extremes.append(t)
-        
         samples = self.sample(x=x, sample_size=sample_size, expand_dim=True)
         if not isinstance(target, list):
             target = [target]
         results = []
         extremes = []
         for t in target:
             if t == "mean":
@@ -120,28 +98,30 @@
 
         Args:
             x (torch.Tensor): new data of predictors of shape [data_size, covariate_dim]
             sample_size (int, optional): new sample size. Defaults to 100.
             expand_dim (bool, optional): whether to expand the sample dimension. Defaults to True.
 
         Returns:
-            torch.Tensor of shape (data_size, response_dim, sample_size), where response_dim could have multiple channels.
+            torch.Tensor of shape (data_size, response_dim, sample_size) if expand_dim else (data_size*sample_size, response_dim), where response_dim could have multiple channels.
         """
-        eval_size = x.size(0)
+        data_size = x.size(0) ## input data size
         with torch.no_grad():
-            # x_rep = torch.repeat_interleave(x, (sample_size * torch.ones(eval_size, device=x.device)).long(), dim=0)
+            ## repeat the data for sample_size times, get a tensor [data, data, ..., data]
             x_rep = x.repeat(sample_size, 1)
+            ## samples of shape (data_size*sample_size, response_dim) such that samples[data_size*(i-1):data_size*i,:] contains one sample for each data point, for i = 1, ..., sample_size
             samples = self.forward(x=x_rep).detach()
         if not expand_dim:
             return samples
         else:
             expand_dim = len(samples.shape)
-            samples = samples.unsqueeze(expand_dim)
-            samples = list(torch.split(samples, eval_size))
-            samples = torch.cat(samples, dim=expand_dim)
+            samples = samples.unsqueeze(expand_dim) ## (data_size*sample_size, response_dim, 1)
+            ## a list of length data_size, each element is a tensor of shape (data_size, response_dim, 1)
+            samples = list(torch.split(samples, data_size)) 
+            samples = torch.cat(samples, dim=expand_dim) ## (data_size, response_dim, sample_size)
             return samples
             # without expanding dimensions:
             # samples.reshape(-1, *samples.shape[1:-1])
         
     def forward(self, x, inject_noise=True):
         x = self.input_layer(x, inject_noise)
         for i in range(self.num_layer - 2):
```

### Comparing `engression-0.0.1/engression/utils.py` & `engression-0.1.0/engression/utils.py`

 * *Files identical despite different names*

### Comparing `engression-0.0.1/engression.egg-info/PKG-INFO` & `engression-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: engression
-Version: 0.0.1
-Summary: Engression
+Version: 0.1.0
+Summary: Engression Modelling
 Home-page: https://github.com/xwshen51/engression
-Author: Xinwei Shen
+Author: Xinwei Shen and Nicolai Meinshausen
 Author-email: xinwei.shen@stat.math.ethz.ch
 License: BSD 3-Clause License
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Engression
 
-Engression is a nonlinear regression methodology proposed in the paper "[*Engression: Extrapolation for Nonlinear Regression?*](https://arxiv.org/abs/2307.00835)" by Xinwei Shen and Nicolai Meinshausen. 
-This directory contains the Python implementation of engression.
+Engression is a nonlinear regression methodology proposed in the paper "[*Engression: Extrapolation for Nonlinear Regression?*](https://arxiv.org/abs/2307.00835)" by Xinwei Shen and Nicolai Meinshausen. This directory contains the Python implementation of engression.
+
+Consider targets $Y\in\mathbb{R}^k$ and predictors $X\in\mathbb{R}^d$; both variables can be univariate or multivariate. Engression can be used to 
+* estimate the conditional mean $\mathbb{E}[Y|X=x]$ (as in least-squares regression), 
+* estimate the conditional quantiles of $Y$ given $X=x$ (as in quantile regression), and 
+* sample from the fitted conditional distribution of $Y$ given $X=x$ (as a generative model).
+
+The results in the paper show the advantages of engression over existing regression approaches in terms of extrapolation. 
+
 
 ## Installation
 The latest release of the Python package can be installed through pip:
 ```sh
 pip install engression
 ```
 
@@ -26,15 +34,15 @@
 ```
 
 
 ## Usage Example
 
 ### Python
 
-Below is one simple demonstration. See [this tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_simu.ipynb) for more details on simulated data and [this tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_air.ipynb) for a real data example.
+Below is one simple demonstration. See [this tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_simu.ipynb) for more details on simulated data and [this tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_air.ipynb) for a real data example. We demonstrate in [another tutorial](https://github.com/xwshen51/engression/blob/main/engression-python/examples/example_bag.ipynb) how to fit a bagged engression model, which also helps with hyperparameter tuning.
 ```python
 from engression import engression
 from engression.data.simulator import preanm_simulator
 
 ## Simulate data
 x, y = preanm_simulator("square", n=10000, x_lower=0, x_upper=2, noise_std=1, train=True, device=device)
 x_eval, y_eval_med, y_eval_mean = preanm_simulator("square", n=1000, x_lower=0, x_upper=4, noise_std=1, train=False, device=device)
```

### Comparing `engression-0.0.1/setup.py` & `engression-0.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 with open('requirements.txt') as f:
     install_requires = [l.strip() for l in f]
     
 
 setup(
     name='engression',
-    version='0.0.1',
-    description='Engression',
+    version='0.1.0',
+    description='Engression Modelling',
     url='https://github.com/xwshen51/engression',
-    author='Xinwei Shen',
+    author='Xinwei Shen and Nicolai Meinshausen',
     author_email='xinwei.shen@stat.math.ethz.ch',
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     license="BSD 3-Clause License",
 )
```

