# Comparing `tmp/gymnasium_trading-0.0.6.tar.gz` & `tmp/gymnasium_trading-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_trading-0.0.6.tar", last modified: Wed Aug  2 16:36:00 2023, max compression
+gzip compressed data, was "gymnasium_trading-0.0.7.tar", last modified: Thu Aug  3 22:14:17 2023, max compression
```

## Comparing `gymnasium_trading-0.0.6.tar` & `gymnasium_trading-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:36:00.165772 gymnasium_trading-0.0.6/
--rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      386 2023-08-02 16:36:00.165772 gymnasium_trading-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:36:00.145533 gymnasium_trading-0.0.6/gymnasium_trading/
--rw-rw-rw-   0        0        0      193 2023-08-02 16:35:28.000000 gymnasium_trading-0.0.6/gymnasium_trading/__init__.py
--rw-rw-rw-   0        0        0     6362 2023-08-01 21:24:08.000000 gymnasium_trading-0.0.6/gymnasium_trading/gym_trading.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:36:00.164730 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/
--rw-rw-rw-   0        0        0      386 2023-08-02 16:35:59.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-08-02 16:36:00.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:35:59.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-02 16:35:59.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-02 16:35:59.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-02 16:36:00.167800 gymnasium_trading-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-08-02 16:35:56.000000 gymnasium_trading-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:14:17.791453 gymnasium_trading-0.0.7/
+-rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      386 2023-08-03 22:14:17.791453 gymnasium_trading-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 22:14:17.765952 gymnasium_trading-0.0.7/gymnasium_trading/
+-rw-rw-rw-   0        0        0      193 2023-08-02 16:35:28.000000 gymnasium_trading-0.0.7/gymnasium_trading/__init__.py
+-rw-rw-rw-   0        0        0     7248 2023-08-03 22:09:20.000000 gymnasium_trading-0.0.7/gymnasium_trading/gym_trading.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:14:17.789453 gymnasium_trading-0.0.7/gymnasium_trading.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-08-03 22:14:17.000000 gymnasium_trading-0.0.7/gymnasium_trading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-08-03 22:14:17.000000 gymnasium_trading-0.0.7/gymnasium_trading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 22:14:17.000000 gymnasium_trading-0.0.7/gymnasium_trading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-03 22:14:17.000000 gymnasium_trading-0.0.7/gymnasium_trading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-03 22:14:17.000000 gymnasium_trading-0.0.7/gymnasium_trading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-03 22:14:17.798048 gymnasium_trading-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-08-03 22:13:16.000000 gymnasium_trading-0.0.7/setup.py
```

### Comparing `gymnasium_trading-0.0.6/LICENSE` & `gymnasium_trading-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_trading-0.0.6/gymnasium_trading/gym_trading.py` & `gymnasium_trading-0.0.7/gymnasium_trading/gym_trading.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import gymnasium as gym
 from gymnasium import spaces
 import pygame
 import numpy as np
 
+# the environment class must inherit from abstract class gym.Env
+
 
 class GymnasiumTradingEnv(gym.Env):
+    # metada . There, you should specify the render-modes that are supported by your environment (e.g. "human", "rgb_array", "ansi") and the framerate
     metadata = {"render_modes": ["human", "rgb_array"], "render_fps": 4}
 
     def __init__(self, render_mode=None, size=5):
         self.size = size  # The size of the square grid
         self.window_size = 512  # The size of the PyGame window
 
         # Observations are dictionaries with the agent's and the target's location.
         # Each location is encoded as an element of {0, ..., `size`}^2, i.e. MultiDiscrete([size, size]).
-        self.observation_space = spaces.Dict(
+        # This observation is a dict space with an agent being a box space of 2x1 dimension of ints from 0 to size-1 and target being the same as agent
+        '''self.observation_space = spaces.Dict(
             {
                 "agent": spaces.Box(0, size - 1, shape=(2,), dtype=int),
                 "target": spaces.Box(0, size - 1, shape=(2,), dtype=int),
             }
-        )
+        )'''
+        # Observation now is a Box space indicating where the agent is located
+        self.observation_space = spaces.Box(
+            0, size - 1, shape=(2,), dtype=int)
 
         # We have 4 actions, corresponding to "right", "up", "left", "down", "right"
         self.action_space = spaces.Discrete(4)
 
         """
         The following dictionary maps abstract actions from `self.action_space` to 
         the direction we will walk in if that action is taken.
@@ -45,35 +52,38 @@
         human-mode. They will remain `None` until human-mode is used for the
         first time.
         """
         self.window = None
         self.clock = None
 
     def _get_obs(self):
-        return {"agent": self._agent_location, "target": self._target_location}
+        # return {"agent": self._agent_location, "target": self._target_location}
+        return self._agent_location
 
     def _get_info(self):
         return {
             "distance": np.linalg.norm(
                 self._agent_location - self._target_location, ord=1
             )
         }
 
     def reset(self, seed=None, options=None):
         # We need the following line to seed self.np_random
+        # For Custom environments, the first line of :meth:`reset` should be ``super().reset(seed=seed)`` which implements
+        # the seeding correctly.
         super().reset(seed=seed)
-
+        self._target_location = np.array([self.size-1, self.size-1], dtype=int)
         # Choose the agent's location uniformly at random
-        self._agent_location = self.np_random.integers(
-            0, self.size, size=2, dtype=int)
-
+        # self._agent_location = self.np_random.integers(
+        #    0, self.size, size=2, dtype=int)
+        self._agent_location = self._target_location
         # We will sample the target's location randomly until it does not coincide with the agent's location
-        self._target_location = self._agent_location
+        # self._target_location = self._agent_location
         while np.array_equal(self._target_location, self._agent_location):
-            self._target_location = self.np_random.integers(
+            self._agent_location = self.np_random.integers(
                 0, self.size, size=2, dtype=int
             )
 
         observation = self._get_obs()
         info = self._get_info()
 
         if self.render_mode == "human":
```

### Comparing `gymnasium_trading-0.0.6/setup.py` & `gymnasium_trading-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name="gymnasium_trading",
-    version="0.0.6",
+    version="0.0.7",
     install_requires=["gymnasium==0.28.1", "pygame==2.5.0"],
     author='Alejandro Rioja Chocrón',
     author_email='archocron@gmail.com',
     url='https://github.com/archocron/gymnasium-trading',
     packages=['gymnasium_trading'],
     license='gpl-3.0',
     description='Gimnasium environment focus on trading strategies',
     # I explain this later on
-    download_url='https://github.com/archocron/gymnasium-trading/archive/refs/tags/0.0.3.tar.gz',
+    download_url='https://github.com/archocron/gymnasium-trading/archive/refs/tags/0.0.7.tar.gz',
 
 )
```

