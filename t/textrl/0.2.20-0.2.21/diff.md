# Comparing `tmp/textrl-0.2.20.tar.gz` & `tmp/textrl-0.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textrl-0.2.20.tar", last modified: Tue Jul 25 02:43:14 2023, max compression
+gzip compressed data, was "textrl-0.2.21.tar", last modified: Thu Aug  3 22:40:59 2023, max compression
```

## Comparing `textrl-0.2.20.tar` & `textrl-0.2.21.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-07-25 02:43:14.941539 textrl-0.2.20/
--rw-r--r--   0 voidful    (501) staff       (20)     4206 2022-12-05 09:09:02.000000 textrl-0.2.20/.gitignore
--rw-r--r--   0 voidful    (501) staff       (20)     1064 2023-02-09 14:54:56.000000 textrl-0.2.20/LICENSE
--rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-07-25 02:43:14.940869 textrl-0.2.20/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)    17515 2023-04-25 10:23:10.000000 textrl-0.2.20/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-07-25 02:43:14.886003 textrl-0.2.20/example/
--rw-r--r--   0 voidful    (501) staff       (20)     7679 2023-03-27 13:57:09.000000 textrl-0.2.20/example/2022-12-10-textrl-elon-musk.ipynb
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-07-25 02:43:14.886796 textrl-0.2.20/img/
--rw-r--r--   0 voidful    (501) staff       (20)   373908 2023-04-17 05:47:18.000000 textrl-0.2.20/img/Designer.png
--rw-r--r--   0 voidful    (501) staff       (20)       61 2022-12-05 09:17:42.000000 textrl-0.2.20/requirement.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2023-07-25 02:43:14.941614 textrl-0.2.20/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)     1095 2023-07-25 02:42:40.000000 textrl-0.2.20/setup.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-07-25 02:43:14.915802 textrl-0.2.20/textrl/
--rw-r--r--   0 voidful    (501) staff       (20)      184 2023-02-13 19:45:54.000000 textrl-0.2.20/textrl/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)    13472 2023-04-26 08:50:57.000000 textrl-0.2.20/textrl/actor.py
--rw-r--r--   0 voidful    (501) staff       (20)     1150 2023-06-20 16:43:55.000000 textrl-0.2.20/textrl/dump.py
--rw-r--r--   0 voidful    (501) staff       (20)     7405 2023-07-25 02:42:31.000000 textrl-0.2.20/textrl/environment.py
--rw-r--r--   0 voidful    (501) staff       (20)    23448 2023-02-13 19:43:59.000000 textrl-0.2.20/textrl/evaluator.py
--rw-r--r--   0 voidful    (501) staff       (20)     7511 2023-02-13 19:43:59.000000 textrl-0.2.20/textrl/trainer.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-07-25 02:43:14.935944 textrl-0.2.20/textrl.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-07-25 02:43:14.000000 textrl-0.2.20/textrl.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      433 2023-07-25 02:43:14.000000 textrl-0.2.20/textrl.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2023-07-25 02:43:14.000000 textrl-0.2.20/textrl.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)       50 2023-07-25 02:43:14.000000 textrl-0.2.20/textrl.egg-info/entry_points.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2022-12-05 09:10:02.000000 textrl-0.2.20/textrl.egg-info/not-zip-safe
--rw-r--r--   0 voidful    (501) staff       (20)       17 2023-07-25 02:43:14.000000 textrl-0.2.20/textrl.egg-info/requires.txt
--rw-r--r--   0 voidful    (501) staff       (20)        7 2023-07-25 02:43:14.000000 textrl-0.2.20/textrl.egg-info/top_level.txt
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.962817 textrl-0.2.21/
+-rw-r--r--   0 voidful    (501) staff       (20)     4206 2022-12-05 09:09:02.000000 textrl-0.2.21/.gitignore
+-rw-r--r--   0 voidful    (501) staff       (20)     1064 2023-02-09 14:54:56.000000 textrl-0.2.21/LICENSE
+-rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-08-03 22:40:59.958844 textrl-0.2.21/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)    17515 2023-04-25 10:23:10.000000 textrl-0.2.21/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.921512 textrl-0.2.21/example/
+-rw-r--r--   0 voidful    (501) staff       (20)     7679 2023-03-27 13:57:09.000000 textrl-0.2.21/example/2022-12-10-textrl-elon-musk.ipynb
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.923474 textrl-0.2.21/img/
+-rw-r--r--   0 voidful    (501) staff       (20)   373908 2023-04-17 05:47:18.000000 textrl-0.2.21/img/Designer.png
+-rw-r--r--   0 voidful    (501) staff       (20)       61 2022-12-05 09:17:42.000000 textrl-0.2.21/requirement.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2023-08-03 22:40:59.962917 textrl-0.2.21/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)     1095 2023-08-03 22:39:44.000000 textrl-0.2.21/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.942741 textrl-0.2.21/textrl/
+-rw-r--r--   0 voidful    (501) staff       (20)      184 2023-02-13 19:45:54.000000 textrl-0.2.21/textrl/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)    13501 2023-08-03 22:39:00.000000 textrl-0.2.21/textrl/actor.py
+-rw-r--r--   0 voidful    (501) staff       (20)     1150 2023-06-20 16:43:55.000000 textrl-0.2.21/textrl/dump.py
+-rw-r--r--   0 voidful    (501) staff       (20)     7405 2023-07-25 02:42:31.000000 textrl-0.2.21/textrl/environment.py
+-rw-r--r--   0 voidful    (501) staff       (20)    23448 2023-02-13 19:43:59.000000 textrl-0.2.21/textrl/evaluator.py
+-rw-r--r--   0 voidful    (501) staff       (20)     7511 2023-02-13 19:43:59.000000 textrl-0.2.21/textrl/trainer.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-03 22:40:59.958170 textrl-0.2.21/textrl.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      433 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       50 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/entry_points.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2022-12-05 09:10:02.000000 textrl-0.2.21/textrl.egg-info/not-zip-safe
+-rw-r--r--   0 voidful    (501) staff       (20)       17 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/requires.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        7 2023-08-03 22:40:59.000000 textrl-0.2.21/textrl.egg-info/top_level.txt
```

### Comparing `textrl-0.2.20/.gitignore` & `textrl-0.2.21/.gitignore`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/LICENSE` & `textrl-0.2.21/LICENSE`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/PKG-INFO` & `textrl-0.2.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textrl
-Version: 0.2.20
+Version: 0.2.21
 Summary: TextRL - use reinforcement learning to adjust text generation results.
 Home-page: https://github.com/voidful/TextRL
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: transformer huggingface nlp generation reinforcement learning deep learning
 Platform: UNKNOWN
