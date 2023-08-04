# Comparing `tmp/ddqla-0.1.14.tar.gz` & `tmp/ddqla-0.1.15.tar.gz`

## Comparing `ddqla-0.1.14.tar` & `ddqla-0.1.15.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqla-0.1.14/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ddqla-0.1.14/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ddqla-0.1.14/src/ddqla/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ddqla-0.1.14/src/ddqla/agents/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 ddqla-0.1.14/src/ddqla/agents/base_agent.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 ddqla-0.1.14/test/test.ipynb
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ddqla-0.1.14/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ddqla-0.1.14/LICENSE
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 ddqla-0.1.14/README.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ddqla-0.1.14/pyproject.toml
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 ddqla-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqla-0.1.15/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ddqla-0.1.15/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ddqla-0.1.15/src/ddqla/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ddqla-0.1.15/src/ddqla/agents/__init__.py
+-rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 ddqla-0.1.15/src/ddqla/agents/base_agent.py
+-rw-r--r--   0        0        0    14676 2020-02-02 00:00:00.000000 ddqla-0.1.15/test/pacchi.ipynb
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ddqla-0.1.15/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ddqla-0.1.15/LICENSE
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 ddqla-0.1.15/README.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ddqla-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 ddqla-0.1.15/PKG-INFO
```

### Comparing `ddqla-0.1.14/.github/workflows/python-publish.yml` & `ddqla-0.1.15/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ddqla-0.1.14/src/ddqla/agents/base_agent.py` & `ddqla-0.1.15/src/ddqla/agents/base_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
             simulation_step.append(p1[i].numpy().item())
         for i in range(0, self._num_actions):
             simulation_step.append(p2[i].numpy().item())
         for i in range(0, self._num_actions):
             simulation_step.append(self.__q[i])
         simulation_step.append(rnd)
         simulation_step.append(self._exploration_rate)
+        simulation_step.append(1 if rnd > self._exploration_rate else 0)
         simulation_step.append(action)
         simulation_step.append(reward)
         simulation_step.append(np.sum(self._cum_rewards))
         self.simulation_log.append(simulation_step)
 
     def get_last_cumulative_rewards(self):
         return np.sum(self._cum_rewards)
@@ -150,14 +151,15 @@
             headers.append("p1_" + str(i))
         for i in range(0, self._num_actions):
             headers.append("p2_" + str(i))
         for i in range(0, self._num_actions):
             headers.append("q_" + str(i))
         headers.append("rnd")
         headers.append("er")
+        headers.append("net")
         headers.append("action")
         headers.append("reward")
         headers.append("cum_reward")
         return headers
 
     def save_simulation_log(self, append_ts=True):
         now = datetime.datetime.now()
@@ -174,21 +176,21 @@
     def summary(self):
         crl = self.cum_rewards_log
         cr_indexes = [i for i, _ in enumerate(crl)]
         cr_values = [x for _, x in enumerate(crl)]
         tl = self.tests_log
         tl_indexes = [i for i, _ in enumerate(tl)]
         tl_values = [x for _, x in enumerate(tl)]
-        plt.figure(figsize=(24, 8))
+        plt.figure(figsize=(24, 4))
         plt.title('Cumulative rewards')
         plt.scatter(cr_indexes, cr_values, label="DDQL Agent", s=1)
         plt.hlines(0, xmin=0, xmax=len(crl), linestyles='--', color='gray')
         plt.legend()
         plt.show()
-        plt.figure(figsize=(24, 8))
+        plt.figure(figsize=(24, 4))
         plt.title('Test Rewards')
         plt.scatter(tl_indexes, tl_values, label="DDQL Agent")
         plt.hlines(0, xmin=0, xmax=len(tl), linestyles='--', color='gray')
         plt.legend()
         plt.show()
 
     @abstractmethod
```

### Comparing `ddqla-0.1.14/LICENSE` & `ddqla-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `ddqla-0.1.14/README.md` & `ddqla-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `ddqla-0.1.14/pyproject.toml` & `ddqla-0.1.15/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ddqla"
-version = "0.1.14"
+version = "0.1.15"
 authors = [{ name="Marco Sarti", email="info@marcosarti.com" }]
 description = "A smart way to create a ddql agent"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `ddqla-0.1.14/PKG-INFO` & `ddqla-0.1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddqla
-Version: 0.1.14
+Version: 0.1.15
 Summary: A smart way to create a ddql agent
 Project-URL: Homepage, https://github.com/marco-sarti/ddqla
 Project-URL: Bug Tracker, https://github.com/marco-sarti/ddqla/issues
 Author-email: Marco Sarti <info@marcosarti.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

