# Comparing `tmp/python_hue_v2-1.0.2.tar.gz` & `tmp/python_hue_v2-1.0.3.tar.gz`

## Comparing `python_hue_v2-1.0.2.tar` & `python_hue_v2-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/pytest.ini
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.idea/hue-v2.iml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/__init__.py
--rw-r--r--   0        0        0     6485 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/bridge.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/grouped_light.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/hue.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/light.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/mdns.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/room/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/room/resource_identifier_get.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/room/room.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/room/room_get.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/__init__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/group.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/meta_data.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/scene.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/target.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/action/__init__.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/action/action.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/action/action_get.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/action/action_post.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/src/python_hue_v2/scene/action/action_put.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/tests/test_hue.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/tests/test_object_convert.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/LICENSE
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/README.md
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 python_hue_v2-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.DS_Store
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/pytest.ini
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/hue-v2.iml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/__init__.py
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/bridge.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/grouped_light.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/hue.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/light.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/mdns.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/room/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/room/resource_identifier_get.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/room/room.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/room/room_get.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/__init__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/group.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/meta_data.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/scene.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/target.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/__init__.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_get.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_post.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_put.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/tests/test_hue.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/tests/test_object_convert.py
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/README.md
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/PKG-INFO
```

### Comparing `python_hue_v2-1.0.2/.github/workflows/python-publish.yml` & `python_hue_v2-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/.idea/inspectionProfiles/Project_Default.xml` & `python_hue_v2-1.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/bridge.py` & `python_hue_v2-1.0.3/src/python_hue_v2/bridge.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,42 +50,52 @@
     @staticmethod
     def _convert_to_data(res: dict) -> List[dict]:
         if res['errors']:
             raise ConnectionError(res['errors'])
         else:
             return res['data']
 
+    @staticmethod
+    def _check_status_code(res: requests.Response):
+        if res.status_code != 403:
+            return res.json()
+        else:
+            raise ConnectionRefusedError()
+
     def _get_by_id(self, category: str, item_id: str) -> dict:
         url = f'{self.base_url}/{category}/{item_id}'
-        res = requests.get(url, headers={self.hue_application_key_name: self.hue_application_key}, verify=False).json()
+        res = self._check_status_code(
+            requests.get(url, headers={self.hue_application_key_name: self.hue_application_key}, verify=False))
         return self._convert_to_data(res)[0]  # data length should be 1, so return first element [0]
 
     def _get(self, category: str) -> List[dict]:
         url = f'{self.base_url}/{category}'
-        res = requests.get(url, headers={self.hue_application_key_name: self.hue_application_key}, verify=False).json()
+        res = self._check_status_code(
+            requests.get(url, headers={self.hue_application_key_name: self.hue_application_key}, verify=False))
         return self._convert_to_data(res)
 
     def _put_by_id(self, category: str, item_id: str, properties: dict) -> dict:
         url = f'{self.base_url}/{category}/{item_id}'
-        res = requests.put(url, data=json.dumps(properties),
-                           headers={self.hue_application_key_name: self.hue_application_key},
-                           verify=False).json()
+        res = self._check_status_code(requests.put(url, data=json.dumps(properties),
+                                                   headers={self.hue_application_key_name: self.hue_application_key},
+                                                   verify=False))
         return self._convert_to_data(res)[0]
 
     def _post(self, category: str, properties: dict) -> list:
         url = f'{self.base_url}/{category}'
-        res = requests.post(url, data=json.dumps(properties),
-                            headers={self.hue_application_key_name: self.hue_application_key},
-                            verify=False).json()
+        res = self._check_status_code(requests.post(url, data=json.dumps(properties),
+                                                    headers={self.hue_application_key_name: self.hue_application_key},
+                                                    verify=False))
         return self._convert_to_data(res)
 
     def _delete_by_id(self, category: str, item_id: str) -> list:
         url = f'{self.base_url}/{category}/{item_id}'
-        res = requests.delete(url, headers={self.hue_application_key_name: self.hue_application_key},
-                              verify=False).json()
+        res = self._check_status_code(
+            requests.delete(url, headers={self.hue_application_key_name: self.hue_application_key},
+                            verify=False))
         return self._convert_to_data(res)
 
     def get_light(self, light_id: str) -> dict:
         return self._get_by_id(self._light_category, light_id)
 
     def get_lights(self) -> List[dict]:
         """
```

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/grouped_light.py` & `python_hue_v2-1.0.3/src/python_hue_v2/grouped_light.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/hue.py` & `python_hue_v2-1.0.3/src/python_hue_v2/hue.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/light.py` & `python_hue_v2-1.0.3/src/python_hue_v2/light.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/mdns.py` & `python_hue_v2-1.0.3/src/python_hue_v2/mdns.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/scene/scene.py` & `python_hue_v2-1.0.3/src/python_hue_v2/scene/scene.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/scene/action/action.py` & `python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/scene/action/action_get.py` & `python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_get.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/src/python_hue_v2/scene/action/action_post.py` & `python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_post.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/tests/test_hue.py` & `python_hue_v2-1.0.3/tests/test_hue.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/.gitignore` & `python_hue_v2-1.0.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -235,7 +235,8 @@
 
 # Editor-based Rest Client
 .idea/httpRequests
 
 # Android studio 3.1+ serialized cache file
 .idea/caches/build_file_checksums.ser
 
+src/.DS_Store
```

### Comparing `python_hue_v2-1.0.2/LICENSE` & `python_hue_v2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/README.md` & `python_hue_v2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/pyproject.toml` & `python_hue_v2-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.2/PKG-INFO` & `python_hue_v2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hue-v2
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python library to control the Philips Hue lighting system.
 Project-URL: Documentation, https://github.com/FengChendian/python-hue-v2#readme
 Project-URL: Issues, https://github.com/FengChendian/python-hue-v2/issues
 Project-URL: Source, https://github.com/FengChendian/python-hue-v2
 Author-email: Yichen Zhao <njuzhaoyichen@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