```

### Comparing `textrl-0.2.20/README.md` & `textrl-0.2.21/README.md`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/example/2022-12-10-textrl-elon-musk.ipynb` & `textrl-0.2.21/example/2022-12-10-textrl-elon-musk.ipynb`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/img/Designer.png` & `textrl-0.2.21/img/Designer.png`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/setup.py` & `textrl-0.2.21/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='textrl',
-    version='0.2.20',
+    version='0.2.21',
     description='TextRL - use reinforcement learning to adjust text generation results.',
     url='https://github.com/voidful/TextRL',
     author='Voidful',
     author_email='voidful.stack@gmail.com',
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     setup_requires=['setuptools-git'],
```

### Comparing `textrl-0.2.20/textrl/actor.py` & `textrl-0.2.21/textrl/actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
             update_interval=update_interval,
             minibatch_size=minibatch_size,
             epochs=epochs,
             clip_eps_vf=None,
             entropy_coef=0,
             gamma=0.95,  # https://arxiv.org/abs/2210.01241
             lambd=1,
+            max_grad_norm=1.0,
             standardize_advantages=True,
             act_deterministically=self.act_deterministically
         )
         self.agent = agent
         return agent
 
     @autocast('cuda')
@@ -292,15 +293,15 @@
     def _lossfun(
             self, entropy, vs_pred, log_probs, vs_pred_old, log_probs_old, advs, vs_teacher
     ):
         prob_ratio = torch.exp(log_probs - log_probs_old)
         loss_policy = -torch.mean(
             torch.min(
                 (prob_ratio * advs),
-                (torch.clamp(prob_ratio, 1 - self.clip_eps, 1 + self.clip_eps) * advs),
+                torch.clamp(prob_ratio, 1 - self.clip_eps, 1 + self.clip_eps) * advs,
             ),
         )
         if self.clip_eps_vf is None:
             loss_value_func = F.mse_loss(vs_pred.squeeze(), vs_teacher.squeeze())
         else:
             clipped_vs_pred = _elementwise_clip(
                 vs_pred,
```

### Comparing `textrl-0.2.20/textrl/dump.py` & `textrl-0.2.21/textrl/dump.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/textrl/environment.py` & `textrl-0.2.21/textrl/environment.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/textrl/evaluator.py` & `textrl-0.2.21/textrl/evaluator.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/textrl/trainer.py` & `textrl-0.2.21/textrl/trainer.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.20/textrl.egg-info/PKG-INFO` & `textrl-0.2.21/textrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textrl
-Version: 0.2.20
+Version: 0.2.21
 Summary: TextRL - use reinforcement learning to adjust text generation results.
 Home-page: https://github.com/voidful/TextRL
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: transformer huggingface nlp generation reinforcement learning deep learning
 Platform: UNKNOWN
```

