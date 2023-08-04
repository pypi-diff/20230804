# Comparing `tmp/python-iq-sim-0.0.3.tar.gz` & `tmp/python-iq-sim-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iq-sim-0.0.3.tar", last modified: Sun Feb 19 21:04:55 2023, max compression
+gzip compressed data, was "python-iq-sim-0.0.4.tar", last modified: Fri Aug  4 21:01:01 2023, max compression
```

## Comparing `python-iq-sim-0.0.3.tar` & `python-iq-sim-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-02-19 21:04:55.449565 python-iq-sim-0.0.3/
--rw-rw-r--   0 eric      (1000) eric      (1000)     3733 2023-02-19 21:04:55.445565 python-iq-sim-0.0.3/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     2303 2023-02-19 20:41:48.000000 python-iq-sim-0.0.3/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-02-19 21:04:55.445565 python-iq-sim-0.0.3/iq_sim/
--rw-rw-r--   0 eric      (1000) eric      (1000)       32 2023-02-19 21:04:36.000000 python-iq-sim-0.0.3/iq_sim/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     6189 2023-02-19 19:31:39.000000 python-iq-sim-0.0.3/iq_sim/iq_sim.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-02-19 21:04:55.445565 python-iq-sim-0.0.3/python_iq_sim.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)     3733 2023-02-19 21:04:55.000000 python-iq-sim-0.0.3/python_iq_sim.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)      238 2023-02-19 21:04:55.000000 python-iq-sim-0.0.3/python_iq_sim.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-02-19 21:04:55.000000 python-iq-sim-0.0.3/python_iq_sim.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        9 2023-02-19 21:04:55.000000 python-iq-sim-0.0.3/python_iq_sim.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        7 2023-02-19 21:04:55.000000 python-iq-sim-0.0.3/python_iq_sim.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-02-19 21:04:55.449565 python-iq-sim-0.0.3/setup.cfg
--rw-rw-r--   0 eric      (1000) eric      (1000)     1128 2023-02-19 21:04:52.000000 python-iq-sim-0.0.3/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-08-04 21:01:01.781585 python-iq-sim-0.0.4/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3733 2023-08-04 21:01:01.781585 python-iq-sim-0.0.4/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2303 2023-02-19 20:41:48.000000 python-iq-sim-0.0.4/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-08-04 21:01:01.781585 python-iq-sim-0.0.4/iq_sim/
+-rw-rw-r--   0 eric      (1000) eric      (1000)       32 2023-02-19 21:04:36.000000 python-iq-sim-0.0.4/iq_sim/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     6363 2023-08-04 20:44:00.000000 python-iq-sim-0.0.4/iq_sim/iq_sim.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-08-04 21:01:01.781585 python-iq-sim-0.0.4/python_iq_sim.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3733 2023-08-04 21:01:01.000000 python-iq-sim-0.0.4/python_iq_sim.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      238 2023-08-04 21:01:01.000000 python-iq-sim-0.0.4/python_iq_sim.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-08-04 21:01:01.000000 python-iq-sim-0.0.4/python_iq_sim.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        9 2023-08-04 21:01:01.000000 python-iq-sim-0.0.4/python_iq_sim.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        7 2023-08-04 21:01:01.000000 python-iq-sim-0.0.4/python_iq_sim.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-08-04 21:01:01.781585 python-iq-sim-0.0.4/setup.cfg
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1128 2023-08-04 20:59:47.000000 python-iq-sim-0.0.4/setup.py
```

### Comparing `python-iq-sim-0.0.3/PKG-INFO` & `python-iq-sim-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iq-sim
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Library for starting and managing simulations in the Intelligent Quads Cloud
 Home-page: UNKNOWN
 Author: Eric Johnson
 Author-email: 
 License: UNKNOWN
 Description: 
         # Python-IQ-Sim
```

### Comparing `python-iq-sim-0.0.3/README.md` & `python-iq-sim-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python-iq-sim-0.0.3/iq_sim/iq_sim.py` & `python-iq-sim-0.0.4/iq_sim/iq_sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         Args:
             sim_id (str, optional): unique id of a simulation. Defaults to None.
 
         Returns:
             Dict: dict in form of {"running_sims": [{"status": str, "sim_id": str, "fc_instances": str, "creation_time" : str}]}
         """
         r = requests.post(self.url + 'running_sims', headers=self.headers)
+        print(r.text)
         result = json.loads(r.text)
         if "error" in result:
             print(result["error"])
             sys.exit(1)
         else:
             if sim_id is None:
                 return result
@@ -120,14 +121,16 @@
         """
 
         if sim_config is None:
             sim_config = self.sim_config
 
         # This is the request that you want to send to the API
         r = requests.post(self.url + 'start', json=sim_config, headers=self.headers)
+        print(r)
+        print(r.text)
         result = json.loads(r.text)
         print(result)
 
         if "status" in result and result["status"] == "success":
             sim_id = result["sim_id"]
             print(f"sim_id: {sim_id}")
             return sim_id
@@ -165,14 +168,18 @@
         Args:
             sim_id (str): unique id of the simulation
             timeout (int, optional): Defaults to 80.
         """        
         time_start = time.time()
         while time.time() - time_start < timeout:
             result = self.get_running_simulations(sim_id)
-            if result["status"] == "Running":
-                return
+            print(result)
+            if result:
+                if result["status"] == "Running":
+                    return
+                else:
+                    time.sleep(1)
             else:
                 time.sleep(1)
 
         print("timed out waiting for sim to start. During High Traffic times, it can take up to a couple of minutes to start a simulation. try setting timeout higher or try again later.")   
         sys.exit(1)
```

### Comparing `python-iq-sim-0.0.3/python_iq_sim.egg-info/PKG-INFO` & `python-iq-sim-0.0.4/python_iq_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iq-sim
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Library for starting and managing simulations in the Intelligent Quads Cloud
 Home-page: UNKNOWN
 Author: Eric Johnson
 Author-email: 
 License: UNKNOWN
 Description: 
         # Python-IQ-Sim
```

### Comparing `python-iq-sim-0.0.3/setup.py` & `python-iq-sim-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Python Library for starting and managing simulations in the Intelligent Quads Cloud'
 LONG_DESCRIPTION = 'Python Library for starting and managing simulations in the Intelligent Quads Cloud'
 
 # Setting up
 setup(
     name="python-iq-sim",
     version=VERSION,
```

