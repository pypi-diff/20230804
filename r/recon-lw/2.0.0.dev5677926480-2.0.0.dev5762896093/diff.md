# Comparing `tmp/recon_lw-2.0.0.dev5677926480.tar.gz` & `tmp/recon_lw-2.0.0.dev5762896093.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5677926480.tar", last modified: Thu Jul 27 07:49:00 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5762896093.tar", last modified: Fri Aug  4 13:42:54 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5677926480.tar` & `recon_lw-2.0.0.dev5762896093.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-27 07:48:38.000000 recon_lw-2.0.0.dev5677926480/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14283 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6405 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    18015 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-04 13:42:27.000000 recon_lw-2.0.0.dev5762896093/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14303 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6405 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18015 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/StateSequenceGenerator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
                         continue
                     first_key = o_lst[0][1]
                     if first_key not in self._state_cache:
                         self._state_cache[first_key] = {"no_state": True}
                     current_state = self._state_cache[first_key]
                     updates_states = []
                     for o, key, new_key in o_lst:
-                        updates_states.append((o,copy.deepcopy(current_state)))
                         self._state_update(o, current_state, self._create_event, self._send_events)
+                        updates_states.append((o,copy.deepcopy(current_state)))
                     last_new_key = o_lst[-1][2]
                     if last_new_key is not None and last_new_key != chain_key:
                         self._state_cache[last_new_key] = self._state_cache.pop(first_key)
                     if self._debug:
                         body = {"ts_key" : ts_key, "chain_key": chain_key, "last_new_key": last_new_key, "stream": stream}
                         body["all_keys"] = {item[1] for item in o_lst}
                         body["all_new_keys"] = {item[2] for item in o_lst}
```

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/recon_lw.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import listdir
 from os import path
 from recon_lw.EventsSaver import EventsSaver
 
 
 def epoch_nano_str_to_ts(s_nanos):
     nanos = int(s_nanos)
-    return {"epochSecond": nanos // 1e9, "nano": nanos % 1e9}
+    return {"epochSecond": nanos // 1_000_000_000, "nano": nanos % 1_000_000_000}
 
 
 def ts_to_epoch_nano_str(ts):
     return f'{ts["epochSecond"]}{str(ts["nano"]).zfill(9)}'
 
 
 def time_stamp_key(ts):
```

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw/recon_oe_ob.py` & `recon_lw-2.0.0.dev5762896093/recon_lw/recon_oe_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/setup.py` & `recon_lw-2.0.0.dev5762896093/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5677926480/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5762896093/test/test_recon_ob.py`

 * *Files identical despite different names*

