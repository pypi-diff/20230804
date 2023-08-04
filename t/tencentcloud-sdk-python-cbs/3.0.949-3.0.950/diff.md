# Comparing `tmp/tencentcloud-sdk-python-cbs-3.0.949.tar.gz` & `tmp/tencentcloud-sdk-python-cbs-3.0.950.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.949.tar", last modified: Thu Aug  3 00:21:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.950.tar", last modified: Fri Aug  4 00:21:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cbs-3.0.949.tar` & `tencentcloud-sdk-python-cbs-3.0.950.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud_sdk_python_cbs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud_sdk_python_cbs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/v20170312/
--rw-r--r--   0 root         (0) root         (0)    51002 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/v20170312/cbs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   227562 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:21:27.000000 tencentcloud-sdk-python-cbs-3.0.949/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud_sdk_python_cbs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud_sdk_python_cbs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:21:23.000000 tencentcloud-sdk-python-cbs-3.0.950/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:21:23.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:21:23.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    51002 2023-08-04 00:21:23.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/v20170312/cbs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:21:23.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-08-04 00:21:23.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   227562 2023-08-04 00:21:23.000000 tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:21:24.000000 tencentcloud-sdk-python-cbs-3.0.950/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:21:23.000000 tencentcloud-sdk-python-cbs-3.0.950/README.rst
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.949/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.950/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.949/setup.py` & `tencentcloud-sdk-python-cbs-3.0.950/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cbs',
-    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cbs SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.949'
+__version__ = '3.0.950'
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/v20170312/cbs_client.py` & `tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/v20170312/cbs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.949/tencentcloud/cbs/v20170312/models.py` & `tencentcloud-sdk-python-cbs-3.0.950/tencentcloud/cbs/v20170312/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4200,42 +4200,42 @@
 class Filter(AbstractModel):
     """描述键值对过滤器，用于条件过滤查询。
 
     """
 
     def __init__(self):
         r"""
-        :param _Values: 一个或者多个过滤值。
-        :type Values: list of str
         :param _Name: 过滤键的名称。
         :type Name: str
+        :param _Values: 一个或者多个过滤值。
+        :type Values: list of str
         """
-        self._Values = None
         self._Name = None
-
-    @property
-    def Values(self):
-        return self._Values
-
-    @Values.setter
-    def Values(self, Values):
-        self._Values = Values
+        self._Values = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
     def Name(self, Name):
         self._Name = Name
 
+    @property
+    def Values(self):
+        return self._Values
+
+    @Values.setter
+    def Values(self, Values):
+        self._Values = Values
+
 
     def _deserialize(self, params):
-        self._Values = params.get("Values")
         self._Name = params.get("Name")
+        self._Values = params.get("Values")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.949/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.950/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.949/README.rst` & `tencentcloud-sdk-python-cbs-3.0.950/README.rst`

 * *Files identical despite different names*

