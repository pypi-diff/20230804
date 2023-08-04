# Comparing `tmp/tencentcloud-sdk-python-iot-3.0.949.tar.gz` & `tmp/tencentcloud-sdk-python-iot-3.0.950.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iot-3.0.949.tar", last modified: Thu Aug  3 00:27:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iot-3.0.950.tar", last modified: Fri Aug  4 00:28:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iot-3.0.949.tar` & `tencentcloud-sdk-python-iot-3.0.950.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud_sdk_python_iot.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud_sdk_python_iot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud_sdk_python_iot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud_sdk_python_iot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud_sdk_python_iot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud_sdk_python_iot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/v20180123/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/v20180123/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6163 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/v20180123/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   171391 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/v20180123/models.py
--rw-r--r--   0 root         (0) root         (0)    40904 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/v20180123/iot_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:27:58.000000 tencentcloud-sdk-python-iot-3.0.949/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud_sdk_python_iot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud_sdk_python_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud_sdk_python_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud_sdk_python_iot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud_sdk_python_iot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud_sdk_python_iot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/v20180123/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/v20180123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6163 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/v20180123/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   171391 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/v20180123/models.py
+-rw-r--r--   0 root         (0) root         (0)    40904 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/v20180123/iot_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:28:44.000000 tencentcloud-sdk-python-iot-3.0.950/README.rst
```

### Comparing `tencentcloud-sdk-python-iot-3.0.949/setup.py` & `tencentcloud-sdk-python-iot-3.0.950/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-iot',
-    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Iot SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-iot-3.0.949/tencentcloud_sdk_python_iot.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iot-3.0.950/tencentcloud_sdk_python_iot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iot
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Iot SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iot-3.0.949/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iot-3.0.950/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/v20180123/errorcodes.py` & `tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/v20180123/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/v20180123/models.py` & `tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/v20180123/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iot-3.0.949/tencentcloud/iot/v20180123/iot_client.py` & `tencentcloud-sdk-python-iot-3.0.950/tencentcloud/iot/v20180123/iot_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iot-3.0.949/PKG-INFO` & `tencentcloud-sdk-python-iot-3.0.950/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iot
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Iot SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iot-3.0.949/README.rst` & `tencentcloud-sdk-python-iot-3.0.950/README.rst`

 * *Files identical despite different names*
